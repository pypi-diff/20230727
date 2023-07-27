# Comparing `tmp/mypy-boto3-m2-1.28.12.tar.gz` & `tmp/mypy-boto3-m2-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-m2-1.28.12.tar", last modified: Thu Jul 27 05:34:58 2023, max compression
+gzip compressed data, was "mypy-boto3-m2-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-m2-1.28.12.tar` & `mypy-boto3-m2-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.160452 mypy-boto3-m2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-07-27 05:34:58.160452 mypy-boto3-m2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.160452 mypy-boto3-m2-1.28.12/mypy_boto3_m2/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27910 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45398 2023-07-27 05:25:41.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45324 2023-07-27 05:25:41.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.160452 mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-07-27 05:34:58.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 05:34:58.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:58.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 05:34:58.000000 mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:58.160452 mypy-boto3-m2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-27 05:25:40.000000 mypy-boto3-m2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/mypy_boto3_m2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27910 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42524 2023-07-18 19:32:27.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42470 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-18 19:32:24.000000 mypy-boto3-m2-1.28.5/setup.py
```

### Comparing `mypy-boto3-m2-1.28.12/LICENSE` & `mypy-boto3-m2-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/PKG-INFO` & `mypy-boto3-m2-1.28.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.28.12
-Summary: Type annotations for boto3.MainframeModernization 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.MainframeModernization 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-m2-1.28.12/README.md` & `mypy-boto3-m2-1.28.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/__init__.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/__init__.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/__main__.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MainframeModernization 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MainframeModernization 1.28.5\nVersion:         1.28.5\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/client.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/client.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/literals.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -289,28 +288,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/literals.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -287,28 +286,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/paginator.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/paginator.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/type_defs.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlternateKeyOutputTypeDef",
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
@@ -150,37 +149,24 @@
     "GetDataSetDetailsResponseTypeDef",
     "DataSetTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
-_RequiredAlternateKeyOutputTypeDef = TypedDict(
-    "_RequiredAlternateKeyOutputTypeDef",
-    {
-        "length": int,
-        "offset": int,
-    },
-)
-_OptionalAlternateKeyOutputTypeDef = TypedDict(
-    "_OptionalAlternateKeyOutputTypeDef",
+AlternateKeyOutputTypeDef = TypedDict(
+    "AlternateKeyOutputTypeDef",
     {
         "allowDuplicates": bool,
+        "length": int,
         "name": str,
+        "offset": int,
     },
-    total=False,
 )
 
-
-class AlternateKeyOutputTypeDef(
-    _RequiredAlternateKeyOutputTypeDef, _OptionalAlternateKeyOutputTypeDef
-):
-    pass
-
-
 _RequiredAlternateKeyTypeDef = TypedDict(
     "_RequiredAlternateKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -189,123 +175,69 @@
     {
         "allowDuplicates": bool,
         "name": str,
     },
     total=False,
 )
 
-
 class AlternateKeyTypeDef(_RequiredAlternateKeyTypeDef, _OptionalAlternateKeyTypeDef):
     pass
 
-
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "applicationArn": str,
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
-        "engineType": EngineTypeType,
-        "name": str,
-        "status": ApplicationLifecycleType,
-    },
-)
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
-    {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
+        "engineType": EngineTypeType,
         "environmentId": str,
         "lastStartTime": datetime,
+        "name": str,
         "roleArn": str,
+        "status": ApplicationLifecycleType,
         "versionStatus": ApplicationVersionLifecycleType,
     },
-    total=False,
 )
 
