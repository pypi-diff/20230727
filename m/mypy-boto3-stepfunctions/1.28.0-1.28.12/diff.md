# Comparing `tmp/mypy-boto3-stepfunctions-1.28.0.tar.gz` & `tmp/mypy-boto3-stepfunctions-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-stepfunctions-1.28.0.tar", last modified: Thu Jul  6 21:00:44 2023, max compression
+gzip compressed data, was "mypy-boto3-stepfunctions-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
```

## Comparing `mypy-boto3-stepfunctions-1.28.0.tar` & `mypy-boto3-stepfunctions-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:44.238445 mypy-boto3-stepfunctions-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18147 2023-07-06 21:00:44.238445 mypy-boto3-stepfunctions-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:44.230445 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-07-06 20:56:47.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-06 20:56:47.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-07-06 20:56:47.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-07-06 20:56:47.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-06 20:56:47.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-06 20:56:47.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43945 2023-07-06 20:56:48.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43880 2023-07-06 20:56:48.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:44.238445 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18147 2023-07-06 21:00:43.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 21:00:44.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:43.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:43.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:43.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 21:00:43.000000 mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:44.238445 mypy-boto3-stepfunctions-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:56:46.000000 mypy-boto3-stepfunctions-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.077344 mypy-boto3-stepfunctions-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-07-27 11:49:44.073344 mypy-boto3-stepfunctions-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.069344 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-27 11:47:40.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-27 11:47:40.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45195 2023-07-27 11:47:41.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45130 2023-07-27 11:47:40.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.073344 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.077344 mypy-boto3-stepfunctions-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/setup.py
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/LICENSE` & `mypy-boto3-stepfunctions-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.0/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.0
-Summary: Type annotations for boto3.SFN 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SFN 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,41 +352,40 @@
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
+    CloudWatchLogsLogGroupOutputTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    CreateActivityOutputTypeDef,
+    ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
-    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
-    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
+    RoutingConfigurationListItemOutputTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
+    TracingConfigurationOutputTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    GetActivityTaskOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -394,77 +393,84 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
-    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
-    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    DescribeExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
+    LogDestinationOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
+    CreateStateMachineOutputTypeDef,
+    DescribeActivityOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    GetActivityTaskOutputTypeDef,
+    ListActivitiesOutputTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    StartExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
+    StopExecutionOutputTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     ListExecutionsOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
-    CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
+    CreateStateMachineInputRequestTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
 def get_structure() -> ActivityFailedEventDetailsTypeDef:
     return {...}
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/README.md` & `mypy-boto3-stepfunctions-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,41 +320,40 @@
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
+    CloudWatchLogsLogGroupOutputTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    CreateActivityOutputTypeDef,
+    ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
-    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
-    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
+    RoutingConfigurationListItemOutputTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
+    TracingConfigurationOutputTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    GetActivityTaskOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -362,77 +361,84 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
-    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
-    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    DescribeExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
+    LogDestinationOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
+    CreateStateMachineOutputTypeDef,
+    DescribeActivityOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    GetActivityTaskOutputTypeDef,
+    ListActivitiesOutputTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    StartExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
+    StopExecutionOutputTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     ListExecutionsOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
-    CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
+    CreateStateMachineInputRequestTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
 def get_structure() -> ActivityFailedEventDetailsTypeDef:
     return {...}
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/__init__.py` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/__init__.pyi` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/__main__.py` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SFN 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SFN 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
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

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/client.py` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/client.pyi` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/literals.py` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,15 @@
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
@@ -314,26 +315,28 @@
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

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/literals.pyi` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
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
@@ -312,26 +313,28 @@
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

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/paginator.py` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,30 +68,30 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 
 class ListActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
         """
 
 
@@ -103,43 +103,43 @@
 
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listexecutionspaginator)
         """
 
 
 class ListMapRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
     """
 
     def paginate(
-        self, *, executionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, executionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMapRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
         """
 
 
 class ListStateMachinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStateMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
         """
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/paginator.pyi` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,29 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 class ListActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listactivitiespaginator)
         """
 
 class ListExecutionsPaginator(Paginator):
