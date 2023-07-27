# Comparing `tmp/glypniro-0.1.2.tar.gz` & `tmp/glypniro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glypniro-0.1.2.tar", max compression
+gzip compressed data, was "glypniro-0.1.3.tar", max compression
```

## Comparing `glypniro-0.1.2.tar` & `glypniro-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.2/glypniro/__init__.py
--rw-r--r--   0        0        0    14386 2023-07-27 01:34:47.027984 glypniro-0.1.2/glypniro/cli.py
--rw-r--r--   0        0        0    49477 2023-07-24 23:51:40.093127 glypniro-0.1.2/glypniro/common.py
--rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.2/glypniro/reformat.py
--rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.2/glypniro/reformat_skyline.py
--rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.2/LICENSE
--rw-r--r--   0        0        0      672 2023-07-27 01:37:24.969523 glypniro-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.2/README.md
--rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.3/glypniro/__init__.py
+-rw-r--r--   0        0        0    14386 2023-07-27 01:40:55.473132 glypniro-0.1.3/glypniro/cli.py
+-rw-r--r--   0        0        0    49477 2023-07-24 23:51:40.093127 glypniro-0.1.3/glypniro/common.py
+-rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.3/glypniro/reformat.py
+-rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.3/glypniro/reformat_skyline.py
+-rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.3/LICENSE
+-rw-r--r--   0        0        0      672 2023-07-27 01:41:00.960403 glypniro-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.3/README.md
+-rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.3/PKG-INFO
```

### Comparing `glypniro-0.1.2/glypniro/cli.py` & `glypniro-0.1.3/glypniro/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 @click.option("--output", "-o", help="Filepath to output", type=click.Path(exists=False))
 @click.option("--score-cutoff", "-s", help="Filter the data by specific Byonic cut-off quality score", type=float, default=200)
 @click.option("--trust-byonic", "-t", help="Enable site specific glycan position parsing from Byonic", is_flag=True)
 @click.option("--get-uniprot", "-g", help="Required internet connection. Enable parsing of UniProt ID from protein name and request the original protein name from the UniProt databas.", is_flag=True)
 @click.option("--parse-uniprot", "-p", help="Attempt to parse UniProt ID from protein name", is_flag=True)
 @click.option("--debug", "-d", help="In conjunction to the final output, the script would also create debug files that contain the "
                          "unique PSM selected for calculation of the data in the final output", is_flag=True)
-@click.option("--mode", "-m", help="Select the mode of operation. 0: Byonic only, 1: PD only, 2: Byonic and PD", type=int, default=2)
+@click.option("--mode", "-m", help="Select the mode of operation. 0: Byonic only, 1: PD only, 2: Byonic and PD", type=int, default=1)
 @click.option("--custom-group", "-c", help="A tabulated text file with two columns, Glycans and Labels. Glycans must be the glycans appear in the result and labels is the custome label for them", type=click.Path(exists=True))
 def main(input_file, output, score_cutoff, trust_byonic, get_uniprot, parse_uniprot, debug, mode, custom_group):
     """
     Automated workflow for processing and combining Byonic and PD output
     """
     print(input_file, output, score_cutoff, trust_byonic, get_uniprot, parse_uniprot, debug, mode, custom_group)
     ex = GlypnirO(trust_byonic=trust_byonic, get_uniprot=get_uniprot, debug=debug,
```

### Comparing `glypniro-0.1.2/glypniro/common.py` & `glypniro-0.1.3/glypniro/common.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.2/glypniro/reformat.py` & `glypniro-0.1.3/glypniro/reformat.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.2/glypniro/reformat_skyline.py` & `glypniro-0.1.3/glypniro/reformat_skyline.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.2/LICENSE` & `glypniro-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.2/pyproject.toml` & `glypniro-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glypniro"
-version = "0.1.2"
+version = "0.1.3"
 description = "A automated script for processing and combining Byonic and PD standard output."
 authors = ["Toan Phung <toan.phungkhoiquoctoan@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 scipy = "^1.11.1"
```

### Comparing `glypniro-0.1.2/README.md` & `glypniro-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.2/PKG-INFO` & `glypniro-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glypniro
-Version: 0.1.2
+Version: 0.1.3
 Summary: A automated script for processing and combining Byonic and PD standard output.
 Author: Toan Phung
 Author-email: toan.phungkhoiquoctoan@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