-
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
-
-
-_RequiredApplicationVersionSummaryTypeDef = TypedDict(
-    "_RequiredApplicationVersionSummaryTypeDef",
+ApplicationVersionSummaryTypeDef = TypedDict(
+    "ApplicationVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "creationTime": datetime,
         "status": ApplicationVersionLifecycleType,
-    },
-)
-_OptionalApplicationVersionSummaryTypeDef = TypedDict(
-    "_OptionalApplicationVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-
-class ApplicationVersionSummaryTypeDef(
-    _RequiredApplicationVersionSummaryTypeDef, _OptionalApplicationVersionSummaryTypeDef
-):
-    pass
-
-
-_RequiredFileBatchJobDefinitionTypeDef = TypedDict(
-    "_RequiredFileBatchJobDefinitionTypeDef",
+FileBatchJobDefinitionTypeDef = TypedDict(
+    "FileBatchJobDefinitionTypeDef",
     {
         "fileName": str,
-    },
-)
-_OptionalFileBatchJobDefinitionTypeDef = TypedDict(
-    "_OptionalFileBatchJobDefinitionTypeDef",
-    {
         "folderPath": str,
     },
-    total=False,
 )
 
-
-class FileBatchJobDefinitionTypeDef(
-    _RequiredFileBatchJobDefinitionTypeDef, _OptionalFileBatchJobDefinitionTypeDef
-):
-    pass
-
-
 ScriptBatchJobDefinitionTypeDef = TypedDict(
     "ScriptBatchJobDefinitionTypeDef",
     {
         "scriptName": str,
     },
 )
 
-_RequiredFileBatchJobIdentifierOutputTypeDef = TypedDict(
-    "_RequiredFileBatchJobIdentifierOutputTypeDef",
+FileBatchJobIdentifierOutputTypeDef = TypedDict(
+    "FileBatchJobIdentifierOutputTypeDef",
     {
         "fileName": str,
-    },
-)
-_OptionalFileBatchJobIdentifierOutputTypeDef = TypedDict(
-    "_OptionalFileBatchJobIdentifierOutputTypeDef",
-    {
         "folderPath": str,
     },
-    total=False,
 )
 
-
-class FileBatchJobIdentifierOutputTypeDef(
-    _RequiredFileBatchJobIdentifierOutputTypeDef, _OptionalFileBatchJobIdentifierOutputTypeDef
-):
-    pass
-
-
 ScriptBatchJobIdentifierOutputTypeDef = TypedDict(
     "ScriptBatchJobIdentifierOutputTypeDef",
     {
         "scriptName": str,
     },
 )
 
@@ -319,21 +251,19 @@
     "_OptionalFileBatchJobIdentifierTypeDef",
     {
         "folderPath": str,
     },
     total=False,
 )
 
-
 class FileBatchJobIdentifierTypeDef(
     _RequiredFileBatchJobIdentifierTypeDef, _OptionalFileBatchJobIdentifierTypeDef
 ):
     pass
 
-
 ScriptBatchJobIdentifierTypeDef = TypedDict(
     "ScriptBatchJobIdentifierTypeDef",
     {
         "scriptName": str,
     },
 )
 
@@ -384,21 +314,19 @@
     "_OptionalCreateDeploymentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
 CreateDeploymentResponseTypeDef = TypedDict(
     "CreateDeploymentResponseTypeDef",
     {
         "deploymentId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -433,52 +361,40 @@
         "inProgress": int,
         "pending": int,
         "succeeded": int,
         "total": int,
     },
 )
 
-_RequiredDataSetSummaryTypeDef = TypedDict(
-    "_RequiredDataSetSummaryTypeDef",
-    {
-        "dataSetName": str,
-    },
-)
-_OptionalDataSetSummaryTypeDef = TypedDict(
-    "_OptionalDataSetSummaryTypeDef",
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
     {
         "creationTime": datetime,
+        "dataSetName": str,
         "dataSetOrg": str,
         "format": str,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
     },
-    total=False,
 )
 
-
-class DataSetSummaryTypeDef(_RequiredDataSetSummaryTypeDef, _OptionalDataSetSummaryTypeDef):
-    pass
-
-
 RecordLengthTypeDef = TypedDict(
     "RecordLengthTypeDef",
     {
         "max": int,
         "min": int,
     },
 )
 
 GdgDetailAttributesTypeDef = TypedDict(
     "GdgDetailAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
-    total=False,
 )
 
 PoDetailAttributesTypeDef = TypedDict(
     "PoDetailAttributesTypeDef",
     {
         "encoding": str,
         "format": str,
@@ -513,38 +429,34 @@
     "_OptionalPoAttributesTypeDef",
     {
         "encoding": str,
     },
     total=False,
 )
 
-
 class PoAttributesTypeDef(_RequiredPoAttributesTypeDef, _OptionalPoAttributesTypeDef):
     pass
 
-
 _RequiredPsAttributesTypeDef = TypedDict(
     "_RequiredPsAttributesTypeDef",
     {
         "format": str,
     },
 )
 _OptionalPsAttributesTypeDef = TypedDict(
     "_OptionalPsAttributesTypeDef",
     {
         "encoding": str,
     },
     total=False,
 )
 
-
 class PsAttributesTypeDef(_RequiredPsAttributesTypeDef, _OptionalPsAttributesTypeDef):
     pass
 
-
 DeleteApplicationFromEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     {
         "applicationId": str,
         "environmentId": str,
     },
 )
@@ -559,62 +471,36 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredDeployedVersionSummaryTypeDef = TypedDict(
-    "_RequiredDeployedVersionSummaryTypeDef",
+DeployedVersionSummaryTypeDef = TypedDict(
+    "DeployedVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeployedVersionSummaryTypeDef = TypedDict(
-    "_OptionalDeployedVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-
-class DeployedVersionSummaryTypeDef(
-    _RequiredDeployedVersionSummaryTypeDef, _OptionalDeployedVersionSummaryTypeDef
-):
-    pass
-
-
-_RequiredDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeploymentSummaryTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
         "environmentId": str,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeploymentSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-
-class DeploymentSummaryTypeDef(
-    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
-):
-    pass
-
-
 EfsStorageConfigurationOutputTypeDef = TypedDict(
     "EfsStorageConfigurationOutputTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -780,22 +666,20 @@
     "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
     _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -803,22 +687,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "environmentId": str,
         "names": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -847,22 +729,20 @@
     {
         "prefix": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
     _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -871,22 +751,20 @@
         "maxResults": int,
         "nextToken": str,
         "prefix": str,
     },
     total=False,
 )
 
-
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
@@ -898,22 +776,20 @@
         "startedBefore": Union[datetime, str],
         "status": BatchJobExecutionStatusType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
     _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
     _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
@@ -926,44 +802,40 @@
         "startedAfter": Union[datetime, str],
         "startedBefore": Union[datetime, str],
         "status": BatchJobExecutionStatusType,
     },
     total=False,
 )
 
-
 class ListBatchJobExecutionsRequestRequestTypeDef(
     _RequiredListBatchJobExecutionsRequestRequestTypeDef,
     _OptionalListBatchJobExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
     "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
     _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -971,22 +843,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
     "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
@@ -994,22 +864,20 @@
     {
         "prefix": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDataSetsRequestListDataSetsPaginateTypeDef(
     _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
     _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -1018,43 +886,39 @@
         "maxResults": int,
         "nextToken": str,
         "prefix": str,
     },
     total=False,
 )
 
-
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
     "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
     _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
     _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1062,21 +926,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
-
 ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
     "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     {
         "engineType": EngineTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1130,47 +992,35 @@
 
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredPrimaryKeyOutputTypeDef = TypedDict(
-    "_RequiredPrimaryKeyOutputTypeDef",
+PrimaryKeyOutputTypeDef = TypedDict(
+    "PrimaryKeyOutputTypeDef",
     {
         "length": int,
-        "offset": int,
-    },
-)
-_OptionalPrimaryKeyOutputTypeDef = TypedDict(
-    "_OptionalPrimaryKeyOutputTypeDef",
-    {
         "name": str,
+        "offset": int,
     },
-    total=False,
 )
 
-
-class PrimaryKeyOutputTypeDef(_RequiredPrimaryKeyOutputTypeDef, _OptionalPrimaryKeyOutputTypeDef):
-    pass
-
-
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -1178,19 +1028,17 @@
     "_OptionalPrimaryKeyTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -1223,21 +1071,19 @@
     "_OptionalStopApplicationRequestRequestTypeDef",
     {
         "forceStop": bool,
     },
     total=False,
 )
 
-
 class StopApplicationRequestRequestTypeDef(
     _RequiredStopApplicationRequestRequestTypeDef, _OptionalStopApplicationRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1272,21 +1118,19 @@
         "engineVersion": str,
         "instanceType": str,
         "preferredMaintenanceWindow": str,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environmentId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1311,24 +1155,22 @@
 
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
-    total=False,
 )
 
 BatchJobIdentifierOutputTypeDef = TypedDict(
     "BatchJobIdentifierOutputTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierOutputTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierOutputTypeDef,
     },
-    total=False,
 )
 
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierTypeDef,
@@ -1352,21 +1194,19 @@
         "kmsKeyId": str,
         "roleArn": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "currentApplicationVersion": int,
     },
 )
