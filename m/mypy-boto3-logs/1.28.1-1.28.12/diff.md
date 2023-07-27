# Comparing `tmp/mypy-boto3-logs-1.28.1.tar.gz` & `tmp/mypy-boto3-logs-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-logs-1.28.1.tar", last modified: Fri Jul  7 19:32:38 2023, max compression
+gzip compressed data, was "mypy-boto3-logs-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
```

## Comparing `mypy-boto3-logs-1.28.1.tar` & `mypy-boto3-logs-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.891384 mypy-boto3-logs-1.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-07-07 19:32:38.891384 mypy-boto3-logs-1.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.891384 mypy-boto3-logs-1.28.1/mypy_boto3_logs/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38327 2023-07-07 19:32:16.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38260 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-07 19:32:16.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-07 19:32:16.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-07 19:32:16.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-07-07 19:32:16.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37076 2023-07-07 19:32:17.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-07 19:32:17.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.891384 mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-07-07 19:32:38.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 19:32:38.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 19:32:38.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 19:32:38.000000 mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:32:38.891384 mypy-boto3-logs-1.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-07 19:32:15.000000 mypy-boto3-logs-1.28.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.772453 mypy-boto3-logs-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-07-27 05:34:57.772453 mypy-boto3-logs-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.768453 mypy-boto3-logs-1.28.12/mypy_boto3_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38327 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38260 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37801 2023-07-27 05:25:34.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37766 2023-07-27 05:25:34.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.772453 mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-07-27 05:34:57.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 05:34:57.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 05:34:57.000000 mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.772453 mypy-boto3-logs-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-27 05:25:33.000000 mypy-boto3-logs-1.28.12/setup.py
```

### Comparing `mypy-boto3-logs-1.28.1/LICENSE` & `mypy-boto3-logs-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.1/PKG-INFO` & `mypy-boto3-logs-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.28.1
-Summary: Type annotations for boto3.CloudWatchLogs 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchLogs 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-logs"></a>
 
 # mypy-boto3-logs
 
 [![PyPI - mypy-boto3-logs](https://img.shields.io/pypi/v/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-logs?color=blue)](https://pypistats.org/packages/mypy-boto3-logs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-logs)](https://pepy.tech/project/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,103 +371,104 @@
 
 ```python
 from mypy_boto3_logs.type_defs import (
     AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateExportTaskResponseTypeDef,
     CreateLogGroupRequestRequestTypeDef,
     CreateLogStreamRequestRequestTypeDef,
     DeleteAccountPolicyRequestRequestTypeDef,
     DeleteDataProtectionPolicyRequestRequestTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteLogGroupRequestRequestTypeDef,
     DeleteLogStreamRequestRequestTypeDef,
     DeleteMetricFilterRequestRequestTypeDef,
     DeleteQueryDefinitionRequestRequestTypeDef,
+    DeleteQueryDefinitionResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteSubscriptionFilterRequestRequestTypeDef,
     DescribeAccountPoliciesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
     DescribeDestinationsRequestRequestTypeDef,
     DestinationTypeDef,
+    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
+    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
     DescribeLogGroupsRequestRequestTypeDef,
     LogGroupTypeDef,
+    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
     DescribeLogStreamsRequestRequestTypeDef,
     LogStreamTypeDef,
+    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
     DescribeMetricFiltersRequestRequestTypeDef,
+    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
     DescribeQueriesRequestRequestTypeDef,
     QueryInfoTypeDef,
     DescribeQueryDefinitionsRequestRequestTypeDef,
     QueryDefinitionTypeDef,
+    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
     DescribeResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
+    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
     DescribeSubscriptionFiltersRequestRequestTypeDef,
     SubscriptionFilterTypeDef,
     DisassociateKmsKeyRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportTaskExecutionInfoTypeDef,
     ExportTaskStatusTypeDef,
+    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     FilterLogEventsRequestRequestTypeDef,
     FilteredLogEventTypeDef,
     SearchedLogStreamTypeDef,
     GetDataProtectionPolicyRequestRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetLogEventsRequestRequestTypeDef,
     OutputLogEventTypeDef,
     GetLogGroupFieldsRequestRequestTypeDef,
     LogGroupFieldTypeDef,
     GetLogRecordRequestRequestTypeDef,
+    GetLogRecordResponseTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     ResultFieldTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupRequestRequestTypeDef,
+    ListTagsLogGroupResponseTypeDef,
     MetricFilterMatchRecordTypeDef,
+    MetricTransformationOutputTypeDef,
     MetricTransformationTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountPolicyRequestRequestTypeDef,
     PutDataProtectionPolicyRequestRequestTypeDef,
+    PutDataProtectionPolicyResponseTypeDef,
     PutDestinationPolicyRequestRequestTypeDef,
     PutDestinationRequestRequestTypeDef,
     RejectedLogEventsInfoTypeDef,
     PutQueryDefinitionRequestRequestTypeDef,
+    PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     PutSubscriptionFilterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
     StopQueryRequestRequestTypeDef,
+    StopQueryResponseTypeDef,
     TagLogGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestMetricFilterRequestRequestTypeDef,
     UntagLogGroupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateExportTaskResponseTypeDef,
-    DeleteQueryDefinitionResponseTypeDef,
     DescribeAccountPoliciesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetLogRecordResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsLogGroupResponseTypeDef,
     PutAccountPolicyResponseTypeDef,
-    PutDataProtectionPolicyResponseTypeDef,
-    PutQueryDefinitionResponseTypeDef,
-    StartQueryResponseTypeDef,
-    StopQueryResponseTypeDef,
-    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
-    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
-    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
-    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
-    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
-    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     DescribeDestinationsResponseTypeDef,
     PutDestinationResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
     DescribeResourcePoliciesResponseTypeDef,
```

### Comparing `mypy-boto3-logs-1.28.1/README.md` & `mypy-boto3-logs-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-logs"></a>
 
 # mypy-boto3-logs
 
 [![PyPI - mypy-boto3-logs](https://img.shields.io/pypi/v/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-logs?color=blue)](https://pypistats.org/packages/mypy-boto3-logs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-logs)](https://pepy.tech/project/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,103 +339,104 @@
 
 ```python
 from mypy_boto3_logs.type_defs import (
     AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateExportTaskResponseTypeDef,
     CreateLogGroupRequestRequestTypeDef,
     CreateLogStreamRequestRequestTypeDef,
     DeleteAccountPolicyRequestRequestTypeDef,
     DeleteDataProtectionPolicyRequestRequestTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteLogGroupRequestRequestTypeDef,
     DeleteLogStreamRequestRequestTypeDef,
     DeleteMetricFilterRequestRequestTypeDef,
     DeleteQueryDefinitionRequestRequestTypeDef,
+    DeleteQueryDefinitionResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteSubscriptionFilterRequestRequestTypeDef,
     DescribeAccountPoliciesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
     DescribeDestinationsRequestRequestTypeDef,
     DestinationTypeDef,
+    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
+    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
     DescribeLogGroupsRequestRequestTypeDef,
     LogGroupTypeDef,
+    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
     DescribeLogStreamsRequestRequestTypeDef,
     LogStreamTypeDef,
+    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
     DescribeMetricFiltersRequestRequestTypeDef,
+    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
     DescribeQueriesRequestRequestTypeDef,
     QueryInfoTypeDef,
     DescribeQueryDefinitionsRequestRequestTypeDef,
     QueryDefinitionTypeDef,
+    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
     DescribeResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
+    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
     DescribeSubscriptionFiltersRequestRequestTypeDef,
     SubscriptionFilterTypeDef,
     DisassociateKmsKeyRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportTaskExecutionInfoTypeDef,
     ExportTaskStatusTypeDef,
+    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     FilterLogEventsRequestRequestTypeDef,
     FilteredLogEventTypeDef,
     SearchedLogStreamTypeDef,
     GetDataProtectionPolicyRequestRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetLogEventsRequestRequestTypeDef,
     OutputLogEventTypeDef,
     GetLogGroupFieldsRequestRequestTypeDef,
     LogGroupFieldTypeDef,
     GetLogRecordRequestRequestTypeDef,
+    GetLogRecordResponseTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     ResultFieldTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupRequestRequestTypeDef,
+    ListTagsLogGroupResponseTypeDef,
     MetricFilterMatchRecordTypeDef,
+    MetricTransformationOutputTypeDef,
     MetricTransformationTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountPolicyRequestRequestTypeDef,
     PutDataProtectionPolicyRequestRequestTypeDef,
+    PutDataProtectionPolicyResponseTypeDef,
     PutDestinationPolicyRequestRequestTypeDef,
     PutDestinationRequestRequestTypeDef,
     RejectedLogEventsInfoTypeDef,
     PutQueryDefinitionRequestRequestTypeDef,
+    PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     PutSubscriptionFilterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
     StopQueryRequestRequestTypeDef,
+    StopQueryResponseTypeDef,
     TagLogGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestMetricFilterRequestRequestTypeDef,
     UntagLogGroupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateExportTaskResponseTypeDef,
-    DeleteQueryDefinitionResponseTypeDef,
     DescribeAccountPoliciesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetLogRecordResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsLogGroupResponseTypeDef,
     PutAccountPolicyResponseTypeDef,
-    PutDataProtectionPolicyResponseTypeDef,
-    PutQueryDefinitionResponseTypeDef,
-    StartQueryResponseTypeDef,
-    StopQueryResponseTypeDef,
-    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
-    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
-    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
-    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
-    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
-    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     DescribeDestinationsResponseTypeDef,
     PutDestinationResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
     DescribeResourcePoliciesResponseTypeDef,
```

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/__init__.py` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/__init__.pyi` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/__main__.py` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchLogs 1.28.1\nVersion:         1.28.1\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudWatchLogs 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.1")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/client.py` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/client.pyi` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/literals.py` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -298,26 +299,28 @@
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

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/literals.pyi` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,15 @@
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
@@ -296,26 +297,28 @@
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

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/paginator.py` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,176 +61,165 @@
     "DescribeMetricFiltersPaginator",
     "DescribeQueriesPaginator",
     "DescribeResourcePoliciesPaginator",
     "DescribeSubscriptionFiltersPaginator",
     "FilterLogEventsPaginator",
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
 class DescribeDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
     """
 
     def paginate(
-        self, *, DestinationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DestinationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
         """
 
-
 class DescribeExportTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
         """
 
-
 class DescribeLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
     """
 
     def paginate(
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         includeLinkedAccounts: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
         """
 
-
 class DescribeLogStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
         """
 
-
 class DescribeMetricFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         metricName: str = ...,
         metricNamespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMetricFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
         """
 
-
 class DescribeQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
         """
 
-
 class DescribeResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
         """
 
-
 class DescribeSubscriptionFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubscriptionFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
         """
 
-
 class FilterLogEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
     """
 
     def paginate(
@@ -241,13 +230,13 @@
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         interleaved: bool = ...,
         unmask: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[FilterLogEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
         """
```

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/paginator.pyi` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,165 +61,176 @@
     "DescribeMetricFiltersPaginator",
     "DescribeQueriesPaginator",
     "DescribeResourcePoliciesPaginator",
     "DescribeSubscriptionFiltersPaginator",
     "FilterLogEventsPaginator",
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
 class DescribeDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
     """
 
     def paginate(
-        self, *, DestinationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DestinationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
         """
 
+
 class DescribeExportTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
         """
 
+
 class DescribeLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
     """
 
     def paginate(
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         includeLinkedAccounts: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
         """
 
+
 class DescribeLogStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
         """
 
+
 class DescribeMetricFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         metricName: str = ...,
         metricNamespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMetricFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
         """
 
+
 class DescribeQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
         """
 
+
 class DescribeResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
         """
 
+
 class DescribeSubscriptionFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubscriptionFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
         """
 
+
 class FilterLogEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
     """
 
     def paginate(
@@ -230,13 +241,13 @@
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         interleaved: bool = ...,
         unmask: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[FilterLogEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
         """
```

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/type_defs.py` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,103 +34,104 @@
 
 
 __all__ = (
     "AccountPolicyTypeDef",
     "AssociateKmsKeyRequestRequestTypeDef",
     "CancelExportTaskRequestRequestTypeDef",
     "CreateExportTaskRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateExportTaskResponseTypeDef",
     "CreateLogGroupRequestRequestTypeDef",
     "CreateLogStreamRequestRequestTypeDef",
     "DeleteAccountPolicyRequestRequestTypeDef",
     "DeleteDataProtectionPolicyRequestRequestTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteLogGroupRequestRequestTypeDef",
     "DeleteLogStreamRequestRequestTypeDef",
     "DeleteMetricFilterRequestRequestTypeDef",
     "DeleteQueryDefinitionRequestRequestTypeDef",
+    "DeleteQueryDefinitionResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRetentionPolicyRequestRequestTypeDef",
     "DeleteSubscriptionFilterRequestRequestTypeDef",
     "DescribeAccountPoliciesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
     "DescribeDestinationsRequestRequestTypeDef",
     "DestinationTypeDef",
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
     "DescribeLogGroupsRequestRequestTypeDef",
     "LogGroupTypeDef",
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
     "DescribeLogStreamsRequestRequestTypeDef",
     "LogStreamTypeDef",
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
     "DescribeMetricFiltersRequestRequestTypeDef",
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
     "DescribeQueriesRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "DescribeQueryDefinitionsRequestRequestTypeDef",
     "QueryDefinitionTypeDef",
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
     "DescribeResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
+    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
     "DescribeSubscriptionFiltersRequestRequestTypeDef",
     "SubscriptionFilterTypeDef",
     "DisassociateKmsKeyRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportTaskExecutionInfoTypeDef",
     "ExportTaskStatusTypeDef",
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
     "FilterLogEventsRequestRequestTypeDef",
     "FilteredLogEventTypeDef",
     "SearchedLogStreamTypeDef",
     "GetDataProtectionPolicyRequestRequestTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
     "GetLogEventsRequestRequestTypeDef",
     "OutputLogEventTypeDef",
     "GetLogGroupFieldsRequestRequestTypeDef",
     "LogGroupFieldTypeDef",
     "GetLogRecordRequestRequestTypeDef",
+    "GetLogRecordResponseTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "ResultFieldTypeDef",
     "InputLogEventTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTagsLogGroupRequestRequestTypeDef",
+    "ListTagsLogGroupResponseTypeDef",
     "MetricFilterMatchRecordTypeDef",
+    "MetricTransformationOutputTypeDef",
     "MetricTransformationTypeDef",
+    "PaginatorConfigTypeDef",
     "PutAccountPolicyRequestRequestTypeDef",
     "PutDataProtectionPolicyRequestRequestTypeDef",
+    "PutDataProtectionPolicyResponseTypeDef",
     "PutDestinationPolicyRequestRequestTypeDef",
     "PutDestinationRequestRequestTypeDef",
     "RejectedLogEventsInfoTypeDef",
     "PutQueryDefinitionRequestRequestTypeDef",
+    "PutQueryDefinitionResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "PutSubscriptionFilterRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartQueryRequestRequestTypeDef",
+    "StartQueryResponseTypeDef",
     "StopQueryRequestRequestTypeDef",
+    "StopQueryResponseTypeDef",
     "TagLogGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestMetricFilterRequestRequestTypeDef",
     "UntagLogGroupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateExportTaskResponseTypeDef",
-    "DeleteQueryDefinitionResponseTypeDef",
     "DescribeAccountPoliciesResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
-    "GetLogRecordResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsLogGroupResponseTypeDef",
     "PutAccountPolicyResponseTypeDef",
-    "PutDataProtectionPolicyResponseTypeDef",
-    "PutQueryDefinitionResponseTypeDef",
-    "StartQueryResponseTypeDef",
-    "StopQueryResponseTypeDef",
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
     "DescribeDestinationsResponseTypeDef",
     "PutDestinationResponseTypeDef",
     "DescribeLogGroupsResponseTypeDef",
     "DescribeLogStreamsResponseTypeDef",
     "DescribeQueriesResponseTypeDef",
     "DescribeQueryDefinitionsResponseTypeDef",
     "DescribeResourcePoliciesResponseTypeDef",
@@ -214,22 +215,19 @@
 
 class CreateExportTaskRequestRequestTypeDef(
     _RequiredCreateExportTaskRequestRequestTypeDef, _OptionalCreateExportTaskRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateExportTaskResponseTypeDef = TypedDict(
+    "CreateExportTaskResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLogGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -307,14 +305,22 @@
 DeleteQueryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteQueryDefinitionRequestRequestTypeDef",
     {
         "queryDefinitionId": str,
     },
 )
 
+DeleteQueryDefinitionResponseTypeDef = TypedDict(
+    "DeleteQueryDefinitionResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
     total=False,
 )
@@ -353,20 +359,19 @@
 class DescribeAccountPoliciesRequestRequestTypeDef(
     _RequiredDescribeAccountPoliciesRequestRequestTypeDef,
     _OptionalDescribeAccountPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DestinationNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDestinationsRequestRequestTypeDef = TypedDict(
     "DescribeDestinationsRequestRequestTypeDef",
     {
@@ -386,25 +391,47 @@
         "accessPolicy": str,
         "arn": str,
         "creationTime": int,
     },
     total=False,
 )
 
+DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
+    {
+        "taskId": str,
+        "statusCode": ExportTaskStatusCodeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
         "taskId": str,
         "statusCode": ExportTaskStatusCodeType,
         "nextToken": str,
         "limit": int,
     },
     total=False,
 )
 
+DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
+    {
+        "accountIdentifiers": Sequence[str],
+        "logGroupNamePrefix": str,
+        "logGroupNamePattern": str,
+        "includeLinkedAccounts": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLogGroupsRequestRequestTypeDef = TypedDict(
     "DescribeLogGroupsRequestRequestTypeDef",
     {
         "accountIdentifiers": Sequence[str],
         "logGroupNamePrefix": str,
         "logGroupNamePattern": str,
         "nextToken": str,
@@ -426,14 +453,27 @@
         "kmsKeyId": str,
         "dataProtectionStatus": DataProtectionStatusType,
         "inheritedProperties": List[Literal["ACCOUNT_DATA_PROTECTION"]],
     },
     total=False,
 )
 
+DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNamePrefix": str,
+        "orderBy": OrderByType,
+        "descending": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLogStreamsRequestRequestTypeDef = TypedDict(
     "DescribeLogStreamsRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logGroupIdentifier": str,
         "logStreamNamePrefix": str,
         "orderBy": OrderByType,
@@ -455,27 +495,49 @@
         "uploadSequenceToken": str,
         "arn": str,
         "storedBytes": int,
     },
     total=False,
 )
 
+DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "filterNamePrefix": str,
+        "metricName": str,
+        "metricNamespace": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMetricFiltersRequestRequestTypeDef = TypedDict(
     "DescribeMetricFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterNamePrefix": str,
         "nextToken": str,
         "limit": int,
         "metricName": str,
         "metricNamespace": str,
     },
     total=False,
 )
 
+DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "status": QueryStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeQueriesRequestRequestTypeDef = TypedDict(
     "DescribeQueriesRequestRequestTypeDef",
     {
         "logGroupName": str,
         "status": QueryStatusType,
         "maxResults": int,
         "nextToken": str,
@@ -513,14 +575,22 @@
         "queryString": str,
         "lastModified": int,
         "logGroupNames": List[str],
     },
     total=False,
 )
 
+DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeResourcePoliciesRequestRequestTypeDef = TypedDict(
     "DescribeResourcePoliciesRequestRequestTypeDef",
     {
         "nextToken": str,
         "limit": int,
     },
     total=False,
@@ -532,14 +602,37 @@
         "policyName": str,
         "policyDocument": str,
         "lastUpdatedTime": int,
     },
     total=False,
 )
 
+_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "filterNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
+    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscriptionFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
@@ -579,14 +672,21 @@
     {
         "logGroupName": str,
         "resourceIdentifier": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportTaskExecutionInfoTypeDef = TypedDict(
     "ExportTaskExecutionInfoTypeDef",
     {
         "creationTime": int,
         "completionTime": int,
     },
     total=False,
@@ -597,14 +697,31 @@
     {
         "code": ExportTaskStatusCodeType,
         "message": str,
     },
     total=False,
 )
 
+FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNames": Sequence[str],
+        "logStreamNamePrefix": str,
+        "startTime": int,
+        "endTime": int,
+        "filterPattern": str,
+        "interleaved": bool,
+        "unmask": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 FilterLogEventsRequestRequestTypeDef = TypedDict(
     "FilterLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logGroupIdentifier": str,
         "logStreamNames": Sequence[str],
         "logStreamNamePrefix": str,
@@ -643,14 +760,24 @@
 GetDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
     },
 )
 
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetLogEventsRequestRequestTypeDef",
     {
         "logStreamName": str,
     },
 )
 _OptionalGetLogEventsRequestRequestTypeDef = TypedDict(
@@ -721,14 +848,22 @@
 
 class GetLogRecordRequestRequestTypeDef(
     _RequiredGetLogRecordRequestRequestTypeDef, _OptionalGetLogRecordRequestRequestTypeDef
 ):
     pass
 
 
+GetLogRecordResponseTypeDef = TypedDict(
+    "GetLogRecordResponseTypeDef",
+    {
+        "logRecord": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryResultsRequestRequestTypeDef = TypedDict(
     "GetQueryResultsRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
@@ -762,56 +897,107 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsLogGroupRequestRequestTypeDef = TypedDict(
     "ListTagsLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 
+ListTagsLogGroupResponseTypeDef = TypedDict(
+    "ListTagsLogGroupResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricFilterMatchRecordTypeDef = TypedDict(
     "MetricFilterMatchRecordTypeDef",
     {
         "eventNumber": int,
         "eventMessage": str,
         "extractedValues": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredMetricTransformationOutputTypeDef = TypedDict(
+    "_RequiredMetricTransformationOutputTypeDef",
+    {
+        "metricName": str,
+        "metricNamespace": str,
+        "metricValue": str,
+    },
+)
+_OptionalMetricTransformationOutputTypeDef = TypedDict(
+    "_OptionalMetricTransformationOutputTypeDef",
+    {
+        "defaultValue": float,
+        "dimensions": Dict[str, str],
+        "unit": StandardUnitType,
+    },
+    total=False,
+)
+
+
+class MetricTransformationOutputTypeDef(
+    _RequiredMetricTransformationOutputTypeDef, _OptionalMetricTransformationOutputTypeDef
+):
+    pass
+
+
 _RequiredMetricTransformationTypeDef = TypedDict(
     "_RequiredMetricTransformationTypeDef",
     {
         "metricName": str,
         "metricNamespace": str,
         "metricValue": str,
     },
 )
 _OptionalMetricTransformationTypeDef = TypedDict(
     "_OptionalMetricTransformationTypeDef",
     {
         "defaultValue": float,
-        "dimensions": Dict[str, str],
+        "dimensions": Mapping[str, str],
         "unit": StandardUnitType,
     },
     total=False,
 )
 
 
 class MetricTransformationTypeDef(
     _RequiredMetricTransformationTypeDef, _OptionalMetricTransformationTypeDef
 ):
     pass
 
 
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
 _RequiredPutAccountPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccountPolicyRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
         "policyType": Literal["DATA_PROTECTION_POLICY"],
     },
@@ -835,14 +1021,24 @@
     "PutDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
         "policyDocument": str,
     },
 )
 
+PutDataProtectionPolicyResponseTypeDef = TypedDict(
+    "PutDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutDestinationPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDestinationPolicyRequestRequestTypeDef",
     {
         "destinationName": str,
         "accessPolicy": str,
     },
 )
@@ -915,14 +1111,22 @@
 class PutQueryDefinitionRequestRequestTypeDef(
     _RequiredPutQueryDefinitionRequestRequestTypeDef,
     _OptionalPutQueryDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
+PutQueryDefinitionResponseTypeDef = TypedDict(
+    "PutQueryDefinitionResponseTypeDef",
+    {
+        "queryDefinitionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
     total=False,
@@ -958,14 +1162,25 @@
 class PutSubscriptionFilterRequestRequestTypeDef(
     _RequiredPutSubscriptionFilterRequestRequestTypeDef,
     _OptionalPutSubscriptionFilterRequestRequestTypeDef,
 ):
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
 _RequiredStartQueryRequestRequestTypeDef = TypedDict(
     "_RequiredStartQueryRequestRequestTypeDef",
     {
         "startTime": int,
         "endTime": int,
         "queryString": str,
     },
@@ -984,21 +1199,37 @@
 
 class StartQueryRequestRequestTypeDef(
     _RequiredStartQueryRequestRequestTypeDef, _OptionalStartQueryRequestRequestTypeDef
 ):
     pass
 
 
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "queryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopQueryRequestRequestTypeDef = TypedDict(
     "StopQueryRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
+StopQueryResponseTypeDef = TypedDict(
+    "StopQueryResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagLogGroupRequestRequestTypeDef = TypedDict(
     "TagLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1031,311 +1262,106 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateExportTaskResponseTypeDef = TypedDict(
-    "CreateExportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteQueryDefinitionResponseTypeDef = TypedDict(
-    "DeleteQueryDefinitionResponseTypeDef",
-    {
-        "success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAccountPoliciesResponseTypeDef = TypedDict(
     "DescribeAccountPoliciesResponseTypeDef",
     {
         "accountPolicies": List[AccountPolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
-    {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLogRecordResponseTypeDef = TypedDict(
-    "GetLogRecordResponseTypeDef",
-    {
-        "logRecord": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsLogGroupResponseTypeDef = TypedDict(
-    "ListTagsLogGroupResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountPolicyResponseTypeDef = TypedDict(
     "PutAccountPolicyResponseTypeDef",
     {
         "accountPolicy": AccountPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutDataProtectionPolicyResponseTypeDef = TypedDict(
-    "PutDataProtectionPolicyResponseTypeDef",
-    {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutQueryDefinitionResponseTypeDef = TypedDict(
-    "PutQueryDefinitionResponseTypeDef",
-    {
-        "queryDefinitionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "queryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopQueryResponseTypeDef = TypedDict(
-    "StopQueryResponseTypeDef",
-    {
-        "success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    {
-        "DestinationNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    {
-        "taskId": str,
-        "statusCode": ExportTaskStatusCodeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    {
-        "accountIdentifiers": Sequence[str],
-        "logGroupNamePrefix": str,
-        "logGroupNamePattern": str,
-        "includeLinkedAccounts": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNamePrefix": str,
-        "orderBy": OrderByType,
-        "descending": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "filterNamePrefix": str,
-        "metricName": str,
-        "metricNamespace": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "status": QueryStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "filterNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
-    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-):
-    pass
-
-
-FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNames": Sequence[str],
-        "logStreamNamePrefix": str,
-        "startTime": int,
-        "endTime": int,
-        "filterPattern": str,
-        "interleaved": bool,
-        "unmask": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeDestinationsResponseTypeDef = TypedDict(
     "DescribeDestinationsResponseTypeDef",
     {
         "destinations": List[DestinationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDestinationResponseTypeDef = TypedDict(
     "PutDestinationResponseTypeDef",
     {
         "destination": DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogGroupsResponseTypeDef = TypedDict(
     "DescribeLogGroupsResponseTypeDef",
     {
         "logGroups": List[LogGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogStreamsResponseTypeDef = TypedDict(
     "DescribeLogStreamsResponseTypeDef",
     {
         "logStreams": List[LogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueriesResponseTypeDef = TypedDict(
     "DescribeQueriesResponseTypeDef",
     {
         "queries": List[QueryInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueryDefinitionsResponseTypeDef = TypedDict(
     "DescribeQueryDefinitionsResponseTypeDef",
     {
         "queryDefinitions": List[QueryDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourcePoliciesResponseTypeDef = TypedDict(
     "DescribeResourcePoliciesResponseTypeDef",
     {
         "resourcePolicies": List[ResourcePolicyTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubscriptionFiltersResponseTypeDef = TypedDict(
     "DescribeSubscriptionFiltersResponseTypeDef",
     {
         "subscriptionFilters": List[SubscriptionFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "taskId": str,
@@ -1353,44 +1379,44 @@
 
 FilterLogEventsResponseTypeDef = TypedDict(
     "FilterLogEventsResponseTypeDef",
     {
         "events": List[FilteredLogEventTypeDef],
         "searchedLogStreams": List[SearchedLogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogEventsResponseTypeDef = TypedDict(
     "GetLogEventsResponseTypeDef",
     {
         "events": List[OutputLogEventTypeDef],
         "nextForwardToken": str,
         "nextBackwardToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogGroupFieldsResponseTypeDef = TypedDict(
     "GetLogGroupFieldsResponseTypeDef",
     {
         "logGroupFields": List[LogGroupFieldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "results": List[List[ResultFieldTypeDef]],
         "statistics": QueryStatisticsTypeDef,
         "status": QueryStatusType,
         "encryptionKey": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -1413,24 +1439,24 @@
     pass
 
 
 TestMetricFilterResponseTypeDef = TypedDict(
     "TestMetricFilterResponseTypeDef",
     {
         "matches": List[MetricFilterMatchRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricFilterTypeDef = TypedDict(
     "MetricFilterTypeDef",
     {
         "filterName": str,
         "filterPattern": str,
-        "metricTransformations": List[MetricTransformationTypeDef],
+        "metricTransformations": List[MetricTransformationOutputTypeDef],
         "creationTime": int,
         "logGroupName": str,
     },
     total=False,
 )
 
 PutMetricFilterRequestRequestTypeDef = TypedDict(
@@ -1444,28 +1470,28 @@
 )
 
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportTasks": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricFiltersResponseTypeDef = TypedDict(
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs/type_defs.pyi` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -33,103 +33,104 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountPolicyTypeDef",
     "AssociateKmsKeyRequestRequestTypeDef",
     "CancelExportTaskRequestRequestTypeDef",
     "CreateExportTaskRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateExportTaskResponseTypeDef",
     "CreateLogGroupRequestRequestTypeDef",
     "CreateLogStreamRequestRequestTypeDef",
     "DeleteAccountPolicyRequestRequestTypeDef",
     "DeleteDataProtectionPolicyRequestRequestTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteLogGroupRequestRequestTypeDef",
     "DeleteLogStreamRequestRequestTypeDef",
     "DeleteMetricFilterRequestRequestTypeDef",
     "DeleteQueryDefinitionRequestRequestTypeDef",
+    "DeleteQueryDefinitionResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRetentionPolicyRequestRequestTypeDef",
     "DeleteSubscriptionFilterRequestRequestTypeDef",
     "DescribeAccountPoliciesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
     "DescribeDestinationsRequestRequestTypeDef",
     "DestinationTypeDef",
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
     "DescribeLogGroupsRequestRequestTypeDef",
     "LogGroupTypeDef",
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
     "DescribeLogStreamsRequestRequestTypeDef",
     "LogStreamTypeDef",
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
     "DescribeMetricFiltersRequestRequestTypeDef",
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
     "DescribeQueriesRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "DescribeQueryDefinitionsRequestRequestTypeDef",
     "QueryDefinitionTypeDef",
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
     "DescribeResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
+    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
     "DescribeSubscriptionFiltersRequestRequestTypeDef",
     "SubscriptionFilterTypeDef",
     "DisassociateKmsKeyRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportTaskExecutionInfoTypeDef",
     "ExportTaskStatusTypeDef",
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
     "FilterLogEventsRequestRequestTypeDef",
     "FilteredLogEventTypeDef",
     "SearchedLogStreamTypeDef",
     "GetDataProtectionPolicyRequestRequestTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
     "GetLogEventsRequestRequestTypeDef",
     "OutputLogEventTypeDef",
     "GetLogGroupFieldsRequestRequestTypeDef",
     "LogGroupFieldTypeDef",
     "GetLogRecordRequestRequestTypeDef",
+    "GetLogRecordResponseTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "ResultFieldTypeDef",
     "InputLogEventTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTagsLogGroupRequestRequestTypeDef",
+    "ListTagsLogGroupResponseTypeDef",
     "MetricFilterMatchRecordTypeDef",
+    "MetricTransformationOutputTypeDef",
     "MetricTransformationTypeDef",
+    "PaginatorConfigTypeDef",
     "PutAccountPolicyRequestRequestTypeDef",
     "PutDataProtectionPolicyRequestRequestTypeDef",
+    "PutDataProtectionPolicyResponseTypeDef",
     "PutDestinationPolicyRequestRequestTypeDef",
     "PutDestinationRequestRequestTypeDef",
     "RejectedLogEventsInfoTypeDef",
     "PutQueryDefinitionRequestRequestTypeDef",
+    "PutQueryDefinitionResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "PutSubscriptionFilterRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartQueryRequestRequestTypeDef",
+    "StartQueryResponseTypeDef",
     "StopQueryRequestRequestTypeDef",
+    "StopQueryResponseTypeDef",
     "TagLogGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestMetricFilterRequestRequestTypeDef",
     "UntagLogGroupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateExportTaskResponseTypeDef",
-    "DeleteQueryDefinitionResponseTypeDef",
     "DescribeAccountPoliciesResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
-    "GetLogRecordResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsLogGroupResponseTypeDef",
     "PutAccountPolicyResponseTypeDef",
-    "PutDataProtectionPolicyResponseTypeDef",
-    "PutQueryDefinitionResponseTypeDef",
-    "StartQueryResponseTypeDef",
-    "StopQueryResponseTypeDef",
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
     "DescribeDestinationsResponseTypeDef",
     "PutDestinationResponseTypeDef",
     "DescribeLogGroupsResponseTypeDef",
     "DescribeLogStreamsResponseTypeDef",
     "DescribeQueriesResponseTypeDef",
     "DescribeQueryDefinitionsResponseTypeDef",
     "DescribeResourcePoliciesResponseTypeDef",
@@ -209,22 +210,19 @@
 )
 
 class CreateExportTaskRequestRequestTypeDef(
     _RequiredCreateExportTaskRequestRequestTypeDef, _OptionalCreateExportTaskRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateExportTaskResponseTypeDef = TypedDict(
+    "CreateExportTaskResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLogGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -300,14 +298,22 @@
 DeleteQueryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteQueryDefinitionRequestRequestTypeDef",
     {
         "queryDefinitionId": str,
     },
 )
 
+DeleteQueryDefinitionResponseTypeDef = TypedDict(
+    "DeleteQueryDefinitionResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
     total=False,
 )
@@ -344,20 +350,19 @@
 
 class DescribeAccountPoliciesRequestRequestTypeDef(
     _RequiredDescribeAccountPoliciesRequestRequestTypeDef,
     _OptionalDescribeAccountPoliciesRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DestinationNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDestinationsRequestRequestTypeDef = TypedDict(
     "DescribeDestinationsRequestRequestTypeDef",
     {
@@ -377,25 +382,47 @@
         "accessPolicy": str,
         "arn": str,
         "creationTime": int,
     },
     total=False,
 )
 
+DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
+    {
+        "taskId": str,
+        "statusCode": ExportTaskStatusCodeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
         "taskId": str,
         "statusCode": ExportTaskStatusCodeType,
         "nextToken": str,
         "limit": int,
     },
     total=False,
 )
 
+DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
+    {
+        "accountIdentifiers": Sequence[str],
+        "logGroupNamePrefix": str,
+        "logGroupNamePattern": str,
+        "includeLinkedAccounts": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLogGroupsRequestRequestTypeDef = TypedDict(
     "DescribeLogGroupsRequestRequestTypeDef",
     {
         "accountIdentifiers": Sequence[str],
         "logGroupNamePrefix": str,
         "logGroupNamePattern": str,
         "nextToken": str,
@@ -417,14 +444,27 @@
         "kmsKeyId": str,
         "dataProtectionStatus": DataProtectionStatusType,
         "inheritedProperties": List[Literal["ACCOUNT_DATA_PROTECTION"]],
     },
     total=False,
 )
 
+DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNamePrefix": str,
+        "orderBy": OrderByType,
+        "descending": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLogStreamsRequestRequestTypeDef = TypedDict(
     "DescribeLogStreamsRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logGroupIdentifier": str,
         "logStreamNamePrefix": str,
         "orderBy": OrderByType,
@@ -446,27 +486,49 @@
         "uploadSequenceToken": str,
         "arn": str,
         "storedBytes": int,
     },
     total=False,
 )
 
+DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "filterNamePrefix": str,
+        "metricName": str,
+        "metricNamespace": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMetricFiltersRequestRequestTypeDef = TypedDict(
     "DescribeMetricFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterNamePrefix": str,
         "nextToken": str,
         "limit": int,
         "metricName": str,
         "metricNamespace": str,
     },
     total=False,
 )
 
+DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "status": QueryStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeQueriesRequestRequestTypeDef = TypedDict(
     "DescribeQueriesRequestRequestTypeDef",
     {
         "logGroupName": str,
         "status": QueryStatusType,
         "maxResults": int,
         "nextToken": str,
@@ -504,14 +566,22 @@
         "queryString": str,
         "lastModified": int,
         "logGroupNames": List[str],
     },
     total=False,
 )
 
+DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeResourcePoliciesRequestRequestTypeDef = TypedDict(
     "DescribeResourcePoliciesRequestRequestTypeDef",
     {
         "nextToken": str,
         "limit": int,
     },
     total=False,
@@ -523,14 +593,35 @@
         "policyName": str,
         "policyDocument": str,
         "lastUpdatedTime": int,
     },
     total=False,
 )
 
+_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "filterNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
+    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscriptionFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
@@ -568,14 +659,21 @@
     {
         "logGroupName": str,
         "resourceIdentifier": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportTaskExecutionInfoTypeDef = TypedDict(
     "ExportTaskExecutionInfoTypeDef",
     {
         "creationTime": int,
         "completionTime": int,
     },
     total=False,
@@ -586,14 +684,31 @@
     {
         "code": ExportTaskStatusCodeType,
         "message": str,
     },
     total=False,
 )
 
+FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNames": Sequence[str],
+        "logStreamNamePrefix": str,
+        "startTime": int,
+        "endTime": int,
+        "filterPattern": str,
+        "interleaved": bool,
+        "unmask": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 FilterLogEventsRequestRequestTypeDef = TypedDict(
     "FilterLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logGroupIdentifier": str,
         "logStreamNames": Sequence[str],
         "logStreamNamePrefix": str,
@@ -632,14 +747,24 @@
 GetDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
     },
 )
 
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetLogEventsRequestRequestTypeDef",
     {
         "logStreamName": str,
     },
 )
 _OptionalGetLogEventsRequestRequestTypeDef = TypedDict(
@@ -706,14 +831,22 @@
 )
 
 class GetLogRecordRequestRequestTypeDef(
     _RequiredGetLogRecordRequestRequestTypeDef, _OptionalGetLogRecordRequestRequestTypeDef
 ):
     pass
 
+GetLogRecordResponseTypeDef = TypedDict(
+    "GetLogRecordResponseTypeDef",
+    {
+        "logRecord": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryResultsRequestRequestTypeDef = TypedDict(
     "GetQueryResultsRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
@@ -747,54 +880,103 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsLogGroupRequestRequestTypeDef = TypedDict(
     "ListTagsLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 
+ListTagsLogGroupResponseTypeDef = TypedDict(
+    "ListTagsLogGroupResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricFilterMatchRecordTypeDef = TypedDict(
     "MetricFilterMatchRecordTypeDef",
     {
         "eventNumber": int,
         "eventMessage": str,
         "extractedValues": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredMetricTransformationOutputTypeDef = TypedDict(
+    "_RequiredMetricTransformationOutputTypeDef",
+    {
+        "metricName": str,
+        "metricNamespace": str,
+        "metricValue": str,
+    },
+)
+_OptionalMetricTransformationOutputTypeDef = TypedDict(
+    "_OptionalMetricTransformationOutputTypeDef",
+    {
+        "defaultValue": float,
+        "dimensions": Dict[str, str],
+        "unit": StandardUnitType,
+    },
+    total=False,
+)
+
+class MetricTransformationOutputTypeDef(
+    _RequiredMetricTransformationOutputTypeDef, _OptionalMetricTransformationOutputTypeDef
+):
+    pass
+
 _RequiredMetricTransformationTypeDef = TypedDict(
     "_RequiredMetricTransformationTypeDef",
     {
         "metricName": str,
         "metricNamespace": str,
         "metricValue": str,
     },
 )
 _OptionalMetricTransformationTypeDef = TypedDict(
     "_OptionalMetricTransformationTypeDef",
     {
         "defaultValue": float,
-        "dimensions": Dict[str, str],
+        "dimensions": Mapping[str, str],
         "unit": StandardUnitType,
     },
     total=False,
 )
 
 class MetricTransformationTypeDef(
     _RequiredMetricTransformationTypeDef, _OptionalMetricTransformationTypeDef
 ):
     pass
 
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
 _RequiredPutAccountPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccountPolicyRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
         "policyType": Literal["DATA_PROTECTION_POLICY"],
     },
@@ -816,14 +998,24 @@
     "PutDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
         "policyDocument": str,
     },
 )
 
+PutDataProtectionPolicyResponseTypeDef = TypedDict(
+    "PutDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutDestinationPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDestinationPolicyRequestRequestTypeDef",
     {
         "destinationName": str,
         "accessPolicy": str,
     },
 )
@@ -890,14 +1082,22 @@
 
 class PutQueryDefinitionRequestRequestTypeDef(
     _RequiredPutQueryDefinitionRequestRequestTypeDef,
     _OptionalPutQueryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+PutQueryDefinitionResponseTypeDef = TypedDict(
+    "PutQueryDefinitionResponseTypeDef",
+    {
+        "queryDefinitionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
     total=False,
@@ -931,14 +1131,25 @@
 
 class PutSubscriptionFilterRequestRequestTypeDef(
     _RequiredPutSubscriptionFilterRequestRequestTypeDef,
     _OptionalPutSubscriptionFilterRequestRequestTypeDef,
 ):
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
 _RequiredStartQueryRequestRequestTypeDef = TypedDict(
     "_RequiredStartQueryRequestRequestTypeDef",
     {
         "startTime": int,
         "endTime": int,
         "queryString": str,
     },
@@ -955,21 +1166,37 @@
 )
 
 class StartQueryRequestRequestTypeDef(
     _RequiredStartQueryRequestRequestTypeDef, _OptionalStartQueryRequestRequestTypeDef
 ):
     pass
 
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "queryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopQueryRequestRequestTypeDef = TypedDict(
     "StopQueryRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
+StopQueryResponseTypeDef = TypedDict(
+    "StopQueryResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagLogGroupRequestRequestTypeDef = TypedDict(
     "TagLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1002,309 +1229,106 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateExportTaskResponseTypeDef = TypedDict(
-    "CreateExportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteQueryDefinitionResponseTypeDef = TypedDict(
-    "DeleteQueryDefinitionResponseTypeDef",
-    {
-        "success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAccountPoliciesResponseTypeDef = TypedDict(
     "DescribeAccountPoliciesResponseTypeDef",
     {
         "accountPolicies": List[AccountPolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
-    {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLogRecordResponseTypeDef = TypedDict(
-    "GetLogRecordResponseTypeDef",
-    {
-        "logRecord": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsLogGroupResponseTypeDef = TypedDict(
-    "ListTagsLogGroupResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountPolicyResponseTypeDef = TypedDict(
     "PutAccountPolicyResponseTypeDef",
     {
         "accountPolicy": AccountPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutDataProtectionPolicyResponseTypeDef = TypedDict(
-    "PutDataProtectionPolicyResponseTypeDef",
-    {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutQueryDefinitionResponseTypeDef = TypedDict(
-    "PutQueryDefinitionResponseTypeDef",
-    {
-        "queryDefinitionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "queryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopQueryResponseTypeDef = TypedDict(
-    "StopQueryResponseTypeDef",
-    {
-        "success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    {
-        "DestinationNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    {
-        "taskId": str,
-        "statusCode": ExportTaskStatusCodeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    {
-        "accountIdentifiers": Sequence[str],
-        "logGroupNamePrefix": str,
-        "logGroupNamePattern": str,
-        "includeLinkedAccounts": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNamePrefix": str,
-        "orderBy": OrderByType,
-        "descending": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "filterNamePrefix": str,
-        "metricName": str,
-        "metricNamespace": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "status": QueryStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "filterNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
-    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-):
-    pass
-
-FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNames": Sequence[str],
-        "logStreamNamePrefix": str,
-        "startTime": int,
-        "endTime": int,
-        "filterPattern": str,
-        "interleaved": bool,
-        "unmask": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeDestinationsResponseTypeDef = TypedDict(
     "DescribeDestinationsResponseTypeDef",
     {
         "destinations": List[DestinationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDestinationResponseTypeDef = TypedDict(
     "PutDestinationResponseTypeDef",
     {
         "destination": DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogGroupsResponseTypeDef = TypedDict(
     "DescribeLogGroupsResponseTypeDef",
     {
         "logGroups": List[LogGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogStreamsResponseTypeDef = TypedDict(
     "DescribeLogStreamsResponseTypeDef",
     {
         "logStreams": List[LogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueriesResponseTypeDef = TypedDict(
     "DescribeQueriesResponseTypeDef",
     {
         "queries": List[QueryInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueryDefinitionsResponseTypeDef = TypedDict(
     "DescribeQueryDefinitionsResponseTypeDef",
     {
         "queryDefinitions": List[QueryDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourcePoliciesResponseTypeDef = TypedDict(
     "DescribeResourcePoliciesResponseTypeDef",
     {
         "resourcePolicies": List[ResourcePolicyTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubscriptionFiltersResponseTypeDef = TypedDict(
     "DescribeSubscriptionFiltersResponseTypeDef",
     {
         "subscriptionFilters": List[SubscriptionFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "taskId": str,
@@ -1322,44 +1346,44 @@
 
 FilterLogEventsResponseTypeDef = TypedDict(
     "FilterLogEventsResponseTypeDef",
     {
         "events": List[FilteredLogEventTypeDef],
         "searchedLogStreams": List[SearchedLogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogEventsResponseTypeDef = TypedDict(
     "GetLogEventsResponseTypeDef",
     {
         "events": List[OutputLogEventTypeDef],
         "nextForwardToken": str,
         "nextBackwardToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogGroupFieldsResponseTypeDef = TypedDict(
     "GetLogGroupFieldsResponseTypeDef",
     {
         "logGroupFields": List[LogGroupFieldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "results": List[List[ResultFieldTypeDef]],
         "statistics": QueryStatisticsTypeDef,
         "status": QueryStatusType,
         "encryptionKey": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -1380,24 +1404,24 @@
 ):
     pass
 
 TestMetricFilterResponseTypeDef = TypedDict(
     "TestMetricFilterResponseTypeDef",
     {
         "matches": List[MetricFilterMatchRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricFilterTypeDef = TypedDict(
     "MetricFilterTypeDef",
     {
         "filterName": str,
         "filterPattern": str,
-        "metricTransformations": List[MetricTransformationTypeDef],
+        "metricTransformations": List[MetricTransformationOutputTypeDef],
         "creationTime": int,
         "logGroupName": str,
     },
     total=False,
 )
 
 PutMetricFilterRequestRequestTypeDef = TypedDict(
@@ -1411,28 +1435,28 @@
 )
 
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportTasks": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricFiltersResponseTypeDef = TypedDict(
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/PKG-INFO` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.28.1
-Summary: Type annotations for boto3.CloudWatchLogs 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchLogs 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-logs"></a>
 
 # mypy-boto3-logs
 
 [![PyPI - mypy-boto3-logs](https://img.shields.io/pypi/v/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-logs?color=blue)](https://pypistats.org/packages/mypy-boto3-logs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-logs)](https://pepy.tech/project/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,103 +371,104 @@
 
 ```python
 from mypy_boto3_logs.type_defs import (
     AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateExportTaskResponseTypeDef,
     CreateLogGroupRequestRequestTypeDef,
     CreateLogStreamRequestRequestTypeDef,
     DeleteAccountPolicyRequestRequestTypeDef,
     DeleteDataProtectionPolicyRequestRequestTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteLogGroupRequestRequestTypeDef,
     DeleteLogStreamRequestRequestTypeDef,
     DeleteMetricFilterRequestRequestTypeDef,
     DeleteQueryDefinitionRequestRequestTypeDef,
+    DeleteQueryDefinitionResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteSubscriptionFilterRequestRequestTypeDef,
     DescribeAccountPoliciesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
     DescribeDestinationsRequestRequestTypeDef,
     DestinationTypeDef,
+    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
+    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
     DescribeLogGroupsRequestRequestTypeDef,
     LogGroupTypeDef,
+    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
     DescribeLogStreamsRequestRequestTypeDef,
     LogStreamTypeDef,
+    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
     DescribeMetricFiltersRequestRequestTypeDef,
+    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
     DescribeQueriesRequestRequestTypeDef,
     QueryInfoTypeDef,
     DescribeQueryDefinitionsRequestRequestTypeDef,
     QueryDefinitionTypeDef,
+    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
     DescribeResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
+    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
     DescribeSubscriptionFiltersRequestRequestTypeDef,
     SubscriptionFilterTypeDef,
     DisassociateKmsKeyRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportTaskExecutionInfoTypeDef,
     ExportTaskStatusTypeDef,
+    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     FilterLogEventsRequestRequestTypeDef,
     FilteredLogEventTypeDef,
     SearchedLogStreamTypeDef,
     GetDataProtectionPolicyRequestRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetLogEventsRequestRequestTypeDef,
     OutputLogEventTypeDef,
     GetLogGroupFieldsRequestRequestTypeDef,
     LogGroupFieldTypeDef,
     GetLogRecordRequestRequestTypeDef,
+    GetLogRecordResponseTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     ResultFieldTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupRequestRequestTypeDef,
+    ListTagsLogGroupResponseTypeDef,
     MetricFilterMatchRecordTypeDef,
+    MetricTransformationOutputTypeDef,
     MetricTransformationTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountPolicyRequestRequestTypeDef,
     PutDataProtectionPolicyRequestRequestTypeDef,
+    PutDataProtectionPolicyResponseTypeDef,
     PutDestinationPolicyRequestRequestTypeDef,
     PutDestinationRequestRequestTypeDef,
     RejectedLogEventsInfoTypeDef,
     PutQueryDefinitionRequestRequestTypeDef,
+    PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     PutSubscriptionFilterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
     StopQueryRequestRequestTypeDef,
+    StopQueryResponseTypeDef,
     TagLogGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestMetricFilterRequestRequestTypeDef,
     UntagLogGroupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateExportTaskResponseTypeDef,
-    DeleteQueryDefinitionResponseTypeDef,
     DescribeAccountPoliciesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetLogRecordResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsLogGroupResponseTypeDef,
     PutAccountPolicyResponseTypeDef,
-    PutDataProtectionPolicyResponseTypeDef,
-    PutQueryDefinitionResponseTypeDef,
-    StartQueryResponseTypeDef,
-    StopQueryResponseTypeDef,
-    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
-    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
-    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
-    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
-    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
-    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     DescribeDestinationsResponseTypeDef,
     PutDestinationResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
     DescribeResourcePoliciesResponseTypeDef,
```

### Comparing `mypy-boto3-logs-1.28.1/mypy_boto3_logs.egg-info/SOURCES.txt` & `mypy-boto3-logs-1.28.12/mypy_boto3_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.1/setup.py` & `mypy-boto3-logs-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-logs",
-    version="1.28.1",
+    version="1.28.12",
     packages=["mypy_boto3_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchLogs 1.28.1 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudWatchLogs 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

