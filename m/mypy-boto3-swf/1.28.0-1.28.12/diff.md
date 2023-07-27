# Comparing `tmp/mypy-boto3-swf-1.28.0.tar.gz` & `tmp/mypy-boto3-swf-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-swf-1.28.0.tar", last modified: Thu Jul  6 21:00:46 2023, max compression
+gzip compressed data, was "mypy-boto3-swf-1.28.12.tar", last modified: Thu Jul 27 11:49:45 2023, max compression
```

## Comparing `mypy-boto3-swf-1.28.0.tar` & `mypy-boto3-swf-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.354449 mypy-boto3-swf-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-07-06 21:00:46.354449 mypy-boto3-swf-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.342449 mypy-boto3-swf-1.28.0/mypy_boto3_swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30971 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-07-06 20:57:02.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-07-06 20:57:02.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    83936 2023-07-06 20:57:04.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83779 2023-07-06 20:57:03.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.354449 mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-07-06 21:00:46.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:46.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:46.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:46.000000 mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:46.354449 mypy-boto3-swf-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:57:01.000000 mypy-boto3-swf-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:45.769408 mypy-boto3-swf-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-27 11:49:45.765408 mypy-boto3-swf-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:45.765408 mypy-boto3-swf-1.28.12/mypy_boto3_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30971 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-07-27 11:47:53.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85198 2023-07-27 11:47:54.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85040 2023-07-27 11:47:53.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:45.765408 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:45.769408 mypy-boto3-swf-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/setup.py
```

### Comparing `mypy-boto3-swf-1.28.0/LICENSE` & `mypy-boto3-swf-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.0/PKG-INFO` & `mypy-boto3-swf-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.28.0
-Summary: Type annotations for boto3.SWF 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SWF 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-swf"></a>
 
 # mypy-boto3-swf
 
 [![PyPI - mypy-boto3-swf](https://img.shields.io/pypi/v/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-swf?color=blue)](https://pypistats.org/packages/mypy-boto3-swf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -379,28 +379,30 @@
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
-    ActivityTypeTypeDef,
-    TaskListTypeDef,
+    ActivityTypeOutputTypeDef,
+    TaskListOutputTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ActivityTaskStatusTypeDef,
+    ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
-    WorkflowExecutionTypeDef,
+    WorkflowExecutionOutputTypeDef,
+    ActivityTypeTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
-    WorkflowTypeTypeDef,
+    WorkflowTypeOutputTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
+    TaskListTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
     ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
@@ -409,19 +411,21 @@
     RecordMarkerDecisionAttributesTypeDef,
     RequestCancelActivityTaskDecisionAttributesTypeDef,
     RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
+    WorkflowTypeTypeDef,
     DescribeDomainInputRequestTypeDef,
+    WorkflowExecutionTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
+    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -437,103 +441,104 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResourceTagTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    ResourceTagOutputTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
+    ResourceTagTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
-    DeprecateActivityTypeInputRequestTypeDef,
-    DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
-    UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
-    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
-    CountPendingActivityTasksInputRequestTypeDef,
-    CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
-    PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    PollForDecisionTaskInputRequestTypeDef,
-    RegisterActivityTypeInputRequestTypeDef,
-    RegisterWorkflowTypeInputRequestTypeDef,
-    ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
+    ActivityTaskStatusTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PendingTaskCountTypeDef,
+    RunTypeDef,
+    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
-    DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
+    DeprecateActivityTypeInputRequestTypeDef,
+    DescribeActivityTypeInputRequestTypeDef,
+    UndeprecateActivityTypeInputRequestTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
     ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
     ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
-    DeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowTypeInputRequestTypeDef,
-    StartChildWorkflowExecutionDecisionAttributesTypeDef,
     StartChildWorkflowExecutionFailedEventAttributesTypeDef,
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
-    StartWorkflowExecutionInputRequestTypeDef,
-    UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
+    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+    CountPendingActivityTasksInputRequestTypeDef,
+    CountPendingDecisionTasksInputRequestTypeDef,
+    PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputRequestTypeDef,
+    RegisterActivityTypeInputRequestTypeDef,
+    RegisterWorkflowTypeInputRequestTypeDef,
+    ScheduleActivityTaskDecisionAttributesTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
+    DeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowTypeInputRequestTypeDef,
+    StartChildWorkflowExecutionDecisionAttributesTypeDef,
+    StartWorkflowExecutionInputRequestTypeDef,
+    UndeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowExecutionInputRequestTypeDef,
+    GetWorkflowExecutionHistoryInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
-    DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
-    RespondDecisionTaskCompletedInputRequestTypeDef,
+    DecisionTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
+    RespondDecisionTaskCompletedInputRequestTypeDef,
 )
 
 
 def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-swf-1.28.0/README.md` & `mypy-boto3-swf-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-swf"></a>
 
 # mypy-boto3-swf
 
 [![PyPI - mypy-boto3-swf](https://img.shields.io/pypi/v/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-swf?color=blue)](https://pypistats.org/packages/mypy-boto3-swf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -347,28 +347,30 @@
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
-    ActivityTypeTypeDef,
-    TaskListTypeDef,
+    ActivityTypeOutputTypeDef,
+    TaskListOutputTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ActivityTaskStatusTypeDef,
+    ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
-    WorkflowExecutionTypeDef,
+    WorkflowExecutionOutputTypeDef,
+    ActivityTypeTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
-    WorkflowTypeTypeDef,
+    WorkflowTypeOutputTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
+    TaskListTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
     ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
@@ -377,19 +379,21 @@
     RecordMarkerDecisionAttributesTypeDef,
     RequestCancelActivityTaskDecisionAttributesTypeDef,
     RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
+    WorkflowTypeTypeDef,
     DescribeDomainInputRequestTypeDef,
+    WorkflowExecutionTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
+    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -405,103 +409,104 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResourceTagTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    ResourceTagOutputTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
+    ResourceTagTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
-    DeprecateActivityTypeInputRequestTypeDef,
-    DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
-    UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
-    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
-    CountPendingActivityTasksInputRequestTypeDef,
-    CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
-    PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    PollForDecisionTaskInputRequestTypeDef,
-    RegisterActivityTypeInputRequestTypeDef,
-    RegisterWorkflowTypeInputRequestTypeDef,
-    ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
+    ActivityTaskStatusTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PendingTaskCountTypeDef,
+    RunTypeDef,
+    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
-    DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
+    DeprecateActivityTypeInputRequestTypeDef,
+    DescribeActivityTypeInputRequestTypeDef,
+    UndeprecateActivityTypeInputRequestTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
     ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
     ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
-    DeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowTypeInputRequestTypeDef,
-    StartChildWorkflowExecutionDecisionAttributesTypeDef,
     StartChildWorkflowExecutionFailedEventAttributesTypeDef,
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
-    StartWorkflowExecutionInputRequestTypeDef,
-    UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
+    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+    CountPendingActivityTasksInputRequestTypeDef,
+    CountPendingDecisionTasksInputRequestTypeDef,
+    PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputRequestTypeDef,
+    RegisterActivityTypeInputRequestTypeDef,
+    RegisterWorkflowTypeInputRequestTypeDef,
+    ScheduleActivityTaskDecisionAttributesTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
+    DeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowTypeInputRequestTypeDef,
+    StartChildWorkflowExecutionDecisionAttributesTypeDef,
+    StartWorkflowExecutionInputRequestTypeDef,
+    UndeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowExecutionInputRequestTypeDef,
+    GetWorkflowExecutionHistoryInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
-    DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
-    RespondDecisionTaskCompletedInputRequestTypeDef,
+    DecisionTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
+    RespondDecisionTaskCompletedInputRequestTypeDef,
 )
 
 
 def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/__init__.py` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/__init__.pyi` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/__main__.py` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SWF 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SWF 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
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

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/client.py` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/client.pyi` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/literals.py` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActivityTaskTimeoutTypeType",
     "CancelTimerFailedCauseType",
     "CancelWorkflowExecutionFailedCauseType",
     "ChildPolicyType",
     "CloseStatusType",
     "CompleteWorkflowExecutionFailedCauseType",
@@ -56,15 +55,14 @@
     "SWFServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActivityTaskTimeoutTypeType = Literal[
     "HEARTBEAT", "SCHEDULE_TO_CLOSE", "SCHEDULE_TO_START", "START_TO_CLOSE"
 ]
 CancelTimerFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "TIMER_ID_UNKNOWN"]
 CancelWorkflowExecutionFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "UNHANDLED_DECISION"]
 ChildPolicyType = Literal["ABANDON", "REQUEST_CANCEL", "TERMINATE"]
 CloseStatusType = Literal[
@@ -337,14 +335,15 @@
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
@@ -423,26 +422,28 @@
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

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/literals.pyi` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActivityTaskTimeoutTypeType",
     "CancelTimerFailedCauseType",
     "CancelWorkflowExecutionFailedCauseType",
     "ChildPolicyType",
     "CloseStatusType",
     "CompleteWorkflowExecutionFailedCauseType",
@@ -55,14 +56,15 @@
     "SWFServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ActivityTaskTimeoutTypeType = Literal[
     "HEARTBEAT", "SCHEDULE_TO_CLOSE", "SCHEDULE_TO_START", "START_TO_CLOSE"
 ]
 CancelTimerFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "TIMER_ID_UNKNOWN"]
 CancelWorkflowExecutionFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "UNHANDLED_DECISION"]
 ChildPolicyType = Literal["ABANDON", "REQUEST_CANCEL", "TERMINATE"]
 CloseStatusType = Literal[
@@ -335,14 +337,15 @@
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
@@ -421,26 +424,28 @@
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

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/paginator.py` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 
@@ -103,15 +103,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listactivitytypespaginator)
         """
 
 
@@ -128,15 +128,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 
@@ -147,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listdomainspaginator)
         """
 
 
@@ -170,15 +170,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 
@@ -191,15 +191,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listworkflowtypespaginator)
         """
 
 
@@ -213,13 +213,13 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
         startAtPreviousStartedEvent: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/paginator.pyi` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 class ListActivityTypesPaginator(Paginator):
@@ -99,15 +99,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listactivitytypespaginator)
         """
 
 class ListClosedWorkflowExecutionsPaginator(Paginator):
@@ -123,15 +123,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 class ListDomainsPaginator(Paginator):
@@ -141,15 +141,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listdomainspaginator)
         """
 
 class ListOpenWorkflowExecutionsPaginator(Paginator):
@@ -163,15 +163,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 class ListWorkflowTypesPaginator(Paginator):
@@ -183,15 +183,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#listworkflowtypespaginator)
         """
 
 class PollForDecisionTaskPaginator(Paginator):
