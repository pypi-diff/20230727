# Comparing `tmp/mypy-boto3-devops-guru-1.28.0.tar.gz` & `tmp/mypy-boto3-devops-guru-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devops-guru-1.28.0.tar", last modified: Thu Jul  6 20:59:23 2023, max compression
+gzip compressed data, was "mypy-boto3-devops-guru-1.28.12.tar", last modified: Thu Jul 27 05:34:34 2023, max compression
```

## Comparing `mypy-boto3-devops-guru-1.28.0.tar` & `mypy-boto3-devops-guru-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:23.370276 mypy-boto3-devops-guru-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-06 20:59:23.370276 mypy-boto3-devops-guru-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21456 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:23.366276 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-06 20:37:47.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-07-06 20:37:47.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62087 2023-07-06 20:37:49.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62022 2023-07-06 20:37:48.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:23.370276 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-06 20:59:23.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 20:59:23.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:23.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:23.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:23.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:23.000000 mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:23.370276 mypy-boto3-devops-guru-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 20:37:45.000000 mypy-boto3-devops-guru-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.056535 mypy-boto3-devops-guru-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23524 2023-07-27 05:34:34.052535 mypy-boto3-devops-guru-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22022 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.052535 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65792 2023-07-27 05:20:13.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65725 2023-07-27 05:20:12.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.052535 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23524 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:34.056535 mypy-boto3-devops-guru-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-27 05:20:10.000000 mypy-boto3-devops-guru-1.28.12/setup.py
```

### Comparing `mypy-boto3-devops-guru-1.28.0/LICENSE` & `mypy-boto3-devops-guru-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/PKG-INFO` & `mypy-boto3-devops-guru-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.0
-Summary: Type annotations for boto3.DevOpsGuru 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DevOpsGuru 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-devops-guru"></a>
 
 # mypy-boto3-devops-guru
 
 [![PyPI - mypy-boto3-devops-guru](https://img.shields.io/pypi/v/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,34 +408,38 @@
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
     AddNotificationChannelResponseTypeDef,
+    AmazonCodeGuruProfilerIntegrationOutputTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
+    CloudFormationCollectionOutputTypeDef,
     CloudFormationCollectionTypeDef,
+    CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
+    TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
-    InsightFeedbackTypeDef,
+    InsightFeedbackOutputTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
     DescribeOrganizationOverviewResponseTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
@@ -445,14 +449,15 @@
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
     GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
     GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
+    InsightFeedbackTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
     ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
@@ -461,104 +466,112 @@
     ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
     ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
+    NotificationFilterConfigOutputTypeDef,
+    SnsChannelConfigOutputTypeDef,
     NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
     PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
+    ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
+    TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
     ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
+    EventSourcesConfigOutputTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
-    PutFeedbackRequestRequestTypeDef,
     ListInsightsClosedStatusFilterTypeDef,
+    PutFeedbackRequestRequestTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
     PerformanceInsightsMetricQueryTypeDef,
     RecommendationRelatedAnomalySourceDetailTypeDef,
     RecommendationRelatedEventTypeDef,
     ResourceCollectionFilterTypeDef,
+    ResourceCollectionOutputTypeDef,
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
     StartCostEstimationRequestRequestTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
     ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
-    AddNotificationChannelRequestRequestTypeDef,
     NotificationChannelTypeDef,
+    AddNotificationChannelRequestRequestTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
-    ListEventsFiltersTypeDef,
     MonitoredResourceIdentifierTypeDef,
     ProactiveInsightSummaryTypeDef,
     ProactiveInsightTypeDef,
     ProactiveOrganizationInsightSummaryTypeDef,
     ReactiveInsightSummaryTypeDef,
     ReactiveInsightTypeDef,
     ReactiveOrganizationInsightSummaryTypeDef,
+    ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
     ListInsightsRequestListInsightsPaginateTypeDef,
     ListInsightsRequestRequestTypeDef,
     ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     ListOrganizationInsightsRequestRequestTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
-    ListEventsRequestListEventsPaginateTypeDef,
-    ListEventsRequestRequestTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     DescribeInsightResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
+    ListEventsRequestListEventsPaginateTypeDef,
+    ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
```

### Comparing `mypy-boto3-devops-guru-1.28.0/README.md` & `mypy-boto3-devops-guru-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-devops-guru"></a>
 
 # mypy-boto3-devops-guru
 
 [![PyPI - mypy-boto3-devops-guru](https://img.shields.io/pypi/v/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,34 +376,38 @@
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
     AddNotificationChannelResponseTypeDef,
+    AmazonCodeGuruProfilerIntegrationOutputTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
+    CloudFormationCollectionOutputTypeDef,
     CloudFormationCollectionTypeDef,
+    CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
+    TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
-    InsightFeedbackTypeDef,
+    InsightFeedbackOutputTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
     DescribeOrganizationOverviewResponseTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
@@ -413,14 +417,15 @@
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
     GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
     GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
+    InsightFeedbackTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
     ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
@@ -429,104 +434,112 @@
     ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
     ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
+    NotificationFilterConfigOutputTypeDef,
+    SnsChannelConfigOutputTypeDef,
     NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
     PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
+    ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
+    TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
     ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
+    EventSourcesConfigOutputTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
-    PutFeedbackRequestRequestTypeDef,
     ListInsightsClosedStatusFilterTypeDef,
+    PutFeedbackRequestRequestTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
     PerformanceInsightsMetricQueryTypeDef,
     RecommendationRelatedAnomalySourceDetailTypeDef,
     RecommendationRelatedEventTypeDef,
     ResourceCollectionFilterTypeDef,
+    ResourceCollectionOutputTypeDef,
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
     StartCostEstimationRequestRequestTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
     ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
-    AddNotificationChannelRequestRequestTypeDef,
     NotificationChannelTypeDef,
+    AddNotificationChannelRequestRequestTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
-    ListEventsFiltersTypeDef,
     MonitoredResourceIdentifierTypeDef,
     ProactiveInsightSummaryTypeDef,
     ProactiveInsightTypeDef,
     ProactiveOrganizationInsightSummaryTypeDef,
     ReactiveInsightSummaryTypeDef,
     ReactiveInsightTypeDef,
     ReactiveOrganizationInsightSummaryTypeDef,
+    ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
     ListInsightsRequestListInsightsPaginateTypeDef,
     ListInsightsRequestRequestTypeDef,
     ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     ListOrganizationInsightsRequestRequestTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
-    ListEventsRequestListEventsPaginateTypeDef,
-    ListEventsRequestRequestTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     DescribeInsightResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
+    ListEventsRequestListEventsPaginateTypeDef,
+    ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
```

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/__init__.py` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/__init__.pyi` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/__main__.py` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DevOpsGuru 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.DevOpsGuru 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
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

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/client.py` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/client.pyi` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/literals.py` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,15 @@
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
@@ -399,26 +400,28 @@
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

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/literals.pyi` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,15 @@
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
@@ -397,26 +398,28 @@
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

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/paginator.py` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/paginator.pyi` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/type_defs.py` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -44,38 +44,41 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountInsightHealthTypeDef",
     "AddNotificationChannelResponseTypeDef",
+    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
+    "CloudFormationCollectionOutputTypeDef",
     "CloudFormationCollectionTypeDef",
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
     "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
     "DescribeAccountOverviewResponseTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
-    "InsightFeedbackTypeDef",
+    "InsightFeedbackOutputTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
     "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
     "DescribeOrganizationOverviewResponseTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
@@ -85,14 +88,15 @@
     "EventResourceTypeDef",
     "EventTimeRangeTypeDef",
     "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
     "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
+    "InsightFeedbackTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
     "StartTimeRangeTypeDef",
     "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
@@ -101,104 +105,112 @@
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
     "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
+    "NotificationFilterConfigOutputTypeDef",
+    "SnsChannelConfigOutputTypeDef",
     "NotificationFilterConfigTypeDef",
     "SnsChannelConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
     "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
+    "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
+    "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
     "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
+    "EventSourcesConfigOutputTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeFeedbackResponseTypeDef",
-    "PutFeedbackRequestRequestTypeDef",
     "ListInsightsClosedStatusFilterTypeDef",
+    "PutFeedbackRequestRequestTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
+    "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "RecommendationRelatedAnomalySourceDetailTypeDef",
     "RecommendationRelatedEventTypeDef",
     "ResourceCollectionFilterTypeDef",
+    "ResourceCollectionOutputTypeDef",
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
     "ListInsightsStatusFilterTypeDef",
     "AnomalousLogGroupTypeDef",
-    "AddNotificationChannelRequestRequestTypeDef",
     "NotificationChannelTypeDef",
+    "AddNotificationChannelRequestRequestTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
-    "ListEventsFiltersTypeDef",
     "MonitoredResourceIdentifierTypeDef",
     "ProactiveInsightSummaryTypeDef",
     "ProactiveInsightTypeDef",
     "ProactiveOrganizationInsightSummaryTypeDef",
     "ReactiveInsightSummaryTypeDef",
     "ReactiveInsightTypeDef",
     "ReactiveOrganizationInsightSummaryTypeDef",
+    "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
     "ListInsightsRequestListInsightsPaginateTypeDef",
     "ListInsightsRequestRequestTypeDef",
     "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     "ListOrganizationInsightsRequestRequestTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
-    "ListEventsRequestListEventsPaginateTypeDef",
-    "ListEventsRequestRequestTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
     "SearchInsightsResponseTypeDef",
     "SearchOrganizationInsightsResponseTypeDef",
     "DescribeInsightResponseTypeDef",
     "ListOrganizationInsightsResponseTypeDef",
+    "ListEventsRequestListEventsPaginateTypeDef",
+    "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     "PerformanceInsightsReferenceDataTypeDef",
     "ListRecommendationsResponseTypeDef",
     "PerformanceInsightsMetricsDetailTypeDef",
@@ -224,14 +236,22 @@
     "AddNotificationChannelResponseTypeDef",
     {
         "Id": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AmazonCodeGuruProfilerIntegrationOutputTypeDef = TypedDict(
+    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
+    {
+        "Status": EventSourceOptInStatusType,
+    },
+    total=False,
+)
+
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
     },
     total=False,
 )
@@ -246,21 +266,19 @@
     "_OptionalAnomalyReportedTimeRangeTypeDef",
     {
         "CloseTime": datetime,
     },
     total=False,
 )
 
-
 class AnomalyReportedTimeRangeTypeDef(
     _RequiredAnomalyReportedTimeRangeTypeDef, _OptionalAnomalyReportedTimeRangeTypeDef
 ):
     pass
 
-
 AnomalyResourceTypeDef = TypedDict(
     "AnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -286,39 +304,53 @@
     "_OptionalAnomalyTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class AnomalyTimeRangeTypeDef(_RequiredAnomalyTimeRangeTypeDef, _OptionalAnomalyTimeRangeTypeDef):
     pass
 
-
 CloudFormationCollectionFilterTypeDef = TypedDict(
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
 
+CloudFormationCollectionOutputTypeDef = TypedDict(
+    "CloudFormationCollectionOutputTypeDef",
+    {
+        "StackNames": List[str],
+    },
+    total=False,
+)
+
 CloudFormationCollectionTypeDef = TypedDict(
     "CloudFormationCollectionTypeDef",
     {
+        "StackNames": Sequence[str],
+    },
+    total=False,
+)
+
+CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
         "StackNames": List[str],
     },
     total=False,
 )
 
 CloudFormationCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     {
-        "StackNames": List[str],
+        "StackNames": Sequence[str],
     },
     total=False,
 )
 
 InsightHealthTypeDef = TypedDict(
     "InsightHealthTypeDef",
     {
@@ -343,19 +375,27 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+TagCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "AppBoundaryKey": str,
+        "TagValues": List[str],
+    },
+)
+
 TagCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "TagCostEstimationResourceCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": List[str],
+        "TagValues": Sequence[str],
     },
 )
 
 CostEstimationTimeRangeTypeDef = TypedDict(
     "CostEstimationTimeRangeTypeDef",
     {
         "StartTime": datetime,
@@ -393,22 +433,20 @@
     "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
     {
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAccountOverviewResponseTypeDef = TypedDict(
     "DescribeAccountOverviewResponseTypeDef",
     {
         "ReactiveInsights": int,
         "ProactiveInsights": int,
         "MeanTimeToRecoverInMilliseconds": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -425,31 +463,29 @@
     "_OptionalDescribeAnomalyRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DescribeAnomalyRequestRequestTypeDef(
     _RequiredDescribeAnomalyRequestRequestTypeDef, _OptionalDescribeAnomalyRequestRequestTypeDef
 ):
     pass
 
-
 DescribeFeedbackRequestRequestTypeDef = TypedDict(
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
 
-InsightFeedbackTypeDef = TypedDict(
-    "InsightFeedbackTypeDef",
+InsightFeedbackOutputTypeDef = TypedDict(
+    "InsightFeedbackOutputTypeDef",
     {
         "Id": str,
         "Feedback": InsightFeedbackOptionType,
     },
     total=False,
 )
 
@@ -463,21 +499,19 @@
     "_OptionalDescribeInsightRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DescribeInsightRequestRequestTypeDef(
     _RequiredDescribeInsightRequestRequestTypeDef, _OptionalDescribeInsightRequestRequestTypeDef
 ):
     pass
 
-
 DescribeOrganizationHealthRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationHealthRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
@@ -506,22 +540,20 @@
         "ToTime": Union[datetime, str],
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeOrganizationOverviewResponseTypeDef = TypedDict(
     "DescribeOrganizationOverviewResponseTypeDef",
     {
         "ReactiveInsights": int,
         "ProactiveInsights": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -540,22 +572,20 @@
         "OrganizationalUnitIds": Sequence[str],
         "MaxResults": int,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -565,66 +595,60 @@
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-
 EndTimeRangeTypeDef = TypedDict(
     "EndTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
@@ -686,43 +710,48 @@
     "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
     _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetResourceCollectionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
+InsightFeedbackTypeDef = TypedDict(
+    "InsightFeedbackTypeDef",
+    {
+        "Id": str,
+        "Feedback": InsightFeedbackOptionType,
+    },
+    total=False,
+)
 
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
@@ -730,19 +759,17 @@
     "_OptionalInsightTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class InsightTimeRangeTypeDef(_RequiredInsightTimeRangeTypeDef, _OptionalInsightTimeRangeTypeDef):
     pass
 
-
 KMSServerSideEncryptionIntegrationConfigTypeDef = TypedDict(
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     {
         "KMSKeyId": str,
         "OptInStatus": OptInStatusType,
         "Type": ServerSideEncryptionTypeType,
     },
@@ -786,22 +813,20 @@
     "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
     _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -809,22 +834,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalousLogGroupsRequestRequestTypeDef(
     _RequiredListAnomalousLogGroupsRequestRequestTypeDef,
     _OptionalListAnomalousLogGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 ListInsightsOngoingStatusFilterTypeDef = TypedDict(
     "ListInsightsOngoingStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
     },
 )
 
@@ -864,22 +887,20 @@
         "Locale": LocaleType,
         "AccountId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
     _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
     _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -888,22 +909,20 @@
         "NextToken": str,
         "Locale": LocaleType,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
 LogAnomalyClassTypeDef = TypedDict(
     "LogAnomalyClassTypeDef",
     {
         "LogStreamName": str,
         "LogAnomalyType": LogAnomalyTypeType,
         "LogAnomalyToken": str,
         "LogEventId": str,
@@ -926,14 +945,31 @@
     "LogsAnomalyDetectionIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
+NotificationFilterConfigOutputTypeDef = TypedDict(
+    "NotificationFilterConfigOutputTypeDef",
+    {
+        "Severities": List[InsightSeverityType],
+        "MessageTypes": List[NotificationMessageTypeType],
+    },
+    total=False,
+)
+
+SnsChannelConfigOutputTypeDef = TypedDict(
+    "SnsChannelConfigOutputTypeDef",
+    {
+        "TopicArn": str,
+    },
+    total=False,
+)
+
 NotificationFilterConfigTypeDef = TypedDict(
     "NotificationFilterConfigTypeDef",
     {
         "Severities": Sequence[InsightSeverityType],
         "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
@@ -1010,20 +1046,26 @@
     "_OptionalPredictionTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
+ServiceCollectionOutputTypeDef = TypedDict(
+    "ServiceCollectionOutputTypeDef",
+    {
+        "ServiceNames": List[ServiceNameType],
+    },
+    total=False,
+)
 
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
@@ -1059,19 +1101,27 @@
     "TagCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
+TagCollectionOutputTypeDef = TypedDict(
+    "TagCollectionOutputTypeDef",
+    {
+        "AppBoundaryKey": str,
+        "TagValues": List[str],
+    },
+)
+
 TagCollectionTypeDef = TypedDict(
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": List[str],
+        "TagValues": Sequence[str],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -1112,14 +1162,22 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
+EventSourcesConfigOutputTypeDef = TypedDict(
+    "EventSourcesConfigOutputTypeDef",
+    {
+        "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationOutputTypeDef,
+    },
+    total=False,
+)
+
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
     total=False,
 )
@@ -1150,47 +1208,56 @@
     {
         "TimestampMetricValuePairList": List[TimestampMetricValuePairTypeDef],
         "StatusCode": CloudWatchMetricDataStatusCodeType,
     },
     total=False,
 )
 
+CostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
+        "Tags": List[TagCostEstimationResourceCollectionFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 CostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CostEstimationResourceCollectionFilterTypeDef",
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
-        "Tags": List[TagCostEstimationResourceCollectionFilterTypeDef],
+        "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
     },
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
-        "InsightFeedback": InsightFeedbackTypeDef,
+        "InsightFeedback": InsightFeedbackOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutFeedbackRequestRequestTypeDef = TypedDict(
-    "PutFeedbackRequestRequestTypeDef",
-    {
-        "InsightFeedback": InsightFeedbackTypeDef,
-    },
-    total=False,
-)
-
 ListInsightsClosedStatusFilterTypeDef = TypedDict(
     "ListInsightsClosedStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
         "EndTimeRange": EndTimeRangeTypeDef,
     },
 )
 
+PutFeedbackRequestRequestTypeDef = TypedDict(
+    "PutFeedbackRequestRequestTypeDef",
+    {
+        "InsightFeedback": InsightFeedbackTypeDef,
+    },
+    total=False,
+)
+
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
@@ -1226,35 +1293,52 @@
     "LogAnomalyShowcaseTypeDef",
     {
         "LogAnomalyClasses": List[LogAnomalyClassTypeDef],
     },
     total=False,
 )
 
+_RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_RequiredNotificationChannelConfigOutputTypeDef",
+    {
+        "Sns": SnsChannelConfigOutputTypeDef,
+    },
+)
+_OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_OptionalNotificationChannelConfigOutputTypeDef",
+    {
+        "Filters": NotificationFilterConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class NotificationChannelConfigOutputTypeDef(
+    _RequiredNotificationChannelConfigOutputTypeDef, _OptionalNotificationChannelConfigOutputTypeDef
+):
+    pass
+
 _RequiredNotificationChannelConfigTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigTypeDef",
     {
         "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigTypeDef = TypedDict(
     "_OptionalNotificationChannelConfigTypeDef",
     {
         "Filters": NotificationFilterConfigTypeDef,
     },
     total=False,
 )
 
-
 class NotificationChannelConfigTypeDef(
     _RequiredNotificationChannelConfigTypeDef, _OptionalNotificationChannelConfigTypeDef
 ):
     pass
 
-
 UpdateServiceIntegrationConfigTypeDef = TypedDict(
     "UpdateServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationConfigTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationConfigTypeDef,
         "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationConfigTypeDef,
     },
@@ -1303,19 +1387,28 @@
     {
         "CloudFormation": CloudFormationCollectionFilterTypeDef,
         "Tags": List[TagCollectionFilterTypeDef],
     },
     total=False,
 )
 
+ResourceCollectionOutputTypeDef = TypedDict(
+    "ResourceCollectionOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCollectionOutputTypeDef,
+        "Tags": List[TagCollectionOutputTypeDef],
+    },
+    total=False,
+)
+
 ResourceCollectionTypeDef = TypedDict(
     "ResourceCollectionTypeDef",
     {
         "CloudFormation": CloudFormationCollectionTypeDef,
-        "Tags": List[TagCollectionTypeDef],
+        "Tags": Sequence[TagCollectionTypeDef],
     },
     total=False,
 )
 
 ServiceHealthTypeDef = TypedDict(
     "ServiceHealthTypeDef",
     {
@@ -1334,15 +1427,15 @@
     },
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
-        "EventSources": EventSourcesConfigTypeDef,
+        "EventSources": EventSourcesConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
@@ -1364,15 +1457,15 @@
     },
     total=False,
 )
 
 GetCostEstimationResponseTypeDef = TypedDict(
     "GetCostEstimationResponseTypeDef",
     {
-        "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
+        "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1388,22 +1481,20 @@
     "_OptionalStartCostEstimationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
@@ -1413,22 +1504,20 @@
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
@@ -1439,22 +1528,20 @@
         "NextToken": str,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
     },
     total=False,
 )
 
-
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
-
 ListInsightsStatusFilterTypeDef = TypedDict(
     "ListInsightsStatusFilterTypeDef",
     {
         "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
         "Closed": ListInsightsClosedStatusFilterTypeDef,
         "Any": ListInsightsAnyStatusFilterTypeDef,
     },
@@ -1469,28 +1556,28 @@
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
         "LogAnomalyShowcases": List[LogAnomalyShowcaseTypeDef],
     },
     total=False,
 )
 
-AddNotificationChannelRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelRequestRequestTypeDef",
+NotificationChannelTypeDef = TypedDict(
+    "NotificationChannelTypeDef",
     {
-        "Config": NotificationChannelConfigTypeDef,
+        "Id": str,
+        "Config": NotificationChannelConfigOutputTypeDef,
     },
+    total=False,
 )
 
-NotificationChannelTypeDef = TypedDict(
-    "NotificationChannelTypeDef",
+AddNotificationChannelRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelRequestRequestTypeDef",
     {
-        "Id": str,
         "Config": NotificationChannelConfigTypeDef,
     },
-    total=False,
 )
 
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
@@ -1530,77 +1617,64 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Id": str,
         "Time": datetime,
         "EventSource": str,
         "Name": str,
         "DataSource": EventDataSourceType,
         "EventClass": EventClassType,
         "Resources": List[EventResourceTypeDef],
     },
     total=False,
 )
 
-ListEventsFiltersTypeDef = TypedDict(
-    "ListEventsFiltersTypeDef",
-    {
-        "InsightId": str,
-        "EventTimeRange": EventTimeRangeTypeDef,
-        "EventClass": EventClassType,
-        "EventSource": str,
-        "DataSource": EventDataSourceType,
-        "ResourceCollection": ResourceCollectionTypeDef,
-    },
-    total=False,
-)
-
 MonitoredResourceIdentifierTypeDef = TypedDict(
     "MonitoredResourceIdentifierTypeDef",
     {
         "MonitoredResourceName": str,
         "Type": str,
         "ResourcePermission": ResourcePermissionType,
         "LastUpdated": datetime,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ProactiveInsightSummaryTypeDef = TypedDict(
     "ProactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ProactiveInsightTypeDef = TypedDict(
     "ProactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ProactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1610,44 +1684,44 @@
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ReactiveInsightSummaryTypeDef = TypedDict(
     "ReactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ReactiveInsightTypeDef = TypedDict(
     "ReactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ReactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1656,16 +1730,29 @@
         "Id": str,
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
+    },
+    total=False,
+)
+
+ListEventsFiltersTypeDef = TypedDict(
+    "ListEventsFiltersTypeDef",
+    {
+        "InsightId": str,
+        "EventTimeRange": EventTimeRangeTypeDef,
+        "EventClass": EventClassType,
+        "EventSource": str,
+        "DataSource": EventDataSourceType,
         "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 SearchInsightsFiltersTypeDef = TypedDict(
     "SearchInsightsFiltersTypeDef",
     {
@@ -1729,22 +1816,20 @@
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
     _OptionalListInsightsRequestListInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestRequestTypeDef = TypedDict(
@@ -1752,21 +1837,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListInsightsRequestRequestTypeDef(
     _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
@@ -1775,22 +1858,20 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
@@ -1800,22 +1881,20 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListOrganizationInsightsRequestRequestTypeDef(
     _RequiredListOrganizationInsightsRequestRequestTypeDef,
     _OptionalListOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
-
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1859,60 +1938,14 @@
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_RequiredListEventsRequestListEventsPaginateTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_OptionalListEventsRequestListEventsPaginateTypeDef",
-    {
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEventsRequestListEventsPaginateTypeDef(
-    _RequiredListEventsRequestListEventsPaginateTypeDef,
-    _OptionalListEventsRequestListEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventsRequestRequestTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
-    },
-    total=False,
-)
-
-
-class ListEventsRequestRequestTypeDef(
-    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
-):
-    pass
-
-
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1963,14 +1996,56 @@
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_RequiredListEventsRequestListEventsPaginateTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_OptionalListEventsRequestListEventsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEventsRequestListEventsPaginateTypeDef(
+    _RequiredListEventsRequestListEventsPaginateTypeDef,
+    _OptionalListEventsRequestListEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredListEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventsRequestRequestTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class ListEventsRequestRequestTypeDef(
+    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
+):
+    pass
+
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -1980,21 +2055,19 @@
         "Filters": SearchInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchInsightsRequestRequestTypeDef(
     _RequiredSearchInsightsRequestRequestTypeDef, _OptionalSearchInsightsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -2003,22 +2076,20 @@
     {
         "Filters": SearchInsightsFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -2029,22 +2100,20 @@
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchOrganizationInsightsRequestRequestTypeDef(
     _RequiredSearchOrganizationInsightsRequestRequestTypeDef,
     _OptionalSearchOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -2054,22 +2123,20 @@
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
-
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
@@ -2114,15 +2181,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2135,15 +2202,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2154,15 +2221,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2174,15 +2241,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
```

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru/type_defs.pyi` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,37 +44,42 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountInsightHealthTypeDef",
     "AddNotificationChannelResponseTypeDef",
+    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
+    "CloudFormationCollectionOutputTypeDef",
     "CloudFormationCollectionTypeDef",
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
     "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
     "DescribeAccountOverviewResponseTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
-    "InsightFeedbackTypeDef",
+    "InsightFeedbackOutputTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
     "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
     "DescribeOrganizationOverviewResponseTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
@@ -84,14 +89,15 @@
     "EventResourceTypeDef",
     "EventTimeRangeTypeDef",
     "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
     "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
+    "InsightFeedbackTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
     "StartTimeRangeTypeDef",
     "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
@@ -100,104 +106,112 @@
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
     "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
+    "NotificationFilterConfigOutputTypeDef",
+    "SnsChannelConfigOutputTypeDef",
     "NotificationFilterConfigTypeDef",
     "SnsChannelConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
     "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
+    "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
+    "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
     "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
+    "EventSourcesConfigOutputTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeFeedbackResponseTypeDef",
-    "PutFeedbackRequestRequestTypeDef",
     "ListInsightsClosedStatusFilterTypeDef",
+    "PutFeedbackRequestRequestTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
+    "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "RecommendationRelatedAnomalySourceDetailTypeDef",
     "RecommendationRelatedEventTypeDef",
     "ResourceCollectionFilterTypeDef",
+    "ResourceCollectionOutputTypeDef",
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
     "ListInsightsStatusFilterTypeDef",
     "AnomalousLogGroupTypeDef",
-    "AddNotificationChannelRequestRequestTypeDef",
     "NotificationChannelTypeDef",
+    "AddNotificationChannelRequestRequestTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
-    "ListEventsFiltersTypeDef",
     "MonitoredResourceIdentifierTypeDef",
     "ProactiveInsightSummaryTypeDef",
     "ProactiveInsightTypeDef",
     "ProactiveOrganizationInsightSummaryTypeDef",
     "ReactiveInsightSummaryTypeDef",
     "ReactiveInsightTypeDef",
     "ReactiveOrganizationInsightSummaryTypeDef",
+    "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
     "ListInsightsRequestListInsightsPaginateTypeDef",
     "ListInsightsRequestRequestTypeDef",
     "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     "ListOrganizationInsightsRequestRequestTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
-    "ListEventsRequestListEventsPaginateTypeDef",
-    "ListEventsRequestRequestTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
     "SearchInsightsResponseTypeDef",
     "SearchOrganizationInsightsResponseTypeDef",
     "DescribeInsightResponseTypeDef",
     "ListOrganizationInsightsResponseTypeDef",
+    "ListEventsRequestListEventsPaginateTypeDef",
+    "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     "PerformanceInsightsReferenceDataTypeDef",
     "ListRecommendationsResponseTypeDef",
     "PerformanceInsightsMetricsDetailTypeDef",
@@ -223,14 +237,22 @@
     "AddNotificationChannelResponseTypeDef",
     {
         "Id": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AmazonCodeGuruProfilerIntegrationOutputTypeDef = TypedDict(
+    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
+    {
+        "Status": EventSourceOptInStatusType,
+    },
+    total=False,
+)
+
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
     },
     total=False,
 )
@@ -245,19 +267,21 @@
     "_OptionalAnomalyReportedTimeRangeTypeDef",
     {
         "CloseTime": datetime,
     },
     total=False,
 )
 
+
 class AnomalyReportedTimeRangeTypeDef(
     _RequiredAnomalyReportedTimeRangeTypeDef, _OptionalAnomalyReportedTimeRangeTypeDef
 ):
     pass
 
+
 AnomalyResourceTypeDef = TypedDict(
     "AnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -283,37 +307,55 @@
     "_OptionalAnomalyTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class AnomalyTimeRangeTypeDef(_RequiredAnomalyTimeRangeTypeDef, _OptionalAnomalyTimeRangeTypeDef):
     pass
 
+
 CloudFormationCollectionFilterTypeDef = TypedDict(
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
 
+CloudFormationCollectionOutputTypeDef = TypedDict(
+    "CloudFormationCollectionOutputTypeDef",
+    {
+        "StackNames": List[str],
+    },
+    total=False,
+)
+
 CloudFormationCollectionTypeDef = TypedDict(
     "CloudFormationCollectionTypeDef",
     {
+        "StackNames": Sequence[str],
+    },
+    total=False,
+)
+
+CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
         "StackNames": List[str],
     },
     total=False,
 )
 
 CloudFormationCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     {
-        "StackNames": List[str],
+        "StackNames": Sequence[str],
     },
     total=False,
 )
 
 InsightHealthTypeDef = TypedDict(
     "InsightHealthTypeDef",
     {
@@ -338,19 +380,27 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+TagCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "AppBoundaryKey": str,
+        "TagValues": List[str],
+    },
+)
+
 TagCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "TagCostEstimationResourceCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": List[str],
+        "TagValues": Sequence[str],
     },
 )
 
 CostEstimationTimeRangeTypeDef = TypedDict(
     "CostEstimationTimeRangeTypeDef",
     {
         "StartTime": datetime,
@@ -388,20 +438,22 @@
     "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
     {
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAccountOverviewResponseTypeDef = TypedDict(
     "DescribeAccountOverviewResponseTypeDef",
     {
         "ReactiveInsights": int,
         "ProactiveInsights": int,
         "MeanTimeToRecoverInMilliseconds": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -418,29 +470,31 @@
     "_OptionalDescribeAnomalyRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DescribeAnomalyRequestRequestTypeDef(
     _RequiredDescribeAnomalyRequestRequestTypeDef, _OptionalDescribeAnomalyRequestRequestTypeDef
 ):
     pass
 
+
 DescribeFeedbackRequestRequestTypeDef = TypedDict(
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
 
-InsightFeedbackTypeDef = TypedDict(
-    "InsightFeedbackTypeDef",
+InsightFeedbackOutputTypeDef = TypedDict(
+    "InsightFeedbackOutputTypeDef",
     {
         "Id": str,
         "Feedback": InsightFeedbackOptionType,
     },
     total=False,
 )
 
@@ -454,19 +508,21 @@
     "_OptionalDescribeInsightRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DescribeInsightRequestRequestTypeDef(
     _RequiredDescribeInsightRequestRequestTypeDef, _OptionalDescribeInsightRequestRequestTypeDef
 ):
     pass
 
+
 DescribeOrganizationHealthRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationHealthRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
@@ -495,20 +551,22 @@
         "ToTime": Union[datetime, str],
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeOrganizationOverviewResponseTypeDef = TypedDict(
     "DescribeOrganizationOverviewResponseTypeDef",
     {
         "ReactiveInsights": int,
         "ProactiveInsights": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -527,20 +585,22 @@
         "OrganizationalUnitIds": Sequence[str],
         "MaxResults": int,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -550,60 +610,66 @@
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
+
 EndTimeRangeTypeDef = TypedDict(
     "EndTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
@@ -665,57 +731,72 @@
     "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
     _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_OptionalGetResourceCollectionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
+
+InsightFeedbackTypeDef = TypedDict(
+    "InsightFeedbackTypeDef",
+    {
+        "Id": str,
+        "Feedback": InsightFeedbackOptionType,
+    },
+    total=False,
+)
+
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
 _OptionalInsightTimeRangeTypeDef = TypedDict(
     "_OptionalInsightTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class InsightTimeRangeTypeDef(_RequiredInsightTimeRangeTypeDef, _OptionalInsightTimeRangeTypeDef):
     pass
 
+
 KMSServerSideEncryptionIntegrationConfigTypeDef = TypedDict(
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     {
         "KMSKeyId": str,
         "OptInStatus": OptInStatusType,
         "Type": ServerSideEncryptionTypeType,
     },
@@ -759,20 +840,22 @@
     "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
     _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -780,20 +863,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalousLogGroupsRequestRequestTypeDef(
     _RequiredListAnomalousLogGroupsRequestRequestTypeDef,
     _OptionalListAnomalousLogGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 ListInsightsOngoingStatusFilterTypeDef = TypedDict(
     "ListInsightsOngoingStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
     },
 )
 
@@ -833,20 +918,22 @@
         "Locale": LocaleType,
         "AccountId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
     _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
     _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -855,20 +942,22 @@
         "NextToken": str,
         "Locale": LocaleType,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+
 LogAnomalyClassTypeDef = TypedDict(
     "LogAnomalyClassTypeDef",
     {
         "LogStreamName": str,
         "LogAnomalyType": LogAnomalyTypeType,
         "LogAnomalyToken": str,
         "LogEventId": str,
@@ -891,14 +980,31 @@
     "LogsAnomalyDetectionIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
+NotificationFilterConfigOutputTypeDef = TypedDict(
+    "NotificationFilterConfigOutputTypeDef",
+    {
+        "Severities": List[InsightSeverityType],
+        "MessageTypes": List[NotificationMessageTypeType],
+    },
+    total=False,
+)
+
+SnsChannelConfigOutputTypeDef = TypedDict(
+    "SnsChannelConfigOutputTypeDef",
+    {
+        "TopicArn": str,
+    },
+    total=False,
+)
+
 NotificationFilterConfigTypeDef = TypedDict(
     "NotificationFilterConfigTypeDef",
     {
         "Severities": Sequence[InsightSeverityType],
         "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
@@ -975,19 +1081,29 @@
     "_OptionalPredictionTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
+
+ServiceCollectionOutputTypeDef = TypedDict(
+    "ServiceCollectionOutputTypeDef",
+    {
+        "ServiceNames": List[ServiceNameType],
+    },
+    total=False,
+)
+
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -1022,19 +1138,27 @@
     "TagCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
+TagCollectionOutputTypeDef = TypedDict(
+    "TagCollectionOutputTypeDef",
+    {
+        "AppBoundaryKey": str,
+        "TagValues": List[str],
+    },
+)
+
 TagCollectionTypeDef = TypedDict(
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": List[str],
+        "TagValues": Sequence[str],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -1075,14 +1199,22 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
+EventSourcesConfigOutputTypeDef = TypedDict(
+    "EventSourcesConfigOutputTypeDef",
+    {
+        "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationOutputTypeDef,
+    },
+    total=False,
+)
+
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
     total=False,
 )
@@ -1113,47 +1245,56 @@
     {
         "TimestampMetricValuePairList": List[TimestampMetricValuePairTypeDef],
         "StatusCode": CloudWatchMetricDataStatusCodeType,
     },
     total=False,
 )
 
+CostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
+        "Tags": List[TagCostEstimationResourceCollectionFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 CostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CostEstimationResourceCollectionFilterTypeDef",
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
-        "Tags": List[TagCostEstimationResourceCollectionFilterTypeDef],
+        "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
     },
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
-        "InsightFeedback": InsightFeedbackTypeDef,
+        "InsightFeedback": InsightFeedbackOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutFeedbackRequestRequestTypeDef = TypedDict(
-    "PutFeedbackRequestRequestTypeDef",
-    {
-        "InsightFeedback": InsightFeedbackTypeDef,
-    },
-    total=False,
-)
-
 ListInsightsClosedStatusFilterTypeDef = TypedDict(
     "ListInsightsClosedStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
         "EndTimeRange": EndTimeRangeTypeDef,
     },
 )
 
+PutFeedbackRequestRequestTypeDef = TypedDict(
+    "PutFeedbackRequestRequestTypeDef",
+    {
+        "InsightFeedback": InsightFeedbackTypeDef,
+    },
+    total=False,
+)
+
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
@@ -1189,33 +1330,56 @@
     "LogAnomalyShowcaseTypeDef",
     {
         "LogAnomalyClasses": List[LogAnomalyClassTypeDef],
     },
     total=False,
 )
 
+_RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_RequiredNotificationChannelConfigOutputTypeDef",
+    {
+        "Sns": SnsChannelConfigOutputTypeDef,
+    },
+)
+_OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_OptionalNotificationChannelConfigOutputTypeDef",
+    {
+        "Filters": NotificationFilterConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class NotificationChannelConfigOutputTypeDef(
+    _RequiredNotificationChannelConfigOutputTypeDef, _OptionalNotificationChannelConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredNotificationChannelConfigTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigTypeDef",
     {
         "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigTypeDef = TypedDict(
     "_OptionalNotificationChannelConfigTypeDef",
     {
         "Filters": NotificationFilterConfigTypeDef,
     },
     total=False,
 )
 
+
 class NotificationChannelConfigTypeDef(
     _RequiredNotificationChannelConfigTypeDef, _OptionalNotificationChannelConfigTypeDef
 ):
     pass
 
+
 UpdateServiceIntegrationConfigTypeDef = TypedDict(
     "UpdateServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationConfigTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationConfigTypeDef,
         "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationConfigTypeDef,
     },
@@ -1264,19 +1428,28 @@
     {
         "CloudFormation": CloudFormationCollectionFilterTypeDef,
         "Tags": List[TagCollectionFilterTypeDef],
     },
     total=False,
 )
 
+ResourceCollectionOutputTypeDef = TypedDict(
+    "ResourceCollectionOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCollectionOutputTypeDef,
+        "Tags": List[TagCollectionOutputTypeDef],
+    },
+    total=False,
+)
+
 ResourceCollectionTypeDef = TypedDict(
     "ResourceCollectionTypeDef",
     {
         "CloudFormation": CloudFormationCollectionTypeDef,
-        "Tags": List[TagCollectionTypeDef],
+        "Tags": Sequence[TagCollectionTypeDef],
     },
     total=False,
 )
 
 ServiceHealthTypeDef = TypedDict(
     "ServiceHealthTypeDef",
     {
@@ -1295,15 +1468,15 @@
     },
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
-        "EventSources": EventSourcesConfigTypeDef,
+        "EventSources": EventSourcesConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
@@ -1325,15 +1498,15 @@
     },
     total=False,
 )
 
 GetCostEstimationResponseTypeDef = TypedDict(
     "GetCostEstimationResponseTypeDef",
     {
-        "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
+        "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1349,20 +1522,22 @@
     "_OptionalStartCostEstimationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
@@ -1372,20 +1547,22 @@
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
@@ -1396,20 +1573,22 @@
         "NextToken": str,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
     },
     total=False,
 )
 
+
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
+
 ListInsightsStatusFilterTypeDef = TypedDict(
     "ListInsightsStatusFilterTypeDef",
     {
         "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
         "Closed": ListInsightsClosedStatusFilterTypeDef,
         "Any": ListInsightsAnyStatusFilterTypeDef,
     },
@@ -1424,28 +1603,28 @@
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
         "LogAnomalyShowcases": List[LogAnomalyShowcaseTypeDef],
     },
     total=False,
 )
 
-AddNotificationChannelRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelRequestRequestTypeDef",
+NotificationChannelTypeDef = TypedDict(
+    "NotificationChannelTypeDef",
     {
-        "Config": NotificationChannelConfigTypeDef,
+        "Id": str,
+        "Config": NotificationChannelConfigOutputTypeDef,
     },
+    total=False,
 )
 
-NotificationChannelTypeDef = TypedDict(
-    "NotificationChannelTypeDef",
+AddNotificationChannelRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelRequestRequestTypeDef",
     {
-        "Id": str,
         "Config": NotificationChannelConfigTypeDef,
     },
-    total=False,
 )
 
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
@@ -1485,77 +1664,64 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Id": str,
         "Time": datetime,
         "EventSource": str,
         "Name": str,
         "DataSource": EventDataSourceType,
         "EventClass": EventClassType,
         "Resources": List[EventResourceTypeDef],
     },
     total=False,
 )
 
-ListEventsFiltersTypeDef = TypedDict(
-    "ListEventsFiltersTypeDef",
-    {
-        "InsightId": str,
-        "EventTimeRange": EventTimeRangeTypeDef,
-        "EventClass": EventClassType,
-        "EventSource": str,
-        "DataSource": EventDataSourceType,
-        "ResourceCollection": ResourceCollectionTypeDef,
-    },
-    total=False,
-)
-
 MonitoredResourceIdentifierTypeDef = TypedDict(
     "MonitoredResourceIdentifierTypeDef",
     {
         "MonitoredResourceName": str,
         "Type": str,
         "ResourcePermission": ResourcePermissionType,
         "LastUpdated": datetime,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ProactiveInsightSummaryTypeDef = TypedDict(
     "ProactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ProactiveInsightTypeDef = TypedDict(
     "ProactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ProactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1565,44 +1731,44 @@
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ReactiveInsightSummaryTypeDef = TypedDict(
     "ReactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ReactiveInsightTypeDef = TypedDict(
     "ReactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ReactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1611,16 +1777,29 @@
         "Id": str,
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
+    },
+    total=False,
+)
+
+ListEventsFiltersTypeDef = TypedDict(
+    "ListEventsFiltersTypeDef",
+    {
+        "InsightId": str,
+        "EventTimeRange": EventTimeRangeTypeDef,
+        "EventClass": EventClassType,
+        "EventSource": str,
+        "DataSource": EventDataSourceType,
         "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 SearchInsightsFiltersTypeDef = TypedDict(
     "SearchInsightsFiltersTypeDef",
     {
@@ -1684,20 +1863,22 @@
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
     _OptionalListInsightsRequestListInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestRequestTypeDef = TypedDict(
@@ -1705,19 +1886,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListInsightsRequestRequestTypeDef(
     _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
@@ -1726,20 +1909,22 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
@@ -1749,20 +1934,22 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListOrganizationInsightsRequestRequestTypeDef(
     _RequiredListOrganizationInsightsRequestRequestTypeDef,
     _OptionalListOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
+
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1806,56 +1993,14 @@
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_RequiredListEventsRequestListEventsPaginateTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_OptionalListEventsRequestListEventsPaginateTypeDef",
-    {
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEventsRequestListEventsPaginateTypeDef(
-    _RequiredListEventsRequestListEventsPaginateTypeDef,
-    _OptionalListEventsRequestListEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventsRequestRequestTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
-    },
-    total=False,
-)
-
-class ListEventsRequestRequestTypeDef(
-    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
-):
-    pass
-
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1906,14 +2051,60 @@
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_RequiredListEventsRequestListEventsPaginateTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_OptionalListEventsRequestListEventsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEventsRequestListEventsPaginateTypeDef(
+    _RequiredListEventsRequestListEventsPaginateTypeDef,
+    _OptionalListEventsRequestListEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventsRequestRequestTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class ListEventsRequestRequestTypeDef(
+    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -1923,19 +2114,21 @@
         "Filters": SearchInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchInsightsRequestRequestTypeDef(
     _RequiredSearchInsightsRequestRequestTypeDef, _OptionalSearchInsightsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -1944,20 +2137,22 @@
     {
         "Filters": SearchInsightsFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -1968,20 +2163,22 @@
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchOrganizationInsightsRequestRequestTypeDef(
     _RequiredSearchOrganizationInsightsRequestRequestTypeDef,
     _OptionalSearchOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -1991,20 +2188,22 @@
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
@@ -2049,15 +2248,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2070,15 +2269,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2089,15 +2288,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2109,15 +2308,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
```

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/PKG-INFO` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.0
-Summary: Type annotations for boto3.DevOpsGuru 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DevOpsGuru 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-devops-guru"></a>
 
 # mypy-boto3-devops-guru
 
 [![PyPI - mypy-boto3-devops-guru](https://img.shields.io/pypi/v/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,34 +408,38 @@
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
     AddNotificationChannelResponseTypeDef,
+    AmazonCodeGuruProfilerIntegrationOutputTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
+    CloudFormationCollectionOutputTypeDef,
     CloudFormationCollectionTypeDef,
+    CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
+    TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
-    InsightFeedbackTypeDef,
+    InsightFeedbackOutputTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
     DescribeOrganizationOverviewResponseTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
@@ -445,14 +449,15 @@
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
     GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
     GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
+    InsightFeedbackTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
     ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
@@ -461,104 +466,112 @@
     ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
     ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
+    NotificationFilterConfigOutputTypeDef,
+    SnsChannelConfigOutputTypeDef,
     NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
     PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
+    ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
+    TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
     ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
+    EventSourcesConfigOutputTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
-    PutFeedbackRequestRequestTypeDef,
     ListInsightsClosedStatusFilterTypeDef,
+    PutFeedbackRequestRequestTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
     PerformanceInsightsMetricQueryTypeDef,
     RecommendationRelatedAnomalySourceDetailTypeDef,
     RecommendationRelatedEventTypeDef,
     ResourceCollectionFilterTypeDef,
+    ResourceCollectionOutputTypeDef,
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
     StartCostEstimationRequestRequestTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
     ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
-    AddNotificationChannelRequestRequestTypeDef,
     NotificationChannelTypeDef,
+    AddNotificationChannelRequestRequestTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
-    ListEventsFiltersTypeDef,
     MonitoredResourceIdentifierTypeDef,
     ProactiveInsightSummaryTypeDef,
     ProactiveInsightTypeDef,
     ProactiveOrganizationInsightSummaryTypeDef,
     ReactiveInsightSummaryTypeDef,
     ReactiveInsightTypeDef,
     ReactiveOrganizationInsightSummaryTypeDef,
+    ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
     ListInsightsRequestListInsightsPaginateTypeDef,
     ListInsightsRequestRequestTypeDef,
     ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     ListOrganizationInsightsRequestRequestTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
-    ListEventsRequestListEventsPaginateTypeDef,
-    ListEventsRequestRequestTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     DescribeInsightResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
+    ListEventsRequestListEventsPaginateTypeDef,
+    ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
```

### Comparing `mypy-boto3-devops-guru-1.28.0/mypy_boto3_devops_guru.egg-info/SOURCES.txt` & `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.0/setup.py` & `mypy-boto3-devops-guru-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devops-guru",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DevOpsGuru 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.DevOpsGuru 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

