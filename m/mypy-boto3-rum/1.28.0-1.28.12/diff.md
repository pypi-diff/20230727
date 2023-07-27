# Comparing `tmp/mypy-boto3-rum-1.28.0.tar.gz` & `tmp/mypy-boto3-rum-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rum-1.28.0.tar", last modified: Thu Jul  6 21:00:29 2023, max compression
+gzip compressed data, was "mypy-boto3-rum-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
```

## Comparing `mypy-boto3-rum-1.28.0.tar` & `mypy-boto3-rum-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.950415 mypy-boto3-rum-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-06 21:00:29.938415 mypy-boto3-rum-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.934415 mypy-boto3-rum-1.28.0/mypy_boto3_rum/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20132 2023-07-06 20:53:51.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.938415 mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-06 21:00:29.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:29.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:29.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:29.000000 mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:29.950415 mypy-boto3-rum-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:53:50.000000 mypy-boto3-rum-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/mypy_boto3_rum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 11:45:00.000000 mypy-boto3-rum-1.28.12/setup.py
```

### Comparing `mypy-boto3-rum-1.28.0/LICENSE` & `mypy-boto3-rum-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.0/PKG-INFO` & `mypy-boto3-rum-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rum"></a>
 
 # mypy-boto3-rum
 
 [![PyPI - mypy-boto3-rum](https://img.shields.io/pypi/v/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rum?color=blue)](https://pypistats.org/packages/mypy-boto3-rum)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,66 +338,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_rum.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rum.type_defs import (
+    AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
-    CustomEventsTypeDef,
+    CustomEventsOutputTypeDef,
+    MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CreateAppMonitorResponseTypeDef,
+    CustomEventsTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
-    GetAppMonitorDataResponseTypeDef,
     GetAppMonitorRequestRequestTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
+    CreateAppMonitorResponseTypeDef,
+    GetAppMonitorDataResponseTypeDef,
+    ListAppMonitorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
+    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
+    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+    CreateAppMonitorRequestRequestTypeDef,
+    UpdateAppMonitorRequestRequestTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
     GetAppMonitorResponseTypeDef,
 )
 
 
-def get_structure() -> AppMonitorConfigurationTypeDef:
+def get_structure() -> AppMonitorConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rum-1.28.0/README.md` & `mypy-boto3-rum-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rum"></a>
 
 # mypy-boto3-rum
 
 [![PyPI - mypy-boto3-rum](https://img.shields.io/pypi/v/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rum?color=blue)](https://pypistats.org/packages/mypy-boto3-rum)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,66 +306,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_rum.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rum.type_defs import (
+    AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
-    CustomEventsTypeDef,
+    CustomEventsOutputTypeDef,
+    MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CreateAppMonitorResponseTypeDef,
+    CustomEventsTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
-    GetAppMonitorDataResponseTypeDef,
     GetAppMonitorRequestRequestTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
+    CreateAppMonitorResponseTypeDef,
+    GetAppMonitorDataResponseTypeDef,
+    ListAppMonitorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
+    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
+    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+    CreateAppMonitorRequestRequestTypeDef,
+    UpdateAppMonitorRequestRequestTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
     GetAppMonitorResponseTypeDef,
 )
 
 
-def get_structure() -> AppMonitorConfigurationTypeDef:
+def get_structure() -> AppMonitorConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/__init__.py` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/__init__.pyi` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/__main__.py` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchRUM 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudWatchRUM 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
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

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/client.py` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/client.pyi` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/literals.py` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
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
@@ -246,26 +247,28 @@
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

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/literals.pyi` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.pyi`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/paginator.py` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,86 +43,80 @@
 __all__ = (
     "BatchGetRumMetricDefinitionsPaginator",
     "GetAppMonitorDataPaginator",
     "ListAppMonitorsPaginator",
     "ListRumMetricsDestinationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class BatchGetRumMetricDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[BatchGetRumMetricDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
         """
 
-
 class GetAppMonitorDataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
     """
 
     def paginate(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAppMonitorDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
         """
 
-
 class ListAppMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
         """
 
-
 class ListRumMetricsDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
     """
 
     def paginate(
-        self, *, AppMonitorName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AppMonitorName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRumMetricsDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
         """
```

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/paginator.pyi` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,80 +43,86 @@
 __all__ = (
     "BatchGetRumMetricDefinitionsPaginator",
     "GetAppMonitorDataPaginator",
     "ListAppMonitorsPaginator",
     "ListRumMetricsDestinationsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class BatchGetRumMetricDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[BatchGetRumMetricDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
         """
 
+
 class GetAppMonitorDataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
     """
 
     def paginate(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAppMonitorDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
         """
 
+
 class ListAppMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
         """
 
+
 class ListRumMetricsDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
     """
 
     def paginate(
-        self, *, AppMonitorName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AppMonitorName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRumMetricsDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
         """
```

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/type_defs.py` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for rum service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rum.type_defs import AppMonitorConfigurationTypeDef
+    from mypy_boto3_rum.type_defs import AppMonitorConfigurationOutputTypeDef
 
-    data: AppMonitorConfigurationTypeDef = {...}
+    data: AppMonitorConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import CustomEventsStatusType, MetricDestinationType, StateEnumType, TelemetryType
@@ -20,64 +20,83 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
-    "CustomEventsTypeDef",
+    "CustomEventsOutputTypeDef",
+    "MetricDefinitionRequestOutputTypeDef",
     "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
-    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
-    "CreateAppMonitorResponseTypeDef",
+    "CustomEventsTypeDef",
     "CwLogTypeDef",
     "DeleteAppMonitorRequestRequestTypeDef",
     "DeleteRumMetricsDestinationRequestRequestTypeDef",
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
-    "GetAppMonitorDataResponseTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
-    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "RumEventTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListAppMonitorsResponseTypeDef",
-    "CreateAppMonitorRequestRequestTypeDef",
-    "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
+    "CreateAppMonitorResponseTypeDef",
+    "GetAppMonitorDataResponseTypeDef",
+    "ListAppMonitorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
+    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
+    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    "CreateAppMonitorRequestRequestTypeDef",
+    "UpdateAppMonitorRequestRequestTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
     "GetAppMonitorResponseTypeDef",
 )
 
+AppMonitorConfigurationOutputTypeDef = TypedDict(
+    "AppMonitorConfigurationOutputTypeDef",
+    {
+        "AllowCookies": bool,
+        "EnableXRay": bool,
+        "ExcludedPages": List[str],
+        "FavoritePages": List[str],
+        "GuestRoleArn": str,
+        "IdentityPoolId": str,
+        "IncludedPages": List[str],
+        "SessionSampleRate": float,
+        "Telemetries": List[TelemetryType],
+    },
+    total=False,
+)
+
 AppMonitorConfigurationTypeDef = TypedDict(
     "AppMonitorConfigurationTypeDef",
     {
         "AllowCookies": bool,
         "EnableXRay": bool,
         "ExcludedPages": Sequence[str],
         "FavoritePages": Sequence[str],
@@ -108,22 +127,47 @@
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
     },
     total=False,
 )
 
-CustomEventsTypeDef = TypedDict(
-    "CustomEventsTypeDef",
+CustomEventsOutputTypeDef = TypedDict(
+    "CustomEventsOutputTypeDef",
     {
         "Status": CustomEventsStatusType,
     },
     total=False,
 )
 
+_RequiredMetricDefinitionRequestOutputTypeDef = TypedDict(
+    "_RequiredMetricDefinitionRequestOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalMetricDefinitionRequestOutputTypeDef = TypedDict(
+    "_OptionalMetricDefinitionRequestOutputTypeDef",
+    {
+        "DimensionKeys": Dict[str, str],
+        "EventPattern": str,
+        "Namespace": str,
+        "UnitLabel": str,
+        "ValueKey": str,
+    },
+    total=False,
+)
+
+
+class MetricDefinitionRequestOutputTypeDef(
+    _RequiredMetricDefinitionRequestOutputTypeDef, _OptionalMetricDefinitionRequestOutputTypeDef
+):
+    pass
+
+
 _RequiredMetricDefinitionRequestTypeDef = TypedDict(
     "_RequiredMetricDefinitionRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalMetricDefinitionRequestTypeDef = TypedDict(
@@ -165,14 +209,25 @@
 )
 
 
 class MetricDefinitionTypeDef(_RequiredMetricDefinitionTypeDef, _OptionalMetricDefinitionTypeDef):
     pass
 
 
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
 BatchDeleteRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinitionId": str,
     },
@@ -198,38 +253,24 @@
 class BatchDeleteRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-    },
-)
-_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DestinationArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
-    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
         "Destination": MetricDestinationType,
     },
 )
@@ -247,20 +288,20 @@
 class BatchGetRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchGetRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
-CreateAppMonitorResponseTypeDef = TypedDict(
-    "CreateAppMonitorResponseTypeDef",
+CustomEventsTypeDef = TypedDict(
+    "CustomEventsTypeDef",
     {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Status": CustomEventsStatusType,
     },
+    total=False,
 )
 
 CwLogTypeDef = TypedDict(
     "CwLogTypeDef",
     {
         "CwLogEnabled": bool,
         "CwLogGroup": str,
@@ -322,69 +363,30 @@
 )
 
 
 class TimeRangeTypeDef(_RequiredTimeRangeTypeDef, _OptionalTimeRangeTypeDef):
     pass
 
 
-GetAppMonitorDataResponseTypeDef = TypedDict(
-    "GetAppMonitorDataResponseTypeDef",
-    {
-        "Events": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAppMonitorRequestRequestTypeDef = TypedDict(
     "GetAppMonitorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppMonitorsRequestRequestTypeDef = TypedDict(
     "ListAppMonitorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-    },
-)
-_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
-    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRumMetricsDestinationsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
     },
 )
 _OptionalListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
@@ -417,33 +419,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Dict[str, str],
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
 _RequiredRumEventTypeDef = TypedDict(
     "_RequiredRumEventTypeDef",
     {
         "details": str,
         "id": str,
         "timestamp": Union[datetime, str],
         "type": str,
@@ -491,25 +474,14 @@
 class PutRumMetricsDestinationRequestRequestTypeDef(
     _RequiredPutRumMetricsDestinationRequestRequestTypeDef,
     _OptionalPutRumMetricsDestinationRequestRequestTypeDef,
 ):
     pass
 
 
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -518,78 +490,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListAppMonitorsResponseTypeDef = TypedDict(
-    "ListAppMonitorsResponseTypeDef",
-    {
-        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppMonitorRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateAppMonitorRequestRequestTypeDef(
-    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Domain": str,
-    },
-    total=False,
-)
-
-
-class UpdateAppMonitorRequestRequestTypeDef(
-    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
-):
-    pass
-
-
 BatchCreateRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "MetricDefinition": MetricDefinitionRequestTypeDef,
+        "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
     },
 )
 
 _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
@@ -639,27 +553,165 @@
 
 
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppMonitorResponseTypeDef = TypedDict(
+    "CreateAppMonitorResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppMonitorDataResponseTypeDef = TypedDict(
+    "GetAppMonitorDataResponseTypeDef",
+    {
+        "Events": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppMonitorsResponseTypeDef = TypedDict(
+    "ListAppMonitorsResponseTypeDef",
+    {
+        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchDeleteRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitionIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+    },
+)
+_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    {
+        "DestinationArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
+    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+):
+    pass
+
+
+ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "AppMonitorName": str,
+    },
+)
+_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
+    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppMonitorRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateAppMonitorRequestRequestTypeDef(
+    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Domain": str,
+    },
+    total=False,
 )
 
+
+class UpdateAppMonitorRequestRequestTypeDef(
+    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
+):
+    pass
+
+
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
         "CwLog": CwLogTypeDef,
     },
     total=False,
 )
@@ -671,15 +723,15 @@
         "TimeRange": TimeRangeTypeDef,
     },
 )
 _OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef = TypedDict(
     "_OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     {
         "Filters": Sequence[QueryFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef(
     _RequiredGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
@@ -713,15 +765,15 @@
 
 
 ListRumMetricsDestinationsResponseTypeDef = TypedDict(
     "ListRumMetricsDestinationsResponseTypeDef",
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRumEventsRequestRequestTypeDef = TypedDict(
     "PutRumEventsRequestRequestTypeDef",
     {
         "AppMonitorDetails": AppMonitorDetailsTypeDef,
@@ -733,24 +785,24 @@
 )
 
 BatchCreateRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchCreateRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "AppMonitorConfiguration": AppMonitorConfigurationOutputTypeDef,
         "Created": str,
-        "CustomEvents": CustomEventsTypeDef,
+        "CustomEvents": CustomEventsOutputTypeDef,
         "DataStorage": DataStorageTypeDef,
         "Domain": str,
         "Id": str,
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
@@ -758,10 +810,10 @@
     total=False,
 )
 
 GetAppMonitorResponseTypeDef = TypedDict(
     "GetAppMonitorResponseTypeDef",
     {
         "AppMonitor": AppMonitorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum/type_defs.pyi` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,81 +2,100 @@
 Type annotations for rum service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rum.type_defs import AppMonitorConfigurationTypeDef
+    from mypy_boto3_rum.type_defs import AppMonitorConfigurationOutputTypeDef
 
-    data: AppMonitorConfigurationTypeDef = {...}
+    data: AppMonitorConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import CustomEventsStatusType, MetricDestinationType, StateEnumType, TelemetryType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
-    "CustomEventsTypeDef",
+    "CustomEventsOutputTypeDef",
+    "MetricDefinitionRequestOutputTypeDef",
     "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
-    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
-    "CreateAppMonitorResponseTypeDef",
+    "CustomEventsTypeDef",
     "CwLogTypeDef",
     "DeleteAppMonitorRequestRequestTypeDef",
     "DeleteRumMetricsDestinationRequestRequestTypeDef",
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
-    "GetAppMonitorDataResponseTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
-    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "RumEventTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListAppMonitorsResponseTypeDef",
-    "CreateAppMonitorRequestRequestTypeDef",
-    "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
+    "CreateAppMonitorResponseTypeDef",
+    "GetAppMonitorDataResponseTypeDef",
+    "ListAppMonitorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
+    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
+    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    "CreateAppMonitorRequestRequestTypeDef",
+    "UpdateAppMonitorRequestRequestTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
     "GetAppMonitorResponseTypeDef",
 )
 
+AppMonitorConfigurationOutputTypeDef = TypedDict(
+    "AppMonitorConfigurationOutputTypeDef",
+    {
+        "AllowCookies": bool,
+        "EnableXRay": bool,
+        "ExcludedPages": List[str],
+        "FavoritePages": List[str],
+        "GuestRoleArn": str,
+        "IdentityPoolId": str,
+        "IncludedPages": List[str],
+        "SessionSampleRate": float,
+        "Telemetries": List[TelemetryType],
+    },
+    total=False,
+)
+
 AppMonitorConfigurationTypeDef = TypedDict(
     "AppMonitorConfigurationTypeDef",
     {
         "AllowCookies": bool,
         "EnableXRay": bool,
         "ExcludedPages": Sequence[str],
         "FavoritePages": Sequence[str],
@@ -107,22 +126,45 @@
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
     },
     total=False,
 )
 
-CustomEventsTypeDef = TypedDict(
-    "CustomEventsTypeDef",
+CustomEventsOutputTypeDef = TypedDict(
+    "CustomEventsOutputTypeDef",
     {
         "Status": CustomEventsStatusType,
     },
     total=False,
 )
 
+_RequiredMetricDefinitionRequestOutputTypeDef = TypedDict(
+    "_RequiredMetricDefinitionRequestOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalMetricDefinitionRequestOutputTypeDef = TypedDict(
+    "_OptionalMetricDefinitionRequestOutputTypeDef",
+    {
+        "DimensionKeys": Dict[str, str],
+        "EventPattern": str,
+        "Namespace": str,
+        "UnitLabel": str,
+        "ValueKey": str,
+    },
+    total=False,
+)
+
+class MetricDefinitionRequestOutputTypeDef(
+    _RequiredMetricDefinitionRequestOutputTypeDef, _OptionalMetricDefinitionRequestOutputTypeDef
+):
+    pass
+
 _RequiredMetricDefinitionRequestTypeDef = TypedDict(
     "_RequiredMetricDefinitionRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalMetricDefinitionRequestTypeDef = TypedDict(
@@ -160,14 +202,25 @@
     },
     total=False,
 )
 
 class MetricDefinitionTypeDef(_RequiredMetricDefinitionTypeDef, _OptionalMetricDefinitionTypeDef):
     pass
 
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
 BatchDeleteRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinitionId": str,
     },
