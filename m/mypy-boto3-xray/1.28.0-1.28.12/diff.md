# Comparing `tmp/mypy-boto3-xray-1.28.0.tar.gz` & `tmp/mypy-boto3-xray-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-xray-1.28.0.tar", last modified: Thu Jul  6 21:00:53 2023, max compression
+gzip compressed data, was "mypy-boto3-xray-1.28.12.tar", last modified: Thu Jul 27 11:49:51 2023, max compression
```

## Comparing `mypy-boto3-xray-1.28.0.tar` & `mypy-boto3-xray-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:53.338463 mypy-boto3-xray-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-07-06 21:00:53.338463 mypy-boto3-xray-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:53.334463 mypy-boto3-xray-1.28.0/mypy_boto3_xray/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43345 2023-07-06 20:58:30.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43296 2023-07-06 20:58:29.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:28.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:53.338463 mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-07-06 21:00:53.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 21:00:53.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:53.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:53.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:53.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:00:53.000000 mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:53.338463 mypy-boto3-xray-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-06 20:58:27.000000 mypy-boto3-xray-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/mypy_boto3_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-07-27 11:49:06.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44354 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/setup.py
```

### Comparing `mypy-boto3-xray-1.28.0/LICENSE` & `mypy-boto3-xray-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.0/PKG-INFO` & `mypy-boto3-xray-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.0
-Summary: Type annotations for boto3.XRay 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.XRay 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-xray"></a>
 
 # mypy-boto3-xray
 
 [![PyPI - mypy-boto3-xray](https://img.shields.io/pypi/v/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-xray?color=blue)](https://pypistats.org/packages/mypy-boto3-xray)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,118 +368,121 @@
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetTracesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
     GetInsightImpactGraphRequestRequestTypeDef,
     GetInsightRequestRequestTypeDef,
     GetInsightSummariesRequestRequestTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
+    InsightsConfigurationOutputTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
-    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
-    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
     TelemetryRecordTypeDef,
-    GroupSummaryTypeDef,
-    GroupTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
-    SamplingRuleRecordTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
+    GroupSummaryTypeDef,
+    GroupTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
+    SamplingRuleRecordTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
     PutTelemetryRecordsRequestRequestTypeDef,
+    EdgeTypeDef,
+    TimeSeriesServiceStatisticsTypeDef,
+    ErrorRootCauseServiceTypeDef,
+    FaultRootCauseServiceTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
+    GetInsightImpactGraphResultTypeDef,
+    ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
-    EdgeTypeDef,
-    TimeSeriesServiceStatisticsTypeDef,
-    ErrorRootCauseServiceTypeDef,
-    FaultRootCauseServiceTypeDef,
-    GetInsightImpactGraphResultTypeDef,
-    ResponseTimeRootCauseTypeDef,
     BatchGetTracesResultTypeDef,
     GetInsightEventsResultTypeDef,
     GetInsightSummariesResultTypeDef,
     GetInsightResultTypeDef,
     ServiceTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     ErrorRootCauseTypeDef,
```

### Comparing `mypy-boto3-xray-1.28.0/README.md` & `mypy-boto3-xray-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-xray"></a>
 
 # mypy-boto3-xray
 
 [![PyPI - mypy-boto3-xray](https://img.shields.io/pypi/v/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-xray?color=blue)](https://pypistats.org/packages/mypy-boto3-xray)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,118 +336,121 @@
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetTracesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
     GetInsightImpactGraphRequestRequestTypeDef,
     GetInsightRequestRequestTypeDef,
     GetInsightSummariesRequestRequestTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
+    InsightsConfigurationOutputTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
-    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
-    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
     TelemetryRecordTypeDef,
-    GroupSummaryTypeDef,
-    GroupTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
-    SamplingRuleRecordTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
+    GroupSummaryTypeDef,
+    GroupTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
+    SamplingRuleRecordTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
     PutTelemetryRecordsRequestRequestTypeDef,
+    EdgeTypeDef,
+    TimeSeriesServiceStatisticsTypeDef,
+    ErrorRootCauseServiceTypeDef,
+    FaultRootCauseServiceTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
+    GetInsightImpactGraphResultTypeDef,
+    ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
-    EdgeTypeDef,
-    TimeSeriesServiceStatisticsTypeDef,
-    ErrorRootCauseServiceTypeDef,
-    FaultRootCauseServiceTypeDef,
-    GetInsightImpactGraphResultTypeDef,
-    ResponseTimeRootCauseTypeDef,
     BatchGetTracesResultTypeDef,
     GetInsightEventsResultTypeDef,
     GetInsightSummariesResultTypeDef,
     GetInsightResultTypeDef,
     ServiceTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     ErrorRootCauseTypeDef,
```

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/__init__.py` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/__init__.pyi` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/client.py` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/client.pyi` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/literals.py` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
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
@@ -262,26 +263,28 @@
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

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/literals.pyi` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
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
@@ -260,26 +261,28 @@
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

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/paginator.py` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,60 +85,60 @@
 class BatchGetTracesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[BatchGetTracesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
         """
 
 
 class GetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
         """
 
 
 class GetSamplingRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSamplingRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
         """
 
 
 class GetSamplingStatisticSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSamplingStatisticSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
         """
 
 
@@ -151,15 +151,15 @@
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
         """
 
 
@@ -175,30 +175,30 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 
 class GetTraceGraphPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTraceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
         """
 
 
@@ -213,43 +213,43 @@
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracesummariespaginator)
         """
 
 
 class ListResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcePoliciesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/paginator.pyi` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,57 +82,57 @@
 class BatchGetTracesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[BatchGetTracesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#batchgettracespaginator)
         """
 
 class GetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getgroupspaginator)
         """
 
 class GetSamplingRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSamplingRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingrulespaginator)
         """
 
 class GetSamplingStatisticSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSamplingStatisticSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getsamplingstatisticsummariespaginator)
         """
 
 class GetServiceGraphPaginator(Paginator):
@@ -144,15 +144,15 @@
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#getservicegraphpaginator)
         """
 
 class GetTimeSeriesServiceStatisticsPaginator(Paginator):
@@ -167,29 +167,29 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 class GetTraceGraphPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTraceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracegraphpaginator)
         """
 
 class GetTraceSummariesPaginator(Paginator):
@@ -203,41 +203,41 @@
         *,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#gettracesummariespaginator)
         """
 
 class ListResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcePoliciesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listresourcepoliciespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/type_defs.py` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,118 +35,121 @@
 
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
-    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "BatchGetTracesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "InsightsConfigurationTypeDef",
     "TagTypeDef",
     "SamplingRuleTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSamplingRuleRequestRequestTypeDef",
     "ErrorStatisticsTypeDef",
     "FaultStatisticsTypeDef",
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
     "GetInsightImpactGraphRequestRequestTypeDef",
     "GetInsightRequestRequestTypeDef",
     "GetInsightSummariesRequestRequestTypeDef",
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
     "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     "GetServiceGraphRequestRequestTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
+    "InsightsConfigurationOutputTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
+    "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
     "TelemetryRecordTypeDef",
-    "GroupSummaryTypeDef",
-    "GroupTypeDef",
+    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
-    "SamplingRuleRecordTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
+    "GroupSummaryTypeDef",
+    "GroupTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
+    "SamplingRuleRecordTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
     "PutTelemetryRecordsRequestRequestTypeDef",
+    "EdgeTypeDef",
+    "TimeSeriesServiceStatisticsTypeDef",
+    "ErrorRootCauseServiceTypeDef",
+    "FaultRootCauseServiceTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
+    "GetInsightImpactGraphResultTypeDef",
+    "ResponseTimeRootCauseTypeDef",
     "CreateSamplingRuleResultTypeDef",
     "DeleteSamplingRuleResultTypeDef",
     "GetSamplingRulesResultTypeDef",
     "UpdateSamplingRuleResultTypeDef",
-    "EdgeTypeDef",
-    "TimeSeriesServiceStatisticsTypeDef",
-    "ErrorRootCauseServiceTypeDef",
-    "FaultRootCauseServiceTypeDef",
-    "GetInsightImpactGraphResultTypeDef",
-    "ResponseTimeRootCauseTypeDef",
     "BatchGetTracesResultTypeDef",
     "GetInsightEventsResultTypeDef",
     "GetInsightSummariesResultTypeDef",
     "GetInsightResultTypeDef",
     "ServiceTypeDef",
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     "ErrorRootCauseTypeDef",
@@ -205,36 +208,24 @@
         "HTTPCode5XXCount": int,
         "UnknownHostCount": int,
         "OtherCount": int,
     },
     total=False,
 )
 
-_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
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
 
-
-class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
-    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestRequestTypeDef = TypedDict(
@@ -248,14 +239,25 @@
 
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
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
 InsightsConfigurationTypeDef = TypedDict(
     "InsightsConfigurationTypeDef",
     {
         "InsightsEnabled": bool,
         "NotificationsEnabled": bool,
     },
     total=False,
@@ -400,22 +402,14 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
-GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetGroupsRequestRequestTypeDef = TypedDict(
     "GetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -496,38 +490,22 @@
 class GetInsightSummariesRequestRequestTypeDef(
     _RequiredGetInsightSummariesRequestRequestTypeDef,
     _OptionalGetInsightSummariesRequestRequestTypeDef,
 ):
     pass
 
 
-GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingStatisticSummariesRequestRequestTypeDef = TypedDict(
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -587,39 +565,14 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -636,42 +589,14 @@
 
 class GetServiceGraphRequestRequestTypeDef(
     _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -692,36 +617,14 @@
 class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
-    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
@@ -744,14 +647,23 @@
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
 )
 
+InsightsConfigurationOutputTypeDef = TypedDict(
+    "InsightsConfigurationOutputTypeDef",
+    {
+        "InsightsEnabled": bool,
+        "NotificationsEnabled": bool,
+    },
+    total=False,
+)
+
 HttpTypeDef = TypedDict(
     "HttpTypeDef",
     {
         "HttpURL": str,
         "HttpStatus": int,
         "HttpMethod": str,
         "UserAgent": str,
@@ -782,22 +694,14 @@
     "InstanceIdDetailTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourcePoliciesRequestRequestTypeDef = TypedDict(
     "ListResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -809,36 +713,14 @@
         "PolicyDocument": str,
         "PolicyRevisionId": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -853,22 +735,20 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
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
 
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
@@ -933,35 +813,56 @@
     "ResourceARNDetailTypeDef",
     {
         "ARN": str,
     },
     total=False,
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
 ResponseTimeRootCauseEntityTypeDef = TypedDict(
     "ResponseTimeRootCauseEntityTypeDef",
     {
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
     total=False,
 )
 
+_RequiredSamplingRuleOutputTypeDef = TypedDict(
+    "_RequiredSamplingRuleOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Priority": int,
+        "FixedRate": float,
+        "ReservoirSize": int,
+        "ServiceName": str,
+        "ServiceType": str,
+        "Host": str,
+        "HTTPMethod": str,
+        "URLPath": str,
+        "Version": int,
+    },
+)
+_OptionalSamplingRuleOutputTypeDef = TypedDict(
+    "_OptionalSamplingRuleOutputTypeDef",
+    {
+        "RuleName": str,
+        "RuleARN": str,
+        "Attributes": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class SamplingRuleOutputTypeDef(
+    _RequiredSamplingRuleOutputTypeDef, _OptionalSamplingRuleOutputTypeDef
+):
+    pass
+
+
 SamplingRuleUpdateTypeDef = TypedDict(
     "SamplingRuleUpdateTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
         "ResourceARN": str,
         "Priority": int,
@@ -1039,36 +940,165 @@
 )
 
 
 class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
     pass
 
 
-GroupSummaryTypeDef = TypedDict(
-    "GroupSummaryTypeDef",
+_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
+    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+):
+    pass
+
+
+GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GroupTypeDef = TypedDict(
-    "GroupTypeDef",
+
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationTypeDef,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
+    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+):
+    pass
+
+
+ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
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
 UpdateGroupRequestRequestTypeDef = TypedDict(
     "UpdateGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -1095,23 +1125,14 @@
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
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
@@ -1134,24 +1155,14 @@
 class CreateSamplingRuleRequestRequestTypeDef(
     _RequiredCreateSamplingRuleRequestRequestTypeDef,
     _OptionalCreateSamplingRuleRequestRequestTypeDef,
 ):
     pass
 
 
-SamplingRuleRecordTypeDef = TypedDict(
-    "SamplingRuleRecordTypeDef",
-    {
-        "SamplingRule": SamplingRuleTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-    },
-    total=False,
-)
-
 EdgeStatisticsTypeDef = TypedDict(
     "EdgeStatisticsTypeDef",
     {
         "OkCount": int,
         "ErrorStatistics": ErrorStatisticsTypeDef,
         "FaultStatistics": FaultStatisticsTypeDef,
         "TotalCount": int,
@@ -1172,23 +1183,23 @@
     total=False,
 )
 
 GetEncryptionConfigResultTypeDef = TypedDict(
     "GetEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEncryptionConfigResultTypeDef = TypedDict(
     "PutEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseEntityTypeDef = TypedDict(
     "ErrorRootCauseEntityTypeDef",
     {
         "Name": str,
@@ -1209,15 +1220,15 @@
 )
 
 GetSamplingStatisticSummariesResultTypeDef = TypedDict(
     "GetSamplingStatisticSummariesResultTypeDef",
     {
         "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSamplingTargetsRequestRequestTypeDef = TypedDict(
     "GetSamplingTargetsRequestRequestTypeDef",
     {
         "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
@@ -1226,15 +1237,15 @@
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
         "LastRuleModification": datetime,
         "UnprocessedStatistics": List[UnprocessedStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "StartTime": Union[datetime, str],
@@ -1244,15 +1255,15 @@
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
@@ -1283,14 +1294,36 @@
 
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
 
+GroupSummaryTypeDef = TypedDict(
+    "GroupSummaryTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+GroupTypeDef = TypedDict(
+    "GroupTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1301,31 +1334,40 @@
 )
 
 ListResourcePoliciesResultTypeDef = TypedDict(
     "ListResourcePoliciesResultTypeDef",
     {
         "ResourcePolicies": List[ResourcePolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResultTypeDef = TypedDict(
     "PutResourcePolicyResultTypeDef",
     {
         "ResourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseServiceTypeDef = TypedDict(
     "ResponseTimeRootCauseServiceTypeDef",
     {
         "Name": str,
@@ -1334,14 +1376,24 @@
         "AccountId": str,
         "EntityPath": List[ResponseTimeRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+SamplingRuleRecordTypeDef = TypedDict(
+    "SamplingRuleRecordTypeDef",
+    {
+        "SamplingRule": SamplingRuleOutputTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+    },
+    total=False,
+)
+
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1427,80 +1479,14 @@
 class PutTelemetryRecordsRequestRequestTypeDef(
     _RequiredPutTelemetryRecordsRequestRequestTypeDef,
     _OptionalPutTelemetryRecordsRequestRequestTypeDef,
 ):
     pass
 
 
-GetGroupsResultTypeDef = TypedDict(
-    "GetGroupsResultTypeDef",
-    {
-        "Groups": List[GroupSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateGroupResultTypeDef = TypedDict(
-    "CreateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetGroupResultTypeDef = TypedDict(
-    "GetGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateGroupResultTypeDef = TypedDict(
-    "UpdateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSamplingRuleResultTypeDef = TypedDict(
-    "CreateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSamplingRuleResultTypeDef = TypedDict(
-    "DeleteSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSamplingRulesResultTypeDef = TypedDict(
-    "GetSamplingRulesResultTypeDef",
-    {
-        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSamplingRuleResultTypeDef = TypedDict(
-    "UpdateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
         "StartTime": datetime,
         "EndTime": datetime,
         "SummaryStatistics": EdgeStatisticsTypeDef,
@@ -1546,70 +1532,136 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+GetGroupsResultTypeDef = TypedDict(
+    "GetGroupsResultTypeDef",
+    {
+        "Groups": List[GroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResultTypeDef = TypedDict(
+    "CreateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResultTypeDef = TypedDict(
+    "GetGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGroupResultTypeDef = TypedDict(
+    "UpdateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
         "ServiceGraphEndTime": datetime,
         "Services": List[InsightImpactGraphServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseTypeDef = TypedDict(
     "ResponseTimeRootCauseTypeDef",
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
         "ClientImpacting": bool,
     },
     total=False,
 )
 
+CreateSamplingRuleResultTypeDef = TypedDict(
+    "CreateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSamplingRuleResultTypeDef = TypedDict(
+    "DeleteSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSamplingRulesResultTypeDef = TypedDict(
+    "GetSamplingRulesResultTypeDef",
+    {
+        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSamplingRuleResultTypeDef = TypedDict(
+    "UpdateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightEventsResultTypeDef = TypedDict(
     "GetInsightEventsResultTypeDef",
     {
         "InsightEvents": List[InsightEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightSummariesResultTypeDef = TypedDict(
     "GetInsightSummariesResultTypeDef",
     {
         "InsightSummaries": List[InsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightResultTypeDef = TypedDict(
     "GetInsightResultTypeDef",
     {
         "Insight": InsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "ReferenceId": int,
@@ -1631,15 +1683,15 @@
 
 GetTimeSeriesServiceStatisticsResultTypeDef = TypedDict(
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     {
         "TimeSeriesServiceStatistics": List[TimeSeriesServiceStatisticsTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseTypeDef = TypedDict(
     "ErrorRootCauseTypeDef",
     {
         "Services": List[ErrorRootCauseServiceTypeDef],
@@ -1661,24 +1713,24 @@
     "GetServiceGraphResultTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
         "Services": List[ServiceTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTraceGraphResultTypeDef = TypedDict(
     "GetTraceGraphResultTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TraceSummaryTypeDef = TypedDict(
     "TraceSummaryTypeDef",
     {
         "Id": str,
@@ -1708,10 +1760,10 @@
 GetTraceSummariesResultTypeDef = TypedDict(
     "GetTraceSummariesResultTypeDef",
     {
         "TraceSummaries": List[TraceSummaryTypeDef],
         "ApproximateTime": datetime,
         "TracesProcessedCount": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray/type_defs.pyi` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,118 +34,121 @@
 
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
-    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "BatchGetTracesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "InsightsConfigurationTypeDef",
     "TagTypeDef",
     "SamplingRuleTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSamplingRuleRequestRequestTypeDef",
     "ErrorStatisticsTypeDef",
     "FaultStatisticsTypeDef",
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
     "GetInsightImpactGraphRequestRequestTypeDef",
     "GetInsightRequestRequestTypeDef",
     "GetInsightSummariesRequestRequestTypeDef",
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
     "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     "GetServiceGraphRequestRequestTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
+    "InsightsConfigurationOutputTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
+    "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
     "TelemetryRecordTypeDef",
-    "GroupSummaryTypeDef",
-    "GroupTypeDef",
+    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
-    "SamplingRuleRecordTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
+    "GroupSummaryTypeDef",
+    "GroupTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
+    "SamplingRuleRecordTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
     "PutTelemetryRecordsRequestRequestTypeDef",
+    "EdgeTypeDef",
+    "TimeSeriesServiceStatisticsTypeDef",
+    "ErrorRootCauseServiceTypeDef",
+    "FaultRootCauseServiceTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
+    "GetInsightImpactGraphResultTypeDef",
+    "ResponseTimeRootCauseTypeDef",
     "CreateSamplingRuleResultTypeDef",
     "DeleteSamplingRuleResultTypeDef",
     "GetSamplingRulesResultTypeDef",
     "UpdateSamplingRuleResultTypeDef",
-    "EdgeTypeDef",
-    "TimeSeriesServiceStatisticsTypeDef",
-    "ErrorRootCauseServiceTypeDef",
-    "FaultRootCauseServiceTypeDef",
-    "GetInsightImpactGraphResultTypeDef",
-    "ResponseTimeRootCauseTypeDef",
     "BatchGetTracesResultTypeDef",
     "GetInsightEventsResultTypeDef",
     "GetInsightSummariesResultTypeDef",
     "GetInsightResultTypeDef",
     "ServiceTypeDef",
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     "ErrorRootCauseTypeDef",
@@ -204,34 +207,24 @@
         "HTTPCode5XXCount": int,
         "UnknownHostCount": int,
         "OtherCount": int,
     },
     total=False,
 )
 