@@ -204,13 +204,13 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
         startAtPreviousStartedEvent: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/type_defs.py` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,34 +43,35 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
-    "ActivityTypeTypeDef",
-    "TaskListTypeDef",
+    "ActivityTypeOutputTypeDef",
+    "TaskListOutputTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
-    "ActivityTaskStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
-    "WorkflowExecutionTypeDef",
+    "WorkflowExecutionOutputTypeDef",
+    "ActivityTypeTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
-    "WorkflowTypeTypeDef",
+    "WorkflowTypeOutputTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
+    "TaskListTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
@@ -79,19 +80,21 @@
     "RecordMarkerDecisionAttributesTypeDef",
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     "RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef",
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
+    "WorkflowTypeTypeDef",
     "DescribeDomainInputRequestTypeDef",
+    "WorkflowExecutionTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
+    "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
     "MarkerRecordedEventAttributesTypeDef",
     "RecordMarkerFailedEventAttributesTypeDef",
@@ -107,103 +110,104 @@
     "TimerFiredEventAttributesTypeDef",
     "TimerStartedEventAttributesTypeDef",
     "WorkflowExecutionCanceledEventAttributesTypeDef",
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
-    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListActivityTypesInputRequestTypeDef",
-    "ListDomainsInputListDomainsPaginateTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResourceTagTypeDef",
-    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    "ResourceTagOutputTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "PendingTaskCountTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
+    "ResourceTagTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "WorkflowExecutionCountTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
-    "DeprecateActivityTypeInputRequestTypeDef",
-    "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
-    "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    "CountPendingActivityTasksInputRequestTypeDef",
-    "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
-    "PollForActivityTaskInputRequestTypeDef",
-    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    "PollForDecisionTaskInputRequestTypeDef",
-    "RegisterActivityTypeInputRequestTypeDef",
-    "RegisterWorkflowTypeInputRequestTypeDef",
-    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
+    "ActivityTaskStatusTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PendingTaskCountTypeDef",
+    "RunTypeDef",
+    "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
-    "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
-    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
+    "DeprecateActivityTypeInputRequestTypeDef",
+    "DescribeActivityTypeInputRequestTypeDef",
+    "UndeprecateActivityTypeInputRequestTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
     "StartChildWorkflowExecutionFailedEventAttributesTypeDef",
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
-    "StartWorkflowExecutionInputRequestTypeDef",
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    "CountPendingActivityTasksInputRequestTypeDef",
+    "CountPendingDecisionTasksInputRequestTypeDef",
+    "PollForActivityTaskInputRequestTypeDef",
+    "PollForDecisionTaskInputRequestTypeDef",
+    "RegisterActivityTypeInputRequestTypeDef",
+    "RegisterWorkflowTypeInputRequestTypeDef",
+    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "CountClosedWorkflowExecutionsInputRequestTypeDef",
     "CountOpenWorkflowExecutionsInputRequestTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListClosedWorkflowExecutionsInputRequestTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListOpenWorkflowExecutionsInputRequestTypeDef",
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    "DescribeWorkflowTypeInputRequestTypeDef",
+    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
+    "StartWorkflowExecutionInputRequestTypeDef",
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
+    "DescribeWorkflowExecutionInputRequestTypeDef",
+    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
+    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    "ListDomainsInputListDomainsPaginateTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
-    "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
-    "RespondDecisionTaskCompletedInputRequestTypeDef",
+    "DecisionTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
+    "RespondDecisionTaskCompletedInputRequestTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "activityId": str,
@@ -222,22 +226,20 @@
     {
         "details": str,
         "latestCancelRequestedEventId": int,
     },
     total=False,
 )
 
-
 class ActivityTaskCanceledEventAttributesTypeDef(
     _RequiredActivityTaskCanceledEventAttributesTypeDef,
     _OptionalActivityTaskCanceledEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredActivityTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -245,22 +247,20 @@
     "_OptionalActivityTaskCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class ActivityTaskCompletedEventAttributesTypeDef(
     _RequiredActivityTaskCompletedEventAttributesTypeDef,
     _OptionalActivityTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -269,32 +269,30 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class ActivityTaskFailedEventAttributesTypeDef(
     _RequiredActivityTaskFailedEventAttributesTypeDef,
     _OptionalActivityTaskFailedEventAttributesTypeDef,
 ):
     pass
 
-
-ActivityTypeTypeDef = TypedDict(
-    "ActivityTypeTypeDef",
+ActivityTypeOutputTypeDef = TypedDict(
+    "ActivityTypeOutputTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-TaskListTypeDef = TypedDict(
-    "TaskListTypeDef",
+TaskListOutputTypeDef = TypedDict(
+    "TaskListOutputTypeDef",
     {
         "name": str,
     },
 )
 
 _RequiredActivityTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskStartedEventAttributesTypeDef",
@@ -306,27 +304,28 @@
     "_OptionalActivityTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
-
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
-
-ActivityTaskStatusTypeDef = TypedDict(
-    "ActivityTaskStatusTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancelRequested": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredActivityTaskTimedOutEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": ActivityTaskTimeoutTypeType,
@@ -338,30 +337,36 @@
     "_OptionalActivityTaskTimedOutEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class ActivityTaskTimedOutEventAttributesTypeDef(
     _RequiredActivityTaskTimedOutEventAttributesTypeDef,
     _OptionalActivityTaskTimedOutEventAttributesTypeDef,
 ):
     pass
 
-
-WorkflowExecutionTypeDef = TypedDict(
-    "WorkflowExecutionTypeDef",
+WorkflowExecutionOutputTypeDef = TypedDict(
+    "WorkflowExecutionOutputTypeDef",
     {
         "workflowId": str,
         "runId": str,
     },
 )
 
+ActivityTypeTypeDef = TypedDict(
+    "ActivityTypeTypeDef",
+    {
+        "name": str,
+        "version": str,
+    },
+)
+
 CancelTimerDecisionAttributesTypeDef = TypedDict(
     "CancelTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
     },
 )
 
@@ -386,16 +391,16 @@
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CancelWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-WorkflowTypeTypeDef = TypedDict(
-    "WorkflowTypeTypeDef",
+WorkflowTypeOutputTypeDef = TypedDict(
+    "WorkflowTypeOutputTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
 CloseStatusFilterTypeDef = TypedDict(
@@ -417,14 +422,21 @@
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CompleteWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
+TaskListTypeDef = TypedDict(
+    "TaskListTypeDef",
+    {
+        "name": str,
+    },
+)
+
 ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -439,21 +451,19 @@
     "_OptionalExecutionTimeFilterTypeDef",
     {
         "latestDate": Union[datetime, str],
     },
     total=False,
 )
 
-
 class ExecutionTimeFilterTypeDef(
     _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
-
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -474,21 +484,19 @@
     "_OptionalWorkflowTypeFilterTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
-
 class WorkflowTypeFilterTypeDef(
     _RequiredWorkflowTypeFilterTypeDef, _OptionalWorkflowTypeFilterTypeDef
 ):
     pass
 
-
 _RequiredDecisionTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -496,44 +504,40 @@
     "_OptionalDecisionTaskCompletedEventAttributesTypeDef",
     {
         "executionContext": str,
     },
     total=False,
 )
 
-
 class DecisionTaskCompletedEventAttributesTypeDef(
     _RequiredDecisionTaskCompletedEventAttributesTypeDef,
     _OptionalDecisionTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 _OptionalDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
-
 class DecisionTaskStartedEventAttributesTypeDef(
     _RequiredDecisionTaskStartedEventAttributesTypeDef,
     _OptionalDecisionTaskStartedEventAttributesTypeDef,
 ):
     pass
 
-
 DecisionTaskTimedOutEventAttributesTypeDef = TypedDict(
     "DecisionTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "scheduledEventId": int,
         "startedEventId": int,
     },
@@ -558,21 +562,19 @@
     "_OptionalRecordMarkerDecisionAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class RecordMarkerDecisionAttributesTypeDef(
     _RequiredRecordMarkerDecisionAttributesTypeDef, _OptionalRecordMarkerDecisionAttributesTypeDef
 ):
     pass
 
-
 RequestCancelActivityTaskDecisionAttributesTypeDef = TypedDict(
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     {
         "activityId": str,
     },
 )
 
@@ -587,22 +589,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
-
 _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef = TypedDict(
     "_RequiredScheduleLambdaFunctionDecisionAttributesTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
@@ -612,22 +612,20 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
-
 class ScheduleLambdaFunctionDecisionAttributesTypeDef(
     _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef,
     _OptionalScheduleLambdaFunctionDecisionAttributesTypeDef,
 ):
     pass
 
-
 _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
     },
 )
@@ -637,22 +635,20 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
-
 class SignalExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
-
 _RequiredStartTimerDecisionAttributesTypeDef = TypedDict(
     "_RequiredStartTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
         "startToFireTimeout": str,
     },
 )
@@ -660,35 +656,49 @@
     "_OptionalStartTimerDecisionAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
-
 class StartTimerDecisionAttributesTypeDef(
     _RequiredStartTimerDecisionAttributesTypeDef, _OptionalStartTimerDecisionAttributesTypeDef
 ):
     pass
 
-
 DeprecateDomainInputRequestTypeDef = TypedDict(
     "DeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+WorkflowTypeTypeDef = TypedDict(
+    "WorkflowTypeTypeDef",
+    {
+        "name": str,
+        "version": str,
+    },
+)
+
 DescribeDomainInputRequestTypeDef = TypedDict(
     "DescribeDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+WorkflowExecutionTypeDef = TypedDict(
+    "WorkflowExecutionTypeDef",
+    {
+        "workflowId": str,
+        "runId": str,
+    },
+)
+
 DomainConfigurationTypeDef = TypedDict(
     "DomainConfigurationTypeDef",
     {
         "workflowExecutionRetentionPeriodInDays": str,
     },
 )
 
@@ -704,34 +714,35 @@
     {
         "description": str,
         "arn": str,
     },
     total=False,
 )
 
-
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
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
 _RequiredLambdaFunctionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -739,22 +750,20 @@
     "_OptionalLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class LambdaFunctionCompletedEventAttributesTypeDef(
     _RequiredLambdaFunctionCompletedEventAttributesTypeDef,
     _OptionalLambdaFunctionCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -763,22 +772,20 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class LambdaFunctionFailedEventAttributesTypeDef(
     _RequiredLambdaFunctionFailedEventAttributesTypeDef,
     _OptionalLambdaFunctionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredLambdaFunctionScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -789,22 +796,20 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
-
 class LambdaFunctionScheduledEventAttributesTypeDef(
     _RequiredLambdaFunctionScheduledEventAttributesTypeDef,
     _OptionalLambdaFunctionScheduledEventAttributesTypeDef,
 ):
     pass
 
-
 LambdaFunctionStartedEventAttributesTypeDef = TypedDict(
     "LambdaFunctionStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 
@@ -819,22 +824,20 @@
     "_OptionalLambdaFunctionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
     },
     total=False,
 )
 
-
 class LambdaFunctionTimedOutEventAttributesTypeDef(
     _RequiredLambdaFunctionTimedOutEventAttributesTypeDef,
     _OptionalLambdaFunctionTimedOutEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredMarkerRecordedEventAttributesTypeDef = TypedDict(
     "_RequiredMarkerRecordedEventAttributesTypeDef",
     {
         "markerName": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -842,21 +845,19 @@
     "_OptionalMarkerRecordedEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class MarkerRecordedEventAttributesTypeDef(
     _RequiredMarkerRecordedEventAttributesTypeDef, _OptionalMarkerRecordedEventAttributesTypeDef
 ):
     pass
 
-
 RecordMarkerFailedEventAttributesTypeDef = TypedDict(
     "RecordMarkerFailedEventAttributesTypeDef",
     {
         "markerName": str,
         "cause": Literal["OPERATION_NOT_PERMITTED"],
         "decisionTaskCompletedEventId": int,
     },
@@ -885,22 +886,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -909,22 +908,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
-
 ScheduleLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "ScheduleLambdaFunctionFailedEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "cause": ScheduleLambdaFunctionFailedCauseType,
         "decisionTaskCompletedEventId": int,
@@ -945,22 +942,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class SignalExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -971,22 +966,20 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
-
 class SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
-
 StartLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "StartLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "cause": Literal["ASSUME_ROLE_FAILED"],
         "message": str,
     },
@@ -1031,65 +1024,59 @@
     "_OptionalTimerStartedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
-
 class TimerStartedEventAttributesTypeDef(
     _RequiredTimerStartedEventAttributesTypeDef, _OptionalTimerStartedEventAttributesTypeDef
 ):
     pass
 
-
 _RequiredWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
@@ -1097,22 +1084,20 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
@@ -1121,55 +1106,28 @@
         "reason": str,
         "details": str,
         "cause": WorkflowExecutionTerminatedCauseType,
     },
     total=False,
 )
 
-
 class WorkflowExecutionTerminatedEventAttributesTypeDef(
     _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef,
     _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef,
 ):
     pass
 
-
 WorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
 
-_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListActivityTypesInputListActivityTypesPaginateTypeDef(
-    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
-    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListActivityTypesInputRequestTypeDef = TypedDict(
     "_RequiredListActivityTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1180,44 +1138,19 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
-
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
-
-_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDomainsInputListDomainsPaginateTypeDef(
-    _RequiredListDomainsInputListDomainsPaginateTypeDef,
-    _OptionalListDomainsInputListDomainsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputRequestTypeDef = TypedDict(
@@ -1226,72 +1159,45 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
-
 class ListDomainsInputRequestTypeDef(
     _RequiredListDomainsInputRequestTypeDef, _OptionalListDomainsInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredResourceTagTypeDef = TypedDict(
-    "_RequiredResourceTagTypeDef",
+_RequiredResourceTagOutputTypeDef = TypedDict(
+    "_RequiredResourceTagOutputTypeDef",
     {
         "key": str,
     },
 )
-_OptionalResourceTagTypeDef = TypedDict(
-    "_OptionalResourceTagTypeDef",
+_OptionalResourceTagOutputTypeDef = TypedDict(
+    "_OptionalResourceTagOutputTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
-class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
-    pass
-
-
-_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
-    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+class ResourceTagOutputTypeDef(
+    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
 ):
     pass
 
-
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1302,61 +1208,55 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
-
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
 ):
     pass
 
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
-PendingTaskCountTypeDef = TypedDict(
-    "PendingTaskCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_OptionalRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class RecordActivityTaskHeartbeatInputRequestTypeDef(
     _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef,
     _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef,
 ):
     pass
 
+_RequiredResourceTagTypeDef = TypedDict(
+    "_RequiredResourceTagTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalResourceTagTypeDef = TypedDict(
+    "_OptionalResourceTagTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
+    pass
 
 _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
@@ -1365,66 +1265,60 @@
     "_OptionalRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "runId": str,
     },
     total=False,
 )
 
-
 class RequestCancelWorkflowExecutionInputRequestTypeDef(
     _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef,
     _OptionalRequestCancelWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class RespondActivityTaskCanceledInputRequestTypeDef(
     _RequiredRespondActivityTaskCanceledInputRequestTypeDef,
     _OptionalRespondActivityTaskCanceledInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class RespondActivityTaskCompletedInputRequestTypeDef(
     _RequiredRespondActivityTaskCompletedInputRequestTypeDef,
     _OptionalRespondActivityTaskCompletedInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskFailedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
@@ -1432,41 +1326,20 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
 ):
     pass
 
-
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
-RunTypeDef = TypedDict(
-    "RunTypeDef",
-    {
-        "runId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
     },
@@ -1476,22 +1349,20 @@
     {
         "runId": str,
         "input": str,
     },
     total=False,
 )
 
-
 class SignalWorkflowExecutionInputRequestTypeDef(
     _RequiredSignalWorkflowExecutionInputRequestTypeDef,
     _OptionalSignalWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredTerminateWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredTerminateWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
 )
@@ -1502,22 +1373,20 @@
         "reason": str,
         "details": str,
         "childPolicy": ChildPolicyType,
     },
     total=False,
 )
 
-
 class TerminateWorkflowExecutionInputRequestTypeDef(
     _RequiredTerminateWorkflowExecutionInputRequestTypeDef,
     _OptionalTerminateWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
-
 UndeprecateDomainInputRequestTypeDef = TypedDict(
     "UndeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -1525,23 +1394,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkflowExecutionCountTypeDef = TypedDict(
-    "WorkflowExecutionCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredWorkflowExecutionOpenCountsTypeDef = TypedDict(
     "_RequiredWorkflowExecutionOpenCountsTypeDef",
     {
         "openActivityTasks": int,
         "openDecisionTasks": int,
         "openTimers": int,
         "openChildWorkflowExecutions": int,
@@ -1551,83 +1411,55 @@
     "_OptionalWorkflowExecutionOpenCountsTypeDef",
     {
         "openLambdaFunctions": int,
     },
     total=False,
 )
 
-
 class WorkflowExecutionOpenCountsTypeDef(
     _RequiredWorkflowExecutionOpenCountsTypeDef, _OptionalWorkflowExecutionOpenCountsTypeDef
 ):
     pass
 
-
 _RequiredActivityTypeInfoTypeDef = TypedDict(
     "_RequiredActivityTypeInfoTypeDef",
     {
-        "activityType": ActivityTypeTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalActivityTypeInfoTypeDef = TypedDict(
     "_OptionalActivityTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
-
 class ActivityTypeInfoTypeDef(_RequiredActivityTypeInfoTypeDef, _OptionalActivityTypeInfoTypeDef):
     pass
 
-
-DeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "DeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
-DescribeActivityTypeInputRequestTypeDef = TypedDict(
-    "DescribeActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
 ScheduleActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
         "activityId": str,
         "cause": ScheduleActivityTaskFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
 _RequiredActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskScheduledEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
         "activityId": str,
-        "taskList": TaskListTypeDef,
+        "taskList": TaskListOutputTypeDef,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalActivityTaskScheduledEventAttributesTypeDef",
     {
         "input": str,
@@ -1637,382 +1469,164 @@
         "startToCloseTimeout": str,
         "taskPriority": str,
         "heartbeatTimeout": str,
     },
     total=False,
 )
 
-
 class ActivityTaskScheduledEventAttributesTypeDef(
     _RequiredActivityTaskScheduledEventAttributesTypeDef,
     _OptionalActivityTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
-
 ActivityTypeConfigurationTypeDef = TypedDict(
     "ActivityTypeConfigurationTypeDef",
     {
         "defaultTaskStartToCloseTimeout": str,
         "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskList": TaskListOutputTypeDef,
         "defaultTaskPriority": str,
         "defaultTaskScheduleToStartTimeout": str,
         "defaultTaskScheduleToCloseTimeout": str,
     },
     total=False,
 )
 
-ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "workflowTypeVersion": str,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-CountPendingActivityTasksInputRequestTypeDef = TypedDict(
-    "CountPendingActivityTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-
-CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
-    "CountPendingDecisionTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-
 _RequiredDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskScheduledEventAttributesTypeDef",
     {
-        "taskList": TaskListTypeDef,
+        "taskList": TaskListOutputTypeDef,
     },
 )
 _OptionalDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskScheduledEventAttributesTypeDef",
     {
         "taskPriority": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
-
 class DecisionTaskScheduledEventAttributesTypeDef(
     _RequiredDecisionTaskScheduledEventAttributesTypeDef,
     _OptionalDecisionTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
-
-_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForActivityTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForActivityTaskInputRequestTypeDef",
-    {
-        "identity": str,
-    },
-    total=False,
-)
-
-
-class PollForActivityTaskInputRequestTypeDef(
-    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
-):
-    pass
-
-
-_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    {
-        "identity": str,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
-    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-):
-    pass
-
-
-_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputRequestTypeDef",
-    {
-        "identity": str,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-    },
-    total=False,
-)
-
-
-class PollForDecisionTaskInputRequestTypeDef(
-    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
-):
-    pass
-
-
-_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterActivityTypeInputRequestTypeDef",
-    {
-        "description": str,
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultTaskScheduleToStartTimeout": str,
-        "defaultTaskScheduleToCloseTimeout": str,
-    },
-    total=False,
-)
-
-
-class RegisterActivityTypeInputRequestTypeDef(
-    _RequiredRegisterActivityTypeInputRequestTypeDef,
-    _OptionalRegisterActivityTypeInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
-    {
-        "description": str,
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultChildPolicy": ChildPolicyType,
-        "defaultLambdaRole": str,
-    },
-    total=False,
-)
-
-
-class RegisterWorkflowTypeInputRequestTypeDef(
-    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
-    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
-    {
-        "activityType": ActivityTypeTypeDef,
-        "activityId": str,
-    },
-)
-_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
-    {
-        "control": str,
-        "input": str,
-        "scheduleToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "scheduleToStartTimeout": str,
-        "startToCloseTimeout": str,
-        "heartbeatTimeout": str,
-    },
-    total=False,
-)
-
-
-class ScheduleActivityTaskDecisionAttributesTypeDef(
-    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
-    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
-):
-    pass
-
-
 _RequiredWorkflowExecutionConfigurationTypeDef = TypedDict(
     "_RequiredWorkflowExecutionConfigurationTypeDef",
     {
         "taskStartToCloseTimeout": str,
         "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
+        "taskList": TaskListOutputTypeDef,
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalWorkflowExecutionConfigurationTypeDef = TypedDict(
     "_OptionalWorkflowExecutionConfigurationTypeDef",
     {
         "taskPriority": str,
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionConfigurationTypeDef(
     _RequiredWorkflowExecutionConfigurationTypeDef, _OptionalWorkflowExecutionConfigurationTypeDef
 ):
     pass
 
-
 WorkflowTypeConfigurationTypeDef = TypedDict(
     "WorkflowTypeConfigurationTypeDef",
     {
         "defaultTaskStartToCloseTimeout": str,
         "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskList": TaskListOutputTypeDef,
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
-ActivityTaskTypeDef = TypedDict(
-    "ActivityTaskTypeDef",
+ActivityTaskStatusTypeDef = TypedDict(
+    "ActivityTaskStatusTypeDef",
     {
-        "taskToken": str,
-        "activityId": str,
-        "startedEventId": int,
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "activityType": ActivityTypeTypeDef,
-        "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cancelRequested": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowExecutionInputRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
-    "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
+PendingTaskCountTypeDef = TypedDict(
+    "PendingTaskCountTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "initiatedEventId": int,
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExternalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
-    "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
+RunTypeDef = TypedDict(
+    "RunTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "initiatedEventId": int,
+        "runId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+WorkflowExecutionCountTypeDef = TypedDict(
+    "WorkflowExecutionCountTypeDef",
     {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+
+ActivityTaskTypeDef = TypedDict(
+    "ActivityTaskTypeDef",
     {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "taskToken": str,
+        "activityId": str,
+        "startedEventId": int,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
+        "input": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
+ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
+    "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "initiatedEventId": int,
     },
 )
-_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
+
+ExternalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
+    "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "initiatedEventId": int,
     },
-    total=False,
 )
 
-
-class GetWorkflowExecutionHistoryInputRequestTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
-):
-    pass
-
-
 WorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "externalWorkflowExecution": WorkflowExecutionTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
         "externalInitiatedEventId": int,
         "cause": Literal["CHILD_POLICY_APPLIED"],
     },
     total=False,
 )
 
 _RequiredWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
@@ -2021,213 +1635,180 @@
         "signalName": str,
     },
 )
 _OptionalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "input": str,
-        "externalWorkflowExecution": WorkflowExecutionTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
         "externalInitiatedEventId": int,
     },
     total=False,
 )
 
-
 class WorkflowExecutionSignaledEventAttributesTypeDef(
     _RequiredWorkflowExecutionSignaledEventAttributesTypeDef,
     _OptionalWorkflowExecutionSignaledEventAttributesTypeDef,
 ):
     pass
 
+DeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "DeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
+DescribeActivityTypeInputRequestTypeDef = TypedDict(
+    "DescribeActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
+UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
 
 _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class ChildWorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class ChildWorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class ChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 ChildWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "timeoutType": Literal["START_TO_CLOSE"],
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
-DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "workflowType": WorkflowTypeTypeDef,
-        "workflowId": str,
-    },
-)
-_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "control": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-
-class StartChildWorkflowExecutionDecisionAttributesTypeDef(
-    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
-    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
-):
-    pass
-
-
 _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "cause": StartChildWorkflowExecutionFailedCauseType,
         "workflowId": str,
         "initiatedEventId": int,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
-
 class StartChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
-        "workflowType": WorkflowTypeTypeDef,
-        "taskList": TaskListTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
+        "taskList": TaskListOutputTypeDef,
         "decisionTaskCompletedEventId": int,
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
@@ -2238,69 +1819,28 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class StartChildWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
-
-_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowId": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "tagList": Sequence[str],
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-
-class StartWorkflowExecutionInputRequestTypeDef(
-    _RequiredStartWorkflowExecutionInputRequestTypeDef,
-    _OptionalStartWorkflowExecutionInputRequestTypeDef,
-):
-    pass
-
-
-UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
 _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "newExecutionRunId": str,
-        "taskList": TaskListTypeDef,
+        "taskList": TaskListOutputTypeDef,
         "childPolicy": ChildPolicyType,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
     },
 )
 _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
@@ -2308,103 +1848,255 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionContinuedAsNewEventAttributesTypeDef(
     _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionInfoTypeDef = TypedDict(
     "_RequiredWorkflowExecutionInfoTypeDef",
     {
-        "execution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "execution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "startTimestamp": datetime,
         "executionStatus": ExecutionStatusType,
     },
 )
 _OptionalWorkflowExecutionInfoTypeDef = TypedDict(
     "_OptionalWorkflowExecutionInfoTypeDef",
     {
         "closeTimestamp": datetime,
         "closeStatus": CloseStatusType,
-        "parent": WorkflowExecutionTypeDef,
+        "parent": WorkflowExecutionOutputTypeDef,
         "tagList": List[str],
         "cancelRequested": bool,
     },
     total=False,
 )
 
-
 class WorkflowExecutionInfoTypeDef(
     _RequiredWorkflowExecutionInfoTypeDef, _OptionalWorkflowExecutionInfoTypeDef
 ):
     pass
 
-
 _RequiredWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
-        "taskList": TaskListTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "taskList": TaskListOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
     },
 )
 _OptionalWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
         "taskStartToCloseTimeout": str,
         "taskPriority": str,
         "tagList": List[str],
         "continuedExecutionRunId": str,
-        "parentWorkflowExecution": WorkflowExecutionTypeDef,
+        "parentWorkflowExecution": WorkflowExecutionOutputTypeDef,
         "parentInitiatedEventId": int,
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionStartedEventAttributesTypeDef(
     _RequiredWorkflowExecutionStartedEventAttributesTypeDef,
     _OptionalWorkflowExecutionStartedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowTypeInfoTypeDef = TypedDict(
     "_RequiredWorkflowTypeInfoTypeDef",
     {
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalWorkflowTypeInfoTypeDef = TypedDict(
     "_OptionalWorkflowTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
-
 class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
+ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "workflowTypeVersion": str,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+CountPendingActivityTasksInputRequestTypeDef = TypedDict(
+    "CountPendingActivityTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
+CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
+    "CountPendingDecisionTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
+_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForActivityTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForActivityTaskInputRequestTypeDef",
+    {
+        "identity": str,
+    },
+    total=False,
+)
+
+class PollForActivityTaskInputRequestTypeDef(
+    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
+):
+    pass
+
+_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputRequestTypeDef",
+    {
+        "identity": str,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+    },
+    total=False,
+)
+
+class PollForDecisionTaskInputRequestTypeDef(
+    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
+):
+    pass
+
+_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterActivityTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultTaskHeartbeatTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultTaskScheduleToStartTimeout": str,
+        "defaultTaskScheduleToCloseTimeout": str,
+    },
+    total=False,
+)
+
+class RegisterActivityTypeInputRequestTypeDef(
+    _RequiredRegisterActivityTypeInputRequestTypeDef,
+    _OptionalRegisterActivityTypeInputRequestTypeDef,
+):
+    pass
+
+_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultExecutionStartToCloseTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultChildPolicy": ChildPolicyType,
+        "defaultLambdaRole": str,
+    },
+    total=False,
+)
+
+class RegisterWorkflowTypeInputRequestTypeDef(
+    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
+    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
+):
+    pass
+
+_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "activityType": ActivityTypeTypeDef,
+        "activityId": str,
+    },
+)
+_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "scheduleToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "scheduleToStartTimeout": str,
+        "startToCloseTimeout": str,
+        "heartbeatTimeout": str,
+    },
+    total=False,
+)
+
+class ScheduleActivityTaskDecisionAttributesTypeDef(
+    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
+    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
+):
+    pass
 
 _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
@@ -2417,22 +2109,20 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
     },
     total=False,
 )
 
-
 class CountClosedWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2442,80 +2132,297 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
-
 class CountOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "startTimeFilter": ExecutionTimeFilterTypeDef,
         "closeTimeFilter": ExecutionTimeFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
         "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
 
-class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
+DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
 
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowTypeInputRequestTypeDef",
     {
         "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+
+_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "workflowType": WorkflowTypeTypeDef,
+        "workflowId": str,
+    },
+)
+_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+class StartChildWorkflowExecutionDecisionAttributesTypeDef(
+    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
+    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
+):
+    pass
+
+_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowId": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "tagList": Sequence[str],
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+class StartWorkflowExecutionInputRequestTypeDef(
+    _RequiredStartWorkflowExecutionInputRequestTypeDef,
+    _OptionalStartWorkflowExecutionInputRequestTypeDef,
+):
+    pass
+
+UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+
+_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+class GetWorkflowExecutionHistoryInputRequestTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
+):
+    pass
+
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
+    {
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
+    {
+        "domainInfos": List[DomainInfoTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "domain": str,
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "name": str,
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListActivityTypesInputListActivityTypesPaginateTypeDef(
+    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
+    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
+):
+    pass
+
+_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     {
         "startTimeFilter": ExecutionTimeFilterTypeDef,
         "closeTimeFilter": ExecutionTimeFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
         "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
+_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDomainsInputListDomainsPaginateTypeDef(
+    _RequiredListDomainsInputListDomainsPaginateTypeDef,
+    _OptionalListDomainsInputListDomainsPaginateTypeDef,
+):
+    pass
 
 _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
@@ -2523,78 +2430,77 @@
 _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
     _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
-
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
+        "name": str,
         "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
+    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
 ):
     pass
 
-
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
+_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "domain": str,
+        "taskList": TaskListTypeDef,
     },
 )
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
+_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "identity": str,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
+    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+):
+    pass
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "tags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[ResourceTagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
         "name": str,
@@ -2606,110 +2512,63 @@
     {
         "description": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
-
 class RegisterDomainInputRequestTypeDef(
     _RequiredRegisterDomainInputRequestTypeDef, _OptionalRegisterDomainInputRequestTypeDef
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
 )
 
 ActivityTypeInfosTypeDef = TypedDict(
     "ActivityTypeInfosTypeDef",
     {
         "typeInfos": List[ActivityTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeDetailTypeDef = TypedDict(
     "ActivityTypeDetailTypeDef",
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDecisionTypeDef = TypedDict(
-    "_RequiredDecisionTypeDef",
-    {
-        "decisionType": DecisionTypeType,
-    },
-)
-_OptionalDecisionTypeDef = TypedDict(
-    "_OptionalDecisionTypeDef",
-    {
-        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
-        "requestCancelActivityTaskDecisionAttributes": (
-            RequestCancelActivityTaskDecisionAttributesTypeDef
-        ),
-        "completeWorkflowExecutionDecisionAttributes": (
-            CompleteWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
-        "cancelWorkflowExecutionDecisionAttributes": (
-            CancelWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "continueAsNewWorkflowExecutionDecisionAttributes": (
-            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
-        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
-        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
-        "signalExternalWorkflowExecutionDecisionAttributes": (
-            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
-            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "startChildWorkflowExecutionDecisionAttributes": (
-            StartChildWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
-    pass
-
-
 WorkflowExecutionDetailTypeDef = TypedDict(
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
         "latestExecutionContext": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowExecutionInfosTypeDef = TypedDict(
     "WorkflowExecutionInfosTypeDef",
     {
         "executionInfos": List[WorkflowExecutionInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHistoryEventTypeDef = TypedDict(
     "_RequiredHistoryEventTypeDef",
     {
         "eventTimestamp": datetime,
@@ -2826,75 +2685,114 @@
             ScheduleLambdaFunctionFailedEventAttributesTypeDef
         ),
         "startLambdaFunctionFailedEventAttributes": StartLambdaFunctionFailedEventAttributesTypeDef,
     },
     total=False,
 )
 
-
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
-
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowTypeInfosTypeDef = TypedDict(
     "WorkflowTypeInfosTypeDef",
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
+_RequiredDecisionTypeDef = TypedDict(
+    "_RequiredDecisionTypeDef",
     {
-        "taskToken": str,
+        "decisionType": DecisionTypeType,
     },
 )
-_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
+_OptionalDecisionTypeDef = TypedDict(
+    "_OptionalDecisionTypeDef",
     {
-        "decisions": Sequence[DecisionTypeDef],
-        "executionContext": str,
+        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
+        "requestCancelActivityTaskDecisionAttributes": (
+            RequestCancelActivityTaskDecisionAttributesTypeDef
+        ),
+        "completeWorkflowExecutionDecisionAttributes": (
+            CompleteWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
+        "cancelWorkflowExecutionDecisionAttributes": (
+            CancelWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionDecisionAttributes": (
+            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
+        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
+        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
+        "signalExternalWorkflowExecutionDecisionAttributes": (
+            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
+            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "startChildWorkflowExecutionDecisionAttributes": (
+            StartChildWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
     },
     total=False,
 )
 
-
-class RespondDecisionTaskCompletedInputRequestTypeDef(
-    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
-    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
-):
+class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
     pass
 
-
 DecisionTaskTypeDef = TypedDict(
     "DecisionTaskTypeDef",
     {
         "taskToken": str,
         "startedEventId": int,
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HistoryTypeDef = TypedDict(
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
+    {
+        "taskToken": str,
+    },
+)
+_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
+    {
+        "decisions": Sequence[DecisionTypeDef],
+        "executionContext": str,
+    },
+    total=False,
+)
+
+class RespondDecisionTaskCompletedInputRequestTypeDef(
+    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
+    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf/type_defs.pyi` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,33 +43,36 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
-    "ActivityTypeTypeDef",
-    "TaskListTypeDef",
+    "ActivityTypeOutputTypeDef",
+    "TaskListOutputTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
-    "ActivityTaskStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
-    "WorkflowExecutionTypeDef",
+    "WorkflowExecutionOutputTypeDef",
+    "ActivityTypeTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
-    "WorkflowTypeTypeDef",
+    "WorkflowTypeOutputTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
+    "TaskListTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
@@ -78,19 +81,21 @@
     "RecordMarkerDecisionAttributesTypeDef",
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     "RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef",
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
+    "WorkflowTypeTypeDef",
     "DescribeDomainInputRequestTypeDef",