@@ -98,41 +98,41 @@
 
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listexecutionspaginator)
         """
 
 class ListMapRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
     """
 
     def paginate(
-        self, *, executionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, executionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMapRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listmaprunspaginator)
         """
 
 class ListStateMachinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStateMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#liststatemachinespaginator)
         """
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/type_defs.py` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,41 +36,40 @@
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
+    "CloudWatchLogsLogGroupOutputTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
-    "CreateActivityOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "RoutingConfigurationListItemTypeDef",
-    "CreateStateMachineAliasOutputTypeDef",
     "TracingConfigurationTypeDef",
-    "CreateStateMachineOutputTypeDef",
     "DeleteActivityInputRequestTypeDef",
     "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
     "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
-    "DescribeActivityOutputTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
     "DescribeStateMachineAliasInputRequestTypeDef",
+    "RoutingConfigurationListItemOutputTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
+    "TracingConfigurationOutputTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
-    "GetActivityTaskOutputTypeDef",
-    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetExecutionHistoryInputRequestTypeDef",
     "LambdaFunctionFailedEventDetailsTypeDef",
     "LambdaFunctionScheduleFailedEventDetailsTypeDef",
     "LambdaFunctionStartFailedEventDetailsTypeDef",
     "LambdaFunctionTimedOutEventDetailsTypeDef",
     "MapIterationEventDetailsTypeDef",
     "MapRunFailedEventDetailsTypeDef",
@@ -78,77 +77,84 @@
     "MapStateStartedEventDetailsTypeDef",
     "TaskFailedEventDetailsTypeDef",
     "TaskStartFailedEventDetailsTypeDef",
     "TaskStartedEventDetailsTypeDef",
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListActivitiesInputRequestTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
-    "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
     "ListStateMachineAliasesInputRequestTypeDef",
     "StateMachineAliasListItemTypeDef",
     "ListStateMachineVersionsInputRequestTypeDef",
     "StateMachineVersionListItemTypeDef",
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PublishStateMachineVersionInputRequestTypeDef",
-    "PublishStateMachineVersionOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
-    "StartExecutionOutputTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
-    "StopExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
-    "UpdateStateMachineAliasOutputTypeDef",
-    "UpdateStateMachineOutputTypeDef",
-    "ListActivitiesOutputTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "StartSyncExecutionOutputTypeDef",
+    "LogDestinationOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateActivityOutputTypeDef",
+    "CreateStateMachineAliasOutputTypeDef",
+    "CreateStateMachineOutputTypeDef",
+    "DescribeActivityOutputTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "GetActivityTaskOutputTypeDef",
+    "ListActivitiesOutputTypeDef",
+    "PublishStateMachineVersionOutputTypeDef",
+    "StartExecutionOutputTypeDef",
+    "StartSyncExecutionOutputTypeDef",
+    "StopExecutionOutputTypeDef",
+    "UpdateStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineOutputTypeDef",
     "CreateStateMachineAliasInputRequestTypeDef",
-    "DescribeStateMachineAliasOutputTypeDef",
     "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
+    "DescribeStateMachineAliasOutputTypeDef",
     "ListExecutionsOutputTypeDef",
+    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    "ListMapRunsInputListMapRunsPaginateTypeDef",
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -214,14 +220,22 @@
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     {
         "included": bool,
     },
     total=False,
 )
 
+CloudWatchLogsLogGroupOutputTypeDef = TypedDict(
+    "CloudWatchLogsLogGroupOutputTypeDef",
+    {
+        "logGroupArn": str,
+    },
+    total=False,
+)
+
 CloudWatchLogsLogGroupTypeDef = TypedDict(
     "CloudWatchLogsLogGroupTypeDef",
     {
         "logGroupArn": str,
     },
     total=False,
 )
@@ -231,58 +245,41 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-CreateActivityOutputTypeDef = TypedDict(
-    "CreateActivityOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "activityArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 RoutingConfigurationListItemTypeDef = TypedDict(
     "RoutingConfigurationListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "weight": int,
     },
 )
 
-CreateStateMachineAliasOutputTypeDef = TypedDict(
-    "CreateStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
-CreateStateMachineOutputTypeDef = TypedDict(
-    "CreateStateMachineOutputTypeDef",
-    {
-        "stateMachineArn": str,
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
@@ -310,24 +307,14 @@
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
-DescribeActivityOutputTypeDef = TypedDict(
-    "DescribeActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "name": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExecutionInputRequestTypeDef = TypedDict(
     "DescribeExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -369,21 +356,37 @@
 DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
     "DescribeStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 
+RoutingConfigurationListItemOutputTypeDef = TypedDict(
+    "RoutingConfigurationListItemOutputTypeDef",
+    {
+        "stateMachineVersionArn": str,
+        "weight": int,
+    },
+)
+
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
+TracingConfigurationOutputTypeDef = TypedDict(
+    "TracingConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+    total=False,
+)
+
 DescribeStateMachineInputRequestTypeDef = TypedDict(
     "DescribeStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
@@ -460,47 +463,24 @@
 
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
 
-GetActivityTaskOutputTypeDef = TypedDict(
-    "GetActivityTaskOutputTypeDef",
-    {
-        "taskToken": str,
-        "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "reverseOrder": bool,
-        "includeExecutionData": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
-    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetExecutionHistoryInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalGetExecutionHistoryInputRequestTypeDef = TypedDict(
@@ -695,76 +675,35 @@
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
 
-ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivitiesInputRequestTypeDef = TypedDict(
     "ListActivitiesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "stateMachineArn": str,
-        "statusFilter": ExecutionStatusType,
-        "mapRunArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExecutionsInputRequestTypeDef = TypedDict(
     "ListExecutionsInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "statusFilter": ExecutionStatusType,
         "maxResults": int,
         "nextToken": str,
         "mapRunArn": str,
     },
     total=False,
 )
 
-_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMapRunsInputListMapRunsPaginateTypeDef(
-    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
-    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMapRunsInputRequestTypeDef = TypedDict(
     "_RequiredListMapRunsInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalListMapRunsInputRequestTypeDef = TypedDict(
@@ -863,22 +802,14 @@
     "StateMachineVersionListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "creationDate": datetime,
     },
 )
 
-ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -897,20 +828,19 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "key": str,
+        "value": str,
     },
     total=False,
 )
 
 _RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
     "_RequiredPublishStateMachineVersionInputRequestTypeDef",
     {
@@ -930,34 +860,14 @@
 class PublishStateMachineVersionInputRequestTypeDef(
     _RequiredPublishStateMachineVersionInputRequestTypeDef,
     _OptionalPublishStateMachineVersionInputRequestTypeDef,
 ):
     pass
 
 
-PublishStateMachineVersionOutputTypeDef = TypedDict(
-    "PublishStateMachineVersionOutputTypeDef",
-    {
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -1010,23 +920,14 @@
 
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
 
-StartExecutionOutputTypeDef = TypedDict(
-    "StartExecutionOutputTypeDef",
-    {
-        "executionArn": str,
-        "startDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalStartSyncExecutionInputRequestTypeDef = TypedDict(
@@ -1064,22 +965,14 @@
 
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
 
-StopExecutionOutputTypeDef = TypedDict(
-    "StopExecutionOutputTypeDef",
-    {
-        "stopDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1103,41 +996,14 @@
 
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
 
-UpdateStateMachineAliasOutputTypeDef = TypedDict(
-    "UpdateStateMachineAliasOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStateMachineOutputTypeDef = TypedDict(
-    "UpdateStateMachineOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "revisionId": str,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListActivitiesOutputTypeDef = TypedDict(
-    "ListActivitiesOutputTypeDef",
-    {
-        "activities": List[ActivityListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalActivityScheduledEventDetailsTypeDef = TypedDict(
@@ -1283,14 +1149,97 @@
 
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
 
+LogDestinationOutputTypeDef = TypedDict(
+    "LogDestinationOutputTypeDef",
+    {
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupOutputTypeDef,
+    },
+    total=False,
+)
+
+LogDestinationTypeDef = TypedDict(
+    "LogDestinationTypeDef",
+    {
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateActivityInputRequestTypeDef = TypedDict(
+    "_RequiredCreateActivityInputRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateActivityInputRequestTypeDef = TypedDict(
+    "_OptionalCreateActivityInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateActivityInputRequestTypeDef(
+    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
+):
+    pass
+
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateActivityOutputTypeDef = TypedDict(
+    "CreateActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineAliasOutputTypeDef = TypedDict(
+    "CreateStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineOutputTypeDef = TypedDict(
+    "CreateStateMachineOutputTypeDef",
+    {
+        "stateMachineArn": str,
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeActivityOutputTypeDef = TypedDict(
+    "DescribeActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "name": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeExecutionOutputTypeDef = TypedDict(
     "DescribeExecutionOutputTypeDef",
     {
         "executionArn": str,
         "stateMachineArn": str,
         "name": str,
         "status": ExecutionStatusType,
@@ -1302,15 +1251,51 @@
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
         "stateMachineVersionArn": str,
         "stateMachineAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetActivityTaskOutputTypeDef = TypedDict(
+    "GetActivityTaskOutputTypeDef",
+    {
+        "taskToken": str,
+        "input": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListActivitiesOutputTypeDef = TypedDict(
+    "ListActivitiesOutputTypeDef",
+    {
+        "activities": List[ActivityListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishStateMachineVersionOutputTypeDef = TypedDict(
+    "PublishStateMachineVersionOutputTypeDef",
+    {
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExecutionOutputTypeDef = TypedDict(
+    "StartExecutionOutputTypeDef",
+    {
+        "executionArn": str,
+        "startDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSyncExecutionOutputTypeDef = TypedDict(
     "StartSyncExecutionOutputTypeDef",
     {
         "executionArn": str,
@@ -1323,60 +1308,41 @@
         "cause": str,
         "input": str,
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "billingDetails": BillingDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LogDestinationTypeDef = TypedDict(
-    "LogDestinationTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredCreateActivityInputRequestTypeDef = TypedDict(
-    "_RequiredCreateActivityInputRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateActivityInputRequestTypeDef = TypedDict(
-    "_OptionalCreateActivityInputRequestTypeDef",
+StopExecutionOutputTypeDef = TypedDict(
+    "StopExecutionOutputTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "stopDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateActivityInputRequestTypeDef(
-    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
-):
-    pass
-
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UpdateStateMachineAliasOutputTypeDef = TypedDict(
+    "UpdateStateMachineAliasOutputTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+UpdateStateMachineOutputTypeDef = TypedDict(
+    "UpdateStateMachineOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "updateDate": datetime,
+        "revisionId": str,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineAliasInputRequestTypeDef",
     {
         "name": str,
@@ -1395,27 +1361,14 @@
 class CreateStateMachineAliasInputRequestTypeDef(
     _RequiredCreateStateMachineAliasInputRequestTypeDef,
     _OptionalCreateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
 
-DescribeStateMachineAliasOutputTypeDef = TypedDict(
-    "DescribeStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "name": str,
-        "description": str,
-        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
-        "creationDate": datetime,
-        "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 _OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
@@ -1444,27 +1397,113 @@
         "startDate": datetime,
         "stopDate": datetime,
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
         "itemCounts": MapRunItemCountsTypeDef,
         "executionCounts": MapRunExecutionCountsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStateMachineAliasOutputTypeDef = TypedDict(
+    "DescribeStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "name": str,
+        "description": str,
+        "routingConfiguration": List[RoutingConfigurationListItemOutputTypeDef],
+        "creationDate": datetime,
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "includeExecutionData": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
+    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+
+ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "stateMachineArn": str,
+        "statusFilter": ExecutionStatusType,
+        "mapRunArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMapRunsInputListMapRunsPaginateTypeDef(
+    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
+    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+):
+    pass
+
+
+ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
@@ -1513,45 +1552,63 @@
 
 
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineAliasesOutputTypeDef = TypedDict(
     "ListStateMachineAliasesOutputTypeDef",
     {
         "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineVersionsOutputTypeDef = TypedDict(
     "ListStateMachineVersionsOutputTypeDef",
     {
         "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "level": LogLevelType,
+        "includeExecutionData": bool,
+        "destinations": List[LogDestinationOutputTypeDef],
+    },
+    total=False,
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
         "destinations": Sequence[LogDestinationTypeDef],
     },
@@ -1609,78 +1666,78 @@
 )
 
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
 
-_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineInputRequestTypeDef",
-    {
-        "type": StateMachineTypeType,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
-    },
-    total=False,
-)
-
-
-class CreateStateMachineInputRequestTypeDef(
-    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
-):
-    pass
-
-
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tracingConfiguration": TracingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationOutputTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tracingConfiguration": TracingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationOutputTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
+    },
+)
+_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineInputRequestTypeDef",
+    {
+        "type": StateMachineTypeType,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
     },
+    total=False,
 )
 
+
+class CreateStateMachineInputRequestTypeDef(
+    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
@@ -1704,10 +1761,10 @@
 
 
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions/type_defs.pyi` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -35,41 +35,40 @@
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
+    "CloudWatchLogsLogGroupOutputTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
-    "CreateActivityOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "RoutingConfigurationListItemTypeDef",
-    "CreateStateMachineAliasOutputTypeDef",
     "TracingConfigurationTypeDef",
