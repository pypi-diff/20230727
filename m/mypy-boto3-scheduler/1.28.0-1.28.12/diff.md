# Comparing `tmp/mypy-boto3-scheduler-1.28.0.tar.gz` & `tmp/mypy-boto3-scheduler-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-scheduler-1.28.0.tar", last modified: Thu Jul  6 21:00:33 2023, max compression
+gzip compressed data, was "mypy-boto3-scheduler-1.28.12.tar", last modified: Thu Jul 27 11:49:35 2023, max compression
```

## Comparing `mypy-boto3-scheduler-1.28.0.tar` & `mypy-boto3-scheduler-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.874423 mypy-boto3-scheduler-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-06 21:00:33.862423 mypy-boto3-scheduler-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.858423 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-07-06 20:54:58.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.862423 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-06 21:00:33.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:33.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:33.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:33.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:33.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:33.000000 mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:33.874423 mypy-boto3-scheduler-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-06 20:54:57.000000 mypy-boto3-scheduler-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.945266 mypy-boto3-scheduler-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-27 11:49:35.945266 mypy-boto3-scheduler-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.941266 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-27 11:46:02.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-27 11:46:02.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-27 11:46:02.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-27 11:46:02.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.945266 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-27 11:49:35.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:35.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:35.000000 mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:35.945266 mypy-boto3-scheduler-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-27 11:46:01.000000 mypy-boto3-scheduler-1.28.12/setup.py
```

### Comparing `mypy-boto3-scheduler-1.28.0/LICENSE` & `mypy-boto3-scheduler-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.0/PKG-INFO` & `mypy-boto3-scheduler-1.28.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.0
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-scheduler"></a>
 
 # mypy-boto3-scheduler
 
 [![PyPI - mypy-boto3-scheduler](https://img.shields.io/pypi/v/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-scheduler?color=blue)](https://pypistats.org/packages/mypy-boto3-scheduler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-scheduler)](https://pepy.tech/project/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,61 +331,77 @@
 ### Typed dictionaries
 
 `mypy_boto3_scheduler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
-    CreateScheduleGroupOutputTypeDef,
+    ResponseMetadataTypeDef,
     FlexibleTimeWindowTypeDef,
-    CreateScheduleOutputTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
+    EventBridgeParametersOutputTypeDef,
     EventBridgeParametersTypeDef,
+    FlexibleTimeWindowOutputTypeDef,
     GetScheduleGroupInputRequestTypeDef,
-    GetScheduleGroupOutputTypeDef,
     GetScheduleInputRequestTypeDef,
+    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduleGroupsInputRequestTypeDef,
     ScheduleGroupSummaryTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListSchedulesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
+    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
     TargetSummaryTypeDef,
+    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateScheduleOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     CreateScheduleGroupInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateScheduleGroupOutputTypeDef,
+    CreateScheduleOutputTypeDef,
+    GetScheduleGroupOutputTypeDef,
+    UpdateScheduleOutputTypeDef,
+    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
+    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListScheduleGroupsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     ScheduleSummaryTypeDef,
+    EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
-    CreateScheduleInputRequestTypeDef,
     GetScheduleOutputTypeDef,
+    CreateScheduleInputRequestTypeDef,
     UpdateScheduleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationTypeDef:
+def get_structure() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-scheduler-1.28.0/README.md` & `mypy-boto3-scheduler-1.28.12/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-scheduler"></a>
 
 # mypy-boto3-scheduler
 
 [![PyPI - mypy-boto3-scheduler](https://img.shields.io/pypi/v/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-scheduler?color=blue)](https://pypistats.org/packages/mypy-boto3-scheduler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-scheduler)](https://pepy.tech/project/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,61 +299,77 @@
 ### Typed dictionaries
 
 `mypy_boto3_scheduler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
-    CreateScheduleGroupOutputTypeDef,
+    ResponseMetadataTypeDef,
     FlexibleTimeWindowTypeDef,
-    CreateScheduleOutputTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
+    EventBridgeParametersOutputTypeDef,
     EventBridgeParametersTypeDef,
+    FlexibleTimeWindowOutputTypeDef,
     GetScheduleGroupInputRequestTypeDef,
-    GetScheduleGroupOutputTypeDef,
     GetScheduleInputRequestTypeDef,
+    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduleGroupsInputRequestTypeDef,
     ScheduleGroupSummaryTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListSchedulesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
+    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
     TargetSummaryTypeDef,
+    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateScheduleOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     CreateScheduleGroupInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateScheduleGroupOutputTypeDef,
+    CreateScheduleOutputTypeDef,
+    GetScheduleGroupOutputTypeDef,
+    UpdateScheduleOutputTypeDef,
+    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
+    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListScheduleGroupsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     ScheduleSummaryTypeDef,
+    EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
-    CreateScheduleInputRequestTypeDef,
     GetScheduleOutputTypeDef,
+    CreateScheduleInputRequestTypeDef,
     UpdateScheduleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationTypeDef:
+def get_structure() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/__init__.py` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/__init__.pyi` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/__main__.py` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgeScheduler 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.EventBridgeScheduler 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
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

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/client.py` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/client.pyi` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/literals.py` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,15 @@
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
@@ -250,26 +251,28 @@
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

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/literals.pyi` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
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
@@ -248,26 +249,28 @@
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

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/paginator.py` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -30,51 +30,47 @@
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListScheduleGroupsPaginator", "ListSchedulesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListScheduleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
     """
 
     def paginate(
-        self, *, NamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, NamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScheduleGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
         """
 
-
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
     """
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         NamePrefix: str = ...,
         State: ScheduleStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchedulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/paginator.pyi` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,47 +30,51 @@
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListScheduleGroupsPaginator", "ListSchedulesPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListScheduleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
     """
 
     def paginate(
-        self, *, NamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, NamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScheduleGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListScheduleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulegroupspaginator)
         """
 
+
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
     """
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         NamePrefix: str = ...,
         State: ScheduleStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchedulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/type_defs.py` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/type_defs.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for scheduler service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_scheduler.type_defs import AwsVpcConfigurationTypeDef
+    from mypy_boto3_scheduler.type_defs import AwsVpcConfigurationOutputTypeDef
 
-    data: AwsVpcConfigurationTypeDef = {...}
+    data: AwsVpcConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,61 +30,96 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
+    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
-    "CreateScheduleGroupOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "FlexibleTimeWindowTypeDef",
-    "CreateScheduleOutputTypeDef",
+    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeleteScheduleGroupInputRequestTypeDef",
     "DeleteScheduleInputRequestTypeDef",
+    "PlacementConstraintOutputTypeDef",
+    "PlacementStrategyOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
+    "EventBridgeParametersOutputTypeDef",
     "EventBridgeParametersTypeDef",
+    "FlexibleTimeWindowOutputTypeDef",
     "GetScheduleGroupInputRequestTypeDef",
-    "GetScheduleGroupOutputTypeDef",
     "GetScheduleInputRequestTypeDef",
+    "KinesisParametersOutputTypeDef",
     "KinesisParametersTypeDef",
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListScheduleGroupsInputRequestTypeDef",
     "ScheduleGroupSummaryTypeDef",
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListSchedulesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
+    "RetryPolicyOutputTypeDef",
     "RetryPolicyTypeDef",
+    "SageMakerPipelineParameterOutputTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "TargetSummaryTypeDef",
+    "SqsParametersOutputTypeDef",
     "SqsParametersTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateScheduleOutputTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateScheduleGroupInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateScheduleGroupOutputTypeDef",
+    "CreateScheduleOutputTypeDef",
+    "GetScheduleGroupOutputTypeDef",
+    "UpdateScheduleOutputTypeDef",
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListScheduleGroupsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "ScheduleSummaryTypeDef",
+    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
+    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "CreateScheduleInputRequestTypeDef",
     "GetScheduleOutputTypeDef",
+    "CreateScheduleInputRequestTypeDef",
     "UpdateScheduleInputRequestTypeDef",
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "Subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "AssignPublicIp": AssignPublicIpType,
+        "SecurityGroups": List[str],
+    },
+    total=False,
+)
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "Subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -92,20 +127,39 @@
     {
         "AssignPublicIp": AssignPublicIpType,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "capacityProvider": str,
+    },
+)
+_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "base": int,
+        "weight": int,
+    },
+    total=False,
+)
+
+class CapacityProviderStrategyItemOutputTypeDef(
+    _RequiredCapacityProviderStrategyItemOutputTypeDef,
+    _OptionalCapacityProviderStrategyItemOutputTypeDef,
+):
+    pass
 
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
@@ -114,34 +168,35 @@
     {
         "base": int,
         "weight": int,
     },
     total=False,
 )
 
-
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateScheduleGroupOutputTypeDef = TypedDict(
-    "CreateScheduleGroupOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScheduleGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredFlexibleTimeWindowTypeDef = TypedDict(
     "_RequiredFlexibleTimeWindowTypeDef",
     {
         "Mode": FlexibleTimeWindowModeType,
@@ -151,27 +206,25 @@
     "_OptionalFlexibleTimeWindowTypeDef",
     {
         "MaximumWindowInMinutes": int,
     },
     total=False,
 )
 
-
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
-
-CreateScheduleOutputTypeDef = TypedDict(
-    "CreateScheduleOutputTypeDef",
+DeadLetterConfigOutputTypeDef = TypedDict(
+    "DeadLetterConfigOutputTypeDef",
     {
-        "ScheduleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Arn": str,
     },
+    total=False,
 )
 
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
@@ -188,21 +241,19 @@
     "_OptionalDeleteScheduleGroupInputRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteScheduleGroupInputRequestTypeDef(
     _RequiredDeleteScheduleGroupInputRequestTypeDef, _OptionalDeleteScheduleGroupInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteScheduleInputRequestTypeDef = TypedDict(
     "_RequiredDeleteScheduleInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteScheduleInputRequestTypeDef = TypedDict(
@@ -210,20 +261,36 @@
     {
         "ClientToken": str,
         "GroupName": str,
     },
     total=False,
 )
 
-
 class DeleteScheduleInputRequestTypeDef(
     _RequiredDeleteScheduleInputRequestTypeDef, _OptionalDeleteScheduleInputRequestTypeDef
 ):
     pass
 
+PlacementConstraintOutputTypeDef = TypedDict(
+    "PlacementConstraintOutputTypeDef",
+    {
+        "expression": str,
+        "type": PlacementConstraintTypeType,
+    },
+    total=False,
+)
+
+PlacementStrategyOutputTypeDef = TypedDict(
+    "PlacementStrategyOutputTypeDef",
+    {
+        "field": str,
+        "type": PlacementStrategyTypeType,
+    },
+    total=False,
+)
 
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "expression": str,
         "type": PlacementConstraintTypeType,
     },
@@ -235,38 +302,53 @@
     {
         "field": str,
         "type": PlacementStrategyTypeType,
     },
     total=False,
 )
 
+EventBridgeParametersOutputTypeDef = TypedDict(
+    "EventBridgeParametersOutputTypeDef",
+    {
+        "DetailType": str,
+        "Source": str,
+    },
+)
+
 EventBridgeParametersTypeDef = TypedDict(
     "EventBridgeParametersTypeDef",
     {
         "DetailType": str,
         "Source": str,
     },
 )
 
-GetScheduleGroupInputRequestTypeDef = TypedDict(
-    "GetScheduleGroupInputRequestTypeDef",
+_RequiredFlexibleTimeWindowOutputTypeDef = TypedDict(
+    "_RequiredFlexibleTimeWindowOutputTypeDef",
     {
-        "Name": str,
+        "Mode": FlexibleTimeWindowModeType,
     },
 )
+_OptionalFlexibleTimeWindowOutputTypeDef = TypedDict(
+    "_OptionalFlexibleTimeWindowOutputTypeDef",
+    {
+        "MaximumWindowInMinutes": int,
+    },
+    total=False,
+)
 
-GetScheduleGroupOutputTypeDef = TypedDict(
-    "GetScheduleGroupOutputTypeDef",
+class FlexibleTimeWindowOutputTypeDef(
+    _RequiredFlexibleTimeWindowOutputTypeDef, _OptionalFlexibleTimeWindowOutputTypeDef
+):
+    pass
+
+GetScheduleGroupInputRequestTypeDef = TypedDict(
+    "GetScheduleGroupInputRequestTypeDef",
     {
-        "Arn": str,
-        "CreationDate": datetime,
-        "LastModificationDate": datetime,
         "Name": str,
-        "State": ScheduleGroupStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetScheduleInputRequestTypeDef = TypedDict(
     "_RequiredGetScheduleInputRequestTypeDef",
     {
         "Name": str,
@@ -276,33 +358,39 @@
     "_OptionalGetScheduleInputRequestTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
-
 class GetScheduleInputRequestTypeDef(
     _RequiredGetScheduleInputRequestTypeDef, _OptionalGetScheduleInputRequestTypeDef
 ):
     pass
 
+KinesisParametersOutputTypeDef = TypedDict(
+    "KinesisParametersOutputTypeDef",
+    {
+        "PartitionKey": str,
+    },
+)
 
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
-ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "NamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListScheduleGroupsInputRequestTypeDef = TypedDict(
     "ListScheduleGroupsInputRequestTypeDef",
     {
@@ -321,25 +409,14 @@
         "LastModificationDate": datetime,
         "Name": str,
         "State": ScheduleGroupStateType,
     },
     total=False,
 )
 
-ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
-    {
-        "GroupName": str,
-        "NamePrefix": str,
-        "State": ScheduleStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSchedulesInputRequestTypeDef = TypedDict(
     "ListSchedulesInputRequestTypeDef",
     {
         "GroupName": str,
         "MaxResults": int,
         "NamePrefix": str,
         "NextToken": str,
@@ -351,44 +428,48 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RetryPolicyOutputTypeDef = TypedDict(
+    "RetryPolicyOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MaximumEventAgeInSeconds": int,
+        "MaximumRetryAttempts": int,
     },
+    total=False,
 )
 
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumEventAgeInSeconds": int,
         "MaximumRetryAttempts": int,
     },
     total=False,
 )
 
+SageMakerPipelineParameterOutputTypeDef = TypedDict(
+    "SageMakerPipelineParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -396,14 +477,22 @@
 TargetSummaryTypeDef = TypedDict(
     "TargetSummaryTypeDef",
     {
         "Arn": str,
     },
 )
 
+SqsParametersOutputTypeDef = TypedDict(
+    "SqsParametersOutputTypeDef",
+    {
+        "MessageGroupId": str,
+    },
+    total=False,
+)
+
 SqsParametersTypeDef = TypedDict(
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
@@ -412,20 +501,20 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateScheduleOutputTypeDef = TypedDict(
-    "UpdateScheduleOutputTypeDef",
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
     {
-        "ScheduleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
@@ -443,44 +532,106 @@
     {
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateScheduleGroupInputRequestTypeDef(
     _RequiredCreateScheduleGroupInputRequestTypeDef, _OptionalCreateScheduleGroupInputRequestTypeDef
 ):
     pass
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+CreateScheduleGroupOutputTypeDef = TypedDict(
+    "CreateScheduleGroupOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ScheduleGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+CreateScheduleOutputTypeDef = TypedDict(
+    "CreateScheduleOutputTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ScheduleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetScheduleGroupOutputTypeDef = TypedDict(
+    "GetScheduleGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationDate": datetime,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "State": ScheduleGroupStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduleOutputTypeDef = TypedDict(
+    "UpdateScheduleOutputTypeDef",
+    {
+        "ScheduleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+    {
+        "NamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
+    {
+        "GroupName": str,
+        "NamePrefix": str,
+        "State": ScheduleStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListScheduleGroupsOutputTypeDef = TypedDict(
     "ListScheduleGroupsOutputTypeDef",
     {
         "NextToken": str,
         "ScheduleGroups": List[ScheduleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SageMakerPipelineParametersOutputTypeDef = TypedDict(
+    "SageMakerPipelineParametersOutputTypeDef",
+    {
+        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
     },
+    total=False,
 )
 
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
         "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
     },
@@ -497,14 +648,45 @@
         "Name": str,
         "State": ScheduleStateType,
         "Target": TargetSummaryTypeDef,
     },
     total=False,
 )
 
+_RequiredEcsParametersOutputTypeDef = TypedDict(
+    "_RequiredEcsParametersOutputTypeDef",
+    {
+        "TaskDefinitionArn": str,
+    },
+)
+_OptionalEcsParametersOutputTypeDef = TypedDict(
+    "_OptionalEcsParametersOutputTypeDef",
+    {
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "EnableECSManagedTags": bool,
+        "EnableExecuteCommand": bool,
+        "Group": str,
+        "LaunchType": LaunchTypeType,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
+        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PlatformVersion": str,
+        "PropagateTags": Literal["TASK_DEFINITION"],
+        "ReferenceId": str,
+        "Tags": List[Dict[str, str]],
+        "TaskCount": int,
+    },
+    total=False,
+)
+
+class EcsParametersOutputTypeDef(
+    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
+):
+    pass
+
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
@@ -523,28 +705,51 @@
         "ReferenceId": str,
         "Tags": Sequence[Mapping[str, str]],
         "TaskCount": int,
     },
     total=False,
 )
 
-
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
 
-
 ListSchedulesOutputTypeDef = TypedDict(
     "ListSchedulesOutputTypeDef",
     {
         "NextToken": str,
         "Schedules": List[ScheduleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "Arn": str,
+        "RoleArn": str,
+    },
+)
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "EcsParameters": EcsParametersOutputTypeDef,
+        "EventBridgeParameters": EventBridgeParametersOutputTypeDef,
+        "Input": str,
+        "KinesisParameters": KinesisParametersOutputTypeDef,
+        "RetryPolicy": RetryPolicyOutputTypeDef,
+        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
+        "SqsParameters": SqsParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
+    pass
+
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Arn": str,
         "RoleArn": str,
     },
 )
@@ -559,18 +764,37 @@
         "RetryPolicy": RetryPolicyTypeDef,
         "SageMakerPipelineParameters": SageMakerPipelineParametersTypeDef,
         "SqsParameters": SqsParametersTypeDef,
     },
     total=False,
 )
 
-
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
+GetScheduleOutputTypeDef = TypedDict(
+    "GetScheduleOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationDate": datetime,
+        "Description": str,
+        "EndDate": datetime,
+        "FlexibleTimeWindow": FlexibleTimeWindowOutputTypeDef,
+        "GroupName": str,
+        "KmsKeyArn": str,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "ScheduleExpression": str,
+        "ScheduleExpressionTimezone": str,
+        "StartDate": datetime,
+        "State": ScheduleStateType,
+        "Target": TargetOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
@@ -588,42 +812,19 @@
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
         "State": ScheduleStateType,
     },
     total=False,
 )
 
-
 class CreateScheduleInputRequestTypeDef(
     _RequiredCreateScheduleInputRequestTypeDef, _OptionalCreateScheduleInputRequestTypeDef
 ):
     pass
 
-
-GetScheduleOutputTypeDef = TypedDict(
-    "GetScheduleOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationDate": datetime,
-        "Description": str,
-        "EndDate": datetime,
-        "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
-        "GroupName": str,
-        "KmsKeyArn": str,
-        "LastModificationDate": datetime,
-        "Name": str,
-        "ScheduleExpression": str,
-        "ScheduleExpressionTimezone": str,
-        "StartDate": datetime,
-        "State": ScheduleStateType,
-        "Target": TargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
@@ -640,12 +841,11 @@
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
         "State": ScheduleStateType,
     },
     total=False,
 )
 
-
 class UpdateScheduleInputRequestTypeDef(
     _RequiredUpdateScheduleInputRequestTypeDef, _OptionalUpdateScheduleInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler/type_defs.pyi` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for scheduler service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_scheduler.type_defs import AwsVpcConfigurationTypeDef
+    from mypy_boto3_scheduler.type_defs import AwsVpcConfigurationOutputTypeDef
 
-    data: AwsVpcConfigurationTypeDef = {...}
+    data: AwsVpcConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,60 +30,99 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
+    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
-    "CreateScheduleGroupOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "FlexibleTimeWindowTypeDef",
-    "CreateScheduleOutputTypeDef",
+    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeleteScheduleGroupInputRequestTypeDef",
     "DeleteScheduleInputRequestTypeDef",
+    "PlacementConstraintOutputTypeDef",
+    "PlacementStrategyOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
+    "EventBridgeParametersOutputTypeDef",
     "EventBridgeParametersTypeDef",
+    "FlexibleTimeWindowOutputTypeDef",
     "GetScheduleGroupInputRequestTypeDef",
-    "GetScheduleGroupOutputTypeDef",
     "GetScheduleInputRequestTypeDef",
+    "KinesisParametersOutputTypeDef",
     "KinesisParametersTypeDef",
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListScheduleGroupsInputRequestTypeDef",
     "ScheduleGroupSummaryTypeDef",
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListSchedulesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
+    "RetryPolicyOutputTypeDef",
     "RetryPolicyTypeDef",
+    "SageMakerPipelineParameterOutputTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "TargetSummaryTypeDef",
+    "SqsParametersOutputTypeDef",
     "SqsParametersTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateScheduleOutputTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateScheduleGroupInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateScheduleGroupOutputTypeDef",
+    "CreateScheduleOutputTypeDef",
+    "GetScheduleGroupOutputTypeDef",
+    "UpdateScheduleOutputTypeDef",
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListScheduleGroupsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "ScheduleSummaryTypeDef",
+    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
+    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "CreateScheduleInputRequestTypeDef",
     "GetScheduleOutputTypeDef",
+    "CreateScheduleInputRequestTypeDef",
     "UpdateScheduleInputRequestTypeDef",
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "Subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "AssignPublicIp": AssignPublicIpType,
+        "SecurityGroups": List[str],
+    },
+    total=False,
+)
+
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "Subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -91,19 +130,44 @@
     {
         "AssignPublicIp": AssignPublicIpType,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+
+_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "capacityProvider": str,
+    },
+)
+_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "base": int,
+        "weight": int,
+    },
+    total=False,
+)
+
+
+class CapacityProviderStrategyItemOutputTypeDef(
+    _RequiredCapacityProviderStrategyItemOutputTypeDef,
+    _OptionalCapacityProviderStrategyItemOutputTypeDef,
+):
+    pass
+
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -111,32 +175,37 @@
     {
         "base": int,
         "weight": int,
     },
     total=False,
 )
 