-_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
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
 
-class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
-    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-):
-    pass
-
 _RequiredBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestRequestTypeDef = TypedDict(
@@ -243,14 +236,25 @@
 )
 
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
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
 InsightsConfigurationTypeDef = TypedDict(
     "InsightsConfigurationTypeDef",
     {
         "InsightsEnabled": bool,
         "NotificationsEnabled": bool,
     },
     total=False,
@@ -391,22 +395,14 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
-GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetGroupsRequestRequestTypeDef = TypedDict(
     "GetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -481,38 +477,22 @@
 
 class GetInsightSummariesRequestRequestTypeDef(
     _RequiredGetInsightSummariesRequestRequestTypeDef,
     _OptionalGetInsightSummariesRequestRequestTypeDef,
 ):
     pass
 
-GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingStatisticSummariesRequestRequestTypeDef = TypedDict(
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -570,37 +550,14 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
 _RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -615,40 +572,14 @@
 )
 
 class GetServiceGraphRequestRequestTypeDef(
     _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
@@ -667,34 +598,14 @@
 
 class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
-    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-):
-    pass
-
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
@@ -715,14 +626,23 @@
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
 )
 
+InsightsConfigurationOutputTypeDef = TypedDict(
+    "InsightsConfigurationOutputTypeDef",
+    {
+        "InsightsEnabled": bool,
+        "NotificationsEnabled": bool,
+    },
+    total=False,
+)
+
 HttpTypeDef = TypedDict(
     "HttpTypeDef",
     {
         "HttpURL": str,
         "HttpStatus": int,
         "HttpMethod": str,
         "UserAgent": str,
@@ -753,22 +673,14 @@
     "InstanceIdDetailTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourcePoliciesRequestRequestTypeDef = TypedDict(
     "ListResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -780,34 +692,14 @@
         "PolicyDocument": str,
         "PolicyRevisionId": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -820,22 +712,20 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
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
 
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
@@ -896,35 +786,54 @@
     "ResourceARNDetailTypeDef",
     {
         "ARN": str,
     },
     total=False,
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
 ResponseTimeRootCauseEntityTypeDef = TypedDict(
     "ResponseTimeRootCauseEntityTypeDef",
     {
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
     total=False,
 )
 
+_RequiredSamplingRuleOutputTypeDef = TypedDict(
+    "_RequiredSamplingRuleOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Priority": int,
+        "FixedRate": float,
+        "ReservoirSize": int,
+        "ServiceName": str,
+        "ServiceType": str,
+        "Host": str,
+        "HTTPMethod": str,
+        "URLPath": str,
+        "Version": int,
+    },
+)
+_OptionalSamplingRuleOutputTypeDef = TypedDict(
+    "_OptionalSamplingRuleOutputTypeDef",
+    {
+        "RuleName": str,
+        "RuleARN": str,
+        "Attributes": Dict[str, str],
+    },
+    total=False,
+)
+
+class SamplingRuleOutputTypeDef(
+    _RequiredSamplingRuleOutputTypeDef, _OptionalSamplingRuleOutputTypeDef
+):
+    pass
+
 SamplingRuleUpdateTypeDef = TypedDict(
     "SamplingRuleUpdateTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
         "ResourceARN": str,
         "Priority": int,
@@ -1000,36 +909,155 @@
     },
     total=False,
 )
 
 class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
     pass
 
-GroupSummaryTypeDef = TypedDict(
-    "GroupSummaryTypeDef",
+_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
+    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+):
+    pass
+
+GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GroupTypeDef = TypedDict(
-    "GroupTypeDef",
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationTypeDef,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
+    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+):
+    pass
+
+ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
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
 UpdateGroupRequestRequestTypeDef = TypedDict(
     "UpdateGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -1054,23 +1082,14 @@
 )
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
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
@@ -1091,24 +1110,14 @@
 
 class CreateSamplingRuleRequestRequestTypeDef(
     _RequiredCreateSamplingRuleRequestRequestTypeDef,
     _OptionalCreateSamplingRuleRequestRequestTypeDef,
 ):
     pass
 
-SamplingRuleRecordTypeDef = TypedDict(
-    "SamplingRuleRecordTypeDef",
-    {
-        "SamplingRule": SamplingRuleTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-    },
-    total=False,
-)
-
 EdgeStatisticsTypeDef = TypedDict(
     "EdgeStatisticsTypeDef",
     {
         "OkCount": int,
         "ErrorStatistics": ErrorStatisticsTypeDef,
         "FaultStatistics": FaultStatisticsTypeDef,
         "TotalCount": int,
@@ -1129,23 +1138,23 @@
     total=False,
 )
 
 GetEncryptionConfigResultTypeDef = TypedDict(
     "GetEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEncryptionConfigResultTypeDef = TypedDict(
     "PutEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseEntityTypeDef = TypedDict(
     "ErrorRootCauseEntityTypeDef",
     {
         "Name": str,
@@ -1166,15 +1175,15 @@
 )
 
 GetSamplingStatisticSummariesResultTypeDef = TypedDict(
     "GetSamplingStatisticSummariesResultTypeDef",
     {
         "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSamplingTargetsRequestRequestTypeDef = TypedDict(
     "GetSamplingTargetsRequestRequestTypeDef",
     {
         "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
@@ -1183,15 +1192,15 @@
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
         "LastRuleModification": datetime,
         "UnprocessedStatistics": List[UnprocessedStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "StartTime": Union[datetime, str],
@@ -1201,15 +1210,15 @@
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
@@ -1236,14 +1245,36 @@
 )
 
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
+GroupSummaryTypeDef = TypedDict(
+    "GroupSummaryTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+GroupTypeDef = TypedDict(
+    "GroupTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1254,31 +1285,40 @@
 )
 
 ListResourcePoliciesResultTypeDef = TypedDict(
     "ListResourcePoliciesResultTypeDef",
     {
         "ResourcePolicies": List[ResourcePolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResultTypeDef = TypedDict(
     "PutResourcePolicyResultTypeDef",
     {
         "ResourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseServiceTypeDef = TypedDict(
     "ResponseTimeRootCauseServiceTypeDef",
     {
         "Name": str,
@@ -1287,14 +1327,24 @@
         "AccountId": str,
         "EntityPath": List[ResponseTimeRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+SamplingRuleRecordTypeDef = TypedDict(
+    "SamplingRuleRecordTypeDef",
+    {
+        "SamplingRule": SamplingRuleOutputTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+    },
+    total=False,
+)
+
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1378,80 +1428,14 @@
 
 class PutTelemetryRecordsRequestRequestTypeDef(
     _RequiredPutTelemetryRecordsRequestRequestTypeDef,
     _OptionalPutTelemetryRecordsRequestRequestTypeDef,
 ):
     pass
 
-GetGroupsResultTypeDef = TypedDict(
-    "GetGroupsResultTypeDef",
-    {
-        "Groups": List[GroupSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateGroupResultTypeDef = TypedDict(
-    "CreateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetGroupResultTypeDef = TypedDict(
-    "GetGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateGroupResultTypeDef = TypedDict(
-    "UpdateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSamplingRuleResultTypeDef = TypedDict(
-    "CreateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSamplingRuleResultTypeDef = TypedDict(
-    "DeleteSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSamplingRulesResultTypeDef = TypedDict(
-    "GetSamplingRulesResultTypeDef",
-    {
-        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSamplingRuleResultTypeDef = TypedDict(
-    "UpdateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
         "StartTime": datetime,
         "EndTime": datetime,
         "SummaryStatistics": EdgeStatisticsTypeDef,
@@ -1497,70 +1481,136 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+GetGroupsResultTypeDef = TypedDict(
+    "GetGroupsResultTypeDef",
+    {
+        "Groups": List[GroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResultTypeDef = TypedDict(
+    "CreateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResultTypeDef = TypedDict(
+    "GetGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGroupResultTypeDef = TypedDict(
+    "UpdateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
         "ServiceGraphEndTime": datetime,
         "Services": List[InsightImpactGraphServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseTypeDef = TypedDict(
     "ResponseTimeRootCauseTypeDef",
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
         "ClientImpacting": bool,
     },
     total=False,
 )
 
+CreateSamplingRuleResultTypeDef = TypedDict(
+    "CreateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSamplingRuleResultTypeDef = TypedDict(
+    "DeleteSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSamplingRulesResultTypeDef = TypedDict(
+    "GetSamplingRulesResultTypeDef",
+    {
+        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSamplingRuleResultTypeDef = TypedDict(
+    "UpdateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightEventsResultTypeDef = TypedDict(
     "GetInsightEventsResultTypeDef",
     {
         "InsightEvents": List[InsightEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightSummariesResultTypeDef = TypedDict(
     "GetInsightSummariesResultTypeDef",
     {
         "InsightSummaries": List[InsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightResultTypeDef = TypedDict(
     "GetInsightResultTypeDef",
     {
         "Insight": InsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "ReferenceId": int,
@@ -1582,15 +1632,15 @@
 
 GetTimeSeriesServiceStatisticsResultTypeDef = TypedDict(
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     {
         "TimeSeriesServiceStatistics": List[TimeSeriesServiceStatisticsTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseTypeDef = TypedDict(
     "ErrorRootCauseTypeDef",
     {
         "Services": List[ErrorRootCauseServiceTypeDef],
@@ -1612,24 +1662,24 @@
     "GetServiceGraphResultTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
         "Services": List[ServiceTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTraceGraphResultTypeDef = TypedDict(
     "GetTraceGraphResultTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TraceSummaryTypeDef = TypedDict(
     "TraceSummaryTypeDef",
     {
         "Id": str,
@@ -1659,10 +1709,10 @@
 GetTraceSummariesResultTypeDef = TypedDict(
     "GetTraceSummariesResultTypeDef",
     {
         "TraceSummaries": List[TraceSummaryTypeDef],
         "ApproximateTime": datetime,
         "TracesProcessedCount": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/PKG-INFO` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.0
-Summary: Type annotations for boto3.XRay 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.XRay 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-xray"></a>
 
 # mypy-boto3-xray
 
 [![PyPI - mypy-boto3-xray](https://img.shields.io/pypi/v/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-xray?color=blue)](https://pypistats.org/packages/mypy-boto3-xray)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,118 +368,121 @@
 ```python
 from mypy_boto3_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetTracesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
     GetInsightImpactGraphRequestRequestTypeDef,
     GetInsightRequestRequestTypeDef,
     GetInsightSummariesRequestRequestTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
+    InsightsConfigurationOutputTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
-    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
-    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
     TelemetryRecordTypeDef,
-    GroupSummaryTypeDef,
-    GroupTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
-    SamplingRuleRecordTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
+    GroupSummaryTypeDef,
+    GroupTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
+    SamplingRuleRecordTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
     PutTelemetryRecordsRequestRequestTypeDef,
+    EdgeTypeDef,
+    TimeSeriesServiceStatisticsTypeDef,
+    ErrorRootCauseServiceTypeDef,
+    FaultRootCauseServiceTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
+    GetInsightImpactGraphResultTypeDef,
+    ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
-    EdgeTypeDef,
-    TimeSeriesServiceStatisticsTypeDef,
-    ErrorRootCauseServiceTypeDef,
-    FaultRootCauseServiceTypeDef,
-    GetInsightImpactGraphResultTypeDef,
-    ResponseTimeRootCauseTypeDef,
     BatchGetTracesResultTypeDef,
     GetInsightEventsResultTypeDef,
     GetInsightSummariesResultTypeDef,
     GetInsightResultTypeDef,
     ServiceTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     ErrorRootCauseTypeDef,
```

### Comparing `mypy-boto3-xray-1.28.0/mypy_boto3_xray.egg-info/SOURCES.txt` & `mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.0/setup.py` & `mypy-boto3-xray-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-xray",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.XRay 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.XRay 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