-    "CreateStateMachineOutputTypeDef",
     "DeleteActivityInputRequestTypeDef",
     "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
     "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
-    "DescribeActivityOutputTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
     "DescribeStateMachineAliasInputRequestTypeDef",
+    "RoutingConfigurationListItemOutputTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
+    "TracingConfigurationOutputTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
-    "GetActivityTaskOutputTypeDef",
-    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetExecutionHistoryInputRequestTypeDef",
     "LambdaFunctionFailedEventDetailsTypeDef",
     "LambdaFunctionScheduleFailedEventDetailsTypeDef",
     "LambdaFunctionStartFailedEventDetailsTypeDef",
     "LambdaFunctionTimedOutEventDetailsTypeDef",
     "MapIterationEventDetailsTypeDef",
     "MapRunFailedEventDetailsTypeDef",
@@ -77,77 +76,84 @@
     "MapStateStartedEventDetailsTypeDef",
     "TaskFailedEventDetailsTypeDef",
     "TaskStartFailedEventDetailsTypeDef",
     "TaskStartedEventDetailsTypeDef",
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListActivitiesInputRequestTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
-    "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
     "ListStateMachineAliasesInputRequestTypeDef",
     "StateMachineAliasListItemTypeDef",
     "ListStateMachineVersionsInputRequestTypeDef",
     "StateMachineVersionListItemTypeDef",
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PublishStateMachineVersionInputRequestTypeDef",
-    "PublishStateMachineVersionOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
-    "StartExecutionOutputTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
-    "StopExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
-    "UpdateStateMachineAliasOutputTypeDef",
-    "UpdateStateMachineOutputTypeDef",
-    "ListActivitiesOutputTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "StartSyncExecutionOutputTypeDef",
+    "LogDestinationOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateActivityOutputTypeDef",
+    "CreateStateMachineAliasOutputTypeDef",
+    "CreateStateMachineOutputTypeDef",
+    "DescribeActivityOutputTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "GetActivityTaskOutputTypeDef",
+    "ListActivitiesOutputTypeDef",
+    "PublishStateMachineVersionOutputTypeDef",
+    "StartExecutionOutputTypeDef",
+    "StartSyncExecutionOutputTypeDef",
+    "StopExecutionOutputTypeDef",
+    "UpdateStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineOutputTypeDef",
     "CreateStateMachineAliasInputRequestTypeDef",