+
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateScheduleGroupOutputTypeDef = TypedDict(
-    "CreateScheduleGroupOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScheduleGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredFlexibleTimeWindowTypeDef = TypedDict(
     "_RequiredFlexibleTimeWindowTypeDef",
     {
         "Mode": FlexibleTimeWindowModeType,
@@ -146,25 +215,27 @@
     "_OptionalFlexibleTimeWindowTypeDef",
     {
         "MaximumWindowInMinutes": int,
     },
     total=False,
 )
 
+
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
-CreateScheduleOutputTypeDef = TypedDict(
-    "CreateScheduleOutputTypeDef",
+
+DeadLetterConfigOutputTypeDef = TypedDict(
+    "DeadLetterConfigOutputTypeDef",
     {
-        "ScheduleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Arn": str,
     },
+    total=False,
 )
 
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
@@ -181,19 +252,21 @@
     "_OptionalDeleteScheduleGroupInputRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteScheduleGroupInputRequestTypeDef(
     _RequiredDeleteScheduleGroupInputRequestTypeDef, _OptionalDeleteScheduleGroupInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteScheduleInputRequestTypeDef = TypedDict(
     "_RequiredDeleteScheduleInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteScheduleInputRequestTypeDef = TypedDict(
@@ -201,19 +274,39 @@
     {
         "ClientToken": str,
         "GroupName": str,
     },
     total=False,
 )
 
+
 class DeleteScheduleInputRequestTypeDef(
     _RequiredDeleteScheduleInputRequestTypeDef, _OptionalDeleteScheduleInputRequestTypeDef
 ):
     pass
 
+
+PlacementConstraintOutputTypeDef = TypedDict(
+    "PlacementConstraintOutputTypeDef",
+    {
+        "expression": str,
+        "type": PlacementConstraintTypeType,
+    },
+    total=False,
+)
+
+PlacementStrategyOutputTypeDef = TypedDict(
+    "PlacementStrategyOutputTypeDef",
+    {
+        "field": str,
+        "type": PlacementStrategyTypeType,
+    },
+    total=False,
+)
+
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "expression": str,
         "type": PlacementConstraintTypeType,
     },
     total=False,
@@ -224,38 +317,55 @@
     {
         "field": str,
         "type": PlacementStrategyTypeType,
     },
     total=False,
 )
 
