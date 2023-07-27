# Comparing `tmp/mypy-boto3-rds-data-1.28.0.tar.gz` & `tmp/mypy-boto3-rds-data-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rds-data-1.28.0.tar", last modified: Thu Jul  6 21:00:23 2023, max compression
+gzip compressed data, was "mypy-boto3-rds-data-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
```

## Comparing `mypy-boto3-rds-data-1.28.0.tar` & `mypy-boto3-rds-data-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:23.270402 mypy-boto3-rds-data-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-06 21:00:23.266402 mypy-boto3-rds-data-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:23.258402 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:52:45.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:23.266402 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-06 21:00:23.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 21:00:23.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:23.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:23.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:23.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:23.000000 mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:23.270402 mypy-boto3-rds-data-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-06 20:52:44.000000 mypy-boto3-rds-data-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.657189 mypy-boto3-rds-data-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-27 11:49:27.649188 mypy-boto3-rds-data-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.649188 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-27 11:44:12.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-27 11:44:12.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-07-27 11:44:12.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.649188 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-27 11:49:27.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:27.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:27.000000 mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.657189 mypy-boto3-rds-data-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-27 11:44:11.000000 mypy-boto3-rds-data-1.28.12/setup.py
```

### Comparing `mypy-boto3-rds-data-1.28.0/LICENSE` & `mypy-boto3-rds-data-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-data-1.28.0/PKG-INFO` & `mypy-boto3-rds-data-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds-data
-Version: 1.28.0
-Summary: Type annotations for boto3.RDSDataService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RDSDataService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rds-data"></a>
 
 # mypy-boto3-rds-data
 
 [![PyPI - mypy-boto3-rds-data](https://img.shields.io/pypi/v/mypy-boto3-rds-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rds-data?color=blue)](https://pypistats.org/packages/mypy-boto3-rds-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds-data)](https://pepy.tech/project/mypy-boto3-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDSDataService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[boto3.RDSDataService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rds-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,43 +299,45 @@
 ### Typed dictionaries
 
 `mypy_boto3_rds_data.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rds_data.type_defs import (
+    ArrayValueOutputTypeDef,
     ArrayValueTypeDef,
+    ResponseMetadataTypeDef,
     BeginTransactionRequestRequestTypeDef,
-    BeginTransactionResponseTypeDef,
     ColumnMetadataTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     ExecuteSqlRequestRequestTypeDef,
     ResultSetOptionsTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
     RecordTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTransactionRequestRequestTypeDef,
-    RollbackTransactionResponseTypeDef,
     StructValueTypeDef,
     ValueTypeDef,
+    BeginTransactionResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    RollbackTransactionResponseTypeDef,
     ResultSetMetadataTypeDef,
     ExecuteStatementResponseTypeDef,
-    SqlParameterTypeDef,
     UpdateResultTypeDef,
+    SqlParameterTypeDef,
     ResultFrameTypeDef,
+    BatchExecuteStatementResponseTypeDef,
     BatchExecuteStatementRequestRequestTypeDef,
     ExecuteStatementRequestRequestTypeDef,
-    BatchExecuteStatementResponseTypeDef,
     SqlStatementResultTypeDef,
     ExecuteSqlResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayValueTypeDef:
+def get_structure() -> ArrayValueOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rds-data-1.28.0/README.md` & `mypy-boto3-rds-data-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rds-data"></a>
 
 # mypy-boto3-rds-data
 
 [![PyPI - mypy-boto3-rds-data](https://img.shields.io/pypi/v/mypy-boto3-rds-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rds-data?color=blue)](https://pypistats.org/packages/mypy-boto3-rds-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds-data)](https://pepy.tech/project/mypy-boto3-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDSDataService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[boto3.RDSDataService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rds-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,43 +267,45 @@
 ### Typed dictionaries
 
 `mypy_boto3_rds_data.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rds_data.type_defs import (
+    ArrayValueOutputTypeDef,
     ArrayValueTypeDef,
+    ResponseMetadataTypeDef,
     BeginTransactionRequestRequestTypeDef,
-    BeginTransactionResponseTypeDef,
     ColumnMetadataTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     ExecuteSqlRequestRequestTypeDef,
     ResultSetOptionsTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
     RecordTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTransactionRequestRequestTypeDef,
-    RollbackTransactionResponseTypeDef,
     StructValueTypeDef,
     ValueTypeDef,
+    BeginTransactionResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    RollbackTransactionResponseTypeDef,
     ResultSetMetadataTypeDef,
     ExecuteStatementResponseTypeDef,
-    SqlParameterTypeDef,
     UpdateResultTypeDef,
+    SqlParameterTypeDef,
     ResultFrameTypeDef,
+    BatchExecuteStatementResponseTypeDef,
     BatchExecuteStatementRequestRequestTypeDef,
     ExecuteStatementRequestRequestTypeDef,
-    BatchExecuteStatementResponseTypeDef,
     SqlStatementResultTypeDef,
     ExecuteSqlResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayValueTypeDef:
+def get_structure() -> ArrayValueOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/__main__.py` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RDSDataService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.RDSDataService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/client.py` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/client.pyi` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/literals.py` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -237,26 +238,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/literals.pyi` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -235,26 +236,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/type_defs.py` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,72 +2,96 @@
 Type annotations for rds-data service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rds_data.type_defs import ArrayValueTypeDef
+    from mypy_boto3_rds_data.type_defs import ArrayValueOutputTypeDef
 
-    data: ArrayValueTypeDef = {...}
+    data: ArrayValueOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import DecimalReturnTypeType, LongReturnTypeType, RecordsFormatTypeType, TypeHintType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "ArrayValueOutputTypeDef",
     "ArrayValueTypeDef",
+    "ResponseMetadataTypeDef",
     "BeginTransactionRequestRequestTypeDef",
-    "BeginTransactionResponseTypeDef",
     "ColumnMetadataTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "ExecuteSqlRequestRequestTypeDef",
     "ResultSetOptionsTypeDef",
+    "FieldOutputTypeDef",
     "FieldTypeDef",
     "RecordTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTransactionRequestRequestTypeDef",
-    "RollbackTransactionResponseTypeDef",
     "StructValueTypeDef",
     "ValueTypeDef",
+    "BeginTransactionResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "RollbackTransactionResponseTypeDef",
     "ResultSetMetadataTypeDef",
     "ExecuteStatementResponseTypeDef",
-    "SqlParameterTypeDef",
     "UpdateResultTypeDef",
+    "SqlParameterTypeDef",
     "ResultFrameTypeDef",
+    "BatchExecuteStatementResponseTypeDef",
     "BatchExecuteStatementRequestRequestTypeDef",
     "ExecuteStatementRequestRequestTypeDef",
-    "BatchExecuteStatementResponseTypeDef",
     "SqlStatementResultTypeDef",
     "ExecuteSqlResponseTypeDef",
 )
 
+ArrayValueOutputTypeDef = TypedDict(
+    "ArrayValueOutputTypeDef",
+    {
+        "booleanValues": List[bool],
+        "longValues": List[int],
+        "doubleValues": List[float],
+        "stringValues": List[str],
+        "arrayValues": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 ArrayValueTypeDef = TypedDict(
     "ArrayValueTypeDef",
     {
         "booleanValues": Sequence[bool],
         "longValues": Sequence[int],
         "doubleValues": Sequence[float],
         "stringValues": Sequence[str],
         "arrayValues": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredBeginTransactionRequestRequestTypeDef = TypedDict(
     "_RequiredBeginTransactionRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
     },
 )
@@ -76,29 +100,19 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
-
 class BeginTransactionRequestRequestTypeDef(
     _RequiredBeginTransactionRequestRequestTypeDef, _OptionalBeginTransactionRequestRequestTypeDef
 ):
     pass
 
-
-BeginTransactionResponseTypeDef = TypedDict(
-    "BeginTransactionResponseTypeDef",
-    {
-        "transactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "name": str,
         "type": int,
         "typeName": str,
         "label": str,
@@ -121,22 +135,14 @@
     {
         "resourceArn": str,
         "secretArn": str,
         "transactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "transactionStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteSqlRequestRequestTypeDef = TypedDict(
     "_RequiredExecuteSqlRequestRequestTypeDef",
     {
         "dbClusterOrInstanceArn": str,
         "awsSecretStoreArn": str,
         "sqlStatements": str,
     },
@@ -146,30 +152,42 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
-
 class ExecuteSqlRequestRequestTypeDef(
     _RequiredExecuteSqlRequestRequestTypeDef, _OptionalExecuteSqlRequestRequestTypeDef
 ):
     pass
 
-
 ResultSetOptionsTypeDef = TypedDict(
     "ResultSetOptionsTypeDef",
     {
         "decimalReturnType": DecimalReturnTypeType,
         "longReturnType": LongReturnTypeType,
     },
     total=False,
 )
 
+FieldOutputTypeDef = TypedDict(
+    "FieldOutputTypeDef",
+    {
+        "isNull": bool,
+        "booleanValue": bool,
+        "longValue": int,
+        "doubleValue": float,
+        "stringValue": str,
+        "blobValue": bytes,
+        "arrayValue": "ArrayValueOutputTypeDef",
+    },
+    total=False,
+)
+
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "isNull": bool,
         "booleanValue": bool,
         "longValue": int,
         "doubleValue": float,
@@ -184,42 +202,23 @@
     "RecordTypeDef",
     {
         "values": List["ValueTypeDef"],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RollbackTransactionRequestRequestTypeDef = TypedDict(
     "RollbackTransactionRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "transactionId": str,
     },
 )
 
-RollbackTransactionResponseTypeDef = TypedDict(
-    "RollbackTransactionResponseTypeDef",
-    {
-        "transactionStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StructValueTypeDef = TypedDict(
     "StructValueTypeDef",
     {
         "attributes": List["ValueTypeDef"],
     },
     total=False,
 )
@@ -237,62 +236,94 @@
         "blobValue": bytes,
         "arrayValues": List[Dict[str, Any]],
         "structValue": Dict[str, Any],
     },
     total=False,
 )
 
+BeginTransactionResponseTypeDef = TypedDict(
+    "BeginTransactionResponseTypeDef",
+    {
+        "transactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
+    {
+        "transactionStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackTransactionResponseTypeDef = TypedDict(
+    "RollbackTransactionResponseTypeDef",
+    {
+        "transactionStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "columnCount": int,
         "columnMetadata": List[ColumnMetadataTypeDef],
     },
     total=False,
 )
 
 ExecuteStatementResponseTypeDef = TypedDict(
     "ExecuteStatementResponseTypeDef",
     {
-        "records": List[List[FieldTypeDef]],
+        "records": List[List[FieldOutputTypeDef]],
         "columnMetadata": List[ColumnMetadataTypeDef],
         "numberOfRecordsUpdated": int,
-        "generatedFields": List[FieldTypeDef],
+        "generatedFields": List[FieldOutputTypeDef],
         "formattedRecords": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SqlParameterTypeDef = TypedDict(
-    "SqlParameterTypeDef",
+UpdateResultTypeDef = TypedDict(
+    "UpdateResultTypeDef",
     {
-        "name": str,
-        "value": FieldTypeDef,
-        "typeHint": TypeHintType,
+        "generatedFields": List[FieldOutputTypeDef],
     },
     total=False,
 )
 
-UpdateResultTypeDef = TypedDict(
-    "UpdateResultTypeDef",
+SqlParameterTypeDef = TypedDict(
+    "SqlParameterTypeDef",
     {
-        "generatedFields": List[FieldTypeDef],
+        "name": str,
+        "value": FieldTypeDef,
+        "typeHint": TypeHintType,
     },
     total=False,
 )
 
 ResultFrameTypeDef = TypedDict(
     "ResultFrameTypeDef",
     {
         "resultSetMetadata": ResultSetMetadataTypeDef,
         "records": List[RecordTypeDef],
     },
     total=False,
 )
 
+BatchExecuteStatementResponseTypeDef = TypedDict(
+    "BatchExecuteStatementResponseTypeDef",
+    {
+        "updateResults": List[UpdateResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "sql": str,
     },
@@ -304,22 +335,20 @@
         "schema": str,
         "parameterSets": Sequence[Sequence[SqlParameterTypeDef]],
         "transactionId": str,
     },
     total=False,
 )
 
-
 class BatchExecuteStatementRequestRequestTypeDef(
     _RequiredBatchExecuteStatementRequestRequestTypeDef,
     _OptionalBatchExecuteStatementRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "sql": str,
     },
@@ -335,38 +364,28 @@
         "continueAfterTimeout": bool,
         "resultSetOptions": ResultSetOptionsTypeDef,
         "formatRecordsAs": RecordsFormatTypeType,
     },
     total=False,
 )
 
-
 class ExecuteStatementRequestRequestTypeDef(
     _RequiredExecuteStatementRequestRequestTypeDef, _OptionalExecuteStatementRequestRequestTypeDef
 ):
     pass
 
-
-BatchExecuteStatementResponseTypeDef = TypedDict(
-    "BatchExecuteStatementResponseTypeDef",
-    {
-        "updateResults": List[UpdateResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SqlStatementResultTypeDef = TypedDict(
     "SqlStatementResultTypeDef",
     {
         "resultFrame": ResultFrameTypeDef,
         "numberOfRecordsUpdated": int,
     },
     total=False,
 )
 
 ExecuteSqlResponseTypeDef = TypedDict(
     "ExecuteSqlResponseTypeDef",
     {
         "sqlStatementResults": List[SqlStatementResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data/type_defs.pyi` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,71 +2,97 @@
 Type annotations for rds-data service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rds_data.type_defs import ArrayValueTypeDef
+    from mypy_boto3_rds_data.type_defs import ArrayValueOutputTypeDef
 
-    data: ArrayValueTypeDef = {...}
+    data: ArrayValueOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import DecimalReturnTypeType, LongReturnTypeType, RecordsFormatTypeType, TypeHintType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "ArrayValueOutputTypeDef",
     "ArrayValueTypeDef",
+    "ResponseMetadataTypeDef",
     "BeginTransactionRequestRequestTypeDef",
-    "BeginTransactionResponseTypeDef",
     "ColumnMetadataTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "ExecuteSqlRequestRequestTypeDef",
     "ResultSetOptionsTypeDef",
+    "FieldOutputTypeDef",
     "FieldTypeDef",
     "RecordTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTransactionRequestRequestTypeDef",
-    "RollbackTransactionResponseTypeDef",
     "StructValueTypeDef",
     "ValueTypeDef",
+    "BeginTransactionResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "RollbackTransactionResponseTypeDef",
     "ResultSetMetadataTypeDef",
     "ExecuteStatementResponseTypeDef",
-    "SqlParameterTypeDef",
     "UpdateResultTypeDef",
+    "SqlParameterTypeDef",
     "ResultFrameTypeDef",
+    "BatchExecuteStatementResponseTypeDef",
     "BatchExecuteStatementRequestRequestTypeDef",
     "ExecuteStatementRequestRequestTypeDef",
-    "BatchExecuteStatementResponseTypeDef",
     "SqlStatementResultTypeDef",
     "ExecuteSqlResponseTypeDef",
 )
 
+ArrayValueOutputTypeDef = TypedDict(
+    "ArrayValueOutputTypeDef",
+    {
+        "booleanValues": List[bool],
+        "longValues": List[int],
+        "doubleValues": List[float],
+        "stringValues": List[str],
+        "arrayValues": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 ArrayValueTypeDef = TypedDict(
     "ArrayValueTypeDef",
     {
         "booleanValues": Sequence[bool],
         "longValues": Sequence[int],
         "doubleValues": Sequence[float],
         "stringValues": Sequence[str],
         "arrayValues": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredBeginTransactionRequestRequestTypeDef = TypedDict(
     "_RequiredBeginTransactionRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
     },
 )
@@ -75,26 +101,20 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
+
 class BeginTransactionRequestRequestTypeDef(
     _RequiredBeginTransactionRequestRequestTypeDef, _OptionalBeginTransactionRequestRequestTypeDef
 ):
     pass
 
-BeginTransactionResponseTypeDef = TypedDict(
-    "BeginTransactionResponseTypeDef",
-    {
-        "transactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "name": str,
         "type": int,
         "typeName": str,
@@ -118,22 +138,14 @@
     {
         "resourceArn": str,
         "secretArn": str,
         "transactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "transactionStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteSqlRequestRequestTypeDef = TypedDict(
     "_RequiredExecuteSqlRequestRequestTypeDef",
     {
         "dbClusterOrInstanceArn": str,
         "awsSecretStoreArn": str,
         "sqlStatements": str,
     },
@@ -143,28 +155,44 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
+
 class ExecuteSqlRequestRequestTypeDef(
     _RequiredExecuteSqlRequestRequestTypeDef, _OptionalExecuteSqlRequestRequestTypeDef
 ):
     pass
 
+
 ResultSetOptionsTypeDef = TypedDict(
     "ResultSetOptionsTypeDef",
     {
         "decimalReturnType": DecimalReturnTypeType,
         "longReturnType": LongReturnTypeType,
     },
     total=False,
 )
 
+FieldOutputTypeDef = TypedDict(
+    "FieldOutputTypeDef",
+    {
+        "isNull": bool,
+        "booleanValue": bool,
+        "longValue": int,
+        "doubleValue": float,
+        "stringValue": str,
+        "blobValue": bytes,
+        "arrayValue": "ArrayValueOutputTypeDef",
+    },
+    total=False,
+)
+
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "isNull": bool,
         "booleanValue": bool,
         "longValue": int,
         "doubleValue": float,
@@ -179,42 +207,23 @@
     "RecordTypeDef",
     {
         "values": List["ValueTypeDef"],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RollbackTransactionRequestRequestTypeDef = TypedDict(
     "RollbackTransactionRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "transactionId": str,
     },
 )
 
-RollbackTransactionResponseTypeDef = TypedDict(
-    "RollbackTransactionResponseTypeDef",
-    {
-        "transactionStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StructValueTypeDef = TypedDict(
     "StructValueTypeDef",
     {
         "attributes": List["ValueTypeDef"],
     },
     total=False,
 )
@@ -232,62 +241,94 @@
         "blobValue": bytes,
         "arrayValues": List[Dict[str, Any]],
         "structValue": Dict[str, Any],
     },
     total=False,
 )
 
+BeginTransactionResponseTypeDef = TypedDict(
+    "BeginTransactionResponseTypeDef",
+    {
+        "transactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
+    {
+        "transactionStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackTransactionResponseTypeDef = TypedDict(
+    "RollbackTransactionResponseTypeDef",
+    {
+        "transactionStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "columnCount": int,
         "columnMetadata": List[ColumnMetadataTypeDef],
     },
     total=False,
 )
 
 ExecuteStatementResponseTypeDef = TypedDict(
     "ExecuteStatementResponseTypeDef",
     {
-        "records": List[List[FieldTypeDef]],
+        "records": List[List[FieldOutputTypeDef]],
         "columnMetadata": List[ColumnMetadataTypeDef],
         "numberOfRecordsUpdated": int,
-        "generatedFields": List[FieldTypeDef],
+        "generatedFields": List[FieldOutputTypeDef],
         "formattedRecords": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SqlParameterTypeDef = TypedDict(
-    "SqlParameterTypeDef",
+UpdateResultTypeDef = TypedDict(
+    "UpdateResultTypeDef",
     {
-        "name": str,
-        "value": FieldTypeDef,
-        "typeHint": TypeHintType,
+        "generatedFields": List[FieldOutputTypeDef],
     },
     total=False,
 )
 
-UpdateResultTypeDef = TypedDict(
-    "UpdateResultTypeDef",
+SqlParameterTypeDef = TypedDict(
+    "SqlParameterTypeDef",
     {
-        "generatedFields": List[FieldTypeDef],
+        "name": str,
+        "value": FieldTypeDef,
+        "typeHint": TypeHintType,
     },
     total=False,
 )
 
 ResultFrameTypeDef = TypedDict(
     "ResultFrameTypeDef",
     {
         "resultSetMetadata": ResultSetMetadataTypeDef,
         "records": List[RecordTypeDef],
     },
     total=False,
 )
 
+BatchExecuteStatementResponseTypeDef = TypedDict(
+    "BatchExecuteStatementResponseTypeDef",
+    {
+        "updateResults": List[UpdateResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "sql": str,
     },
@@ -299,20 +340,22 @@
         "schema": str,
         "parameterSets": Sequence[Sequence[SqlParameterTypeDef]],
         "transactionId": str,
     },
     total=False,
 )
 
+
 class BatchExecuteStatementRequestRequestTypeDef(
     _RequiredBatchExecuteStatementRequestRequestTypeDef,
     _OptionalBatchExecuteStatementRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "sql": str,
     },
@@ -328,36 +371,30 @@
         "continueAfterTimeout": bool,
         "resultSetOptions": ResultSetOptionsTypeDef,
         "formatRecordsAs": RecordsFormatTypeType,
     },
     total=False,
 )
 
+
 class ExecuteStatementRequestRequestTypeDef(
     _RequiredExecuteStatementRequestRequestTypeDef, _OptionalExecuteStatementRequestRequestTypeDef
 ):
     pass
 
-BatchExecuteStatementResponseTypeDef = TypedDict(
-    "BatchExecuteStatementResponseTypeDef",
-    {
-        "updateResults": List[UpdateResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SqlStatementResultTypeDef = TypedDict(
     "SqlStatementResultTypeDef",
     {
         "resultFrame": ResultFrameTypeDef,
         "numberOfRecordsUpdated": int,
     },
     total=False,
 )
 
 ExecuteSqlResponseTypeDef = TypedDict(
     "ExecuteSqlResponseTypeDef",
     {
         "sqlStatementResults": List[SqlStatementResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/PKG-INFO` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds-data
-Version: 1.28.0
-Summary: Type annotations for boto3.RDSDataService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RDSDataService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rds-data"></a>
 
 # mypy-boto3-rds-data
 
 [![PyPI - mypy-boto3-rds-data](https://img.shields.io/pypi/v/mypy-boto3-rds-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rds-data?color=blue)](https://pypistats.org/packages/mypy-boto3-rds-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds-data)](https://pepy.tech/project/mypy-boto3-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDSDataService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[boto3.RDSDataService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rds-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,43 +299,45 @@
 ### Typed dictionaries
 
 `mypy_boto3_rds_data.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rds_data.type_defs import (
+    ArrayValueOutputTypeDef,
     ArrayValueTypeDef,
+    ResponseMetadataTypeDef,
     BeginTransactionRequestRequestTypeDef,
-    BeginTransactionResponseTypeDef,
     ColumnMetadataTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     ExecuteSqlRequestRequestTypeDef,
     ResultSetOptionsTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
     RecordTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTransactionRequestRequestTypeDef,
-    RollbackTransactionResponseTypeDef,
     StructValueTypeDef,
     ValueTypeDef,
+    BeginTransactionResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    RollbackTransactionResponseTypeDef,
     ResultSetMetadataTypeDef,
     ExecuteStatementResponseTypeDef,
-    SqlParameterTypeDef,
     UpdateResultTypeDef,
+    SqlParameterTypeDef,
     ResultFrameTypeDef,
+    BatchExecuteStatementResponseTypeDef,
     BatchExecuteStatementRequestRequestTypeDef,
     ExecuteStatementRequestRequestTypeDef,
-    BatchExecuteStatementResponseTypeDef,
     SqlStatementResultTypeDef,
     ExecuteSqlResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayValueTypeDef:
+def get_structure() -> ArrayValueOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rds-data-1.28.0/mypy_boto3_rds_data.egg-info/SOURCES.txt` & `mypy-boto3-rds-data-1.28.12/mypy_boto3_rds_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-data-1.28.0/setup.py` & `mypy-boto3-rds-data-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rds-data",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_rds_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RDSDataService 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.RDSDataService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