@@ -1375,21 +1215,19 @@
     {
         "definition": DefinitionTypeDef,
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1443,15 +1281,14 @@
 
 StorageConfigurationOutputTypeDef = TypedDict(
     "StorageConfigurationOutputTypeDef",
     {
         "efs": EfsStorageConfigurationOutputTypeDef,
         "fsx": FsxStorageConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
         "fsx": FsxStorageConfigurationTypeDef,
@@ -1488,28 +1325,26 @@
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
-    total=False,
 )
 
 VsamDetailAttributesTypeDef = TypedDict(
     "VsamDetailAttributesTypeDef",
     {
         "alternateKeys": List[AlternateKeyOutputTypeDef],
         "cacheAtStartup": bool,
         "compressed": bool,
         "encoding": str,
         "primaryKey": PrimaryKeyOutputTypeDef,
         "recordFormat": str,
     },
-    total=False,
 )
 
 _RequiredVsamAttributesTypeDef = TypedDict(
     "_RequiredVsamAttributesTypeDef",
     {
         "format": str,
     },
@@ -1521,57 +1356,42 @@
         "compressed": bool,
         "encoding": str,
         "primaryKey": PrimaryKeyTypeDef,
     },
     total=False,
 )
 
-
 class VsamAttributesTypeDef(_RequiredVsamAttributesTypeDef, _OptionalVsamAttributesTypeDef):
     pass
 
-
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
+BatchJobExecutionSummaryTypeDef = TypedDict(
+    "BatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
         "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
+        "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
     },
-    total=False,
 )
 
