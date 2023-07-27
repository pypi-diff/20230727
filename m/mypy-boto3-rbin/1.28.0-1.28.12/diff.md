# Comparing `tmp/mypy-boto3-rbin-1.28.0.tar.gz` & `tmp/mypy-boto3-rbin-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rbin-1.28.0.tar", last modified: Thu Jul  6 21:00:23 2023, max compression
+gzip compressed data, was "mypy-boto3-rbin-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
```

## Comparing `mypy-boto3-rbin-1.28.0.tar` & `mypy-boto3-rbin-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:23.290402 mypy-boto3-rbin-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-06 21:00:23.290402 mypy-boto3-rbin-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:23.286402 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-06 20:52:25.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-06 20:52:25.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-06 20:52:25.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-07-06 20:52:25.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:23.290402 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-06 21:00:23.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 21:00:23.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:23.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:23.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:23.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:00:23.000000 mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:23.290402 mypy-boto3-rbin-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-06 20:52:24.000000 mypy-boto3-rbin-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.637188 mypy-boto3-rbin-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-07-27 11:49:27.633188 mypy-boto3-rbin-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.621188 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.633188 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.637188 mypy-boto3-rbin-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/setup.py
```

### Comparing `mypy-boto3-rbin-1.28.0/LICENSE` & `mypy-boto3-rbin-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.0/PKG-INFO` & `mypy-boto3-rbin-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.28.0
-Summary: Type annotations for boto3.RecycleBin 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RecycleBin 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rbin"></a>
 
 # mypy-boto3-rbin
 
 [![PyPI - mypy-boto3-rbin](https://img.shields.io/pypi/v/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rbin?color=blue)](https://pypistats.org/packages/mypy-boto3-rbin)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,37 +326,42 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
+    ResourceTagOutputTypeDef,
+    ResponseMetadataTypeDef,
+    RetentionPeriodOutputTypeDef,
+    TagOutputTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    UnlockDelayOutputTypeDef,
     UnlockDelayTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    RuleSummaryTypeDef,
     UpdateRuleResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    LockConfigurationOutputTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
-    LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
+    LockRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ResourceTagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-rbin-1.28.0/README.md` & `mypy-boto3-rbin-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rbin"></a>
 
 # mypy-boto3-rbin
 
 [![PyPI - mypy-boto3-rbin](https://img.shields.io/pypi/v/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rbin?color=blue)](https://pypistats.org/packages/mypy-boto3-rbin)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,37 +294,42 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
+    ResourceTagOutputTypeDef,
+    ResponseMetadataTypeDef,
+    RetentionPeriodOutputTypeDef,
+    TagOutputTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    UnlockDelayOutputTypeDef,
     UnlockDelayTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    RuleSummaryTypeDef,
     UpdateRuleResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    LockConfigurationOutputTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
-    LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
+    LockRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ResourceTagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/__init__.py` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/__init__.pyi` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/__main__.py` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RecycleBin 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.RecycleBin 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin\nOther"
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

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/client.py` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/client.pyi` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/literals.py` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
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
@@ -242,26 +243,28 @@
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

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/literals.pyi` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
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
@@ -240,26 +241,28 @@
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

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/paginator.py` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -24,36 +24,33 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import LockStateType, ResourceTypeType
 from .type_defs import ListRulesResponseTypeDef, PaginatorConfigTypeDef, ResourceTagTypeDef
 
 __all__ = ("ListRulesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/paginators/#listrulespaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceType: ResourceTypeType,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
         LockState: LockStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/paginator.pyi` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,33 +24,36 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import LockStateType, ResourceTypeType
 from .type_defs import ListRulesResponseTypeDef, PaginatorConfigTypeDef, ResourceTagTypeDef
 
 __all__ = ("ListRulesPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/paginators/#listrulespaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceType: ResourceTypeType,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
         LockState: LockStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/type_defs.py` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,37 +27,42 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ResourceTagTypeDef",
     "RetentionPeriodTypeDef",
     "TagTypeDef",
+    "ResourceTagOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "RetentionPeriodOutputTypeDef",
+    "TagOutputTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "UnlockDelayOutputTypeDef",
     "UnlockDelayTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UnlockRuleRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "RuleSummaryTypeDef",
     "UpdateRuleRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "RuleSummaryTypeDef",
     "UpdateRuleResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "LockConfigurationOutputTypeDef",
     "LockConfigurationTypeDef",
     "ListRulesResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
-    "LockRuleRequestRequestTypeDef",
     "LockRuleResponseTypeDef",
     "UnlockRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "LockRuleRequestRequestTypeDef",
 )
 
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "ResourceTagKey": str,
     },
@@ -87,61 +92,106 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+_RequiredResourceTagOutputTypeDef = TypedDict(
+    "_RequiredResourceTagOutputTypeDef",
+    {
+        "ResourceTagKey": str,
+    },
+)
+_OptionalResourceTagOutputTypeDef = TypedDict(
+    "_OptionalResourceTagOutputTypeDef",
+    {
+        "ResourceTagValue": str,
+    },
+    total=False,
+)
+
+
+class ResourceTagOutputTypeDef(
+    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
+):
+    pass
+
+
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
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
+    {
+        "RetentionPeriodValue": int,
+        "RetentionPeriodUnit": Literal["DAYS"],
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-UnlockDelayTypeDef = TypedDict(
-    "UnlockDelayTypeDef",
+UnlockDelayOutputTypeDef = TypedDict(
+    "UnlockDelayOutputTypeDef",
     {
         "UnlockDelayValue": int,
         "UnlockDelayUnit": Literal["DAYS"],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UnlockDelayTypeDef = TypedDict(
+    "UnlockDelayTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "UnlockDelayValue": int,
+        "UnlockDelayUnit": Literal["DAYS"],
     },
 )
 
 UnlockRuleRequestRequestTypeDef = TypedDict(
     "UnlockRuleRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -152,38 +202,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockState": LockStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListRulesRequestRequestTypeDef = TypedDict(
@@ -200,25 +226,14 @@
 
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
 
-RuleSummaryTypeDef = TypedDict(
-    "RuleSummaryTypeDef",
-    {
-        "Identifier": str,
-        "Description": str,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "LockState": LockStateType,
-    },
-    total=False,
-)
-
 _RequiredUpdateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 _OptionalUpdateRuleRequestRequestTypeDef = TypedDict(
@@ -235,42 +250,84 @@
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+RuleSummaryTypeDef = TypedDict(
+    "RuleSummaryTypeDef",
+    {
+        "Identifier": str,
+        "Description": str,
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "LockState": LockStateType,
+    },
+    total=False,
+)
+
 UpdateRuleResponseTypeDef = TypedDict(
     "UpdateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodTypeDef,
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockState": LockStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+
+LockConfigurationOutputTypeDef = TypedDict(
+    "LockConfigurationOutputTypeDef",
+    {
+        "UnlockDelay": UnlockDelayOutputTypeDef,
     },
 )
 
 LockConfigurationTypeDef = TypedDict(
     "LockConfigurationTypeDef",
     {
         "UnlockDelay": UnlockDelayTypeDef,
@@ -278,106 +335,106 @@
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockConfiguration": LockConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodTypeDef,
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
         "Description": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LockRuleRequestRequestTypeDef = TypedDict(
-    "LockRuleRequestRequestTypeDef",
-    {
-        "Identifier": str,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LockRuleResponseTypeDef = TypedDict(
     "LockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UnlockRuleResponseTypeDef = TypedDict(
     "UnlockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockConfiguration": LockConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+
+LockRuleRequestRequestTypeDef = TypedDict(
+    "LockRuleRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "LockConfiguration": LockConfigurationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin/type_defs.pyi` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -26,37 +26,42 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ResourceTagTypeDef",
     "RetentionPeriodTypeDef",
     "TagTypeDef",
+    "ResourceTagOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "RetentionPeriodOutputTypeDef",
+    "TagOutputTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "UnlockDelayOutputTypeDef",
     "UnlockDelayTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UnlockRuleRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "RuleSummaryTypeDef",
     "UpdateRuleRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "RuleSummaryTypeDef",
     "UpdateRuleResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "LockConfigurationOutputTypeDef",
     "LockConfigurationTypeDef",
     "ListRulesResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
-    "LockRuleRequestRequestTypeDef",
     "LockRuleResponseTypeDef",
     "UnlockRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "LockRuleRequestRequestTypeDef",
 )
 
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "ResourceTagKey": str,
     },
@@ -84,61 +89,104 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+_RequiredResourceTagOutputTypeDef = TypedDict(
+    "_RequiredResourceTagOutputTypeDef",
+    {
+        "ResourceTagKey": str,
+    },
+)
+_OptionalResourceTagOutputTypeDef = TypedDict(
+    "_OptionalResourceTagOutputTypeDef",
+    {
+        "ResourceTagValue": str,
+    },
+    total=False,
+)
+
+class ResourceTagOutputTypeDef(
+    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
+):
+    pass
+
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
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
+    {
+        "RetentionPeriodValue": int,
+        "RetentionPeriodUnit": Literal["DAYS"],
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-UnlockDelayTypeDef = TypedDict(
-    "UnlockDelayTypeDef",
+UnlockDelayOutputTypeDef = TypedDict(
+    "UnlockDelayOutputTypeDef",
     {
         "UnlockDelayValue": int,
         "UnlockDelayUnit": Literal["DAYS"],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UnlockDelayTypeDef = TypedDict(
+    "UnlockDelayTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "UnlockDelayValue": int,
+        "UnlockDelayUnit": Literal["DAYS"],
     },
 )
 
 UnlockRuleRequestRequestTypeDef = TypedDict(
     "UnlockRuleRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -149,36 +197,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockState": LockStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListRulesRequestRequestTypeDef = TypedDict(
@@ -193,25 +219,14 @@
 )
 
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
-RuleSummaryTypeDef = TypedDict(
-    "RuleSummaryTypeDef",
-    {
-        "Identifier": str,
-        "Description": str,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "LockState": LockStateType,
-    },
-    total=False,
-)
-
 _RequiredUpdateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 _OptionalUpdateRuleRequestRequestTypeDef = TypedDict(
@@ -226,42 +241,82 @@
 )
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+RuleSummaryTypeDef = TypedDict(
+    "RuleSummaryTypeDef",
+    {
+        "Identifier": str,
+        "Description": str,
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "LockState": LockStateType,
+    },
+    total=False,
+)
+
 UpdateRuleResponseTypeDef = TypedDict(
     "UpdateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodTypeDef,
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockState": LockStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+LockConfigurationOutputTypeDef = TypedDict(
+    "LockConfigurationOutputTypeDef",
+    {
+        "UnlockDelay": UnlockDelayOutputTypeDef,
     },
 )
 
 LockConfigurationTypeDef = TypedDict(
     "LockConfigurationTypeDef",
     {
         "UnlockDelay": UnlockDelayTypeDef,
@@ -269,104 +324,104 @@
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockConfiguration": LockConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodTypeDef,
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
         "Description": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LockRuleRequestRequestTypeDef = TypedDict(
-    "LockRuleRequestRequestTypeDef",
-    {
-        "Identifier": str,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LockRuleResponseTypeDef = TypedDict(
     "LockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UnlockRuleResponseTypeDef = TypedDict(
     "UnlockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceTags": List[ResourceTagTypeDef],
+        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationTypeDef,
+        "LockConfiguration": LockConfigurationOutputTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockConfiguration": LockConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+LockRuleRequestRequestTypeDef = TypedDict(
+    "LockRuleRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "LockConfiguration": LockConfigurationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/PKG-INFO` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.28.0
-Summary: Type annotations for boto3.RecycleBin 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RecycleBin 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rbin"></a>
 
 # mypy-boto3-rbin
 
 [![PyPI - mypy-boto3-rbin](https://img.shields.io/pypi/v/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rbin?color=blue)](https://pypistats.org/packages/mypy-boto3-rbin)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,37 +326,42 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
+    ResourceTagOutputTypeDef,
+    ResponseMetadataTypeDef,
+    RetentionPeriodOutputTypeDef,
+    TagOutputTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    UnlockDelayOutputTypeDef,
     UnlockDelayTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    RuleSummaryTypeDef,
     UpdateRuleResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    LockConfigurationOutputTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
-    LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
+    LockRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ResourceTagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-rbin-1.28.0/mypy_boto3_rbin.egg-info/SOURCES.txt` & `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.0/setup.py` & `mypy-boto3-rbin-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rbin",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_rbin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RecycleBin 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.RecycleBin 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

