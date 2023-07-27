# Comparing `tmp/mypy-boto3-sagemaker-runtime-1.28.0.tar.gz` & `tmp/mypy-boto3-sagemaker-runtime-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-runtime-1.28.0.tar", last modified: Thu Jul  6 21:00:33 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-runtime-1.28.12.tar", last modified: Thu Jul 27 11:49:35 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-runtime-1.28.0.tar` & `mypy-boto3-sagemaker-runtime-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.322422 mypy-boto3-sagemaker-runtime-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-06 21:00:33.310422 mypy-boto3-sagemaker-runtime-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.306422 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-07-06 20:54:55.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-06 20:54:55.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-06 20:54:55.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-06 20:54:55.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.310422 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-06 21:00:33.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 21:00:33.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:33.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:33.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:33.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 21:00:33.000000 mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:33.322422 mypy-boto3-sagemaker-runtime-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-runtime-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.873265 mypy-boto3-sagemaker-runtime-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-07-27 11:49:35.869265 mypy-boto3-sagemaker-runtime-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.869265 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:00.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.869265 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:35.873265 mypy-boto3-sagemaker-runtime-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-runtime-1.28.12/setup.py
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/LICENSE` & `mypy-boto3-sagemaker-runtime-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/PKG-INFO` & `mypy-boto3-sagemaker-runtime-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakerRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SageMakerRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-runtime"></a>
 
 # mypy-boto3-sagemaker-runtime
 
 [![PyPI - mypy-boto3-sagemaker-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,18 +298,18 @@
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
     InvokeEndpointAsyncInputRequestTypeDef,
-    InvokeEndpointAsyncOutputTypeDef,
+    ResponseMetadataTypeDef,
     InvokeEndpointInputRequestTypeDef,
+    InvokeEndpointAsyncOutputTypeDef,
     InvokeEndpointOutputTypeDef,
-    ResponseMetadataTypeDef,
 )
 
 
 def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/README.md` & `mypy-boto3-sagemaker-runtime-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-runtime"></a>
 
 # mypy-boto3-sagemaker-runtime
 
 [![PyPI - mypy-boto3-sagemaker-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,18 +266,18 @@
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
     InvokeEndpointAsyncInputRequestTypeDef,
-    InvokeEndpointAsyncOutputTypeDef,
+    ResponseMetadataTypeDef,
     InvokeEndpointInputRequestTypeDef,
+    InvokeEndpointAsyncOutputTypeDef,
     InvokeEndpointOutputTypeDef,
-    ResponseMetadataTypeDef,
 )
 
 
 def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/__main__.py` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerRuntime 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SageMakerRuntime 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime\nOther"
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

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/client.py` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/client.pyi` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/literals.py` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/literals.py`

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

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/literals.pyi` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/literals.pyi`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/type_defs.py` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "InvokeEndpointAsyncInputRequestTypeDef",
-    "InvokeEndpointAsyncOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "InvokeEndpointInputRequestTypeDef",
+    "InvokeEndpointAsyncOutputTypeDef",
     "InvokeEndpointOutputTypeDef",
-    "ResponseMetadataTypeDef",
 )
 
 _RequiredInvokeEndpointAsyncInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointAsyncInputRequestTypeDef",
     {
         "EndpointName": str,
         "InputLocation": str,
@@ -53,21 +53,22 @@
 
 class InvokeEndpointAsyncInputRequestTypeDef(
     _RequiredInvokeEndpointAsyncInputRequestTypeDef, _OptionalInvokeEndpointAsyncInputRequestTypeDef
 ):
     pass
 
 
-InvokeEndpointAsyncOutputTypeDef = TypedDict(
-    "InvokeEndpointAsyncOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "InferenceId": str,
-        "OutputLocation": str,
-        "FailureLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredInvokeEndpointInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
@@ -92,28 +93,27 @@
 
 class InvokeEndpointInputRequestTypeDef(
     _RequiredInvokeEndpointInputRequestTypeDef, _OptionalInvokeEndpointInputRequestTypeDef
 ):
     pass
 
 
+InvokeEndpointAsyncOutputTypeDef = TypedDict(
+    "InvokeEndpointAsyncOutputTypeDef",
+    {
+        "InferenceId": str,
+        "OutputLocation": str,
+        "FailureLocation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 InvokeEndpointOutputTypeDef = TypedDict(
     "InvokeEndpointOutputTypeDef",
     {
         "Body": StreamingBody,
         "ContentType": str,
         "InvokedProductionVariant": str,
         "CustomAttributes": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "InvokeEndpointAsyncInputRequestTypeDef",
-    "InvokeEndpointAsyncOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "InvokeEndpointInputRequestTypeDef",
+    "InvokeEndpointAsyncOutputTypeDef",
     "InvokeEndpointOutputTypeDef",
-    "ResponseMetadataTypeDef",
 )
 
 _RequiredInvokeEndpointAsyncInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointAsyncInputRequestTypeDef",
     {
         "EndpointName": str,
         "InputLocation": str,
@@ -50,21 +50,22 @@
 )
 
 class InvokeEndpointAsyncInputRequestTypeDef(
     _RequiredInvokeEndpointAsyncInputRequestTypeDef, _OptionalInvokeEndpointAsyncInputRequestTypeDef
 ):
     pass
 
-InvokeEndpointAsyncOutputTypeDef = TypedDict(
-    "InvokeEndpointAsyncOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "InferenceId": str,
-        "OutputLocation": str,
-        "FailureLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredInvokeEndpointInputRequestTypeDef = TypedDict(
     "_RequiredInvokeEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
@@ -87,28 +88,27 @@
 )
 
 class InvokeEndpointInputRequestTypeDef(
     _RequiredInvokeEndpointInputRequestTypeDef, _OptionalInvokeEndpointInputRequestTypeDef
 ):
     pass
 
+InvokeEndpointAsyncOutputTypeDef = TypedDict(
+    "InvokeEndpointAsyncOutputTypeDef",
+    {
+        "InferenceId": str,
+        "OutputLocation": str,
+        "FailureLocation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 InvokeEndpointOutputTypeDef = TypedDict(
     "InvokeEndpointOutputTypeDef",
     {
         "Body": StreamingBody,
         "ContentType": str,
         "InvokedProductionVariant": str,
         "CustomAttributes": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakerRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SageMakerRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-runtime"></a>
 
 # mypy-boto3-sagemaker-runtime
 
 [![PyPI - mypy-boto3-sagemaker-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
+[boto3.SageMakerRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
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
 [mypy-boto3-sagemaker-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,18 +298,18 @@
 
 `mypy_boto3_sagemaker_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_runtime.type_defs import (
     InvokeEndpointAsyncInputRequestTypeDef,
-    InvokeEndpointAsyncOutputTypeDef,
+    ResponseMetadataTypeDef,
     InvokeEndpointInputRequestTypeDef,
+    InvokeEndpointAsyncOutputTypeDef,
     InvokeEndpointOutputTypeDef,
-    ResponseMetadataTypeDef,
 )
 
 
 def get_structure() -> InvokeEndpointAsyncInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-runtime-1.28.12/mypy_boto3_sagemaker_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-runtime-1.28.0/setup.py` & `mypy-boto3-sagemaker-runtime-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-runtime",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sagemaker_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerRuntime 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SageMakerRuntime 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

