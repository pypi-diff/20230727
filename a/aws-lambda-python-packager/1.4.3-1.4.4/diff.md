# Comparing `tmp/aws_lambda_python_packager-1.4.3.tar.gz` & `tmp/aws_lambda_python_packager-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_python_packager-1.4.3.tar", max compression
+gzip compressed data, was "aws_lambda_python_packager-1.4.4.tar", max compression
```

## Comparing `aws_lambda_python_packager-1.4.3.tar` & `aws_lambda_python_packager-1.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     7652 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/LICENSE
--rw-r--r--   0        0        0      916 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/README.md
--rw-r--r--   0        0        0     4339 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/__init__.py
--rw-r--r--   0        0        0      637 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/__main__.py
--rw-r--r--   0        0        0     2714 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/arrow_fetcher.py
--rw-r--r--   0        0        0        0 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/__init__.py
--rw-r--r--   0        0        0     7517 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/build.py
--rw-r--r--   0        0        0     3609 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/unify.py
--rw-r--r--   0        0        0    14295 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/dep_analyzer.py
--rw-r--r--   0        0        0    14538 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/lambda_packager.py
--rw-r--r--   0        0        0     3546 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/pip_analyzer.py
--rw-r--r--   0        0        0     6002 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/poetry_analyzer.py
--rw-r--r--   0        0        0        0 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/py.typed
--rw-r--r--   0        0        0     4516 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/util.py
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 aws_lambda_python_packager-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     7652 2022-11-03 14:20:31.707890 aws_lambda_python_packager-1.4.4/LICENSE
+-rw-r--r--   0        0        0      916 2023-03-08 20:12:38.102170 aws_lambda_python_packager-1.4.4/README.md
+-rw-r--r--   0        0        0     4339 2023-07-14 17:28:48.421678 aws_lambda_python_packager-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-14 17:28:48.421678 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/__init__.py
+-rw-r--r--   0        0        0      685 2023-07-14 16:57:52.182647 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/__main__.py
+-rw-r--r--   0        0        0     2728 2023-07-14 16:56:47.570254 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/arrow_fetcher.py
+-rw-r--r--   0        0        0        0 2022-11-03 14:20:31.711890 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/cli/__init__.py
+-rw-r--r--   0        0        0     7517 2023-05-26 02:15:39.968175 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/cli/build.py
+-rw-r--r--   0        0        0     3609 2023-05-26 02:15:39.908175 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/cli/unify.py
+-rw-r--r--   0        0        0    14295 2023-05-26 02:20:00.944552 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/dep_analyzer.py
+-rw-r--r--   0        0        0    15187 2023-07-14 16:46:06.157064 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/lambda_packager.py
+-rw-r--r--   0        0        0     3546 2023-05-26 02:19:26.196502 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/pip_analyzer.py
+-rw-r--r--   0        0        0     6002 2023-05-26 02:19:26.192502 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/poetry_analyzer.py
+-rw-r--r--   0        0        0        0 2022-11-03 14:20:31.711890 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/py.typed
+-rw-r--r--   0        0        0     4516 2023-05-26 02:17:40.908351 aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/util.py
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 aws_lambda_python_packager-1.4.4/PKG-INFO
```

### Comparing `aws_lambda_python_packager-1.4.3/LICENSE` & `aws_lambda_python_packager-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/README.md` & `aws_lambda_python_packager-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/pyproject.toml` & `aws_lambda_python_packager-1.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-lambda-python-packager"
-version = "1.4.3"
+version = "1.4.4"
 description = "Description"
 authors = ["Daniel Sullivan <mumblepins@users.noreply.github.com>"]
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/mumblepins/aws-lambda-python-packager/"
 documentation = "https://mumblepins.github.io/aws-lambda-python-packager/"
 readme = "README.md"
 packages = [{ include = "aws_lambda_python_packager", from = "src" }]
