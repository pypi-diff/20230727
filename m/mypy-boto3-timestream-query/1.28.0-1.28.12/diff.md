# Comparing `tmp/mypy-boto3-timestream-query-1.28.0.tar.gz` & `tmp/mypy-boto3-timestream-query-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-query-1.28.0.tar", last modified: Thu Jul  6 21:00:47 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-query-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
```

## Comparing `mypy-boto3-timestream-query-1.28.0.tar` & `mypy-boto3-timestream-query-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.990450 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-06 20:57:13.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-06 20:57:13.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.485435 mypy-boto3-timestream-query-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-27 11:49:46.481435 mypy-boto3-timestream-query-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.473435 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.481435 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.485435 mypy-boto3-timestream-query-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/setup.py
```

### Comparing `mypy-boto3-timestream-query-1.28.0/LICENSE` & `mypy-boto3-timestream-query-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.0/PKG-INFO` & `mypy-boto3-timestream-query-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.0
-Summary: Type annotations for boto3.TimestreamQuery 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.TimestreamQuery 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-timestream-query"></a>
 
 # mypy-boto3-timestream-query
 
 [![PyPI - mypy-boto3-timestream-query](https://img.shields.io/pypi/v/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,67 +339,79 @@
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
+    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    EmptyResponseMetadataTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    SnsConfigurationOutputTypeDef,
     SnsConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ResponseMetadataTypeDef,
+    ScheduleConfigurationOutputTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateScheduledQueryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
+    ErrorReportConfigurationOutputTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    QueryRequestQueryPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MixedMeasureMappingOutputTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
+    TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
-    CreateScheduledQueryRequestRequestTypeDef,
     ScheduledQueryDescriptionTypeDef,
+    CreateScheduledQueryRequestRequestTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
 def get_structure() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-timestream-query-1.28.0/README.md` & `mypy-boto3-timestream-query-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-timestream-query"></a>
 
 # mypy-boto3-timestream-query
 
 [![PyPI - mypy-boto3-timestream-query](https://img.shields.io/pypi/v/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,67 +307,79 @@
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
+    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    EmptyResponseMetadataTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    SnsConfigurationOutputTypeDef,
     SnsConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ResponseMetadataTypeDef,
+    ScheduleConfigurationOutputTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateScheduledQueryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
+    ErrorReportConfigurationOutputTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    QueryRequestQueryPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MixedMeasureMappingOutputTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
+    TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
-    CreateScheduledQueryRequestRequestTypeDef,
     ScheduledQueryDescriptionTypeDef,
+    CreateScheduledQueryRequestRequestTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
 def get_structure() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.py` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.pyi` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__main__.py` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamQuery 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.TimestreamQuery 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.py` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.pyi` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.py` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
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
@@ -266,26 +267,28 @@
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

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.pyi` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,15 @@
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
@@ -264,26 +265,28 @@
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

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.py` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,30 +50,30 @@
 class ListScheduledQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScheduledQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
         """
 
 
@@ -84,13 +84,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.pyi` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,29 +47,29 @@
 class ListScheduledQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScheduledQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listscheduledqueriespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#listtagsforresourcepaginator)
         """
 
 class QueryPaginator(Paginator):
@@ -79,13 +79,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.py` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -29,85 +29,99 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
-    "CreateScheduledQueryResponseTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
+    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ExecutionStatsTypeDef",
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
+    "SnsConfigurationOutputTypeDef",
     "SnsConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
-    "QueryRequestQueryPaginateTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
-    "ResponseMetadataTypeDef",
+    "ScheduleConfigurationOutputTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateScheduledQueryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "ErrorReportConfigurationOutputTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "QueryRequestQueryPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
+    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "CreateScheduledQueryRequestRequestTypeDef",
     "ScheduledQueryDescriptionTypeDef",
+    "CreateScheduledQueryRequestRequestTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CancellationMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Type": Dict[str, Any],
@@ -117,19 +131,17 @@
     "_OptionalColumnInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class ColumnInfoTypeDef(_RequiredColumnInfoTypeDef, _OptionalColumnInfoTypeDef):
     pass
 
-
 ScheduleConfigurationTypeDef = TypedDict(
     "ScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
@@ -137,26 +149,18 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateScheduledQueryResponseTypeDef = TypedDict(
-    "CreateScheduledQueryResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List[Dict[str, Any]],
+        "Data": List["DatumTypeDef"],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
@@ -182,28 +186,49 @@
 DescribeScheduledQueryRequestRequestTypeDef = TypedDict(
     "DescribeScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
     },
 )
 
+DimensionMappingOutputTypeDef = TypedDict(
+    "DimensionMappingOutputTypeDef",
+    {
+        "Name": str,
+        "DimensionValueType": Literal["VARCHAR"],
+    },
+)
+
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_RequiredS3ConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3ConfigurationOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BucketName": str,
     },
 )
+_OptionalS3ConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3ConfigurationOutputTypeDef",
+    {
+        "ObjectKeyPrefix": str,
+        "EncryptionOption": S3EncryptionOptionType,
+    },
+    total=False,
+)
+
+class S3ConfigurationOutputTypeDef(
+    _RequiredS3ConfigurationOutputTypeDef, _OptionalS3ConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
@@ -212,19 +237,17 @@
     {
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
     },
     total=False,
 )
 
-
 class S3ConfigurationTypeDef(_RequiredS3ConfigurationTypeDef, _OptionalS3ConfigurationTypeDef):
     pass
 
-
 S3ReportLocationTypeDef = TypedDict(
     "S3ReportLocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
@@ -241,96 +264,101 @@
     "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ExecuteScheduledQueryRequestRequestTypeDef(
     _RequiredExecuteScheduledQueryRequestRequestTypeDef,
     _OptionalExecuteScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
-
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
         "QueryResultRows": int,
     },
     total=False,
 )
 
-ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListScheduledQueriesRequestRequestTypeDef = TypedDict(
     "ListScheduledQueriesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+class ListTagsForResourceRequestRequestTypeDef(
+    _RequiredListTagsForResourceRequestRequestTypeDef,
+    _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
 
-_RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestRequestTypeDef",
+_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
     {
-        "ResourceARN": str,
+        "SourceColumn": str,
+        "MeasureValueType": ScalarMeasureValueTypeType,
     },
 )
-_OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestRequestTypeDef",
+_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
-
-class ListTagsForResourceRequestRequestTypeDef(
-    _RequiredListTagsForResourceRequestRequestTypeDef,
-    _OptionalListTagsForResourceRequestRequestTypeDef,
+class MultiMeasureAttributeMappingOutputTypeDef(
+    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
+    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
 ):
     pass
 
-
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
 )
@@ -338,36 +366,31 @@
     "_OptionalMultiMeasureAttributeMappingTypeDef",
     {
         "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-
-SnsConfigurationTypeDef = TypedDict(
-    "SnsConfigurationTypeDef",
+SnsConfigurationOutputTypeDef = TypedDict(
+    "SnsConfigurationOutputTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+SnsConfigurationTypeDef = TypedDict(
+    "SnsConfigurationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TopicArn": str,
     },
-    total=False,
 )
 
 ParameterMappingTypeDef = TypedDict(
     "ParameterMappingTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
@@ -384,55 +407,31 @@
     "_OptionalPrepareQueryRequestRequestTypeDef",
     {
         "ValidateOnly": bool,
     },
     total=False,
 )
 
-
 class PrepareQueryRequestRequestTypeDef(
     _RequiredPrepareQueryRequestRequestTypeDef, _OptionalPrepareQueryRequestRequestTypeDef
 ):
     pass
 
-
 SelectColumnTypeDef = TypedDict(
     "SelectColumnTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
         "DatabaseName": str,
         "TableName": str,
         "Aliased": bool,
     },
     total=False,
 )
 
-_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryRequestQueryPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryRequestQueryPaginateTypeDef",
-    {
-        "ClientToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryRequestQueryPaginateTypeDef(
-    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
-):
-    pass
-
-
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -441,39 +440,33 @@
         "ClientToken": str,
         "NextToken": str,
         "MaxRows": int,
     },
     total=False,
 )
 
-
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
-
 QueryStatusTypeDef = TypedDict(
     "QueryStatusTypeDef",
     {
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ScheduleConfigurationOutputTypeDef = TypedDict(
+    "ScheduleConfigurationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScheduleExpression": str,
     },
 )
 
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
@@ -505,20 +498,34 @@
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CancellationMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledQueryResponseTypeDef = TypedDict(
+    "CreateScheduledQueryResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -538,15 +545,22 @@
     total=False,
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ErrorReportConfigurationOutputTypeDef = TypedDict(
+    "ErrorReportConfigurationOutputTypeDef",
+    {
+        "S3Configuration": S3ConfigurationOutputTypeDef,
     },
 )
 
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -557,14 +571,112 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
+ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryRequestQueryPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryRequestQueryPaginateTypeDef",
+    {
+        "ClientToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class QueryRequestQueryPaginateTypeDef(
+    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
+):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_RequiredMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+    },
+)
+_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_OptionalMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureName": str,
+        "SourceColumn": str,
+        "TargetMeasureName": str,
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class MixedMeasureMappingOutputTypeDef(
+    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
+):
+    pass
+
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -574,68 +686,71 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
-
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+NotificationConfigurationOutputTypeDef = TypedDict(
+    "NotificationConfigurationOutputTypeDef",
+    {
+        "SnsConfiguration": SnsConfigurationOutputTypeDef,
+    },
+)
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "SnsConfiguration": SnsConfigurationTypeDef,
     },
 )
 
 PrepareQueryResponseTypeDef = TypedDict(
     "PrepareQueryResponseTypeDef",
     {
         "QueryString": str,
         "Columns": List[SelectColumnTypeDef],
         "Parameters": List[ParameterMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": TimestreamDestinationTypeDef,
@@ -652,14 +767,38 @@
         "ExecutionStats": ExecutionStatsTypeDef,
         "ErrorReportLocation": ErrorReportLocationTypeDef,
         "FailureReason": str,
     },
     total=False,
 )
 
+_RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTimestreamConfigurationOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "TimeColumn": str,
+        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+    },
+)
+_OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTimestreamConfigurationOutputTypeDef",
+    {
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+class TimestreamConfigurationOutputTypeDef(
+    _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -671,127 +810,126 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class TimestreamConfigurationTypeDef(
     _RequiredTimestreamConfigurationTypeDef, _OptionalTimestreamConfigurationTypeDef
 ):
     pass
 
-
 _RequiredScheduledQueryTypeDef = TypedDict(
     "_RequiredScheduledQueryTypeDef",
     {
         "Arn": str,
         "Name": str,
         "State": ScheduledQueryStateType,
     },
 )
 _OptionalScheduledQueryTypeDef = TypedDict(
     "_OptionalScheduledQueryTypeDef",
     {
         "CreationTime": datetime,
         "PreviousInvocationTime": datetime,
         "NextInvocationTime": datetime,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
         "TargetDestination": TargetDestinationTypeDef,
         "LastRunStatus": ScheduledQueryRunStatusType,
     },
     total=False,
 )
 
-
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
+    },
+)
 
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
 
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
+_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
+    "_RequiredScheduledQueryDescriptionTypeDef",
     {
+        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "State": ScheduledQueryStateType,
+        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
+        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
     },
 )
-_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
+_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
+    "_OptionalScheduledQueryDescriptionTypeDef",
     {
-        "TargetConfiguration": TargetConfigurationTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
+        "PreviousInvocationTime": datetime,
+        "NextInvocationTime": datetime,
+        "TargetConfiguration": TargetConfigurationOutputTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
+        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
+        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-
-class CreateScheduledQueryRequestRequestTypeDef(
-    _RequiredCreateScheduledQueryRequestRequestTypeDef,
-    _OptionalCreateScheduledQueryRequestRequestTypeDef,
+class ScheduledQueryDescriptionTypeDef(
+    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
-
-_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
-    "_RequiredScheduledQueryDescriptionTypeDef",
+_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
-        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
-    "_OptionalScheduledQueryDescriptionTypeDef",
+_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
     {
-        "CreationTime": datetime,
-        "PreviousInvocationTime": datetime,
-        "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
-        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-
-class ScheduledQueryDescriptionTypeDef(
-    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
+class CreateScheduledQueryRequestRequestTypeDef(
+    _RequiredCreateScheduledQueryRequestRequestTypeDef,
+    _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.pyi` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,84 +29,100 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
-    "CreateScheduledQueryResponseTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
+    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ExecutionStatsTypeDef",
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
+    "SnsConfigurationOutputTypeDef",
     "SnsConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
-    "QueryRequestQueryPaginateTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
-    "ResponseMetadataTypeDef",
+    "ScheduleConfigurationOutputTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateScheduledQueryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "ErrorReportConfigurationOutputTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "QueryRequestQueryPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
+    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "CreateScheduledQueryRequestRequestTypeDef",
     "ScheduledQueryDescriptionTypeDef",
+    "CreateScheduledQueryRequestRequestTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CancellationMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Type": Dict[str, Any],
@@ -116,17 +132,19 @@
     "_OptionalColumnInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class ColumnInfoTypeDef(_RequiredColumnInfoTypeDef, _OptionalColumnInfoTypeDef):
     pass
 
+
 ScheduleConfigurationTypeDef = TypedDict(
     "ScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
@@ -134,26 +152,18 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateScheduledQueryResponseTypeDef = TypedDict(
-    "CreateScheduledQueryResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List[Dict[str, Any]],
+        "Data": List["DatumTypeDef"],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
@@ -179,28 +189,51 @@
 DescribeScheduledQueryRequestRequestTypeDef = TypedDict(
     "DescribeScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
     },
 )
 
+DimensionMappingOutputTypeDef = TypedDict(
+    "DimensionMappingOutputTypeDef",
+    {
+        "Name": str,
+        "DimensionValueType": Literal["VARCHAR"],
+    },
+)
+
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_RequiredS3ConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3ConfigurationOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BucketName": str,
     },
 )
+_OptionalS3ConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3ConfigurationOutputTypeDef",
+    {
+        "ObjectKeyPrefix": str,
+        "EncryptionOption": S3EncryptionOptionType,
+    },
+    total=False,
+)
+
+
+class S3ConfigurationOutputTypeDef(
+    _RequiredS3ConfigurationOutputTypeDef, _OptionalS3ConfigurationOutputTypeDef
+):
+    pass
+
 
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
@@ -209,17 +242,19 @@
     {
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
     },
     total=False,
 )
 
+
 class S3ConfigurationTypeDef(_RequiredS3ConfigurationTypeDef, _OptionalS3ConfigurationTypeDef):
     pass
 
+
 S3ReportLocationTypeDef = TypedDict(
     "S3ReportLocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
@@ -236,90 +271,107 @@
     "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ExecuteScheduledQueryRequestRequestTypeDef(
     _RequiredExecuteScheduledQueryRequestRequestTypeDef,
     _OptionalExecuteScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
+
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
         "QueryResultRows": int,
     },
     total=False,
 )
 
-ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListScheduledQueriesRequestRequestTypeDef = TypedDict(
     "ListScheduledQueriesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+_OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+
+class ListTagsForResourceRequestRequestTypeDef(
+    _RequiredListTagsForResourceRequestRequestTypeDef,
+    _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestRequestTypeDef",
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "ResourceARN": str,
+        "Key": str,
+        "Value": str,
     },
 )
-_OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestRequestTypeDef",
+
+_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "SourceColumn": str,
+        "MeasureValueType": ScalarMeasureValueTypeType,
+    },
+)
+_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
+    {
+        "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
-class ListTagsForResourceRequestRequestTypeDef(
-    _RequiredListTagsForResourceRequestRequestTypeDef,
-    _OptionalListTagsForResourceRequestRequestTypeDef,
+
+class MultiMeasureAttributeMappingOutputTypeDef(
+    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
+    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
 ):
     pass
 
+
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
 )
@@ -327,34 +379,33 @@
     "_OptionalMultiMeasureAttributeMappingTypeDef",
     {
         "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-SnsConfigurationTypeDef = TypedDict(
-    "SnsConfigurationTypeDef",
+
+SnsConfigurationOutputTypeDef = TypedDict(
+    "SnsConfigurationOutputTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+SnsConfigurationTypeDef = TypedDict(
+    "SnsConfigurationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TopicArn": str,
     },
-    total=False,
 )
 
 ParameterMappingTypeDef = TypedDict(
     "ParameterMappingTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
@@ -371,51 +422,33 @@
     "_OptionalPrepareQueryRequestRequestTypeDef",
     {
         "ValidateOnly": bool,
     },
     total=False,
 )
 
+
 class PrepareQueryRequestRequestTypeDef(
     _RequiredPrepareQueryRequestRequestTypeDef, _OptionalPrepareQueryRequestRequestTypeDef
 ):
     pass
 
+
 SelectColumnTypeDef = TypedDict(
     "SelectColumnTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
         "DatabaseName": str,
         "TableName": str,
         "Aliased": bool,
     },
     total=False,
 )
 