@@ -191,36 +244,24 @@
 
 class BatchDeleteRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-    },
-)
-_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DestinationArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
-    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-):
-    pass
-
 _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
         "Destination": MetricDestinationType,
     },
 )
@@ -236,20 +277,20 @@
 
 class BatchGetRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchGetRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
-CreateAppMonitorResponseTypeDef = TypedDict(
-    "CreateAppMonitorResponseTypeDef",
+CustomEventsTypeDef = TypedDict(
+    "CustomEventsTypeDef",
     {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Status": CustomEventsStatusType,
     },
+    total=False,
 )
 
 CwLogTypeDef = TypedDict(
     "CwLogTypeDef",
     {
         "CwLogEnabled": bool,
         "CwLogGroup": str,
@@ -307,67 +348,30 @@
     },
     total=False,
 )
 
 class TimeRangeTypeDef(_RequiredTimeRangeTypeDef, _OptionalTimeRangeTypeDef):
     pass
 
-GetAppMonitorDataResponseTypeDef = TypedDict(
-    "GetAppMonitorDataResponseTypeDef",
-    {
-        "Events": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAppMonitorRequestRequestTypeDef = TypedDict(
     "GetAppMonitorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppMonitorsRequestRequestTypeDef = TypedDict(
     "ListAppMonitorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-    },
-)
-_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
-    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRumMetricsDestinationsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
     },
 )
 _OptionalListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
@@ -398,33 +402,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Dict[str, str],
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
 _RequiredRumEventTypeDef = TypedDict(
     "_RequiredRumEventTypeDef",
     {
         "details": str,
         "id": str,
         "timestamp": Union[datetime, str],
         "type": str,
@@ -468,25 +453,14 @@
 
 class PutRumMetricsDestinationRequestRequestTypeDef(
     _RequiredPutRumMetricsDestinationRequestRequestTypeDef,
     _OptionalPutRumMetricsDestinationRequestRequestTypeDef,
 ):
     pass
 
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -495,74 +469,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListAppMonitorsResponseTypeDef = TypedDict(
-    "ListAppMonitorsResponseTypeDef",
-    {
-        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppMonitorRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateAppMonitorRequestRequestTypeDef(
-    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Domain": str,
-    },
-    total=False,
-)
-
-class UpdateAppMonitorRequestRequestTypeDef(
-    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
-):
-    pass
-
 BatchCreateRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "MetricDefinition": MetricDefinitionRequestTypeDef,
+        "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
     },
 )
 
 _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
@@ -608,27 +528,157 @@
     pass
 
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppMonitorResponseTypeDef = TypedDict(
+    "CreateAppMonitorResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppMonitorDataResponseTypeDef = TypedDict(
+    "GetAppMonitorDataResponseTypeDef",
+    {
+        "Events": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppMonitorsResponseTypeDef = TypedDict(
+    "ListAppMonitorsResponseTypeDef",
+    {
+        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchDeleteRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitionIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+    },
+)
+_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    {
+        "DestinationArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
+    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+):
+    pass
+
+ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "AppMonitorName": str,
+    },
+)
+_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
+    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+):
+    pass
+
+_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppMonitorRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateAppMonitorRequestRequestTypeDef(
+    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Domain": str,
+    },
+    total=False,
+)
+
+class UpdateAppMonitorRequestRequestTypeDef(
+    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
+):
+    pass
+
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
         "CwLog": CwLogTypeDef,
     },
     total=False,
 )
