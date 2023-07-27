# Comparing `tmp/mypy-boto3-resourcegroupstaggingapi-1.28.0.tar.gz` & `tmp/mypy-boto3-resourcegroupstaggingapi-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resourcegroupstaggingapi-1.28.0.tar", last modified: Thu Jul  6 21:00:26 2023, max compression
+gzip compressed data, was "mypy-boto3-resourcegroupstaggingapi-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0.tar` & `mypy-boto3-resourcegroupstaggingapi-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.678409 mypy-boto3-resourcegroupstaggingapi-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-06 21:00:26.674409 mypy-boto3-resourcegroupstaggingapi-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.662409 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-06 20:53:21.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.674409 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-06 21:00:26.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 21:00:26.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:26.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 21:00:26.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:26.678409 mypy-boto3-resourcegroupstaggingapi-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-06 20:53:20.000000 mypy-boto3-resourcegroupstaggingapi-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.325214 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-27 11:44:42.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-27 11:44:41.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/setup.py
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/LICENSE` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/PKG-INFO` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resourcegroupstaggingapi
-Version: 1.28.0
-Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resourcegroupstaggingapi"></a>
 
 # mypy-boto3-resourcegroupstaggingapi
 
 [![PyPI - mypy-boto3-resourcegroupstaggingapi](https://img.shields.io/pypi/v/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/mypy-boto3-resourcegroupstaggingapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resourcegroupstaggingapi)](https://pepy.tech/project/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,34 +337,34 @@
 
 `mypy_boto3_resourcegroupstaggingapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    DescribeReportCreationOutputTypeDef,
+    ResponseMetadataTypeDef,
     FailureInfoTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
-    GetTagValuesOutputTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
+    DescribeReportCreationOutputTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/README.md` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resourcegroupstaggingapi"></a>
 
 # mypy-boto3-resourcegroupstaggingapi
 
 [![PyPI - mypy-boto3-resourcegroupstaggingapi](https://img.shields.io/pypi/v/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/mypy-boto3-resourcegroupstaggingapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resourcegroupstaggingapi)](https://pepy.tech/project/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,34 +305,34 @@
 
 `mypy_boto3_resourcegroupstaggingapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    DescribeReportCreationOutputTypeDef,
+    ResponseMetadataTypeDef,
     FailureInfoTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
-    GetTagValuesOutputTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
+    DescribeReportCreationOutputTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/__init__.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/__init__.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/__main__.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI\nOther"
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/client.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/client.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/literals.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,15 @@
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
@@ -244,26 +245,28 @@
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/literals.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.pyi`

 * *Files 4% similar despite different names*

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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/paginator.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 
@@ -90,43 +90,43 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
 
 
 class GetTagKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTagKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
         """
 
 
 class GetTagValuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
     """
 
     def paginate(
-        self, *, Key: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Key: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTagValuesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
         """
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/paginator.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 class GetResourcesPaginator(Paginator):
@@ -86,41 +86,41 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
 
 class GetTagKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTagKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
         """
 
 class GetTagValuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
     """
 
     def paginate(
-        self, *, Key: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Key: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTagValuesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
         """
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/type_defs.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,34 +20,34 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ComplianceDetailsTypeDef",
-    "DescribeReportCreationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "FailureInfoTypeDef",
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetComplianceSummaryInputRequestTypeDef",
     "SummaryTypeDef",
     "TagFilterTypeDef",
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
     "GetTagKeysInputRequestTypeDef",
-    "GetTagKeysOutputTypeDef",
-    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetTagValuesInputRequestTypeDef",
-    "GetTagValuesOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "StartReportCreationInputRequestTypeDef",
     "TagResourcesInputRequestTypeDef",
     "UntagResourcesInputRequestTypeDef",
+    "DescribeReportCreationOutputTypeDef",
+    "GetTagKeysOutputTypeDef",
+    "GetTagValuesOutputTypeDef",
     "TagResourcesOutputTypeDef",
     "UntagResourcesOutputTypeDef",
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetComplianceSummaryOutputTypeDef",
     "GetResourcesInputGetResourcesPaginateTypeDef",
     "GetResourcesInputRequestTypeDef",
     "ResourceTagMappingTypeDef",
     "GetResourcesOutputTypeDef",
 )
 
@@ -57,43 +57,41 @@
         "NoncompliantKeys": List[str],
         "KeysWithNoncompliantValues": List[str],
         "ComplianceStatus": bool,
     },
     total=False,
 )
 
-DescribeReportCreationOutputTypeDef = TypedDict(
-    "DescribeReportCreationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "S3Location": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "StatusCode": int,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TargetIdFilters": Sequence[str],
-        "RegionFilters": Sequence[str],
-        "ResourceTypeFilters": Sequence[str],
-        "TagKeyFilters": Sequence[str],
-        "GroupBy": Sequence[GroupByAttributeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetComplianceSummaryInputRequestTypeDef = TypedDict(
     "GetComplianceSummaryInputRequestTypeDef",
     {
@@ -126,61 +124,22 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetTagKeysInputRequestTypeDef = TypedDict(
     "GetTagKeysInputRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
-GetTagKeysOutputTypeDef = TypedDict(
-    "GetTagKeysOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagKeys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTagValuesInputGetTagValuesPaginateTypeDef(
-    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
-    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTagValuesInputRequestTypeDef = TypedDict(
     "_RequiredGetTagValuesInputRequestTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalGetTagValuesInputRequestTypeDef = TypedDict(
@@ -194,52 +153,22 @@
 
 class GetTagValuesInputRequestTypeDef(
     _RequiredGetTagValuesInputRequestTypeDef, _OptionalGetTagValuesInputRequestTypeDef
 ):
     pass
 
 
-GetTagValuesOutputTypeDef = TypedDict(
-    "GetTagValuesOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 StartReportCreationInputRequestTypeDef = TypedDict(
     "StartReportCreationInputRequestTypeDef",
     {
         "S3Bucket": str,
     },
 )
 
@@ -255,49 +184,120 @@
     "UntagResourcesInputRequestTypeDef",
     {
         "ResourceARNList": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeReportCreationOutputTypeDef = TypedDict(
+    "DescribeReportCreationOutputTypeDef",
+    {
+        "Status": str,
+        "S3Location": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagKeysOutputTypeDef = TypedDict(
+    "GetTagKeysOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagKeys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagValuesOutputTypeDef = TypedDict(
+    "GetTagValuesOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourcesOutputTypeDef = TypedDict(
     "TagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UntagResourcesOutputTypeDef = TypedDict(
     "UntagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    {
+        "TargetIdFilters": Sequence[str],
+        "RegionFilters": Sequence[str],
+        "ResourceTypeFilters": Sequence[str],
+        "TagKeyFilters": Sequence[str],
+        "GroupBy": Sequence[GroupByAttributeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "Key": str,
     },
 )
+_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTagValuesInputGetTagValuesPaginateTypeDef(
+    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
+    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
+):
+    pass
+
 
 GetComplianceSummaryOutputTypeDef = TypedDict(
     "GetComplianceSummaryOutputTypeDef",
     {
         "SummaryList": List[SummaryTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesInputGetResourcesPaginateTypeDef = TypedDict(
     "GetResourcesInputGetResourcesPaginateTypeDef",
     {
         "TagFilters": Sequence[TagFilterTypeDef],
         "TagsPerPage": int,
         "ResourceTypeFilters": Sequence[str],
         "IncludeComplianceDetails": bool,
         "ExcludeCompliantResources": bool,
         "ResourceARNList": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetResourcesInputRequestTypeDef = TypedDict(
     "GetResourcesInputRequestTypeDef",
     {
@@ -324,10 +324,10 @@
 )
 
 GetResourcesOutputTypeDef = TypedDict(
     "GetResourcesOutputTypeDef",
     {
         "PaginationToken": str,
         "ResourceTagMappingList": List[ResourceTagMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ComplianceDetailsTypeDef",
-    "DescribeReportCreationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "FailureInfoTypeDef",
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetComplianceSummaryInputRequestTypeDef",
     "SummaryTypeDef",
     "TagFilterTypeDef",
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
     "GetTagKeysInputRequestTypeDef",
-    "GetTagKeysOutputTypeDef",
-    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetTagValuesInputRequestTypeDef",
-    "GetTagValuesOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "StartReportCreationInputRequestTypeDef",
     "TagResourcesInputRequestTypeDef",
     "UntagResourcesInputRequestTypeDef",
+    "DescribeReportCreationOutputTypeDef",
+    "GetTagKeysOutputTypeDef",
+    "GetTagValuesOutputTypeDef",
     "TagResourcesOutputTypeDef",
     "UntagResourcesOutputTypeDef",
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetComplianceSummaryOutputTypeDef",
     "GetResourcesInputGetResourcesPaginateTypeDef",
     "GetResourcesInputRequestTypeDef",
     "ResourceTagMappingTypeDef",
     "GetResourcesOutputTypeDef",
 )
 
@@ -56,43 +56,41 @@
         "NoncompliantKeys": List[str],
         "KeysWithNoncompliantValues": List[str],
         "ComplianceStatus": bool,
     },
     total=False,
 )
 
-DescribeReportCreationOutputTypeDef = TypedDict(
-    "DescribeReportCreationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "S3Location": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "StatusCode": int,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TargetIdFilters": Sequence[str],
-        "RegionFilters": Sequence[str],
-        "ResourceTypeFilters": Sequence[str],
-        "TagKeyFilters": Sequence[str],
-        "GroupBy": Sequence[GroupByAttributeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetComplianceSummaryInputRequestTypeDef = TypedDict(
     "GetComplianceSummaryInputRequestTypeDef",
     {
@@ -125,59 +123,22 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetTagKeysInputRequestTypeDef = TypedDict(
     "GetTagKeysInputRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
-GetTagKeysOutputTypeDef = TypedDict(
-    "GetTagKeysOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagKeys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTagValuesInputGetTagValuesPaginateTypeDef(
-    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
-    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetTagValuesInputRequestTypeDef = TypedDict(
     "_RequiredGetTagValuesInputRequestTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalGetTagValuesInputRequestTypeDef = TypedDict(
@@ -189,52 +150,22 @@
 )
 
 class GetTagValuesInputRequestTypeDef(
     _RequiredGetTagValuesInputRequestTypeDef, _OptionalGetTagValuesInputRequestTypeDef
 ):
     pass
 
-GetTagValuesOutputTypeDef = TypedDict(
-    "GetTagValuesOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 StartReportCreationInputRequestTypeDef = TypedDict(
     "StartReportCreationInputRequestTypeDef",
     {
         "S3Bucket": str,
     },
 )
 
@@ -250,49 +181,118 @@
     "UntagResourcesInputRequestTypeDef",
     {
         "ResourceARNList": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeReportCreationOutputTypeDef = TypedDict(
+    "DescribeReportCreationOutputTypeDef",
+    {
+        "Status": str,
+        "S3Location": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagKeysOutputTypeDef = TypedDict(
+    "GetTagKeysOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagKeys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagValuesOutputTypeDef = TypedDict(
+    "GetTagValuesOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourcesOutputTypeDef = TypedDict(
     "TagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UntagResourcesOutputTypeDef = TypedDict(
     "UntagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    {
+        "TargetIdFilters": Sequence[str],
+        "RegionFilters": Sequence[str],
+        "ResourceTypeFilters": Sequence[str],
+        "TagKeyFilters": Sequence[str],
+        "GroupBy": Sequence[GroupByAttributeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTagValuesInputGetTagValuesPaginateTypeDef(
+    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
+    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
+):
+    pass
+
 GetComplianceSummaryOutputTypeDef = TypedDict(
     "GetComplianceSummaryOutputTypeDef",
     {
         "SummaryList": List[SummaryTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesInputGetResourcesPaginateTypeDef = TypedDict(
     "GetResourcesInputGetResourcesPaginateTypeDef",
     {
         "TagFilters": Sequence[TagFilterTypeDef],
         "TagsPerPage": int,
         "ResourceTypeFilters": Sequence[str],
         "IncludeComplianceDetails": bool,
         "ExcludeCompliantResources": bool,
         "ResourceARNList": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetResourcesInputRequestTypeDef = TypedDict(
     "GetResourcesInputRequestTypeDef",
     {
@@ -319,10 +319,10 @@
 )
 
 GetResourcesOutputTypeDef = TypedDict(
     "GetResourcesOutputTypeDef",
     {
         "PaginationToken": str,
         "ResourceTagMappingList": List[ResourceTagMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resourcegroupstaggingapi
-Version: 1.28.0
-Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resourcegroupstaggingapi"></a>
 
 # mypy-boto3-resourcegroupstaggingapi
 
 [![PyPI - mypy-boto3-resourcegroupstaggingapi](https://img.shields.io/pypi/v/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/mypy-boto3-resourcegroupstaggingapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resourcegroupstaggingapi)](https://pepy.tech/project/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,34 +337,34 @@
 
 `mypy_boto3_resourcegroupstaggingapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    DescribeReportCreationOutputTypeDef,
+    ResponseMetadataTypeDef,
     FailureInfoTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
-    GetTagValuesOutputTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
+    DescribeReportCreationOutputTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.0/setup.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resourcegroupstaggingapi",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_resourcegroupstaggingapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

