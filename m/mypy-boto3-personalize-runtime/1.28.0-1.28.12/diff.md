# Comparing `tmp/mypy-boto3-personalize-runtime-1.28.0.tar.gz` & `tmp/mypy-boto3-personalize-runtime-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-runtime-1.28.0.tar", last modified: Thu Jul  6 21:00:18 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-runtime-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-personalize-runtime-1.28.0.tar` & `mypy-boto3-personalize-runtime-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.689160 mypy-boto3-personalize-runtime-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-07-27 11:49:24.681160 mypy-boto3-personalize-runtime-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11119 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.673160 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.681160 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-07-27 11:49:24.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 11:49:24.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:24.000000 mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.689160 mypy-boto3-personalize-runtime-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 11:41:20.000000 mypy-boto3-personalize-runtime-1.28.12/setup.py
```

### Comparing `mypy-boto3-personalize-runtime-1.28.0/LICENSE` & `mypy-boto3-personalize-runtime-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.28.0/PKG-INFO` & `mypy-boto3-personalize-runtime-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.PersonalizeRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PersonalizeRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-personalize-runtime"></a>
 
 # mypy-boto3-personalize-runtime
 
 [![PyPI - mypy-boto3-personalize-runtime](https://img.shields.io/pypi/v/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-runtime)](https://pepy.tech/project/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
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
 [mypy-boto3-personalize-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,16 +298,16 @@
 `mypy_boto3_personalize_runtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_runtime.type_defs import (
     GetPersonalizedRankingRequestRequestTypeDef,
     PredictedItemTypeDef,
-    PromotionTypeDef,
     ResponseMetadataTypeDef,
+    PromotionTypeDef,
     GetPersonalizedRankingResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetPersonalizedRankingRequestRequestTypeDef:
```

### Comparing `mypy-boto3-personalize-runtime-1.28.0/README.md` & `mypy-boto3-personalize-runtime-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-personalize-runtime"></a>
 
 # mypy-boto3-personalize-runtime
 
 [![PyPI - mypy-boto3-personalize-runtime](https://img.shields.io/pypi/v/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-runtime)](https://pepy.tech/project/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
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
 [mypy-boto3-personalize-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,16 +266,16 @@
 `mypy_boto3_personalize_runtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_runtime.type_defs import (
     GetPersonalizedRankingRequestRequestTypeDef,
     PredictedItemTypeDef,
-    PromotionTypeDef,
     ResponseMetadataTypeDef,
+    PromotionTypeDef,
     GetPersonalizedRankingResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetPersonalizedRankingRequestRequestTypeDef:
```

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__main__.py` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PersonalizeRuntime 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PersonalizeRuntime 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime\nOther"
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

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.py` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.pyi` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.py` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/literals.py`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.pyi` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/literals.pyi`

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

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.py` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "GetPersonalizedRankingRequestRequestTypeDef",
     "PredictedItemTypeDef",
-    "PromotionTypeDef",
     "ResponseMetadataTypeDef",
+    "PromotionTypeDef",
     "GetPersonalizedRankingResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
 )
 
 _RequiredGetPersonalizedRankingRequestRequestTypeDef = TypedDict(
     "_RequiredGetPersonalizedRankingRequestRequestTypeDef",
@@ -62,51 +62,51 @@
         "itemId": str,
         "score": float,
         "promotionName": str,
     },
     total=False,
 )
 
-PromotionTypeDef = TypedDict(
-    "PromotionTypeDef",
-    {
-        "name": str,
-        "percentPromotedItems": int,
-        "filterArn": str,
-        "filterValues": Mapping[str, str],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+PromotionTypeDef = TypedDict(
+    "PromotionTypeDef",
+    {
+        "name": str,
+        "percentPromotedItems": int,
+        "filterArn": str,
+        "filterValues": Mapping[str, str],
+    },
+    total=False,
+)
+
 GetPersonalizedRankingResponseTypeDef = TypedDict(
     "GetPersonalizedRankingResponseTypeDef",
     {
         "personalizedRanking": List[PredictedItemTypeDef],
         "recommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "itemList": List[PredictedItemTypeDef],
         "recommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsRequestRequestTypeDef = TypedDict(
     "GetRecommendationsRequestRequestTypeDef",
     {
         "campaignArn": str,
```

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.pyi` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "GetPersonalizedRankingRequestRequestTypeDef",
     "PredictedItemTypeDef",
-    "PromotionTypeDef",
     "ResponseMetadataTypeDef",
+    "PromotionTypeDef",
     "GetPersonalizedRankingResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
 )
 
 _RequiredGetPersonalizedRankingRequestRequestTypeDef = TypedDict(
     "_RequiredGetPersonalizedRankingRequestRequestTypeDef",
@@ -59,51 +59,51 @@
         "itemId": str,
         "score": float,
         "promotionName": str,
     },
     total=False,
 )
 
-PromotionTypeDef = TypedDict(
-    "PromotionTypeDef",
-    {
-        "name": str,
-        "percentPromotedItems": int,
-        "filterArn": str,
-        "filterValues": Mapping[str, str],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+PromotionTypeDef = TypedDict(
+    "PromotionTypeDef",
+    {
+        "name": str,
+        "percentPromotedItems": int,
+        "filterArn": str,
+        "filterValues": Mapping[str, str],
+    },
+    total=False,
+)
+
 GetPersonalizedRankingResponseTypeDef = TypedDict(
     "GetPersonalizedRankingResponseTypeDef",
     {
         "personalizedRanking": List[PredictedItemTypeDef],
         "recommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "itemList": List[PredictedItemTypeDef],
         "recommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsRequestRequestTypeDef = TypedDict(
     "GetRecommendationsRequestRequestTypeDef",
     {
         "campaignArn": str,
```

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/PKG-INFO` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.PersonalizeRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PersonalizeRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-personalize-runtime"></a>
 
 # mypy-boto3-personalize-runtime
 
 [![PyPI - mypy-boto3-personalize-runtime](https://img.shields.io/pypi/v/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-runtime)](https://pepy.tech/project/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
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
 [mypy-boto3-personalize-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,16 +298,16 @@
 `mypy_boto3_personalize_runtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_runtime.type_defs import (
     GetPersonalizedRankingRequestRequestTypeDef,
     PredictedItemTypeDef,
-    PromotionTypeDef,
     ResponseMetadataTypeDef,
+    PromotionTypeDef,
     GetPersonalizedRankingResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetPersonalizedRankingRequestRequestTypeDef:
```

### Comparing `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt` & `mypy-boto3-personalize-runtime-1.28.12/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.28.0/setup.py` & `mypy-boto3-personalize-runtime-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize-runtime",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_personalize_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PersonalizeRuntime 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.PersonalizeRuntime 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