-
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
-
 GetBatchJobExecutionResponseTypeDef = TypedDict(
     "GetBatchJobExecutionResponseTypeDef",
     {
         "applicationId": str,
         "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
         "executionId": str,
@@ -1598,21 +1418,19 @@
     "_OptionalStartBatchJobRequestRequestTypeDef",
     {
         "jobParams": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartBatchJobRequestRequestTypeDef(
     _RequiredStartBatchJobRequestRequestTypeDef, _OptionalStartBatchJobRequestRequestTypeDef
 ):
     pass
 
-
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1640,21 +1458,19 @@
         "storageConfigurations": Sequence[StorageConfigurationTypeDef],
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "actualCapacity": int,
         "creationTime": datetime,
         "description": str,
         "engineType": EngineTypeType,
@@ -1684,15 +1500,14 @@
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
         "po": PoDetailAttributesTypeDef,
         "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
-    total=False,
 )
 
 DatasetOrgAttributesTypeDef = TypedDict(
     "DatasetOrgAttributesTypeDef",
     {
         "gdg": GdgAttributesTypeDef,
         "po": PoAttributesTypeDef,
@@ -1739,19 +1554,17 @@
     {
         "relativePath": str,
         "storageType": str,
     },
     total=False,
 )
 
-
 class DataSetTypeDef(_RequiredDataSetTypeDef, _OptionalDataSetTypeDef):
     pass
 
-
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
         "externalLocation": ExternalLocationTypeDef,
     },
 )
@@ -1776,13 +1589,12 @@
     "_OptionalCreateDataSetImportTaskRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateDataSetImportTaskRequestRequestTypeDef(
     _RequiredCreateDataSetImportTaskRequestRequestTypeDef,
     _OptionalCreateDataSetImportTaskRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2/type_defs.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlternateKeyOutputTypeDef",
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
@@ -149,35 +150,24 @@
     "GetDataSetDetailsResponseTypeDef",
     "DataSetTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
-_RequiredAlternateKeyOutputTypeDef = TypedDict(
-    "_RequiredAlternateKeyOutputTypeDef",
-    {
-        "length": int,
-        "offset": int,
-    },
-)
-_OptionalAlternateKeyOutputTypeDef = TypedDict(
-    "_OptionalAlternateKeyOutputTypeDef",
+AlternateKeyOutputTypeDef = TypedDict(
+    "AlternateKeyOutputTypeDef",
     {
         "allowDuplicates": bool,
+        "length": int,
         "name": str,
+        "offset": int,
     },
-    total=False,
 )
 
-class AlternateKeyOutputTypeDef(
-    _RequiredAlternateKeyOutputTypeDef, _OptionalAlternateKeyOutputTypeDef
-):
-    pass
-
 _RequiredAlternateKeyTypeDef = TypedDict(
     "_RequiredAlternateKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -186,113 +176,71 @@
     {
         "allowDuplicates": bool,
         "name": str,
     },
     total=False,
 )
 
+
 class AlternateKeyTypeDef(_RequiredAlternateKeyTypeDef, _OptionalAlternateKeyTypeDef):
     pass
 
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "applicationArn": str,
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
-        "engineType": EngineTypeType,
-        "name": str,
-        "status": ApplicationLifecycleType,
-    },
-)
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
-    {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
+        "engineType": EngineTypeType,
         "environmentId": str,
         "lastStartTime": datetime,
+        "name": str,
         "roleArn": str,
+        "status": ApplicationLifecycleType,
         "versionStatus": ApplicationVersionLifecycleType,
     },