+    "WorkflowExecutionTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
+    "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
     "MarkerRecordedEventAttributesTypeDef",
     "RecordMarkerFailedEventAttributesTypeDef",
@@ -106,103 +111,104 @@
     "TimerFiredEventAttributesTypeDef",
     "TimerStartedEventAttributesTypeDef",
     "WorkflowExecutionCanceledEventAttributesTypeDef",
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
-    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListActivityTypesInputRequestTypeDef",
-    "ListDomainsInputListDomainsPaginateTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResourceTagTypeDef",
-    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    "ResourceTagOutputTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "PendingTaskCountTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
+    "ResourceTagTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "WorkflowExecutionCountTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
-    "DeprecateActivityTypeInputRequestTypeDef",
-    "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
-    "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    "CountPendingActivityTasksInputRequestTypeDef",
-    "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
-    "PollForActivityTaskInputRequestTypeDef",
-    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    "PollForDecisionTaskInputRequestTypeDef",
-    "RegisterActivityTypeInputRequestTypeDef",
-    "RegisterWorkflowTypeInputRequestTypeDef",
-    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
+    "ActivityTaskStatusTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PendingTaskCountTypeDef",
+    "RunTypeDef",
+    "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
-    "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
-    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
+    "DeprecateActivityTypeInputRequestTypeDef",
+    "DescribeActivityTypeInputRequestTypeDef",
+    "UndeprecateActivityTypeInputRequestTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
     "StartChildWorkflowExecutionFailedEventAttributesTypeDef",
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
-    "StartWorkflowExecutionInputRequestTypeDef",
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    "CountPendingActivityTasksInputRequestTypeDef",
+    "CountPendingDecisionTasksInputRequestTypeDef",
+    "PollForActivityTaskInputRequestTypeDef",
+    "PollForDecisionTaskInputRequestTypeDef",
+    "RegisterActivityTypeInputRequestTypeDef",
+    "RegisterWorkflowTypeInputRequestTypeDef",
+    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "CountClosedWorkflowExecutionsInputRequestTypeDef",
     "CountOpenWorkflowExecutionsInputRequestTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListClosedWorkflowExecutionsInputRequestTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListOpenWorkflowExecutionsInputRequestTypeDef",
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    "DescribeWorkflowTypeInputRequestTypeDef",
+    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
+    "StartWorkflowExecutionInputRequestTypeDef",
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
+    "DescribeWorkflowExecutionInputRequestTypeDef",
+    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
+    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    "ListDomainsInputListDomainsPaginateTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
-    "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
-    "RespondDecisionTaskCompletedInputRequestTypeDef",
+    "DecisionTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
+    "RespondDecisionTaskCompletedInputRequestTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "activityId": str,
@@ -221,20 +227,22 @@
     {
         "details": str,
         "latestCancelRequestedEventId": int,
     },
     total=False,
 )
 
