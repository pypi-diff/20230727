# Comparing `tmp/mypy-boto3-lex-runtime-1.28.0.tar.gz` & `tmp/mypy-boto3-lex-runtime-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-runtime-1.28.0.tar", last modified: Thu Jul  6 20:59:57 2023, max compression
+gzip compressed data, was "mypy-boto3-lex-runtime-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
```

## Comparing `mypy-boto3-lex-runtime-1.28.0.tar` & `mypy-boto3-lex-runtime-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.842350 mypy-boto3-lex-runtime-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-06 20:59:57.838350 mypy-boto3-lex-runtime-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.830350 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-06 20:45:18.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.838350 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-06 20:59:57.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 20:59:57.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:57.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:57.000000 mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:57.842350 mypy-boto3-lex-runtime-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:45:17.000000 mypy-boto3-lex-runtime-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/setup.py
```

### Comparing `mypy-boto3-lex-runtime-1.28.0/LICENSE` & `mypy-boto3-lex-runtime-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.0/PKG-INFO` & `mypy-boto3-lex-runtime-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.LexRuntimeService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LexRuntimeService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lex-runtime"></a>
 
 # mypy-boto3-lex-runtime
 
 [![PyPI - mypy-boto3-lex-runtime](https://img.shields.io/pypi/v/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,39 +302,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
+    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
     DeleteSessionResponseTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
+    IntentSummaryTypeDef,
     PostContentRequestRequestTypeDef,
     PostContentResponseTypeDef,
     SentimentResponseTypeDef,
     PutSessionResponseTypeDef,
     ResponseMetadataTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_structure() -> ActiveContextTimeToLiveOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.0/README.md` & `mypy-boto3-lex-runtime-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lex-runtime"></a>
 
 # mypy-boto3-lex-runtime
 
 [![PyPI - mypy-boto3-lex-runtime](https://img.shields.io/pypi/v/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,39 +270,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
+    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
     DeleteSessionResponseTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
+    IntentSummaryTypeDef,
     PostContentRequestRequestTypeDef,
     PostContentResponseTypeDef,
     SentimentResponseTypeDef,
     PutSessionResponseTypeDef,
     ResponseMetadataTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_structure() -> ActiveContextTimeToLiveOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/__main__.py` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexRuntimeService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LexRuntimeService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/client.py` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/client.pyi` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/literals.py` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
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
@@ -243,26 +244,28 @@
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

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/literals.pyi` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
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
@@ -241,26 +242,28 @@
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

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/type_defs.py` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
+    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveOutputTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -31,37 +31,50 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ActiveContextTimeToLiveOutputTypeDef",
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "DeleteSessionResponseTypeDef",
+    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentSummaryTypeDef",
+    "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
+    "IntentSummaryTypeDef",
     "PostContentRequestRequestTypeDef",
     "PostContentResponseTypeDef",
     "SentimentResponseTypeDef",
     "PutSessionResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "GenericAttachmentTypeDef",
     "PredictedIntentTypeDef",
     "GetSessionResponseTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
     "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
+ActiveContextTimeToLiveOutputTypeDef = TypedDict(
+    "ActiveContextTimeToLiveOutputTypeDef",
+    {
+        "timeToLiveInSeconds": int,
+        "turnsToLive": int,
+    },
+    total=False,
+)
+
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
@@ -91,25 +104,51 @@
         "botAlias": str,
         "userId": str,
         "sessionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDialogActionOutputTypeDef = TypedDict(
+    "_RequiredDialogActionOutputTypeDef",
+    {
+        "type": DialogActionTypeType,
+    },
+)
+_OptionalDialogActionOutputTypeDef = TypedDict(
+    "_OptionalDialogActionOutputTypeDef",
+    {
+        "intentName": str,
+        "slots": Dict[str, str],
+        "slotToElicit": str,
+        "fulfillmentState": FulfillmentStateType,
+        "message": str,
+        "messageFormat": MessageFormatTypeType,
+    },
+    total=False,
+)
+
+
+class DialogActionOutputTypeDef(
+    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
+):
+    pass
+
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
     "_OptionalDialogActionTypeDef",
     {
         "intentName": str,
-        "slots": Dict[str, str],
+        "slots": Mapping[str, str],
         "slotToElicit": str,
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
@@ -138,46 +177,72 @@
 
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredIntentSummaryTypeDef = TypedDict(
-    "_RequiredIntentSummaryTypeDef",
+_RequiredIntentSummaryOutputTypeDef = TypedDict(
+    "_RequiredIntentSummaryOutputTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
-_OptionalIntentSummaryTypeDef = TypedDict(
-    "_OptionalIntentSummaryTypeDef",
+_OptionalIntentSummaryOutputTypeDef = TypedDict(
+    "_OptionalIntentSummaryOutputTypeDef",
     {
         "intentName": str,
         "checkpointLabel": str,
         "slots": Dict[str, str],
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
 
-class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
+class IntentSummaryOutputTypeDef(
+    _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
+):
     pass
 
 
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
+_RequiredIntentSummaryTypeDef = TypedDict(
+    "_RequiredIntentSummaryTypeDef",
+    {
+        "dialogActionType": DialogActionTypeType,
+    },
+)
+_OptionalIntentSummaryTypeDef = TypedDict(
+    "_OptionalIntentSummaryTypeDef",
+    {
+        "intentName": str,
+        "checkpointLabel": str,
+        "slots": Mapping[str, str],
+        "confirmationStatus": ConfirmationStatusType,
+        "fulfillmentState": FulfillmentStateType,
+        "slotToElicit": str,
+    },
+    total=False,
+)
+
+
+class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
+    pass
+
+
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "contentType": str,
@@ -262,20 +327,29 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveOutputTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
+        "parameters": Mapping[str, str],
     },
 )
 
 GenericAttachmentTypeDef = TypedDict(
     "GenericAttachmentTypeDef",
     {
         "title": str,
@@ -296,19 +370,19 @@
     },
     total=False,
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
-        "recentIntentSummaryView": List[IntentSummaryTypeDef],
+        "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
-        "dialogAction": DialogActionTypeDef,
-        "activeContexts": List[ActiveContextTypeDef],
+        "dialogAction": DialogActionOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
@@ -384,11 +458,11 @@
         "sentimentResponse": SentimentResponseTypeDef,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
-        "activeContexts": List[ActiveContextTypeDef],
+        "activeContexts": List[ActiveContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime/type_defs.pyi` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
+    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveOutputTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -30,37 +30,50 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ActiveContextTimeToLiveOutputTypeDef",
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "DeleteSessionResponseTypeDef",
+    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentSummaryTypeDef",
+    "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
+    "IntentSummaryTypeDef",
     "PostContentRequestRequestTypeDef",
     "PostContentResponseTypeDef",
     "SentimentResponseTypeDef",
     "PutSessionResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "GenericAttachmentTypeDef",
     "PredictedIntentTypeDef",
     "GetSessionResponseTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
     "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
+ActiveContextTimeToLiveOutputTypeDef = TypedDict(
+    "ActiveContextTimeToLiveOutputTypeDef",
+    {
+        "timeToLiveInSeconds": int,
+        "turnsToLive": int,
+    },
+    total=False,
+)
+
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
@@ -90,25 +103,49 @@
         "botAlias": str,
         "userId": str,
         "sessionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDialogActionOutputTypeDef = TypedDict(
+    "_RequiredDialogActionOutputTypeDef",
+    {
+        "type": DialogActionTypeType,
+    },
+)
+_OptionalDialogActionOutputTypeDef = TypedDict(
+    "_OptionalDialogActionOutputTypeDef",
+    {
+        "intentName": str,
+        "slots": Dict[str, str],
+        "slotToElicit": str,
+        "fulfillmentState": FulfillmentStateType,
+        "message": str,
+        "messageFormat": MessageFormatTypeType,
+    },
+    total=False,
+)
+
+class DialogActionOutputTypeDef(
+    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
+):
+    pass
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
     "_OptionalDialogActionTypeDef",
     {
         "intentName": str,
-        "slots": Dict[str, str],
+        "slots": Mapping[str, str],
         "slotToElicit": str,
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
@@ -133,44 +170,68 @@
 )
 
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-_RequiredIntentSummaryTypeDef = TypedDict(
-    "_RequiredIntentSummaryTypeDef",
+_RequiredIntentSummaryOutputTypeDef = TypedDict(
+    "_RequiredIntentSummaryOutputTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
-_OptionalIntentSummaryTypeDef = TypedDict(
-    "_OptionalIntentSummaryTypeDef",
+_OptionalIntentSummaryOutputTypeDef = TypedDict(
+    "_OptionalIntentSummaryOutputTypeDef",
     {
         "intentName": str,
         "checkpointLabel": str,
         "slots": Dict[str, str],
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
+class IntentSummaryOutputTypeDef(
+    _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
+):
     pass
 
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
+_RequiredIntentSummaryTypeDef = TypedDict(
+    "_RequiredIntentSummaryTypeDef",
+    {
+        "dialogActionType": DialogActionTypeType,
+    },
+)
+_OptionalIntentSummaryTypeDef = TypedDict(
+    "_OptionalIntentSummaryTypeDef",
+    {
+        "intentName": str,
+        "checkpointLabel": str,
+        "slots": Mapping[str, str],
+        "confirmationStatus": ConfirmationStatusType,
+        "fulfillmentState": FulfillmentStateType,
+        "slotToElicit": str,
+    },
+    total=False,
+)
+
+class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
+    pass
+
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "contentType": str,
@@ -253,20 +314,29 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveOutputTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
+        "parameters": Mapping[str, str],
     },
 )
 
 GenericAttachmentTypeDef = TypedDict(
     "GenericAttachmentTypeDef",
     {
         "title": str,
@@ -287,19 +357,19 @@
     },
     total=False,
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
-        "recentIntentSummaryView": List[IntentSummaryTypeDef],
+        "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
-        "dialogAction": DialogActionTypeDef,
-        "activeContexts": List[ActiveContextTypeDef],
+        "dialogAction": DialogActionOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
@@ -371,11 +441,11 @@
         "sentimentResponse": SentimentResponseTypeDef,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
-        "activeContexts": List[ActiveContextTypeDef],
+        "activeContexts": List[ActiveContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/PKG-INFO` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.LexRuntimeService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LexRuntimeService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lex-runtime"></a>
 
 # mypy-boto3-lex-runtime
 
 [![PyPI - mypy-boto3-lex-runtime](https://img.shields.io/pypi/v/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,39 +302,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
+    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
     DeleteSessionResponseTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
+    IntentSummaryTypeDef,
     PostContentRequestRequestTypeDef,
     PostContentResponseTypeDef,
     SentimentResponseTypeDef,
     PutSessionResponseTypeDef,
     ResponseMetadataTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_structure() -> ActiveContextTimeToLiveOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.0/mypy_boto3_lex_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.0/setup.py` & `mypy-boto3-lex-runtime-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-runtime",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.LexRuntimeService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