-    "DescribeStateMachineAliasOutputTypeDef",
     "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
+    "DescribeStateMachineAliasOutputTypeDef",
     "ListExecutionsOutputTypeDef",
+    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    "ListMapRunsInputListMapRunsPaginateTypeDef",
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -213,14 +219,22 @@
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     {
         "included": bool,
     },
     total=False,
 )
 
+CloudWatchLogsLogGroupOutputTypeDef = TypedDict(
+    "CloudWatchLogsLogGroupOutputTypeDef",
+    {
+        "logGroupArn": str,
+    },
+    total=False,
+)
+
 CloudWatchLogsLogGroupTypeDef = TypedDict(
     "CloudWatchLogsLogGroupTypeDef",
     {
         "logGroupArn": str,
     },
     total=False,
 )
@@ -230,58 +244,41 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-CreateActivityOutputTypeDef = TypedDict(
-    "CreateActivityOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "activityArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 RoutingConfigurationListItemTypeDef = TypedDict(
     "RoutingConfigurationListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "weight": int,
     },
 )
 
-CreateStateMachineAliasOutputTypeDef = TypedDict(
-    "CreateStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
-CreateStateMachineOutputTypeDef = TypedDict(
-    "CreateStateMachineOutputTypeDef",
-    {
-        "stateMachineArn": str,
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
@@ -309,24 +306,14 @@
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
-DescribeActivityOutputTypeDef = TypedDict(
-    "DescribeActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "name": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExecutionInputRequestTypeDef = TypedDict(
     "DescribeExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -368,21 +355,37 @@
 DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
     "DescribeStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 
+RoutingConfigurationListItemOutputTypeDef = TypedDict(
+    "RoutingConfigurationListItemOutputTypeDef",
+    {
+        "stateMachineVersionArn": str,
+        "weight": int,
+    },
+)
+
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
+TracingConfigurationOutputTypeDef = TypedDict(
+    "TracingConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+    total=False,
+)
+
 DescribeStateMachineInputRequestTypeDef = TypedDict(
     "DescribeStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
@@ -455,45 +458,24 @@
 )
 
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
-GetActivityTaskOutputTypeDef = TypedDict(
-    "GetActivityTaskOutputTypeDef",
-    {
-        "taskToken": str,
-        "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "reverseOrder": bool,
-        "includeExecutionData": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
-    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetExecutionHistoryInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalGetExecutionHistoryInputRequestTypeDef = TypedDict(
@@ -678,74 +660,35 @@
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
 
-ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivitiesInputRequestTypeDef = TypedDict(
     "ListActivitiesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "stateMachineArn": str,
-        "statusFilter": ExecutionStatusType,
-        "mapRunArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExecutionsInputRequestTypeDef = TypedDict(
     "ListExecutionsInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "statusFilter": ExecutionStatusType,
         "maxResults": int,
         "nextToken": str,
         "mapRunArn": str,
     },
     total=False,
 )
 
-_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMapRunsInputListMapRunsPaginateTypeDef(
-    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
-    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMapRunsInputRequestTypeDef = TypedDict(
     "_RequiredListMapRunsInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalListMapRunsInputRequestTypeDef = TypedDict(
@@ -836,22 +779,14 @@
     "StateMachineVersionListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "creationDate": datetime,
     },
 )
 
-ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -870,20 +805,19 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "key": str,
+        "value": str,
     },
     total=False,
 )
 
 _RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
     "_RequiredPublishStateMachineVersionInputRequestTypeDef",
     {
@@ -901,34 +835,14 @@
 
 class PublishStateMachineVersionInputRequestTypeDef(
     _RequiredPublishStateMachineVersionInputRequestTypeDef,
     _OptionalPublishStateMachineVersionInputRequestTypeDef,
 ):
     pass
 
-PublishStateMachineVersionOutputTypeDef = TypedDict(
-    "PublishStateMachineVersionOutputTypeDef",
-    {
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -977,23 +891,14 @@
 )
 
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
-StartExecutionOutputTypeDef = TypedDict(
-    "StartExecutionOutputTypeDef",
-    {
-        "executionArn": str,
-        "startDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalStartSyncExecutionInputRequestTypeDef = TypedDict(
@@ -1027,22 +932,14 @@
 )
 
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
-StopExecutionOutputTypeDef = TypedDict(
-    "StopExecutionOutputTypeDef",
-    {
-        "stopDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1064,41 +961,14 @@
 )
 
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
-UpdateStateMachineAliasOutputTypeDef = TypedDict(
-    "UpdateStateMachineAliasOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStateMachineOutputTypeDef = TypedDict(
-    "UpdateStateMachineOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "revisionId": str,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListActivitiesOutputTypeDef = TypedDict(
-    "ListActivitiesOutputTypeDef",
-    {
-        "activities": List[ActivityListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalActivityScheduledEventDetailsTypeDef = TypedDict(
@@ -1234,14 +1104,95 @@
 )
 
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
+LogDestinationOutputTypeDef = TypedDict(
+    "LogDestinationOutputTypeDef",
+    {
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupOutputTypeDef,
+    },
+    total=False,
+)
+
+LogDestinationTypeDef = TypedDict(
+    "LogDestinationTypeDef",
+    {
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateActivityInputRequestTypeDef = TypedDict(
+    "_RequiredCreateActivityInputRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateActivityInputRequestTypeDef = TypedDict(
+    "_OptionalCreateActivityInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateActivityInputRequestTypeDef(
+    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
+):
+    pass
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateActivityOutputTypeDef = TypedDict(
+    "CreateActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineAliasOutputTypeDef = TypedDict(
+    "CreateStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineOutputTypeDef = TypedDict(
+    "CreateStateMachineOutputTypeDef",
+    {
+        "stateMachineArn": str,
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeActivityOutputTypeDef = TypedDict(
+    "DescribeActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "name": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeExecutionOutputTypeDef = TypedDict(
     "DescribeExecutionOutputTypeDef",
     {
         "executionArn": str,
         "stateMachineArn": str,
         "name": str,
         "status": ExecutionStatusType,
@@ -1253,15 +1204,51 @@
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
         "stateMachineVersionArn": str,
         "stateMachineAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetActivityTaskOutputTypeDef = TypedDict(
+    "GetActivityTaskOutputTypeDef",
+    {
+        "taskToken": str,
+        "input": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListActivitiesOutputTypeDef = TypedDict(
+    "ListActivitiesOutputTypeDef",
+    {
+        "activities": List[ActivityListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishStateMachineVersionOutputTypeDef = TypedDict(
+    "PublishStateMachineVersionOutputTypeDef",
+    {
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExecutionOutputTypeDef = TypedDict(
+    "StartExecutionOutputTypeDef",
+    {
+        "executionArn": str,
+        "startDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSyncExecutionOutputTypeDef = TypedDict(
     "StartSyncExecutionOutputTypeDef",
     {
         "executionArn": str,
@@ -1274,58 +1261,41 @@
         "cause": str,
         "input": str,
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "billingDetails": BillingDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogDestinationTypeDef = TypedDict(
-    "LogDestinationTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateActivityInputRequestTypeDef = TypedDict(
-    "_RequiredCreateActivityInputRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateActivityInputRequestTypeDef = TypedDict(
-    "_OptionalCreateActivityInputRequestTypeDef",
+StopExecutionOutputTypeDef = TypedDict(
+    "StopExecutionOutputTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "stopDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateActivityInputRequestTypeDef(
-    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
-):
-    pass
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UpdateStateMachineAliasOutputTypeDef = TypedDict(
+    "UpdateStateMachineAliasOutputTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+UpdateStateMachineOutputTypeDef = TypedDict(
+    "UpdateStateMachineOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "updateDate": datetime,
+        "revisionId": str,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineAliasInputRequestTypeDef",
     {
         "name": str,
@@ -1342,27 +1312,14 @@
 
 class CreateStateMachineAliasInputRequestTypeDef(
     _RequiredCreateStateMachineAliasInputRequestTypeDef,
     _OptionalCreateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
-DescribeStateMachineAliasOutputTypeDef = TypedDict(
-    "DescribeStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "name": str,
-        "description": str,
-        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
-        "creationDate": datetime,
-        "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 _OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
@@ -1389,25 +1346,107 @@
         "startDate": datetime,
         "stopDate": datetime,
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
         "itemCounts": MapRunItemCountsTypeDef,
         "executionCounts": MapRunExecutionCountsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStateMachineAliasOutputTypeDef = TypedDict(
+    "DescribeStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "name": str,
+        "description": str,
+        "routingConfiguration": List[RoutingConfigurationListItemOutputTypeDef],
+        "creationDate": datetime,
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "includeExecutionData": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
+    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "stateMachineArn": str,
+        "statusFilter": ExecutionStatusType,
+        "mapRunArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMapRunsInputListMapRunsPaginateTypeDef(
+    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
+    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+):
+    pass
+
+ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 _RequiredLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
@@ -1454,45 +1493,63 @@
     pass
 
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineAliasesOutputTypeDef = TypedDict(
     "ListStateMachineAliasesOutputTypeDef",
     {
         "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineVersionsOutputTypeDef = TypedDict(
     "ListStateMachineVersionsOutputTypeDef",
     {
         "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "level": LogLevelType,
+        "includeExecutionData": bool,
+        "destinations": List[LogDestinationOutputTypeDef],
+    },
+    total=False,
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
         "destinations": Sequence[LogDestinationTypeDef],
     },
@@ -1548,76 +1605,76 @@
     },
     total=False,
 )
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
-_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineInputRequestTypeDef",
-    {
-        "type": StateMachineTypeType,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
-    },
-    total=False,
-)
-
-class CreateStateMachineInputRequestTypeDef(
-    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
-):
-    pass
-
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tracingConfiguration": TracingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationOutputTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tracingConfiguration": TracingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationOutputTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
+    },
+)
+_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineInputRequestTypeDef",
+    {
+        "type": StateMachineTypeType,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
+    },
+    total=False,
+)
+
+class CreateStateMachineInputRequestTypeDef(
+    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
+):
+    pass
+
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
@@ -1639,10 +1696,10 @@
     pass
 
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.0
-Summary: Type annotations for boto3.SFN 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SFN 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,41 +352,40 @@
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
+    CloudWatchLogsLogGroupOutputTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    CreateActivityOutputTypeDef,
+    ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
-    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
-    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
+    RoutingConfigurationListItemOutputTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
+    TracingConfigurationOutputTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    GetActivityTaskOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -394,77 +393,84 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
-    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
-    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    DescribeExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
+    LogDestinationOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
+    CreateStateMachineOutputTypeDef,
+    DescribeActivityOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    GetActivityTaskOutputTypeDef,
+    ListActivitiesOutputTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    StartExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
+    StopExecutionOutputTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     ListExecutionsOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
-    CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
+    CreateStateMachineInputRequestTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
 def get_structure() -> ActivityFailedEventDetailsTypeDef:
     return {...}
```

### Comparing `mypy-boto3-stepfunctions-1.28.0/mypy_boto3_stepfunctions.egg-info/SOURCES.txt` & `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.0/setup.py` & `mypy-boto3-stepfunctions-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-stepfunctions",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SFN 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SFN 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

