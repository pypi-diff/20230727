# Comparing `tmp/data_linter-6.2.1.tar.gz` & `tmp/data_linter-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_linter-6.2.1.tar", max compression
+gzip compressed data, was "data_linter-6.2.2.tar", max compression
```

## Comparing `data_linter-6.2.1.tar` & `data_linter-6.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10520 2023-05-10 09:37:19.258138 data_linter-6.2.1/README.md
--rw-r--r--   0        0        0       22 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/__init__.py
--rw-r--r--   0        0        0      490 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/command_line.py
--rw-r--r--   0        0        0      137 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/constants.py
--rw-r--r--   0        0        0     1881 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/iam.py
--rw-r--r--   0        0        0     5474 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/log_explorer_utils.py
--rw-r--r--   0        0        0     3206 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/logging_functions.py
--rw-r--r--   0        0        0    25362 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/schemas/config-schema.json
--rw-r--r--   0        0        0     7623 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/utils.py
--rw-r--r--   0        0        0    26887 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validation.py
--rw-r--r--   0        0        0      109 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/__init__.py
--rw-r--r--   0        0        0     5745 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/base.py
--rw-r--r--   0        0        0    16469 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/pandas_validator.py
--rw-r--r--   0        0        0     3316 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/parquet_validator.py
--rw-r--r--   0        0        0     1195 2023-05-10 09:37:19.262138 data_linter-6.2.1/pyproject.toml
--rw-r--r--   0        0        0    11559 1970-01-01 00:00:00.000000 data_linter-6.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10520 2023-07-27 10:28:14.886849 data_linter-6.2.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/__init__.py
+-rw-r--r--   0        0        0      490 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/command_line.py
+-rw-r--r--   0        0        0      137 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/constants.py
+-rw-r--r--   0        0        0     1881 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/iam.py
+-rw-r--r--   0        0        0     5474 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/log_explorer_utils.py
+-rw-r--r--   0        0        0     3206 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/logging_functions.py
+-rw-r--r--   0        0        0    25362 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/schemas/config-schema.json
+-rw-r--r--   0        0        0     7623 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/utils.py
+-rw-r--r--   0        0        0    26887 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/validation.py
+-rw-r--r--   0        0        0      109 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/validators/__init__.py
+-rw-r--r--   0        0        0     5745 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/validators/base.py
+-rw-r--r--   0        0        0    16469 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/validators/pandas_validator.py
+-rw-r--r--   0        0        0     3316 2023-07-27 10:28:14.886849 data_linter-6.2.2/data_linter/validators/parquet_validator.py
+-rw-r--r--   0        0        0     1192 2023-07-27 10:28:14.890849 data_linter-6.2.2/pyproject.toml
+-rw-r--r--   0        0        0    11616 1970-01-01 00:00:00.000000 data_linter-6.2.2/PKG-INFO
```

### Comparing `data_linter-6.2.1/README.md` & `data_linter-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/iam.py` & `data_linter-6.2.2/data_linter/iam.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/log_explorer_utils.py` & `data_linter-6.2.2/data_linter/log_explorer_utils.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/logging_functions.py` & `data_linter-6.2.2/data_linter/logging_functions.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/schemas/config-schema.json` & `data_linter-6.2.2/data_linter/schemas/config-schema.json`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/utils.py` & `data_linter-6.2.2/data_linter/utils.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/validation.py` & `data_linter-6.2.2/data_linter/validation.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/validators/base.py` & `data_linter-6.2.2/data_linter/validators/base.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/validators/pandas_validator.py` & `data_linter-6.2.2/data_linter/validators/pandas_validator.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/data_linter/validators/parquet_validator.py` & `data_linter-6.2.2/data_linter/validators/parquet_validator.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.1/pyproject.toml` & `data_linter-6.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "data_linter"
-version = "6.2.1"
+version = "6.2.2"
 description = "data linter"
 authors = ["Thomas Hirsch <thomas.hirsch@digital.justice.gov.uk>",
            "George Kelly <george.kelly@digital.justice.gov.uk>",
            "Tapan Perkins <tapan.perkins@digital.justice.gov.uk>",
            "Karik Isichei <karik.isichei@digital.justice.gov.uk>",
            "Stephen Bias <stephen.bias@digital.justice.gov.uk>"]
 
 readme = "README.md"
 repository = "https://github.com/moj-analytical-services/data_linter"
 homepage = "https://github.com/moj-analytical-services/data_linter"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<4.0"
 dataengineeringutils3 = "^1.0.1"
 boto3 = "^1.14.7"
 jsonschema = "^4.10.0"
-PyYAML = ">= 5.4.1"
+PyYAML = "^6.0.1"
 iam_builder = "^4.1.0"
 pandas = "^1.2"
 mojap-metadata = {version = "^1.10.0", extras = ["arrow"]}
 arrow-pd-parser = ">=1.3.0,<2"
 awswrangler = "^2.3.0"
 toml = "^0.10"
```

### Comparing `data_linter-6.2.1/PKG-INFO` & `data_linter-6.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: data-linter
-Version: 6.2.1
+Version: 6.2.2
 Summary: data linter
 Home-page: https://github.com/moj-analytical-services/data_linter
 Author: Thomas Hirsch
 Author-email: thomas.hirsch@digital.justice.gov.uk
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: frictionless
 Provides-Extra: ge
-Requires-Dist: PyYAML (>=5.4.1)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: arrow-pd-parser (>=1.3.0,<2)
 Requires-Dist: awswrangler (>=2.3.0,<3.0.0)
 Requires-Dist: boto3 (>=1.14.7,<2.0.0)
 Requires-Dist: dataengineeringutils3 (>=1.0.1,<2.0.0)
 Requires-Dist: iam_builder (>=4.1.0,<5.0.0)
 Requires-Dist: jsonschema (>=4.10.0,<5.0.0)
 Requires-Dist: mojap-metadata[arrow] (>=1.10.0,<2.0.0)
```

