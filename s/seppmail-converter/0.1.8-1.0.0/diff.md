# Comparing `tmp/seppmail_converter-0.1.8.tar.gz` & `tmp/seppmail_converter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail_converter-0.1.8.tar", max compression
+gzip compressed data, was "seppmail_converter-1.0.0.tar", max compression
```

## Comparing `seppmail_converter-0.1.8.tar` & `seppmail_converter-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      939 2023-05-05 11:44:24.721586 seppmail_converter-0.1.8/README.md
--rw-r--r--   0        0        0      541 2023-05-05 11:30:27.127632 seppmail_converter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-05 11:29:48.040535 seppmail_converter-0.1.8/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      133 2023-04-13 20:35:22.726388 seppmail_converter-0.1.8/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     5072 2023-05-05 11:44:56.671543 seppmail_converter-0.1.8/seppmail_converter/main.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 seppmail_converter-0.1.8/setup.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 seppmail_converter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-27 12:41:16.281587 seppmail_converter-1.0.0/README.md
+-rw-r--r--   0        0        0      839 2023-07-27 12:41:46.705465 seppmail_converter-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-27 12:41:46.785465 seppmail_converter-1.0.0/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-27 12:41:16.281587 seppmail_converter-1.0.0/seppmail_converter/crawler.py
+-rw-r--r--   0        0        0      133 2023-07-27 12:41:16.281587 seppmail_converter-1.0.0/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     5336 2023-07-27 12:41:16.281587 seppmail_converter-1.0.0/seppmail_converter/main.py
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 seppmail_converter-1.0.0/PKG-INFO
```

### Comparing `seppmail_converter-0.1.8/README.md` & `seppmail_converter-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,19 @@
   -p, --password TEXT
   -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
   -o, --overwrite      Overwrite output file if it exists
   -e, --extract        Extract attachments from .eml file
   -q, --quiet          Suppress all output except final path
+  -v, --version        Show the version and exit.
   --help               Show this message and exit.
 ```
 
 Relevant environment variables:
 
-| Name | Description |
-| ---- | ----------- |
-| `SEPPMAIL_USERNAME` | Email supplied during login |
-| `SEPPMAIL_PASSWORD` | Password supplied during login|
+| Name                | Description                    |
+|---------------------|--------------------------------|
+| `SEPPMAIL_USERNAME` | Email supplied during login    |
+| `SEPPMAIL_PASSWORD` | Password supplied during login |
 
 Unless specified, the script will place the output file next to the input file and name it after the original file.
```

### Comparing `seppmail_converter-0.1.8/seppmail_converter/main.py` & `seppmail_converter-1.0.0/seppmail_converter/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from email import policy
 
 import click
 import requests
 from bs4 import BeautifulSoup
 
 from seppmail_converter.exceptions import AuthenticationError, ExportError
+from seppmail_converter import __version__
 
 
 def get_valid_filename(name):
     s = str(name).strip().replace(" ", "_")
     s = re.sub(r"(?u)[^-\w.]", "", s)
     if s in {"", ".", ".."}:
         return None
@@ -71,32 +72,35 @@
 @click.option(
     "--quiet",
     "-q",
     help="Suppress all output except final path",
     type=click.BOOL,
     is_flag=True,
 )
+@click.version_option(__version__, "-v", "--version", message="%(version)s")
 def cli(
     input_file: pathlib.Path,
     output: pathlib.Path,
     username: str,
     password: str,
     force: bool,
     delete: bool,
     overwrite: bool,
     extract: bool,
     quiet: bool,
 ):
+    input_file_data = input_file.read_text("utf-8")
+
     # Extract key-value pairs from form
-    if "secmail" not in input_file.read_text("utf-8") and not force:
+    if "secmail" not in input_file_data and not force:
         raise click.FileError(
             str(input_file.absolute()), "The input file provided seems to be invalid"
         )
 
-    soup = BeautifulSoup(input_file.read_text("utf-8"), "lxml")
+    soup = BeautifulSoup(input_file_data, "lxml")
     value_map = {
         node.attrs.get("name"): node.attrs.get("value")
         for node in soup.find_all("input")
     }
 
     # Submit the created form to receive session
     target_url = soup.find("form").attrs["action"]
@@ -162,16 +166,18 @@
     else:
         click.echo(
             f"Decoded {click.format_filename(input_file.absolute())} to {click.format_filename(output.absolute())}"
         )
 
     if extract:
         msg = email.message_from_bytes(output.read_bytes(), policy=policy.default)
-        msg.get_payload()
         for attachment in msg.iter_attachments():
+            if not attachment.get_content_disposition() == "attachment":
+                # Skip over inline attachments
+                continue
             try:
                 attachment_filename = attachment.get_filename()
             except AttributeError:
                 continue
             if not attachment_filename:
                 continue
             attachment_output = pathlib.Path(
```

### Comparing `seppmail_converter-0.1.8/PKG-INFO` & `seppmail_converter-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 0.1.8
+Version: 1.0.0
 Summary: Decode SEPPMail emails into EML files
 License: MIT
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: requests (>=2.30,<3.0)
+Requires-Dist: click (>=8.1.6,<9.0.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
+Requires-Dist: requests (>=2.31,<3.0)
 Description-Content-Type: text/markdown
 
 # SEPPMail Converter
 
 This python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.
 
 ## Usage
@@ -31,19 +31,20 @@
   -p, --password TEXT
   -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
   -o, --overwrite      Overwrite output file if it exists
   -e, --extract        Extract attachments from .eml file
   -q, --quiet          Suppress all output except final path
+  -v, --version        Show the version and exit.
   --help               Show this message and exit.
 ```
 
 Relevant environment variables:
 
-| Name | Description |
-| ---- | ----------- |
-| `SEPPMAIL_USERNAME` | Email supplied during login |
-| `SEPPMAIL_PASSWORD` | Password supplied during login|
+| Name                | Description                    |
+|---------------------|--------------------------------|
+| `SEPPMAIL_USERNAME` | Email supplied during login    |
+| `SEPPMAIL_PASSWORD` | Password supplied during login |
 
 Unless specified, the script will place the output file next to the input file and name it after the original file.
```