-_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryRequestQueryPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryRequestQueryPaginateTypeDef",
-    {
-        "ClientToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class QueryRequestQueryPaginateTypeDef(
-    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
-):
-    pass
-
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -424,37 +457,35 @@
         "ClientToken": str,
         "NextToken": str,
         "MaxRows": int,
     },
     total=False,
 )
 
+
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
+
 QueryStatusTypeDef = TypedDict(
     "QueryStatusTypeDef",
     {
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ScheduleConfigurationOutputTypeDef = TypedDict(
+    "ScheduleConfigurationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScheduleExpression": str,
     },
 )
 
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
@@ -486,20 +517,34 @@
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CancellationMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledQueryResponseTypeDef = TypedDict(
+    "CreateScheduledQueryResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -519,15 +564,22 @@
     total=False,
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ErrorReportConfigurationOutputTypeDef = TypedDict(
+    "ErrorReportConfigurationOutputTypeDef",
+    {
+        "S3Configuration": S3ConfigurationOutputTypeDef,
     },
 )
 
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -538,14 +590,120 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
+ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryRequestQueryPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryRequestQueryPaginateTypeDef",
+    {
+        "ClientToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryRequestQueryPaginateTypeDef(
+    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
+):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_RequiredMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+    },
+)
+_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_OptionalMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureName": str,
+        "SourceColumn": str,
+        "TargetMeasureName": str,
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class MixedMeasureMappingOutputTypeDef(
+    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
+):
+    pass
+
+
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
+
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -555,64 +713,75 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+
+NotificationConfigurationOutputTypeDef = TypedDict(
+    "NotificationConfigurationOutputTypeDef",
+    {
+        "SnsConfiguration": SnsConfigurationOutputTypeDef,
+    },
+)
+
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "SnsConfiguration": SnsConfigurationTypeDef,
     },
 )
 
 PrepareQueryResponseTypeDef = TypedDict(
     "PrepareQueryResponseTypeDef",
     {
         "QueryString": str,
         "Columns": List[SelectColumnTypeDef],
         "Parameters": List[ParameterMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": TimestreamDestinationTypeDef,
@@ -629,14 +798,40 @@
         "ExecutionStats": ExecutionStatsTypeDef,
         "ErrorReportLocation": ErrorReportLocationTypeDef,
         "FailureReason": str,
     },
     total=False,
 )
 
+_RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTimestreamConfigurationOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "TimeColumn": str,
+        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+    },
+)
+_OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTimestreamConfigurationOutputTypeDef",
+    {
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+
+class TimestreamConfigurationOutputTypeDef(
+    _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -648,119 +843,134 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class TimestreamConfigurationTypeDef(
     _RequiredTimestreamConfigurationTypeDef, _OptionalTimestreamConfigurationTypeDef
 ):
     pass
 
+
 _RequiredScheduledQueryTypeDef = TypedDict(
     "_RequiredScheduledQueryTypeDef",
     {
         "Arn": str,
         "Name": str,
         "State": ScheduledQueryStateType,
     },
 )
 _OptionalScheduledQueryTypeDef = TypedDict(
     "_OptionalScheduledQueryTypeDef",
     {
         "CreationTime": datetime,
         "PreviousInvocationTime": datetime,
         "NextInvocationTime": datetime,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
         "TargetDestination": TargetDestinationTypeDef,
         "LastRunStatus": ScheduledQueryRunStatusType,
     },
     total=False,
 )
 
+
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
+
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
+    },
+)
+
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
 
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
+_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
+    "_RequiredScheduledQueryDescriptionTypeDef",
     {
+        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "State": ScheduledQueryStateType,
+        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
+        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
     },
 )
