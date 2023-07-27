# Comparing `tmp/mypy-boto3-codeguruprofiler-1.28.0.tar.gz` & `tmp/mypy-boto3-codeguruprofiler-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguruprofiler-1.28.0.tar", last modified: Thu Jul  6 20:59:15 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguruprofiler-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
```

## Comparing `mypy-boto3-codeguruprofiler-1.28.0.tar` & `mypy-boto3-codeguruprofiler-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.646258 mypy-boto3-codeguruprofiler-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-06 20:59:15.646258 mypy-boto3-codeguruprofiler-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.646258 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19828 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-07-06 20:36:08.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.646258 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-06 20:59:15.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 20:59:15.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:15.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:15.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:15.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:59:15.000000 mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:15.646258 mypy-boto3-codeguruprofiler-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:36:07.000000 mypy-boto3-codeguruprofiler-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.012550 mypy-boto3-codeguruprofiler-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-27 05:34:29.008550 mypy-boto3-codeguruprofiler-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.004550 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19828 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23179 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.008550 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.012550 mypy-boto3-codeguruprofiler-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/setup.py
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/LICENSE` & `mypy-boto3-codeguruprofiler-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeGuruProfiler 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeGuruProfiler 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguruprofiler"></a>
 
 # mypy-boto3-codeguruprofiler
 
 [![PyPI - mypy-boto3-codeguruprofiler](https://img.shields.io/pypi/v/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguruprofiler?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguruprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,24 +330,27 @@
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
     AgentConfigurationTypeDef,
+    AgentOrchestrationConfigOutputTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
+    ChannelOutputTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
@@ -368,31 +371,31 @@
     RemovePermissionRequestRequestTypeDef,
     RemovePermissionResponseTypeDef,
     ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
-    FrameMetricDatumTypeDef,
+    NotificationConfigurationTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/README.md` & `mypy-boto3-codeguruprofiler-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeguruprofiler"></a>
 
 # mypy-boto3-codeguruprofiler
 
 [![PyPI - mypy-boto3-codeguruprofiler](https://img.shields.io/pypi/v/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguruprofiler?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguruprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,24 +298,27 @@
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
     AgentConfigurationTypeDef,
+    AgentOrchestrationConfigOutputTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
+    ChannelOutputTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
@@ -336,31 +339,31 @@
     RemovePermissionRequestRequestTypeDef,
     RemovePermissionResponseTypeDef,
     ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
-    FrameMetricDatumTypeDef,
+    NotificationConfigurationTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/__init__.py` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/__init__.pyi` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/__main__.py` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruProfiler 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeGuruProfiler 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler\nOther"
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

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/client.py` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/client.pyi` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/literals.py` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.pyi`

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
     "ActionGroupType",
     "AgentParameterFieldType",
     "AggregationPeriodType",
     "ComputePlatformType",
     "EventPublisherType",
     "FeedbackTypeType",
@@ -32,15 +31,14 @@
     "OrderByType",
     "CodeGuruProfilerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ActionGroupType = Literal["agentPermissions"]
 AgentParameterFieldType = Literal[
     "MaxStackDepth",
     "MemoryUsageLimitPercent",
     "MinimumTimeForReportingInMilliseconds",
     "ReportingIntervalInMilliseconds",
     "SamplingIntervalInMilliseconds",
@@ -179,14 +177,15 @@
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
@@ -265,26 +264,28 @@
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

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/literals.pyi` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionGroupType",
     "AgentParameterFieldType",
     "AggregationPeriodType",
     "ComputePlatformType",
     "EventPublisherType",
     "FeedbackTypeType",
@@ -31,14 +32,15 @@
     "OrderByType",
     "CodeGuruProfilerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ActionGroupType = Literal["agentPermissions"]
 AgentParameterFieldType = Literal[
     "MaxStackDepth",
     "MemoryUsageLimitPercent",
     "MinimumTimeForReportingInMilliseconds",
     "ReportingIntervalInMilliseconds",
     "SamplingIntervalInMilliseconds",
@@ -177,14 +179,15 @@
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
@@ -263,26 +266,28 @@
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

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/paginator.py` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/paginator.pyi` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/type_defs.py` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,24 +35,27 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChannelTypeDef",
     "AgentConfigurationTypeDef",
+    "AgentOrchestrationConfigOutputTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
     "FrameMetricTypeDef",
     "TimestampStructureTypeDef",
+    "ChannelOutputTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
+    "FrameMetricOutputTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyResponseTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetProfileResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
@@ -73,31 +76,31 @@
     "RemovePermissionRequestRequestTypeDef",
     "RemovePermissionResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddNotificationChannelsRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
     "BatchGetFrameMetricDataRequestRequestTypeDef",
-    "FrameMetricDatumTypeDef",
+    "NotificationConfigurationTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
+    "FrameMetricDatumTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
@@ -140,14 +143,21 @@
 
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
 
+AgentOrchestrationConfigOutputTypeDef = TypedDict(
+    "AgentOrchestrationConfigOutputTypeDef",
+    {
+        "profilingEnabled": bool,
+    },
+)
+
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -188,14 +198,34 @@
 TimestampStructureTypeDef = TypedDict(
     "TimestampStructureTypeDef",
     {
         "value": datetime,
     },
 )
 
+_RequiredChannelOutputTypeDef = TypedDict(
+    "_RequiredChannelOutputTypeDef",
+    {
+        "eventPublishers": List[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelOutputTypeDef = TypedDict(
+    "_OptionalChannelOutputTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+
+class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
+    pass
+
+
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalConfigureAgentRequestRequestTypeDef = TypedDict(
@@ -236,14 +266,23 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
+FrameMetricOutputTypeDef = TypedDict(
+    "FrameMetricOutputTypeDef",
+    {
+        "frameName": str,
+        "threadStates": List[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
 GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
@@ -612,22 +651,14 @@
     "AddNotificationChannelsRequestRequestTypeDef",
     {
         "channels": Sequence[ChannelTypeDef],
         "profilingGroupName": str,
     },
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
-    {
-        "channels": List[ChannelTypeDef],
-    },
-    total=False,
-)
-
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -718,20 +749,20 @@
 class BatchGetFrameMetricDataRequestRequestTypeDef(
     _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
     _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
 ):
     pass
 
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
     {
-        "frameMetric": FrameMetricTypeDef,
-        "values": List[float],
+        "channels": List[ChannelOutputTypeDef],
     },
+    total=False,
 )
 
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
@@ -744,14 +775,22 @@
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricOutputTypeDef,
+        "values": List[float],
+    },
+)
+
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -765,14 +804,38 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
+    {
+        "agentOrchestrationConfig": AgentOrchestrationConfigOutputTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
+    },
+)
+
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -789,38 +852,14 @@
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
-    {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
-    },
-)
-
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler/type_defs.pyi` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChannelTypeDef",
     "AgentConfigurationTypeDef",
+    "AgentOrchestrationConfigOutputTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
     "FrameMetricTypeDef",
     "TimestampStructureTypeDef",
+    "ChannelOutputTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
+    "FrameMetricOutputTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyResponseTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetProfileResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
@@ -72,31 +75,31 @@
     "RemovePermissionRequestRequestTypeDef",
     "RemovePermissionResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddNotificationChannelsRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
     "BatchGetFrameMetricDataRequestRequestTypeDef",
-    "FrameMetricDatumTypeDef",
+    "NotificationConfigurationTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
+    "FrameMetricDatumTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
@@ -135,14 +138,21 @@
 )
 
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
+AgentOrchestrationConfigOutputTypeDef = TypedDict(
+    "AgentOrchestrationConfigOutputTypeDef",
+    {
+        "profilingEnabled": bool,
+    },
+)
+
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -183,14 +193,32 @@
 TimestampStructureTypeDef = TypedDict(
     "TimestampStructureTypeDef",
     {
         "value": datetime,
     },
 )
 
+_RequiredChannelOutputTypeDef = TypedDict(
+    "_RequiredChannelOutputTypeDef",
+    {
+        "eventPublishers": List[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelOutputTypeDef = TypedDict(
+    "_OptionalChannelOutputTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
+    pass
+
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalConfigureAgentRequestRequestTypeDef = TypedDict(
@@ -229,14 +257,23 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
+FrameMetricOutputTypeDef = TypedDict(
+    "FrameMetricOutputTypeDef",
+    {
+        "frameName": str,
+        "threadStates": List[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
 GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
@@ -589,22 +626,14 @@
     "AddNotificationChannelsRequestRequestTypeDef",
     {
         "channels": Sequence[ChannelTypeDef],
         "profilingGroupName": str,
     },
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
-    {
-        "channels": List[ChannelTypeDef],
-    },
-    total=False,
-)
-
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -689,20 +718,20 @@
 
 class BatchGetFrameMetricDataRequestRequestTypeDef(
     _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
     _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
 ):
     pass
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
     {
-        "frameMetric": FrameMetricTypeDef,
-        "values": List[float],
+        "channels": List[ChannelOutputTypeDef],
     },
+    total=False,
 )
 
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
@@ -715,14 +744,22 @@
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricOutputTypeDef,
+        "values": List[float],
+    },
+)
+
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -736,14 +773,38 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
+    {
+        "agentOrchestrationConfig": AgentOrchestrationConfigOutputTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
+    },
+)
+
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -760,38 +821,14 @@
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
-    {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
-    },
-)
-
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeGuruProfiler 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeGuruProfiler 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguruprofiler"></a>
 
 # mypy-boto3-codeguruprofiler
 
 [![PyPI - mypy-boto3-codeguruprofiler](https://img.shields.io/pypi/v/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguruprofiler?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguruprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,24 +330,27 @@
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
     AgentConfigurationTypeDef,
+    AgentOrchestrationConfigOutputTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
+    ChannelOutputTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
@@ -368,31 +371,31 @@
     RemovePermissionRequestRequestTypeDef,
     RemovePermissionResponseTypeDef,
     ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
-    FrameMetricDatumTypeDef,
+    NotificationConfigurationTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt` & `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.0/setup.py` & `mypy-boto3-codeguruprofiler-1.28.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguruprofiler",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_codeguruprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruProfiler 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CodeGuruProfiler 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