@@ -640,15 +690,15 @@
         "TimeRange": TimeRangeTypeDef,
     },
 )
 _OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef = TypedDict(
     "_OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     {
         "Filters": Sequence[QueryFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef(
     _RequiredGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     _OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
@@ -678,15 +728,15 @@
     pass
 
 ListRumMetricsDestinationsResponseTypeDef = TypedDict(
     "ListRumMetricsDestinationsResponseTypeDef",
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRumEventsRequestRequestTypeDef = TypedDict(
     "PutRumEventsRequestRequestTypeDef",
     {
         "AppMonitorDetails": AppMonitorDetailsTypeDef,
@@ -698,24 +748,24 @@
 )
 
 BatchCreateRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchCreateRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "AppMonitorConfiguration": AppMonitorConfigurationOutputTypeDef,
         "Created": str,
-        "CustomEvents": CustomEventsTypeDef,
+        "CustomEvents": CustomEventsOutputTypeDef,
         "DataStorage": DataStorageTypeDef,
         "Domain": str,
         "Id": str,
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
@@ -723,10 +773,10 @@
     total=False,
 )
 
 GetAppMonitorResponseTypeDef = TypedDict(
     "GetAppMonitorResponseTypeDef",
     {
         "AppMonitor": AppMonitorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/PKG-INFO` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rum"></a>
 
 # mypy-boto3-rum
 
 [![PyPI - mypy-boto3-rum](https://img.shields.io/pypi/v/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rum?color=blue)](https://pypistats.org/packages/mypy-boto3-rum)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,66 +338,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_rum.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rum.type_defs import (
+    AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
-    CustomEventsTypeDef,
+    CustomEventsOutputTypeDef,
+    MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CreateAppMonitorResponseTypeDef,
+    CustomEventsTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
-    GetAppMonitorDataResponseTypeDef,
     GetAppMonitorRequestRequestTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
+    CreateAppMonitorResponseTypeDef,
+    GetAppMonitorDataResponseTypeDef,
+    ListAppMonitorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
+    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
+    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+    CreateAppMonitorRequestRequestTypeDef,
+    UpdateAppMonitorRequestRequestTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
     GetAppMonitorResponseTypeDef,
 )
 
 
-def get_structure() -> AppMonitorConfigurationTypeDef:
+def get_structure() -> AppMonitorConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rum-1.28.0/mypy_boto3_rum.egg-info/SOURCES.txt` & `mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.0/setup.py` & `mypy-boto3-rum-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rum",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchRUM 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudWatchRUM 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