-_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
+_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
+    "_OptionalScheduledQueryDescriptionTypeDef",
     {
-        "TargetConfiguration": TargetConfigurationTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
+        "PreviousInvocationTime": datetime,
+        "NextInvocationTime": datetime,
+        "TargetConfiguration": TargetConfigurationOutputTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
+        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
+        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-class CreateScheduledQueryRequestRequestTypeDef(
-    _RequiredCreateScheduledQueryRequestRequestTypeDef,
-    _OptionalCreateScheduledQueryRequestRequestTypeDef,
+
+class ScheduledQueryDescriptionTypeDef(
+    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
-_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
-    "_RequiredScheduledQueryDescriptionTypeDef",
+
+_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
-        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
-    "_OptionalScheduledQueryDescriptionTypeDef",
+_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
     {
-        "CreationTime": datetime,
-        "PreviousInvocationTime": datetime,
-        "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
-        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-class ScheduledQueryDescriptionTypeDef(
-    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
+
+class CreateScheduledQueryRequestRequestTypeDef(
+    _RequiredCreateScheduledQueryRequestRequestTypeDef,
+    _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/PKG-INFO` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.0
-Summary: Type annotations for boto3.TimestreamQuery 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.TimestreamQuery 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-timestream-query"></a>
 
 # mypy-boto3-timestream-query
 
 [![PyPI - mypy-boto3-timestream-query](https://img.shields.io/pypi/v/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,67 +339,79 @@
 
 `mypy_boto3_timestream_query.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
+    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    EmptyResponseMetadataTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    SnsConfigurationOutputTypeDef,
     SnsConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ResponseMetadataTypeDef,
+    ScheduleConfigurationOutputTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateScheduledQueryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
+    ErrorReportConfigurationOutputTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    QueryRequestQueryPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MixedMeasureMappingOutputTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
+    TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
-    CreateScheduledQueryRequestRequestTypeDef,
     ScheduledQueryDescriptionTypeDef,
+    CreateScheduledQueryRequestRequestTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
 def get_structure() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt` & `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.0/setup.py` & `mypy-boto3-timestream-query-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-query",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamQuery 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.TimestreamQuery 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