-    total=False,
 )
 
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
-
-_RequiredApplicationVersionSummaryTypeDef = TypedDict(
-    "_RequiredApplicationVersionSummaryTypeDef",
+ApplicationVersionSummaryTypeDef = TypedDict(
+    "ApplicationVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "creationTime": datetime,
         "status": ApplicationVersionLifecycleType,
-    },
-)
-_OptionalApplicationVersionSummaryTypeDef = TypedDict(
-    "_OptionalApplicationVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-class ApplicationVersionSummaryTypeDef(
-    _RequiredApplicationVersionSummaryTypeDef, _OptionalApplicationVersionSummaryTypeDef
-):
-    pass
-
-_RequiredFileBatchJobDefinitionTypeDef = TypedDict(
-    "_RequiredFileBatchJobDefinitionTypeDef",
+FileBatchJobDefinitionTypeDef = TypedDict(
+    "FileBatchJobDefinitionTypeDef",
     {
         "fileName": str,
-    },
-)
-_OptionalFileBatchJobDefinitionTypeDef = TypedDict(
-    "_OptionalFileBatchJobDefinitionTypeDef",
-    {
         "folderPath": str,
     },
-    total=False,
 )
 
-class FileBatchJobDefinitionTypeDef(
-    _RequiredFileBatchJobDefinitionTypeDef, _OptionalFileBatchJobDefinitionTypeDef
-):
-    pass
-
 ScriptBatchJobDefinitionTypeDef = TypedDict(
     "ScriptBatchJobDefinitionTypeDef",
     {
         "scriptName": str,
     },
 )
 
-_RequiredFileBatchJobIdentifierOutputTypeDef = TypedDict(
-    "_RequiredFileBatchJobIdentifierOutputTypeDef",
+FileBatchJobIdentifierOutputTypeDef = TypedDict(
+    "FileBatchJobIdentifierOutputTypeDef",
     {
         "fileName": str,
-    },
-)
-_OptionalFileBatchJobIdentifierOutputTypeDef = TypedDict(
-    "_OptionalFileBatchJobIdentifierOutputTypeDef",
-    {
         "folderPath": str,
     },
-    total=False,
 )
 
-class FileBatchJobIdentifierOutputTypeDef(
-    _RequiredFileBatchJobIdentifierOutputTypeDef, _OptionalFileBatchJobIdentifierOutputTypeDef
-):
-    pass
-
 ScriptBatchJobIdentifierOutputTypeDef = TypedDict(
     "ScriptBatchJobIdentifierOutputTypeDef",
     {
         "scriptName": str,
     },
 )
 
@@ -306,19 +254,21 @@
     "_OptionalFileBatchJobIdentifierTypeDef",
     {
         "folderPath": str,
     },
     total=False,
 )
 
+
 class FileBatchJobIdentifierTypeDef(
     _RequiredFileBatchJobIdentifierTypeDef, _OptionalFileBatchJobIdentifierTypeDef
 ):
     pass
 
+
 ScriptBatchJobIdentifierTypeDef = TypedDict(
     "ScriptBatchJobIdentifierTypeDef",
     {
         "scriptName": str,
     },
 )
 
@@ -369,19 +319,21 @@
     "_OptionalCreateDeploymentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+
 CreateDeploymentResponseTypeDef = TypedDict(
     "CreateDeploymentResponseTypeDef",
     {
         "deploymentId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -416,50 +368,40 @@
         "inProgress": int,
         "pending": int,
         "succeeded": int,
         "total": int,
     },
 )
 
-_RequiredDataSetSummaryTypeDef = TypedDict(
-    "_RequiredDataSetSummaryTypeDef",
-    {
-        "dataSetName": str,
-    },
-)
-_OptionalDataSetSummaryTypeDef = TypedDict(
-    "_OptionalDataSetSummaryTypeDef",
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
     {
         "creationTime": datetime,
+        "dataSetName": str,
         "dataSetOrg": str,
         "format": str,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
     },
-    total=False,
 )
 
-class DataSetSummaryTypeDef(_RequiredDataSetSummaryTypeDef, _OptionalDataSetSummaryTypeDef):
-    pass
-
 RecordLengthTypeDef = TypedDict(
     "RecordLengthTypeDef",
     {
         "max": int,
         "min": int,
     },
 )
 
 GdgDetailAttributesTypeDef = TypedDict(
     "GdgDetailAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
-    total=False,
 )
 
 PoDetailAttributesTypeDef = TypedDict(
     "PoDetailAttributesTypeDef",
     {
         "encoding": str,
         "format": str,
@@ -494,34 +436,38 @@
     "_OptionalPoAttributesTypeDef",
     {
         "encoding": str,
     },
     total=False,
 )
 
+
 class PoAttributesTypeDef(_RequiredPoAttributesTypeDef, _OptionalPoAttributesTypeDef):
     pass
 
+
 _RequiredPsAttributesTypeDef = TypedDict(
     "_RequiredPsAttributesTypeDef",
     {
         "format": str,
     },
 )
 _OptionalPsAttributesTypeDef = TypedDict(
     "_OptionalPsAttributesTypeDef",
     {
         "encoding": str,
     },
     total=False,
 )
 
+
 class PsAttributesTypeDef(_RequiredPsAttributesTypeDef, _OptionalPsAttributesTypeDef):
     pass
 
+
 DeleteApplicationFromEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     {
         "applicationId": str,
         "environmentId": str,
     },
 )
@@ -536,58 +482,36 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredDeployedVersionSummaryTypeDef = TypedDict(
-    "_RequiredDeployedVersionSummaryTypeDef",
+DeployedVersionSummaryTypeDef = TypedDict(
+    "DeployedVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeployedVersionSummaryTypeDef = TypedDict(
-    "_OptionalDeployedVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-class DeployedVersionSummaryTypeDef(
-    _RequiredDeployedVersionSummaryTypeDef, _OptionalDeployedVersionSummaryTypeDef
-):
-    pass
-
-_RequiredDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeploymentSummaryTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
         "environmentId": str,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeploymentSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-class DeploymentSummaryTypeDef(
-    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
-):
-    pass
-
 EfsStorageConfigurationOutputTypeDef = TypedDict(
     "EfsStorageConfigurationOutputTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -753,20 +677,22 @@
     "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
     _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -774,20 +700,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "environmentId": str,
         "names": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -816,20 +744,22 @@
     {
         "prefix": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
     _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -838,20 +768,22 @@
         "maxResults": int,
         "nextToken": str,
         "prefix": str,
     },
     total=False,
 )
 
+
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
@@ -863,20 +795,22 @@
         "startedBefore": Union[datetime, str],
         "status": BatchJobExecutionStatusType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
     _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
     _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
@@ -889,40 +823,44 @@
         "startedAfter": Union[datetime, str],
         "startedBefore": Union[datetime, str],
         "status": BatchJobExecutionStatusType,
     },
     total=False,
 )
 