```

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/arrow_fetcher.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/arrow_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,13 +74,13 @@
     package_version: str,
     python_version="3.9",
     arch="x86_64",
 ):
     if (pkg_url := get_arrow_version(package_version, python_version, arch)) is None:
         raise ValueError(f"Could not find package  arrow with version {package_version}")
     with open_zip_file(pkg_url) as zfh, tempfile.TemporaryDirectory() as tmpdir:
-        zfh.extractall(tmpdir)
+        zfh.extractall(tmpdir)  # nosec B202
 
         Path(output_dir).mkdir(parents=True, exist_ok=True)
         for p in (Path(tmpdir) / "python").glob("*"):
             shutil.copytree(p, Path(output_dir) / p.name, dirs_exist_ok=True)
         return package_version
```

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/build.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/cli/build.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/unify.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/cli/unify.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/dep_analyzer.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/dep_analyzer.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/lambda_packager.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/lambda_packager.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import json
 import logging
 import os
 import platform
 import re
 import shutil
 import subprocess  # nosec B404
+import tempfile
 from compileall import compile_dir
 from datetime import datetime
 from pathlib import Path
 from py_compile import PycInvalidationMode
 from tempfile import TemporaryDirectory
 from zipfile import ZIP_DEFLATED, ZipFile
 
@@ -192,36 +193,46 @@
         for p in self.output_dir.glob("**/*"):
             if p.is_file() and p.suffix in OTHER_FILE_EXTENSIONS:
                 LOG.debug("Stripping file %s", p)
                 p.unlink()
 
     def compress_boto(self):
         LOG.warning("(Re)Compressing botocore and boto3 data files")
-        f: Path
-        for f in self.output_dir.glob("**/boto[3c]*/data/**/*.json*"):
-            if f.name.endswith(".json.gz"):
-                _open = gzip.open
-                new_name = f
-                delete = False
-            else:
-                _open = open
-                new_name = f.with_suffix(".json.gz")
-                delete = True
-            try:
-                with _open(f, "rt") as fh, gzip.GzipFile(
-                    new_name, "wb", compresslevel=9, mtime=0
-                ) as zfh:
-                    # load and dump to decrease unnecessary whitespace,set mtime to 0 to make builds repeatable
-                    json_data = json.load(fh)
-                    zfh.write(json.dumps(json_data, separators=(",", ":")).encode("utf8"))
-            except json.decoder.JSONDecodeError:
-                delete = False
-            finally:
-                if delete:
-                    f.unlink(missing_ok=True)
+        old_file: Path
+        with tempfile.TemporaryDirectory() as td:
+            for old_file in list(self.output_dir.glob("**/boto[3c]*/data/**/*.json*")):
+                delete_new = False
+                if old_file.name.endswith(".json.gz"):
+                    _open = gzip.open
+                    new_temp_file = Path(td, old_file.name)
+                    new_file = old_file
+                    delete_old = False
+                else:
+                    _open = open
+                    new_temp_file = Path(td, old_file.name + ".gz")
+                    new_file = old_file.with_suffix(".json.gz")
+                    delete_old = True
+                try:
+                    with _open(old_file, "rt") as fh, gzip.GzipFile(
+                        new_temp_file, "wb", compresslevel=9, mtime=0
+                    ) as zfh:
+                        # load and dump to decrease unnecessary whitespace,set mtime to 0 to make builds repeatable
+                        json_data = json.load(fh)
+                        zfh.write(json.dumps(json_data, separators=(",", ":")).encode("utf8"))
+                    shutil.move(new_temp_file, new_file)
+                except json.decoder.JSONDecodeError as e:
+                    print(e)
+                    print("AAAA")
+                    delete_old = False
+                    delete_new = True
+                finally:
+                    if delete_old:
+                        old_file.unlink(missing_ok=True)
+                    if delete_new:
+                        new_temp_file.unlink(missing_ok=True)
 
     def strip_libraries(self):
         # noinspection PyBroadException
         try:
             LOG.warning("Stripping libraries")
             strip_command = get_strip_binary(self.architecture)
             for p in self.output_dir.glob("**/*.so*"):
```

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/pip_analyzer.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/pip_analyzer.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/poetry_analyzer.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/poetry_analyzer.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/util.py` & `aws_lambda_python_packager-1.4.4/src/aws_lambda_python_packager/util.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.4.3/PKG-INFO` & `aws_lambda_python_packager-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-lambda-python-packager
-Version: 1.4.3
+Version: 1.4.4
 Summary: Description
 Home-page: https://github.com/mumblepins/aws-lambda-python-packager/
 License: LGPL-3.0-or-later
 Author: Daniel Sullivan
 Author-email: mumblepins@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

