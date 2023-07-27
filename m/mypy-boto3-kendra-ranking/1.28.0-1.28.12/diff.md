# Comparing `tmp/mypy-boto3-kendra-ranking-1.28.0.tar.gz` & `tmp/mypy-boto3-kendra-ranking-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-ranking-1.28.0.tar", last modified: Thu Jul  6 20:59:53 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-ranking-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
```

## Comparing `mypy-boto3-kendra-ranking-1.28.0.tar` & `mypy-boto3-kendra-ranking-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:53.894342 mypy-boto3-kendra-ranking-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-07-06 20:59:53.894342 mypy-boto3-kendra-ranking-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:53.878342 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-06 20:44:38.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-06 20:44:38.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-06 20:44:38.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-06 20:44:38.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:53.894342 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-07-06 20:59:53.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 20:59:53.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:53.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:53.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:53.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:53.000000 mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:53.894342 mypy-boto3-kendra-ranking-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:44:37.000000 mypy-boto3-kendra-ranking-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.064470 mypy-boto3-kendra-ranking-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-07-27 05:34:53.064470 mypy-boto3-kendra-ranking-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.060470 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-27 05:24:37.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-27 05:24:37.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-27 05:24:37.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.064470 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-07-27 05:34:52.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 05:34:52.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:52.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:52.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:52.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:52.000000 mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.064470 mypy-boto3-kendra-ranking-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:24:36.000000 mypy-boto3-kendra-ranking-1.28.12/setup.py
```

### Comparing `mypy-boto3-kendra-ranking-1.28.0/LICENSE` & `mypy-boto3-kendra-ranking-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-ranking-1.28.0/PKG-INFO` & `mypy-boto3-kendra-ranking-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra-ranking
-Version: 1.28.0
-Summary: Type annotations for boto3.KendraRanking 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KendraRanking 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kendra-ranking"></a>
 
 # mypy-boto3-kendra-ranking
 
 [![PyPI - mypy-boto3-kendra-ranking](https://img.shields.io/pypi/v/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra-ranking?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra-ranking)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra-ranking)](https://pepy.tech/project/mypy-boto3-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KendraRanking 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[boto3.KendraRanking 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
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
 [mypy-boto3-kendra-ranking docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,39 +298,41 @@
 ### Typed dictionaries
 
 `mypy_boto3_kendra_ranking.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra_ranking.type_defs import (
+    CapacityUnitsConfigurationOutputTypeDef,
     CapacityUnitsConfigurationTypeDef,
     TagTypeDef,
     CreateRescoreExecutionPlanResponseTypeDef,
     DeleteRescoreExecutionPlanRequestRequestTypeDef,
     DescribeRescoreExecutionPlanRequestRequestTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     ListRescoreExecutionPlansRequestRequestTypeDef,
     RescoreExecutionPlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RescoreResultItemTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     DescribeRescoreExecutionPlanResponseTypeDef,
     UpdateRescoreExecutionPlanRequestRequestTypeDef,
     CreateRescoreExecutionPlanRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     RescoreRequestRequestTypeDef,
     ListRescoreExecutionPlansResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RescoreResultTypeDef,
 )
 
 
-def get_structure() -> CapacityUnitsConfigurationTypeDef:
+def get_structure() -> CapacityUnitsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kendra-ranking-1.28.0/README.md` & `mypy-boto3-kendra-ranking-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kendra-ranking"></a>
 
 # mypy-boto3-kendra-ranking
 
 [![PyPI - mypy-boto3-kendra-ranking](https://img.shields.io/pypi/v/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra-ranking?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra-ranking)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra-ranking)](https://pepy.tech/project/mypy-boto3-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KendraRanking 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[boto3.KendraRanking 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
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
 [mypy-boto3-kendra-ranking docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,39 +266,41 @@
 ### Typed dictionaries
 
 `mypy_boto3_kendra_ranking.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra_ranking.type_defs import (
+    CapacityUnitsConfigurationOutputTypeDef,
     CapacityUnitsConfigurationTypeDef,
     TagTypeDef,
     CreateRescoreExecutionPlanResponseTypeDef,
     DeleteRescoreExecutionPlanRequestRequestTypeDef,
     DescribeRescoreExecutionPlanRequestRequestTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     ListRescoreExecutionPlansRequestRequestTypeDef,
     RescoreExecutionPlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RescoreResultItemTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     DescribeRescoreExecutionPlanResponseTypeDef,
     UpdateRescoreExecutionPlanRequestRequestTypeDef,
     CreateRescoreExecutionPlanRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     RescoreRequestRequestTypeDef,
     ListRescoreExecutionPlansResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RescoreResultTypeDef,
 )
 
 
-def get_structure() -> CapacityUnitsConfigurationTypeDef:
+def get_structure() -> CapacityUnitsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/__main__.py` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KendraRanking 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.KendraRanking 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking\nOther"
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

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/client.py` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/client.pyi` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/literals.py` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
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
@@ -231,26 +232,28 @@
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

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/literals.pyi` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
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
@@ -229,26 +230,28 @@
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

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/type_defs.py` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kendra-ranking service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kendra_ranking.type_defs import CapacityUnitsConfigurationTypeDef
+    from mypy_boto3_kendra_ranking.type_defs import CapacityUnitsConfigurationOutputTypeDef
 
-    data: CapacityUnitsConfigurationTypeDef = {...}
+    data: CapacityUnitsConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import RescoreExecutionPlanStatusType
@@ -20,37 +20,46 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "CapacityUnitsConfigurationOutputTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "TagTypeDef",
     "CreateRescoreExecutionPlanResponseTypeDef",
     "DeleteRescoreExecutionPlanRequestRequestTypeDef",
     "DescribeRescoreExecutionPlanRequestRequestTypeDef",
     "DocumentTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListRescoreExecutionPlansRequestRequestTypeDef",
     "RescoreExecutionPlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RescoreResultItemTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DescribeRescoreExecutionPlanResponseTypeDef",
     "UpdateRescoreExecutionPlanRequestRequestTypeDef",
     "CreateRescoreExecutionPlanRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "RescoreRequestRequestTypeDef",
     "ListRescoreExecutionPlansResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RescoreResultTypeDef",
 )
 
+CapacityUnitsConfigurationOutputTypeDef = TypedDict(
+    "CapacityUnitsConfigurationOutputTypeDef",
+    {
+        "RescoreCapacityUnits": int,
+    },
+)
+
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
     {
         "RescoreCapacityUnits": int,
     },
 )
 
@@ -140,14 +149,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 RescoreResultItemTypeDef = TypedDict(
     "RescoreResultItemTypeDef",
     {
         "DocumentId": str,
         "Score": float,
     },
     total=False,
@@ -175,15 +192,15 @@
 DescribeRescoreExecutionPlanResponseTypeDef = TypedDict(
     "DescribeRescoreExecutionPlanResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "CapacityUnits": CapacityUnitsConfigurationOutputTypeDef,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": RescoreExecutionPlanStatusType,
         "ErrorMessage": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -233,22 +250,14 @@
 class CreateRescoreExecutionPlanRequestRequestTypeDef(
     _RequiredCreateRescoreExecutionPlanRequestRequestTypeDef,
     _OptionalCreateRescoreExecutionPlanRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -267,14 +276,22 @@
     {
         "SummaryItems": List[RescoreExecutionPlanSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RescoreResultTypeDef = TypedDict(
     "RescoreResultTypeDef",
     {
         "RescoreId": str,
         "ResultItems": List[RescoreResultItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking/type_defs.pyi` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,54 +2,63 @@
 Type annotations for kendra-ranking service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kendra_ranking.type_defs import CapacityUnitsConfigurationTypeDef
+    from mypy_boto3_kendra_ranking.type_defs import CapacityUnitsConfigurationOutputTypeDef
 
-    data: CapacityUnitsConfigurationTypeDef = {...}
+    data: CapacityUnitsConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import RescoreExecutionPlanStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "CapacityUnitsConfigurationOutputTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "TagTypeDef",
     "CreateRescoreExecutionPlanResponseTypeDef",
     "DeleteRescoreExecutionPlanRequestRequestTypeDef",
     "DescribeRescoreExecutionPlanRequestRequestTypeDef",
     "DocumentTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListRescoreExecutionPlansRequestRequestTypeDef",
     "RescoreExecutionPlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RescoreResultItemTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DescribeRescoreExecutionPlanResponseTypeDef",
     "UpdateRescoreExecutionPlanRequestRequestTypeDef",
     "CreateRescoreExecutionPlanRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "RescoreRequestRequestTypeDef",
     "ListRescoreExecutionPlansResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RescoreResultTypeDef",
 )
 
+CapacityUnitsConfigurationOutputTypeDef = TypedDict(
+    "CapacityUnitsConfigurationOutputTypeDef",
+    {
+        "RescoreCapacityUnits": int,
+    },
+)
+
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
     {
         "RescoreCapacityUnits": int,
     },
 )
 
@@ -137,14 +146,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 RescoreResultItemTypeDef = TypedDict(
     "RescoreResultItemTypeDef",
     {
         "DocumentId": str,
         "Score": float,
     },
     total=False,
@@ -172,15 +189,15 @@
 DescribeRescoreExecutionPlanResponseTypeDef = TypedDict(
     "DescribeRescoreExecutionPlanResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "CapacityUnits": CapacityUnitsConfigurationOutputTypeDef,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": RescoreExecutionPlanStatusType,
         "ErrorMessage": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -226,22 +243,14 @@
 
 class CreateRescoreExecutionPlanRequestRequestTypeDef(
     _RequiredCreateRescoreExecutionPlanRequestRequestTypeDef,
     _OptionalCreateRescoreExecutionPlanRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -260,14 +269,22 @@
     {
         "SummaryItems": List[RescoreExecutionPlanSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RescoreResultTypeDef = TypedDict(
     "RescoreResultTypeDef",
     {
         "RescoreId": str,
         "ResultItems": List[RescoreResultItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/PKG-INFO` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra-ranking
-Version: 1.28.0
-Summary: Type annotations for boto3.KendraRanking 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KendraRanking 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kendra-ranking"></a>
 
 # mypy-boto3-kendra-ranking
 
 [![PyPI - mypy-boto3-kendra-ranking](https://img.shields.io/pypi/v/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra-ranking.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra-ranking)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra-ranking?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra-ranking)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra-ranking)](https://pepy.tech/project/mypy-boto3-kendra-ranking)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KendraRanking 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
+[boto3.KendraRanking 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking)
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
 [mypy-boto3-kendra-ranking docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,39 +298,41 @@
 ### Typed dictionaries
 
 `mypy_boto3_kendra_ranking.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra_ranking.type_defs import (
+    CapacityUnitsConfigurationOutputTypeDef,
     CapacityUnitsConfigurationTypeDef,
     TagTypeDef,
     CreateRescoreExecutionPlanResponseTypeDef,
     DeleteRescoreExecutionPlanRequestRequestTypeDef,
     DescribeRescoreExecutionPlanRequestRequestTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     ListRescoreExecutionPlansRequestRequestTypeDef,
     RescoreExecutionPlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RescoreResultItemTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     DescribeRescoreExecutionPlanResponseTypeDef,
     UpdateRescoreExecutionPlanRequestRequestTypeDef,
     CreateRescoreExecutionPlanRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     RescoreRequestRequestTypeDef,
     ListRescoreExecutionPlansResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RescoreResultTypeDef,
 )
 
 
-def get_structure() -> CapacityUnitsConfigurationTypeDef:
+def get_structure() -> CapacityUnitsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kendra-ranking-1.28.0/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt` & `mypy-boto3-kendra-ranking-1.28.12/mypy_boto3_kendra_ranking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-ranking-1.28.0/setup.py` & `mypy-boto3-kendra-ranking-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra-ranking",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kendra_ranking"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KendraRanking 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.KendraRanking 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