+
 class ListBatchJobExecutionsRequestRequestTypeDef(
     _RequiredListBatchJobExecutionsRequestRequestTypeDef,
     _OptionalListBatchJobExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
     "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
     _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -930,20 +868,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
     "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
@@ -951,20 +891,22 @@
     {
         "prefix": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDataSetsRequestListDataSetsPaginateTypeDef(
     _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
     _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -973,39 +915,43 @@
         "maxResults": int,
         "nextToken": str,
         "prefix": str,
     },
     total=False,
 )
 
+
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
     "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
     _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
     _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1013,19 +959,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
+
 ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
     "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     {
         "engineType": EngineTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1079,45 +1027,35 @@
 
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredPrimaryKeyOutputTypeDef = TypedDict(
-    "_RequiredPrimaryKeyOutputTypeDef",
+PrimaryKeyOutputTypeDef = TypedDict(
+    "PrimaryKeyOutputTypeDef",
     {
         "length": int,
-        "offset": int,
-    },
-)
-_OptionalPrimaryKeyOutputTypeDef = TypedDict(
-    "_OptionalPrimaryKeyOutputTypeDef",
-    {
         "name": str,
+        "offset": int,
     },
-    total=False,
 )
 
-class PrimaryKeyOutputTypeDef(_RequiredPrimaryKeyOutputTypeDef, _OptionalPrimaryKeyOutputTypeDef):
-    pass
-
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -1125,17 +1063,19 @@
     "_OptionalPrimaryKeyTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
+
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -1168,19 +1108,21 @@
     "_OptionalStopApplicationRequestRequestTypeDef",
     {
         "forceStop": bool,
     },
     total=False,
 )
 
+
 class StopApplicationRequestRequestTypeDef(
     _RequiredStopApplicationRequestRequestTypeDef, _OptionalStopApplicationRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1215,19 +1157,21 @@
         "engineVersion": str,
         "instanceType": str,
         "preferredMaintenanceWindow": str,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environmentId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1252,24 +1196,22 @@
 
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
-    total=False,
 )
 
 BatchJobIdentifierOutputTypeDef = TypedDict(
     "BatchJobIdentifierOutputTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierOutputTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierOutputTypeDef,
     },
-    total=False,
 )
 
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierTypeDef,
@@ -1293,19 +1235,21 @@
         "kmsKeyId": str,
         "roleArn": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "currentApplicationVersion": int,
     },
 )
