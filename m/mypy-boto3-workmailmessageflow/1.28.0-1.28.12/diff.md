# Comparing `tmp/mypy-boto3-workmailmessageflow-1.28.0.tar.gz` & `tmp/mypy-boto3-workmailmessageflow-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workmailmessageflow-1.28.0.tar", last modified: Thu Jul  6 21:00:52 2023, max compression
+gzip compressed data, was "mypy-boto3-workmailmessageflow-1.28.12.tar", last modified: Thu Jul 27 11:49:50 2023, max compression
```

## Comparing `mypy-boto3-workmailmessageflow-1.28.0.tar` & `mypy-boto3-workmailmessageflow-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.894462 mypy-boto3-workmailmessageflow-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-07-06 21:00:52.894462 mypy-boto3-workmailmessageflow-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.890462 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.894462 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-07-06 21:00:52.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 21:00:52.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:52.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:52.000000 mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:52.894462 mypy-boto3-workmailmessageflow-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 20:58:17.000000 mypy-boto3-workmailmessageflow-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.937505 mypy-boto3-workmailmessageflow-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-27 11:49:50.937505 mypy-boto3-workmailmessageflow-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.937505 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.937505 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-27 11:49:50.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 11:49:50.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:50.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:50.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:50.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:50.000000 mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:50.937505 mypy-boto3-workmailmessageflow-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-27 11:48:57.000000 mypy-boto3-workmailmessageflow-1.28.12/setup.py
```

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/LICENSE` & `mypy-boto3-workmailmessageflow-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/PKG-INFO` & `mypy-boto3-workmailmessageflow-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmailmessageflow
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkMailMessageFlow 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkMailMessageFlow 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workmailmessageflow"></a>
 
 # mypy-boto3-workmailmessageflow
 
 [![PyPI - mypy-boto3-workmailmessageflow](https://img.shields.io/pypi/v/mypy-boto3-workmailmessageflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmailmessageflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmailmessageflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmailmessageflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workmailmessageflow?color=blue)](https://pypistats.org/packages/mypy-boto3-workmailmessageflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmailmessageflow)](https://pepy.tech/project/mypy-boto3-workmailmessageflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMailMessageFlow 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
+[boto3.WorkMailMessageFlow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
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
 [mypy-boto3-workmailmessageflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,17 +297,17 @@
 
 `mypy_boto3_workmailmessageflow.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workmailmessageflow.type_defs import (
     GetRawMessageContentRequestRequestTypeDef,
-    GetRawMessageContentResponseTypeDef,
-    S3ReferenceTypeDef,
     ResponseMetadataTypeDef,
+    S3ReferenceTypeDef,
+    GetRawMessageContentResponseTypeDef,
     RawMessageContentTypeDef,
     PutRawMessageContentRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRawMessageContentRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/README.md` & `mypy-boto3-workmailmessageflow-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workmailmessageflow"></a>
 
 # mypy-boto3-workmailmessageflow
 
 [![PyPI - mypy-boto3-workmailmessageflow](https://img.shields.io/pypi/v/mypy-boto3-workmailmessageflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmailmessageflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmailmessageflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmailmessageflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workmailmessageflow?color=blue)](https://pypistats.org/packages/mypy-boto3-workmailmessageflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmailmessageflow)](https://pepy.tech/project/mypy-boto3-workmailmessageflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMailMessageFlow 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
+[boto3.WorkMailMessageFlow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
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
 [mypy-boto3-workmailmessageflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,17 +265,17 @@
 
 `mypy_boto3_workmailmessageflow.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workmailmessageflow.type_defs import (
     GetRawMessageContentRequestRequestTypeDef,
-    GetRawMessageContentResponseTypeDef,
-    S3ReferenceTypeDef,
     ResponseMetadataTypeDef,
+    S3ReferenceTypeDef,
+    GetRawMessageContentResponseTypeDef,
     RawMessageContentTypeDef,
     PutRawMessageContentRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRawMessageContentRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/__main__.py` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkMailMessageFlow 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.WorkMailMessageFlow 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow\nOther"
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

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/client.py` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/client.pyi` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/literals.py` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
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
@@ -224,26 +225,28 @@
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

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/literals.pyi` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
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
@@ -222,26 +223,28 @@
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

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/type_defs.py` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,33 +20,36 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "GetRawMessageContentRequestRequestTypeDef",
-    "GetRawMessageContentResponseTypeDef",
-    "S3ReferenceTypeDef",
     "ResponseMetadataTypeDef",
+    "S3ReferenceTypeDef",
+    "GetRawMessageContentResponseTypeDef",
     "RawMessageContentTypeDef",
     "PutRawMessageContentRequestRequestTypeDef",
 )
 
 GetRawMessageContentRequestRequestTypeDef = TypedDict(
     "GetRawMessageContentRequestRequestTypeDef",
     {
         "messageId": str,
     },
 )
 
-GetRawMessageContentResponseTypeDef = TypedDict(
-    "GetRawMessageContentResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "messageContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredS3ReferenceTypeDef = TypedDict(
     "_RequiredS3ReferenceTypeDef",
     {
         "bucket": str,
@@ -62,22 +65,19 @@
 )
 
 
 class S3ReferenceTypeDef(_RequiredS3ReferenceTypeDef, _OptionalS3ReferenceTypeDef):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetRawMessageContentResponseTypeDef = TypedDict(
+    "GetRawMessageContentResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "messageContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RawMessageContentTypeDef = TypedDict(
     "RawMessageContentTypeDef",
     {
         "s3Reference": S3ReferenceTypeDef,
```

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow/type_defs.pyi` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,33 +19,36 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "GetRawMessageContentRequestRequestTypeDef",
-    "GetRawMessageContentResponseTypeDef",
-    "S3ReferenceTypeDef",
     "ResponseMetadataTypeDef",
+    "S3ReferenceTypeDef",
+    "GetRawMessageContentResponseTypeDef",
     "RawMessageContentTypeDef",
     "PutRawMessageContentRequestRequestTypeDef",
 )
 
 GetRawMessageContentRequestRequestTypeDef = TypedDict(
     "GetRawMessageContentRequestRequestTypeDef",
     {
         "messageId": str,
     },
 )
 
-GetRawMessageContentResponseTypeDef = TypedDict(
-    "GetRawMessageContentResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "messageContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredS3ReferenceTypeDef = TypedDict(
     "_RequiredS3ReferenceTypeDef",
     {
         "bucket": str,
@@ -59,22 +62,19 @@
     },
     total=False,
 )
 
 class S3ReferenceTypeDef(_RequiredS3ReferenceTypeDef, _OptionalS3ReferenceTypeDef):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetRawMessageContentResponseTypeDef = TypedDict(
+    "GetRawMessageContentResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "messageContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RawMessageContentTypeDef = TypedDict(
     "RawMessageContentTypeDef",
     {
         "s3Reference": S3ReferenceTypeDef,
```

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/PKG-INFO` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmailmessageflow
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkMailMessageFlow 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkMailMessageFlow 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workmailmessageflow"></a>
 
 # mypy-boto3-workmailmessageflow
 
 [![PyPI - mypy-boto3-workmailmessageflow](https://img.shields.io/pypi/v/mypy-boto3-workmailmessageflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmailmessageflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmailmessageflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmailmessageflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workmailmessageflow?color=blue)](https://pypistats.org/packages/mypy-boto3-workmailmessageflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmailmessageflow)](https://pepy.tech/project/mypy-boto3-workmailmessageflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMailMessageFlow 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
+[boto3.WorkMailMessageFlow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
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
 [mypy-boto3-workmailmessageflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmailmessageflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,17 +297,17 @@
 
 `mypy_boto3_workmailmessageflow.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workmailmessageflow.type_defs import (
     GetRawMessageContentRequestRequestTypeDef,
-    GetRawMessageContentResponseTypeDef,
-    S3ReferenceTypeDef,
     ResponseMetadataTypeDef,
+    S3ReferenceTypeDef,
+    GetRawMessageContentResponseTypeDef,
     RawMessageContentTypeDef,
     PutRawMessageContentRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRawMessageContentRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/mypy_boto3_workmailmessageflow.egg-info/SOURCES.txt` & `mypy-boto3-workmailmessageflow-1.28.12/mypy_boto3_workmailmessageflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmailmessageflow-1.28.0/setup.py` & `mypy-boto3-workmailmessageflow-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workmailmessageflow",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_workmailmessageflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkMailMessageFlow 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.WorkMailMessageFlow 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