+EventBridgeParametersOutputTypeDef = TypedDict(
+    "EventBridgeParametersOutputTypeDef",
+    {
+        "DetailType": str,
+        "Source": str,
+    },
+)
+
 EventBridgeParametersTypeDef = TypedDict(
     "EventBridgeParametersTypeDef",
     {
         "DetailType": str,
         "Source": str,
     },
 )
 
-GetScheduleGroupInputRequestTypeDef = TypedDict(
-    "GetScheduleGroupInputRequestTypeDef",
+_RequiredFlexibleTimeWindowOutputTypeDef = TypedDict(
+    "_RequiredFlexibleTimeWindowOutputTypeDef",
     {
-        "Name": str,
+        "Mode": FlexibleTimeWindowModeType,
     },
 )
+_OptionalFlexibleTimeWindowOutputTypeDef = TypedDict(
+    "_OptionalFlexibleTimeWindowOutputTypeDef",
+    {
+        "MaximumWindowInMinutes": int,
+    },
+    total=False,
+)
 
-GetScheduleGroupOutputTypeDef = TypedDict(
-    "GetScheduleGroupOutputTypeDef",
+
+class FlexibleTimeWindowOutputTypeDef(
+    _RequiredFlexibleTimeWindowOutputTypeDef, _OptionalFlexibleTimeWindowOutputTypeDef
+):
+    pass
+
+
+GetScheduleGroupInputRequestTypeDef = TypedDict(
+    "GetScheduleGroupInputRequestTypeDef",
     {
-        "Arn": str,
-        "CreationDate": datetime,
-        "LastModificationDate": datetime,
         "Name": str,
-        "State": ScheduleGroupStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetScheduleInputRequestTypeDef = TypedDict(
     "_RequiredGetScheduleInputRequestTypeDef",
     {
         "Name": str,
@@ -265,31 +375,41 @@
     "_OptionalGetScheduleInputRequestTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
+
 class GetScheduleInputRequestTypeDef(
     _RequiredGetScheduleInputRequestTypeDef, _OptionalGetScheduleInputRequestTypeDef
 ):
     pass
 
+
+KinesisParametersOutputTypeDef = TypedDict(
+    "KinesisParametersOutputTypeDef",
+    {
+        "PartitionKey": str,
+    },
+)
+
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
-ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
-    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "NamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListScheduleGroupsInputRequestTypeDef = TypedDict(
     "ListScheduleGroupsInputRequestTypeDef",
     {
@@ -308,25 +428,14 @@
         "LastModificationDate": datetime,
         "Name": str,
         "State": ScheduleGroupStateType,
     },
     total=False,
 )
 
-ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesInputListSchedulesPaginateTypeDef",
-    {
-        "GroupName": str,
-        "NamePrefix": str,
-        "State": ScheduleStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSchedulesInputRequestTypeDef = TypedDict(
     "ListSchedulesInputRequestTypeDef",
     {
         "GroupName": str,
         "MaxResults": int,
         "NamePrefix": str,
         "NextToken": str,
@@ -338,44 +447,48 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RetryPolicyOutputTypeDef = TypedDict(
+    "RetryPolicyOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MaximumEventAgeInSeconds": int,
+        "MaximumRetryAttempts": int,
     },
+    total=False,
 )
 
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumEventAgeInSeconds": int,
         "MaximumRetryAttempts": int,
     },
     total=False,
 )
 
+SageMakerPipelineParameterOutputTypeDef = TypedDict(
+    "SageMakerPipelineParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -383,14 +496,22 @@
 TargetSummaryTypeDef = TypedDict(
     "TargetSummaryTypeDef",
     {
         "Arn": str,
     },
 )
 
+SqsParametersOutputTypeDef = TypedDict(
+    "SqsParametersOutputTypeDef",
+    {
+        "MessageGroupId": str,
+    },
+    total=False,
+)
+
 SqsParametersTypeDef = TypedDict(
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
@@ -399,20 +520,20 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateScheduleOutputTypeDef = TypedDict(
-    "UpdateScheduleOutputTypeDef",
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
     {
-        "ScheduleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
@@ -430,42 +551,108 @@
     {
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateScheduleGroupInputRequestTypeDef(
     _RequiredCreateScheduleGroupInputRequestTypeDef, _OptionalCreateScheduleGroupInputRequestTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateScheduleGroupOutputTypeDef = TypedDict(
+    "CreateScheduleGroupOutputTypeDef",
+    {
+        "ScheduleGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduleOutputTypeDef = TypedDict(
+    "CreateScheduleOutputTypeDef",
+    {
+        "ScheduleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetScheduleGroupOutputTypeDef = TypedDict(
+    "GetScheduleGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationDate": datetime,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "State": ScheduleGroupStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduleOutputTypeDef = TypedDict(
+    "UpdateScheduleOutputTypeDef",
+    {
+        "ScheduleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef = TypedDict(
+    "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
+    {
+        "NamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSchedulesInputListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesInputListSchedulesPaginateTypeDef",
+    {
+        "GroupName": str,
+        "NamePrefix": str,
+        "State": ScheduleStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListScheduleGroupsOutputTypeDef = TypedDict(
     "ListScheduleGroupsOutputTypeDef",
     {
         "NextToken": str,
         "ScheduleGroups": List[ScheduleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SageMakerPipelineParametersOutputTypeDef = TypedDict(
+    "SageMakerPipelineParametersOutputTypeDef",
+    {
+        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
     },
+    total=False,
 )
 
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
         "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
     },
@@ -482,14 +669,47 @@
         "Name": str,
         "State": ScheduleStateType,
         "Target": TargetSummaryTypeDef,
     },
     total=False,
 )
 
+_RequiredEcsParametersOutputTypeDef = TypedDict(
+    "_RequiredEcsParametersOutputTypeDef",
+    {
+        "TaskDefinitionArn": str,
+    },
+)
+_OptionalEcsParametersOutputTypeDef = TypedDict(
+    "_OptionalEcsParametersOutputTypeDef",
+    {
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "EnableECSManagedTags": bool,
+        "EnableExecuteCommand": bool,
+        "Group": str,
+        "LaunchType": LaunchTypeType,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
+        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PlatformVersion": str,
+        "PropagateTags": Literal["TASK_DEFINITION"],
+        "ReferenceId": str,
+        "Tags": List[Dict[str, str]],
+        "TaskCount": int,
+    },
+    total=False,
+)
+
+
+class EcsParametersOutputTypeDef(
+    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
+):
+    pass
+
+
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
@@ -508,25 +728,54 @@
         "ReferenceId": str,
         "Tags": Sequence[Mapping[str, str]],
         "TaskCount": int,
     },
     total=False,
 )
 
+
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
 
+
 ListSchedulesOutputTypeDef = TypedDict(
     "ListSchedulesOutputTypeDef",
     {
         "NextToken": str,
         "Schedules": List[ScheduleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "Arn": str,
+        "RoleArn": str,
     },
 )
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "EcsParameters": EcsParametersOutputTypeDef,
+        "EventBridgeParameters": EventBridgeParametersOutputTypeDef,
+        "Input": str,
+        "KinesisParameters": KinesisParametersOutputTypeDef,
+        "RetryPolicy": RetryPolicyOutputTypeDef,
+        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
+        "SqsParameters": SqsParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
+    pass
+
 
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Arn": str,
         "RoleArn": str,
     },
@@ -542,17 +791,40 @@
         "RetryPolicy": RetryPolicyTypeDef,
         "SageMakerPipelineParameters": SageMakerPipelineParametersTypeDef,
         "SqsParameters": SqsParametersTypeDef,
     },
     total=False,
 )
 
+
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
+
+GetScheduleOutputTypeDef = TypedDict(
+    "GetScheduleOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationDate": datetime,
+        "Description": str,
+        "EndDate": datetime,
+        "FlexibleTimeWindow": FlexibleTimeWindowOutputTypeDef,
+        "GroupName": str,
+        "KmsKeyArn": str,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "ScheduleExpression": str,
+        "ScheduleExpressionTimezone": str,
+        "StartDate": datetime,
+        "State": ScheduleStateType,
+        "Target": TargetOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
@@ -569,39 +841,20 @@
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
         "State": ScheduleStateType,
     },
     total=False,
 )
 
+
 class CreateScheduleInputRequestTypeDef(
     _RequiredCreateScheduleInputRequestTypeDef, _OptionalCreateScheduleInputRequestTypeDef
 ):
     pass
 
-GetScheduleOutputTypeDef = TypedDict(
-    "GetScheduleOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationDate": datetime,
-        "Description": str,
-        "EndDate": datetime,
-        "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
-        "GroupName": str,
-        "KmsKeyArn": str,
-        "LastModificationDate": datetime,
-        "Name": str,
-        "ScheduleExpression": str,
-        "ScheduleExpressionTimezone": str,
-        "StartDate": datetime,
-        "State": ScheduleStateType,
-        "Target": TargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
@@ -619,11 +872,12 @@
         "ScheduleExpressionTimezone": str,
         "StartDate": Union[datetime, str],
         "State": ScheduleStateType,
     },
     total=False,
 )
 
+
 class UpdateScheduleInputRequestTypeDef(
     _RequiredUpdateScheduleInputRequestTypeDef, _OptionalUpdateScheduleInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/PKG-INFO` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.0
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-scheduler"></a>
 
 # mypy-boto3-scheduler
 
 [![PyPI - mypy-boto3-scheduler](https://img.shields.io/pypi/v/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-scheduler.svg?color=blue)](https://pypi.org/project/mypy-boto3-scheduler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-scheduler?color=blue)](https://pypistats.org/packages/mypy-boto3-scheduler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-scheduler)](https://pepy.tech/project/mypy-boto3-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgeScheduler 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[boto3.EventBridgeScheduler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,61 +331,77 @@
 ### Typed dictionaries
 
 `mypy_boto3_scheduler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
-    CreateScheduleGroupOutputTypeDef,
+    ResponseMetadataTypeDef,
     FlexibleTimeWindowTypeDef,
-    CreateScheduleOutputTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
+    EventBridgeParametersOutputTypeDef,
     EventBridgeParametersTypeDef,
+    FlexibleTimeWindowOutputTypeDef,
     GetScheduleGroupInputRequestTypeDef,
-    GetScheduleGroupOutputTypeDef,
     GetScheduleInputRequestTypeDef,
+    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduleGroupsInputRequestTypeDef,
     ScheduleGroupSummaryTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListSchedulesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
+    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
     TargetSummaryTypeDef,
+    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateScheduleOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     CreateScheduleGroupInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateScheduleGroupOutputTypeDef,
+    CreateScheduleOutputTypeDef,
+    GetScheduleGroupOutputTypeDef,
+    UpdateScheduleOutputTypeDef,
+    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
+    ListSchedulesInputListSchedulesPaginateTypeDef,
     ListScheduleGroupsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     ScheduleSummaryTypeDef,
+    EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
-    CreateScheduleInputRequestTypeDef,
     GetScheduleOutputTypeDef,
+    CreateScheduleInputRequestTypeDef,
     UpdateScheduleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationTypeDef:
+def get_structure() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-scheduler-1.28.0/mypy_boto3_scheduler.egg-info/SOURCES.txt` & `mypy-boto3-scheduler-1.28.12/mypy_boto3_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.0/setup.py` & `mypy-boto3-scheduler-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-scheduler",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridgeScheduler 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EventBridgeScheduler 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