@@ -1314,19 +1258,21 @@
     {
         "definition": DefinitionTypeDef,
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1380,15 +1326,14 @@
 
 StorageConfigurationOutputTypeDef = TypedDict(
     "StorageConfigurationOutputTypeDef",
     {
         "efs": EfsStorageConfigurationOutputTypeDef,
         "fsx": FsxStorageConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
         "fsx": FsxStorageConfigurationTypeDef,
@@ -1425,28 +1370,26 @@
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
-    total=False,
 )
 
 VsamDetailAttributesTypeDef = TypedDict(
     "VsamDetailAttributesTypeDef",
     {
         "alternateKeys": List[AlternateKeyOutputTypeDef],
         "cacheAtStartup": bool,
         "compressed": bool,
         "encoding": str,
         "primaryKey": PrimaryKeyOutputTypeDef,
         "recordFormat": str,
     },
-    total=False,
 )
 
 _RequiredVsamAttributesTypeDef = TypedDict(
     "_RequiredVsamAttributesTypeDef",
     {
         "format": str,
     },
@@ -1458,53 +1401,44 @@
         "compressed": bool,
         "encoding": str,
         "primaryKey": PrimaryKeyTypeDef,
     },
     total=False,
 )
 
+
 class VsamAttributesTypeDef(_RequiredVsamAttributesTypeDef, _OptionalVsamAttributesTypeDef):
     pass
 
+
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
+BatchJobExecutionSummaryTypeDef = TypedDict(
+    "BatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
         "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
+        "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
     },
-    total=False,
 )
 
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
 GetBatchJobExecutionResponseTypeDef = TypedDict(
     "GetBatchJobExecutionResponseTypeDef",
     {
         "applicationId": str,
         "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
         "executionId": str,
@@ -1531,19 +1465,21 @@
     "_OptionalStartBatchJobRequestRequestTypeDef",
     {
         "jobParams": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartBatchJobRequestRequestTypeDef(
     _RequiredStartBatchJobRequestRequestTypeDef, _OptionalStartBatchJobRequestRequestTypeDef
 ):
     pass
 
+
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1571,19 +1507,21 @@
         "storageConfigurations": Sequence[StorageConfigurationTypeDef],
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "actualCapacity": int,
         "creationTime": datetime,
         "description": str,
         "engineType": EngineTypeType,
@@ -1613,15 +1551,14 @@
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
         "po": PoDetailAttributesTypeDef,
         "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
-    total=False,
 )
 
 DatasetOrgAttributesTypeDef = TypedDict(
     "DatasetOrgAttributesTypeDef",
     {
         "gdg": GdgAttributesTypeDef,
         "po": PoAttributesTypeDef,
@@ -1668,17 +1605,19 @@
     {
         "relativePath": str,
         "storageType": str,
     },
     total=False,
 )
 
+
 class DataSetTypeDef(_RequiredDataSetTypeDef, _OptionalDataSetTypeDef):
     pass
 
+
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
         "externalLocation": ExternalLocationTypeDef,
     },
 )
@@ -1703,12 +1642,13 @@
     "_OptionalCreateDataSetImportTaskRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateDataSetImportTaskRequestRequestTypeDef(
     _RequiredCreateDataSetImportTaskRequestRequestTypeDef,
     _OptionalCreateDataSetImportTaskRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/PKG-INFO` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.28.12
-Summary: Type annotations for boto3.MainframeModernization 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.MainframeModernization 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-m2-1.28.12/mypy_boto3_m2.egg-info/SOURCES.txt` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.12/setup.py` & `mypy-boto3-m2-1.28.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-m2",
-    version="1.28.12",
+    version="1.28.5",
     packages=["mypy_boto3_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MainframeModernization 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MainframeModernization 1.28.5 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