+
 class ActivityTaskCanceledEventAttributesTypeDef(
     _RequiredActivityTaskCanceledEventAttributesTypeDef,
     _OptionalActivityTaskCanceledEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredActivityTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -242,20 +250,22 @@
     "_OptionalActivityTaskCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class ActivityTaskCompletedEventAttributesTypeDef(
     _RequiredActivityTaskCompletedEventAttributesTypeDef,
     _OptionalActivityTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -264,30 +274,32 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class ActivityTaskFailedEventAttributesTypeDef(
     _RequiredActivityTaskFailedEventAttributesTypeDef,
     _OptionalActivityTaskFailedEventAttributesTypeDef,
 ):
     pass
 
-ActivityTypeTypeDef = TypedDict(
-    "ActivityTypeTypeDef",
+
+ActivityTypeOutputTypeDef = TypedDict(
+    "ActivityTypeOutputTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-TaskListTypeDef = TypedDict(
-    "TaskListTypeDef",
+TaskListOutputTypeDef = TypedDict(
+    "TaskListOutputTypeDef",
     {
         "name": str,
     },
 )
 
 _RequiredActivityTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskStartedEventAttributesTypeDef",
@@ -299,25 +311,30 @@
     "_OptionalActivityTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
+
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
-ActivityTaskStatusTypeDef = TypedDict(
-    "ActivityTaskStatusTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancelRequested": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredActivityTaskTimedOutEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": ActivityTaskTimeoutTypeType,
@@ -329,28 +346,38 @@
     "_OptionalActivityTaskTimedOutEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class ActivityTaskTimedOutEventAttributesTypeDef(
     _RequiredActivityTaskTimedOutEventAttributesTypeDef,
     _OptionalActivityTaskTimedOutEventAttributesTypeDef,
 ):
     pass
 
-WorkflowExecutionTypeDef = TypedDict(
-    "WorkflowExecutionTypeDef",
+
+WorkflowExecutionOutputTypeDef = TypedDict(
+    "WorkflowExecutionOutputTypeDef",
     {
         "workflowId": str,
         "runId": str,
     },
 )
 
+ActivityTypeTypeDef = TypedDict(
+    "ActivityTypeTypeDef",
+    {
+        "name": str,
+        "version": str,
+    },
+)
+
 CancelTimerDecisionAttributesTypeDef = TypedDict(
     "CancelTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
     },
 )
 
@@ -375,16 +402,16 @@
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CancelWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-WorkflowTypeTypeDef = TypedDict(
-    "WorkflowTypeTypeDef",
+WorkflowTypeOutputTypeDef = TypedDict(
+    "WorkflowTypeOutputTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
 CloseStatusFilterTypeDef = TypedDict(
@@ -406,14 +433,21 @@
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CompleteWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
+TaskListTypeDef = TypedDict(
+    "TaskListTypeDef",
+    {
+        "name": str,
+    },
+)
+
 ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -428,19 +462,21 @@
     "_OptionalExecutionTimeFilterTypeDef",
     {
         "latestDate": Union[datetime, str],
     },
     total=False,
 )
 
+
 class ExecutionTimeFilterTypeDef(
     _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
+
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -461,19 +497,21 @@
     "_OptionalWorkflowTypeFilterTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
+
 class WorkflowTypeFilterTypeDef(
     _RequiredWorkflowTypeFilterTypeDef, _OptionalWorkflowTypeFilterTypeDef
 ):
     pass
 
+
 _RequiredDecisionTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -481,40 +519,44 @@
     "_OptionalDecisionTaskCompletedEventAttributesTypeDef",
     {
         "executionContext": str,
     },
     total=False,
 )
 
+
 class DecisionTaskCompletedEventAttributesTypeDef(
     _RequiredDecisionTaskCompletedEventAttributesTypeDef,
     _OptionalDecisionTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 _OptionalDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
+
 class DecisionTaskStartedEventAttributesTypeDef(
     _RequiredDecisionTaskStartedEventAttributesTypeDef,
     _OptionalDecisionTaskStartedEventAttributesTypeDef,
 ):
     pass
 
+
 DecisionTaskTimedOutEventAttributesTypeDef = TypedDict(
     "DecisionTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "scheduledEventId": int,
         "startedEventId": int,
     },
@@ -539,19 +581,21 @@
     "_OptionalRecordMarkerDecisionAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class RecordMarkerDecisionAttributesTypeDef(
     _RequiredRecordMarkerDecisionAttributesTypeDef, _OptionalRecordMarkerDecisionAttributesTypeDef
 ):
     pass
 
+
 RequestCancelActivityTaskDecisionAttributesTypeDef = TypedDict(
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     {
         "activityId": str,
     },
 )
 
@@ -566,20 +610,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
+
 _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef = TypedDict(
     "_RequiredScheduleLambdaFunctionDecisionAttributesTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
@@ -589,20 +635,22 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
+
 class ScheduleLambdaFunctionDecisionAttributesTypeDef(
     _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef,
     _OptionalScheduleLambdaFunctionDecisionAttributesTypeDef,
 ):
     pass
 
+
 _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
     },
 )
@@ -612,20 +660,22 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
+
 class SignalExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
+
 _RequiredStartTimerDecisionAttributesTypeDef = TypedDict(
     "_RequiredStartTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
         "startToFireTimeout": str,
     },
 )
@@ -633,33 +683,51 @@
     "_OptionalStartTimerDecisionAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
+
 class StartTimerDecisionAttributesTypeDef(
     _RequiredStartTimerDecisionAttributesTypeDef, _OptionalStartTimerDecisionAttributesTypeDef
 ):
     pass
 
+
 DeprecateDomainInputRequestTypeDef = TypedDict(
     "DeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+WorkflowTypeTypeDef = TypedDict(
+    "WorkflowTypeTypeDef",
+    {
+        "name": str,
+        "version": str,
+    },
+)
+
 DescribeDomainInputRequestTypeDef = TypedDict(
     "DescribeDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+WorkflowExecutionTypeDef = TypedDict(
+    "WorkflowExecutionTypeDef",
+    {
+        "workflowId": str,
+        "runId": str,
+    },
+)
+
 DomainConfigurationTypeDef = TypedDict(
     "DomainConfigurationTypeDef",
     {
         "workflowExecutionRetentionPeriodInDays": str,
     },
 )
 
@@ -675,32 +743,37 @@
     {
         "description": str,
         "arn": str,
     },
     total=False,
 )
 
+
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
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
 _RequiredLambdaFunctionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -708,20 +781,22 @@
     "_OptionalLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class LambdaFunctionCompletedEventAttributesTypeDef(
     _RequiredLambdaFunctionCompletedEventAttributesTypeDef,
     _OptionalLambdaFunctionCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -730,20 +805,22 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class LambdaFunctionFailedEventAttributesTypeDef(
     _RequiredLambdaFunctionFailedEventAttributesTypeDef,
     _OptionalLambdaFunctionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredLambdaFunctionScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -754,20 +831,22 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
+
 class LambdaFunctionScheduledEventAttributesTypeDef(
     _RequiredLambdaFunctionScheduledEventAttributesTypeDef,
     _OptionalLambdaFunctionScheduledEventAttributesTypeDef,
 ):
     pass
 
+
 LambdaFunctionStartedEventAttributesTypeDef = TypedDict(
     "LambdaFunctionStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 
@@ -782,20 +861,22 @@
     "_OptionalLambdaFunctionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
     },
     total=False,
 )
 
+
 class LambdaFunctionTimedOutEventAttributesTypeDef(
     _RequiredLambdaFunctionTimedOutEventAttributesTypeDef,
     _OptionalLambdaFunctionTimedOutEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredMarkerRecordedEventAttributesTypeDef = TypedDict(
     "_RequiredMarkerRecordedEventAttributesTypeDef",
     {
         "markerName": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -803,19 +884,21 @@
     "_OptionalMarkerRecordedEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class MarkerRecordedEventAttributesTypeDef(
     _RequiredMarkerRecordedEventAttributesTypeDef, _OptionalMarkerRecordedEventAttributesTypeDef
 ):
     pass
 
+
 RecordMarkerFailedEventAttributesTypeDef = TypedDict(
     "RecordMarkerFailedEventAttributesTypeDef",
     {
         "markerName": str,
         "cause": Literal["OPERATION_NOT_PERMITTED"],
         "decisionTaskCompletedEventId": int,
     },
@@ -844,20 +927,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -866,20 +951,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
+
 ScheduleLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "ScheduleLambdaFunctionFailedEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "cause": ScheduleLambdaFunctionFailedCauseType,
         "decisionTaskCompletedEventId": int,
@@ -900,20 +987,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class SignalExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -924,20 +1013,22 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
+
 class SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
+
 StartLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "StartLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "cause": Literal["ASSUME_ROLE_FAILED"],
         "message": str,
     },
@@ -982,59 +1073,65 @@
     "_OptionalTimerStartedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
+
 class TimerStartedEventAttributesTypeDef(
     _RequiredTimerStartedEventAttributesTypeDef, _OptionalTimerStartedEventAttributesTypeDef
 ):
     pass
 
+
 _RequiredWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
@@ -1042,20 +1139,22 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
@@ -1064,51 +1163,30 @@
         "reason": str,
         "details": str,
         "cause": WorkflowExecutionTerminatedCauseType,
     },
     total=False,
 )
 
+
 class WorkflowExecutionTerminatedEventAttributesTypeDef(
     _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef,
     _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef,
 ):
     pass
 
+
 WorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
 
-_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListActivityTypesInputListActivityTypesPaginateTypeDef(
-    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
-    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListActivityTypesInputRequestTypeDef = TypedDict(
     "_RequiredListActivityTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1119,39 +1197,20 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
+
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
-_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDomainsInputListDomainsPaginateTypeDef(
-    _RequiredListDomainsInputListDomainsPaginateTypeDef,
-    _OptionalListDomainsInputListDomainsPaginateTypeDef,
-):
-    pass
 
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1161,66 +1220,49 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
+
 class ListDomainsInputRequestTypeDef(
     _RequiredListDomainsInputRequestTypeDef, _OptionalListDomainsInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredResourceTagTypeDef = TypedDict(
-    "_RequiredResourceTagTypeDef",
+_RequiredResourceTagOutputTypeDef = TypedDict(
+    "_RequiredResourceTagOutputTypeDef",
     {
         "key": str,
     },
 )
-_OptionalResourceTagTypeDef = TypedDict(
-    "_OptionalResourceTagTypeDef",
+_OptionalResourceTagOutputTypeDef = TypedDict(
+    "_OptionalResourceTagOutputTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
-    pass
-
-_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
-class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
-    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+class ResourceTagOutputTypeDef(
+    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
 ):
     pass
 
+
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1231,37 +1273,20 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
+
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
 ):
     pass
 
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
-PendingTaskCountTypeDef = TypedDict(
-    "PendingTaskCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
@@ -1269,20 +1294,41 @@
     "_OptionalRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class RecordActivityTaskHeartbeatInputRequestTypeDef(
     _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef,
     _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredResourceTagTypeDef = TypedDict(
+    "_RequiredResourceTagTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalResourceTagTypeDef = TypedDict(
+    "_OptionalResourceTagTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
+    pass
+
+
 _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
 )
@@ -1290,60 +1336,66 @@
     "_OptionalRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "runId": str,
     },
     total=False,
 )
 
+
 class RequestCancelWorkflowExecutionInputRequestTypeDef(
     _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef,
     _OptionalRequestCancelWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class RespondActivityTaskCanceledInputRequestTypeDef(
     _RequiredRespondActivityTaskCanceledInputRequestTypeDef,
     _OptionalRespondActivityTaskCanceledInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class RespondActivityTaskCompletedInputRequestTypeDef(
     _RequiredRespondActivityTaskCompletedInputRequestTypeDef,
     _OptionalRespondActivityTaskCompletedInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskFailedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
@@ -1351,38 +1403,21 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
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
-RunTypeDef = TypedDict(
-    "RunTypeDef",
-    {
-        "runId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
@@ -1393,20 +1428,22 @@
     {
         "runId": str,
         "input": str,
     },
     total=False,
 )
 
+
 class SignalWorkflowExecutionInputRequestTypeDef(
     _RequiredSignalWorkflowExecutionInputRequestTypeDef,
     _OptionalSignalWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredTerminateWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredTerminateWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
 )
@@ -1417,20 +1454,22 @@
         "reason": str,
         "details": str,
         "childPolicy": ChildPolicyType,
     },
     total=False,
 )
 
+
 class TerminateWorkflowExecutionInputRequestTypeDef(
     _RequiredTerminateWorkflowExecutionInputRequestTypeDef,
     _OptionalTerminateWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
+
 UndeprecateDomainInputRequestTypeDef = TypedDict(
     "UndeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -1438,23 +1477,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkflowExecutionCountTypeDef = TypedDict(
-    "WorkflowExecutionCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredWorkflowExecutionOpenCountsTypeDef = TypedDict(
     "_RequiredWorkflowExecutionOpenCountsTypeDef",
     {
         "openActivityTasks": int,
         "openDecisionTasks": int,
         "openTimers": int,
         "openChildWorkflowExecutions": int,
@@ -1464,79 +1494,59 @@
     "_OptionalWorkflowExecutionOpenCountsTypeDef",
     {
         "openLambdaFunctions": int,
     },
     total=False,
 )
 
+
 class WorkflowExecutionOpenCountsTypeDef(
     _RequiredWorkflowExecutionOpenCountsTypeDef, _OptionalWorkflowExecutionOpenCountsTypeDef
 ):
     pass
 
+
 _RequiredActivityTypeInfoTypeDef = TypedDict(
     "_RequiredActivityTypeInfoTypeDef",
     {
-        "activityType": ActivityTypeTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalActivityTypeInfoTypeDef = TypedDict(
     "_OptionalActivityTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
+
 class ActivityTypeInfoTypeDef(_RequiredActivityTypeInfoTypeDef, _OptionalActivityTypeInfoTypeDef):
     pass
 
-DeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "DeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
-DescribeActivityTypeInputRequestTypeDef = TypedDict(
-    "DescribeActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
 
 ScheduleActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
         "activityId": str,
         "cause": ScheduleActivityTaskFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
 _RequiredActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskScheduledEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
         "activityId": str,
-        "taskList": TaskListTypeDef,
+        "taskList": TaskListOutputTypeDef,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalActivityTaskScheduledEventAttributesTypeDef",
     {
         "input": str,
@@ -1546,360 +1556,170 @@
         "startToCloseTimeout": str,
         "taskPriority": str,
         "heartbeatTimeout": str,
     },
     total=False,
 )
 
+
 class ActivityTaskScheduledEventAttributesTypeDef(
     _RequiredActivityTaskScheduledEventAttributesTypeDef,
     _OptionalActivityTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
+
 ActivityTypeConfigurationTypeDef = TypedDict(
     "ActivityTypeConfigurationTypeDef",
     {
         "defaultTaskStartToCloseTimeout": str,
         "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskList": TaskListOutputTypeDef,
         "defaultTaskPriority": str,
         "defaultTaskScheduleToStartTimeout": str,
         "defaultTaskScheduleToCloseTimeout": str,
     },
     total=False,
 )
 
-ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "workflowTypeVersion": str,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-CountPendingActivityTasksInputRequestTypeDef = TypedDict(
-    "CountPendingActivityTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-
-CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
-    "CountPendingDecisionTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-
 _RequiredDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskScheduledEventAttributesTypeDef",
     {
-        "taskList": TaskListTypeDef,
+        "taskList": TaskListOutputTypeDef,
     },
 )
 _OptionalDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskScheduledEventAttributesTypeDef",
     {
         "taskPriority": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
+
 class DecisionTaskScheduledEventAttributesTypeDef(
     _RequiredDecisionTaskScheduledEventAttributesTypeDef,
     _OptionalDecisionTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
-_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForActivityTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForActivityTaskInputRequestTypeDef",
-    {
-        "identity": str,
-    },
-    total=False,
-)
-
-class PollForActivityTaskInputRequestTypeDef(
-    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
-):
-    pass
 
-_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+_RequiredWorkflowExecutionConfigurationTypeDef = TypedDict(
+    "_RequiredWorkflowExecutionConfigurationTypeDef",
     {
-        "domain": str,
-        "taskList": TaskListTypeDef,
+        "taskStartToCloseTimeout": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListOutputTypeDef,
+        "childPolicy": ChildPolicyType,
     },
 )
-_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
+_OptionalWorkflowExecutionConfigurationTypeDef = TypedDict(
+    "_OptionalWorkflowExecutionConfigurationTypeDef",
     {
-        "identity": str,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "taskPriority": str,
+        "lambdaRole": str,
     },
     total=False,
 )
 
-class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
-    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-):
-    pass
-
-_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputRequestTypeDef",
-    {
-        "identity": str,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-    },
-    total=False,
-)
 
-class PollForDecisionTaskInputRequestTypeDef(
-    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
+class WorkflowExecutionConfigurationTypeDef(
+    _RequiredWorkflowExecutionConfigurationTypeDef, _OptionalWorkflowExecutionConfigurationTypeDef
 ):
     pass
 
-_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterActivityTypeInputRequestTypeDef",
-    {
-        "description": str,
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultTaskScheduleToStartTimeout": str,
-        "defaultTaskScheduleToCloseTimeout": str,
-    },
-    total=False,
-)
 
-class RegisterActivityTypeInputRequestTypeDef(
-    _RequiredRegisterActivityTypeInputRequestTypeDef,
-    _OptionalRegisterActivityTypeInputRequestTypeDef,
-):
-    pass
-
-_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
+WorkflowTypeConfigurationTypeDef = TypedDict(
+    "WorkflowTypeConfigurationTypeDef",
     {
-        "description": str,
         "defaultTaskStartToCloseTimeout": str,
         "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskList": TaskListOutputTypeDef,
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
-class RegisterWorkflowTypeInputRequestTypeDef(
-    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
-    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
-):
-    pass
-
-_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
+ActivityTaskStatusTypeDef = TypedDict(
+    "ActivityTaskStatusTypeDef",
     {
-        "activityType": ActivityTypeTypeDef,
-        "activityId": str,
+        "cancelRequested": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "control": str,
-        "input": str,
-        "scheduleToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "scheduleToStartTimeout": str,
-        "startToCloseTimeout": str,
-        "heartbeatTimeout": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ScheduleActivityTaskDecisionAttributesTypeDef(
-    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
-    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
-):
-    pass
-
-_RequiredWorkflowExecutionConfigurationTypeDef = TypedDict(
-    "_RequiredWorkflowExecutionConfigurationTypeDef",
+PendingTaskCountTypeDef = TypedDict(
+    "PendingTaskCountTypeDef",
     {
-        "taskStartToCloseTimeout": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "childPolicy": ChildPolicyType,
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalWorkflowExecutionConfigurationTypeDef = TypedDict(
-    "_OptionalWorkflowExecutionConfigurationTypeDef",
+
+RunTypeDef = TypedDict(
+    "RunTypeDef",
     {
-        "taskPriority": str,
-        "lambdaRole": str,
+        "runId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class WorkflowExecutionConfigurationTypeDef(
-    _RequiredWorkflowExecutionConfigurationTypeDef, _OptionalWorkflowExecutionConfigurationTypeDef
-):
-    pass
-
-WorkflowTypeConfigurationTypeDef = TypedDict(
-    "WorkflowTypeConfigurationTypeDef",
+WorkflowExecutionCountTypeDef = TypedDict(
+    "WorkflowExecutionCountTypeDef",
     {
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultChildPolicy": ChildPolicyType,
-        "defaultLambdaRole": str,
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ActivityTaskTypeDef = TypedDict(
     "ActivityTaskTypeDef",
     {
         "taskToken": str,
         "activityId": str,
         "startedEventId": int,
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "activityType": ActivityTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "activityType": ActivityTypeOutputTypeDef,
         "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowExecutionInputRequestTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
         "initiatedEventId": int,
     },
 )
 
 ExternalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
         "initiatedEventId": int,
     },
 )
 
-_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
-    {
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-    },
-    total=False,
-)
-
-class GetWorkflowExecutionHistoryInputRequestTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
-):
-    pass
-
 WorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "externalWorkflowExecution": WorkflowExecutionTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
         "externalInitiatedEventId": int,
         "cause": Literal["CHILD_POLICY_APPLIED"],
     },
     total=False,
 )
 
 _RequiredWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
@@ -1908,201 +1728,190 @@
         "signalName": str,
     },
 )
 _OptionalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "input": str,
-        "externalWorkflowExecution": WorkflowExecutionTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
         "externalInitiatedEventId": int,
     },
     total=False,
 )
 
+
 class WorkflowExecutionSignaledEventAttributesTypeDef(
     _RequiredWorkflowExecutionSignaledEventAttributesTypeDef,
     _OptionalWorkflowExecutionSignaledEventAttributesTypeDef,
 ):
     pass
 
+
+DeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "DeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
+DescribeActivityTypeInputRequestTypeDef = TypedDict(
+    "DescribeActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
+UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
 _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class ChildWorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class ChildWorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class ChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 ChildWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "timeoutType": Literal["START_TO_CLOSE"],
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
-DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "workflowType": WorkflowTypeTypeDef,
-        "workflowId": str,
-    },
-)
-_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "control": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-class StartChildWorkflowExecutionDecisionAttributesTypeDef(
-    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
-    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
-):
-    pass
-
 _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "cause": StartChildWorkflowExecutionFailedCauseType,
         "workflowId": str,
         "initiatedEventId": int,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
+
 class StartChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
-        "workflowType": WorkflowTypeTypeDef,
-        "taskList": TaskListTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
+        "taskList": TaskListOutputTypeDef,
         "decisionTaskCompletedEventId": int,
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
@@ -2113,65 +1922,30 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
+
 class StartChildWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
-_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowId": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "tagList": Sequence[str],
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-class StartWorkflowExecutionInputRequestTypeDef(
-    _RequiredStartWorkflowExecutionInputRequestTypeDef,
-    _OptionalStartWorkflowExecutionInputRequestTypeDef,
-):
-    pass
-
-UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
 
 _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "newExecutionRunId": str,
-        "taskList": TaskListTypeDef,
+        "taskList": TaskListOutputTypeDef,
         "childPolicy": ChildPolicyType,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
     },
 )
 _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
@@ -2179,96 +1953,274 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionContinuedAsNewEventAttributesTypeDef(
     _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionInfoTypeDef = TypedDict(
     "_RequiredWorkflowExecutionInfoTypeDef",
     {
-        "execution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "execution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "startTimestamp": datetime,
         "executionStatus": ExecutionStatusType,
     },
 )
 _OptionalWorkflowExecutionInfoTypeDef = TypedDict(
     "_OptionalWorkflowExecutionInfoTypeDef",
     {
         "closeTimestamp": datetime,
         "closeStatus": CloseStatusType,
-        "parent": WorkflowExecutionTypeDef,
+        "parent": WorkflowExecutionOutputTypeDef,
         "tagList": List[str],
         "cancelRequested": bool,
     },
     total=False,
 )
 
+
 class WorkflowExecutionInfoTypeDef(
     _RequiredWorkflowExecutionInfoTypeDef, _OptionalWorkflowExecutionInfoTypeDef
 ):
     pass
 
+
 _RequiredWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
-        "taskList": TaskListTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "taskList": TaskListOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
     },
 )
 _OptionalWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
         "taskStartToCloseTimeout": str,
         "taskPriority": str,
         "tagList": List[str],
         "continuedExecutionRunId": str,
-        "parentWorkflowExecution": WorkflowExecutionTypeDef,
+        "parentWorkflowExecution": WorkflowExecutionOutputTypeDef,
         "parentInitiatedEventId": int,
         "lambdaRole": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionStartedEventAttributesTypeDef(
     _RequiredWorkflowExecutionStartedEventAttributesTypeDef,
     _OptionalWorkflowExecutionStartedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowTypeInfoTypeDef = TypedDict(
     "_RequiredWorkflowTypeInfoTypeDef",
     {
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalWorkflowTypeInfoTypeDef = TypedDict(
     "_OptionalWorkflowTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
+
 class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
+
+ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "workflowTypeVersion": str,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+CountPendingActivityTasksInputRequestTypeDef = TypedDict(
+    "CountPendingActivityTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
+CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
+    "CountPendingDecisionTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
+_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForActivityTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForActivityTaskInputRequestTypeDef",
+    {
+        "identity": str,
+    },
+    total=False,
+)
+
+
+class PollForActivityTaskInputRequestTypeDef(
+    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
+):
+    pass
+
+
+_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputRequestTypeDef",
+    {
+        "identity": str,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+    },
+    total=False,
+)
+
+
+class PollForDecisionTaskInputRequestTypeDef(
+    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
+):
+    pass
+
+
+_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterActivityTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultTaskHeartbeatTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultTaskScheduleToStartTimeout": str,
+        "defaultTaskScheduleToCloseTimeout": str,
+    },
+    total=False,
+)
+
+
+class RegisterActivityTypeInputRequestTypeDef(
+    _RequiredRegisterActivityTypeInputRequestTypeDef,
+    _OptionalRegisterActivityTypeInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultExecutionStartToCloseTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultChildPolicy": ChildPolicyType,
+        "defaultLambdaRole": str,
+    },
+    total=False,
+)
+
+
+class RegisterWorkflowTypeInputRequestTypeDef(
+    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
+    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "activityType": ActivityTypeTypeDef,
+        "activityId": str,
+    },
+)
+_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "scheduleToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "scheduleToStartTimeout": str,
+        "startToCloseTimeout": str,
+        "heartbeatTimeout": str,
+    },
+    total=False,
+)
+
+
+class ScheduleActivityTaskDecisionAttributesTypeDef(
+    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
+    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
+):
+    pass
+
+
 _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
@@ -2280,20 +2232,22 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
     },
     total=False,
 )
 
+
 class CountClosedWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2303,149 +2257,401 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
+
 class CountOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "startTimeFilter": ExecutionTimeFilterTypeDef,
         "closeTimeFilter": ExecutionTimeFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
         "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
+DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "workflowType": WorkflowTypeTypeDef,
+        "workflowId": str,
+    },
+)
+_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+
+class StartChildWorkflowExecutionDecisionAttributesTypeDef(
+    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
+    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
+):
+    pass
+
+
+_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowId": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "tagList": Sequence[str],
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+
+class StartWorkflowExecutionInputRequestTypeDef(
+    _RequiredStartWorkflowExecutionInputRequestTypeDef,
+    _OptionalStartWorkflowExecutionInputRequestTypeDef,
+):
+    pass
+
+
+UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+
+_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+
+class GetWorkflowExecutionHistoryInputRequestTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
+):
+    pass
+
+
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
+    {
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
+    {
+        "domainInfos": List[DomainInfoTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "domain": str,
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
+    {
+        "name": str,
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListActivityTypesInputListActivityTypesPaginateTypeDef(
+    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
+    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     {
         "startTimeFilter": ExecutionTimeFilterTypeDef,
         "closeTimeFilter": ExecutionTimeFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
         "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+
+class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+    },
+)
+_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDomainsInputListDomainsPaginateTypeDef(
+    _RequiredListDomainsInputListDomainsPaginateTypeDef,
+    _OptionalListDomainsInputListDomainsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
 _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
     _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+
+_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
+        "name": str,
         "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+
+class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
+    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
 ):
     pass
 
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
+
+_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "domain": str,
+        "taskList": TaskListTypeDef,
     },
 )
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
+_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "identity": str,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
+    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+):
+    pass
+
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "tags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[ResourceTagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
         "name": str,
@@ -2457,106 +2663,65 @@
     {
         "description": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
+
 class RegisterDomainInputRequestTypeDef(
     _RequiredRegisterDomainInputRequestTypeDef, _OptionalRegisterDomainInputRequestTypeDef
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
 )
 
 ActivityTypeInfosTypeDef = TypedDict(
     "ActivityTypeInfosTypeDef",
     {
         "typeInfos": List[ActivityTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeDetailTypeDef = TypedDict(
     "ActivityTypeDetailTypeDef",
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDecisionTypeDef = TypedDict(
-    "_RequiredDecisionTypeDef",
-    {
-        "decisionType": DecisionTypeType,
-    },
-)
-_OptionalDecisionTypeDef = TypedDict(
-    "_OptionalDecisionTypeDef",
-    {
-        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
-        "requestCancelActivityTaskDecisionAttributes": (
-            RequestCancelActivityTaskDecisionAttributesTypeDef
-        ),
-        "completeWorkflowExecutionDecisionAttributes": (
-            CompleteWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
-        "cancelWorkflowExecutionDecisionAttributes": (
-            CancelWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "continueAsNewWorkflowExecutionDecisionAttributes": (
-            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
-        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
-        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
-        "signalExternalWorkflowExecutionDecisionAttributes": (
-            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
-            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "startChildWorkflowExecutionDecisionAttributes": (
-            StartChildWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
-    pass
-
 WorkflowExecutionDetailTypeDef = TypedDict(
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
         "latestExecutionContext": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowExecutionInfosTypeDef = TypedDict(
     "WorkflowExecutionInfosTypeDef",
     {
         "executionInfos": List[WorkflowExecutionInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHistoryEventTypeDef = TypedDict(
     "_RequiredHistoryEventTypeDef",
     {
         "eventTimestamp": datetime,
@@ -2673,71 +2838,119 @@
             ScheduleLambdaFunctionFailedEventAttributesTypeDef
         ),
         "startLambdaFunctionFailedEventAttributes": StartLambdaFunctionFailedEventAttributesTypeDef,
     },
     total=False,
 )
 
+
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
+
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowTypeInfosTypeDef = TypedDict(
     "WorkflowTypeInfosTypeDef",
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
+_RequiredDecisionTypeDef = TypedDict(
+    "_RequiredDecisionTypeDef",
     {
-        "taskToken": str,
+        "decisionType": DecisionTypeType,
     },
 )
-_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
+_OptionalDecisionTypeDef = TypedDict(
+    "_OptionalDecisionTypeDef",
     {
-        "decisions": Sequence[DecisionTypeDef],
-        "executionContext": str,
+        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
+        "requestCancelActivityTaskDecisionAttributes": (
+            RequestCancelActivityTaskDecisionAttributesTypeDef
+        ),
+        "completeWorkflowExecutionDecisionAttributes": (
+            CompleteWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
+        "cancelWorkflowExecutionDecisionAttributes": (
+            CancelWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionDecisionAttributes": (
+            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
+        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
+        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
+        "signalExternalWorkflowExecutionDecisionAttributes": (
+            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
+            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "startChildWorkflowExecutionDecisionAttributes": (
+            StartChildWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
     },
     total=False,
 )
 
-class RespondDecisionTaskCompletedInputRequestTypeDef(
-    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
-    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
-):
+
+class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
     pass
 
+
 DecisionTaskTypeDef = TypedDict(
     "DecisionTaskTypeDef",
     {
         "taskToken": str,
         "startedEventId": int,
-        "workflowExecution": WorkflowExecutionTypeDef,
-        "workflowType": WorkflowTypeTypeDef,
+        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowType": WorkflowTypeOutputTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HistoryTypeDef = TypedDict(
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
+    {
+        "taskToken": str,
+    },
+)
+_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
+    {
+        "decisions": Sequence[DecisionTypeDef],
+        "executionContext": str,
+    },
+    total=False,
+)
+
+
+class RespondDecisionTaskCompletedInputRequestTypeDef(
+    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
+    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/PKG-INFO` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.28.0
-Summary: Type annotations for boto3.SWF 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SWF 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-swf"></a>
 
 # mypy-boto3-swf
 
 [![PyPI - mypy-boto3-swf](https://img.shields.io/pypi/v/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-swf?color=blue)](https://pypistats.org/packages/mypy-boto3-swf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -379,28 +379,30 @@
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
-    ActivityTypeTypeDef,
-    TaskListTypeDef,
+    ActivityTypeOutputTypeDef,
+    TaskListOutputTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ActivityTaskStatusTypeDef,
+    ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
-    WorkflowExecutionTypeDef,
+    WorkflowExecutionOutputTypeDef,
+    ActivityTypeTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
-    WorkflowTypeTypeDef,
+    WorkflowTypeOutputTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
+    TaskListTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
     ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
@@ -409,19 +411,21 @@
     RecordMarkerDecisionAttributesTypeDef,
     RequestCancelActivityTaskDecisionAttributesTypeDef,
     RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
+    WorkflowTypeTypeDef,
     DescribeDomainInputRequestTypeDef,
+    WorkflowExecutionTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
+    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -437,103 +441,104 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResourceTagTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    ResourceTagOutputTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
+    ResourceTagTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
-    DeprecateActivityTypeInputRequestTypeDef,
-    DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
-    UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
-    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
-    CountPendingActivityTasksInputRequestTypeDef,
-    CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
-    PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    PollForDecisionTaskInputRequestTypeDef,
-    RegisterActivityTypeInputRequestTypeDef,
-    RegisterWorkflowTypeInputRequestTypeDef,
-    ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
+    ActivityTaskStatusTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PendingTaskCountTypeDef,
+    RunTypeDef,
+    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
-    DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
+    DeprecateActivityTypeInputRequestTypeDef,
+    DescribeActivityTypeInputRequestTypeDef,
+    UndeprecateActivityTypeInputRequestTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
     ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
     ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
-    DeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowTypeInputRequestTypeDef,
-    StartChildWorkflowExecutionDecisionAttributesTypeDef,
     StartChildWorkflowExecutionFailedEventAttributesTypeDef,
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
-    StartWorkflowExecutionInputRequestTypeDef,
-    UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
+    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+    CountPendingActivityTasksInputRequestTypeDef,
+    CountPendingDecisionTasksInputRequestTypeDef,
+    PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputRequestTypeDef,
+    RegisterActivityTypeInputRequestTypeDef,
+    RegisterWorkflowTypeInputRequestTypeDef,
+    ScheduleActivityTaskDecisionAttributesTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
+    DeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowTypeInputRequestTypeDef,
+    StartChildWorkflowExecutionDecisionAttributesTypeDef,
+    StartWorkflowExecutionInputRequestTypeDef,
+    UndeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowExecutionInputRequestTypeDef,
+    GetWorkflowExecutionHistoryInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
-    DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
-    RespondDecisionTaskCompletedInputRequestTypeDef,
+    DecisionTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
+    RespondDecisionTaskCompletedInputRequestTypeDef,
 )
 
 
 def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-swf-1.28.0/mypy_boto3_swf.egg-info/SOURCES.txt` & `mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.0/setup.py` & `mypy-boto3-swf-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-swf",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SWF 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SWF 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

