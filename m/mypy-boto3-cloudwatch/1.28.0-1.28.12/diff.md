# Comparing `tmp/mypy-boto3-cloudwatch-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudwatch-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudwatch-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudwatch-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
```

## Comparing `mypy-boto3-cloudwatch-1.28.0.tar` & `mypy-boto3-cloudwatch-1.28.12.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19301 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.394250 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-06 20:35:38.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-07-06 20:35:37.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23079 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42495 2023-07-06 20:35:39.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-07-06 20:35:38.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:35:35.000000 mypy-boto3-cloudwatch-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.064556 mypy-boto3-cloudwatch-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-07-27 05:34:27.044556 mypy-boto3-cloudwatch-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.044556 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    45926 2023-07-27 05:18:52.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45877 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.044556 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.064556 mypy-boto3-cloudwatch-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/LICENSE` & `mypy-boto3-cloudwatch-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatch 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatch 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudwatch"></a>
 
 # mypy-boto3-cloudwatch
 
 [![PyPI - mypy-boto3-cloudwatch](https://img.shields.io/pypi/v/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -446,21 +446,23 @@
 
 `mypy_boto3_cloudwatch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
+    RangeOutputTypeDef,
     RangeTypeDef,
-    DimensionTypeDef,
+    DimensionOutputTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
+    DimensionTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
     DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
@@ -478,82 +480,92 @@
     GetDashboardInputRequestTypeDef,
     GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
-    MetricStreamFilterTypeDef,
+    MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
     GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
     ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ManagedRuleStateTypeDef,
+    TagTypeDef,
     StatisticSetTypeDef,
+    MetricStreamFilterTypeDef,
+    MetricStreamStatisticsMetricOutputTypeDef,
     MetricStreamStatisticsMetricTypeDef,
     PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
     PutMetricStreamOutputTypeDef,
     ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
+    AnomalyDetectorConfigurationOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
+    MetricOutputTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
     DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
     EnableInsightRulesOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    ManagedRuleDescriptionTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
+    MetricStatOutputTypeDef,
     MetricStatTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
-    PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
+    PutManagedInsightRulesInputRequestTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
     PutMetricStreamInputRequestTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
+    MetricAlarmTypeDef,
+    MetricMathAnomalyDetectorOutputTypeDef,
     GetMetricDataInputGetMetricDataPaginateTypeDef,
     GetMetricDataInputRequestTypeDef,
-    MetricAlarmTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
     PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/README.md` & `mypy-boto3-cloudwatch-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudwatch"></a>
 
 # mypy-boto3-cloudwatch
 
 [![PyPI - mypy-boto3-cloudwatch](https://img.shields.io/pypi/v/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -414,21 +414,23 @@
 
 `mypy_boto3_cloudwatch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
+    RangeOutputTypeDef,
     RangeTypeDef,
-    DimensionTypeDef,
+    DimensionOutputTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
+    DimensionTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
     DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
@@ -446,82 +448,92 @@
     GetDashboardInputRequestTypeDef,
     GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
-    MetricStreamFilterTypeDef,
+    MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
     GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
     ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ManagedRuleStateTypeDef,
+    TagTypeDef,
     StatisticSetTypeDef,
+    MetricStreamFilterTypeDef,
+    MetricStreamStatisticsMetricOutputTypeDef,
     MetricStreamStatisticsMetricTypeDef,
     PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
     PutMetricStreamOutputTypeDef,
     ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
+    AnomalyDetectorConfigurationOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
+    MetricOutputTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
     DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
     EnableInsightRulesOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    ManagedRuleDescriptionTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
+    MetricStatOutputTypeDef,
     MetricStatTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
-    PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
+    PutManagedInsightRulesInputRequestTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
     PutMetricStreamInputRequestTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
+    MetricAlarmTypeDef,
+    MetricMathAnomalyDetectorOutputTypeDef,
     GetMetricDataInputGetMetricDataPaginateTypeDef,
     GetMetricDataInputRequestTypeDef,
-    MetricAlarmTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
     PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.pyi` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__main__.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatch 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudWatch 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
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

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.pyi` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,15 @@
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
@@ -311,26 +312,28 @@
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

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.pyi` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,15 @@
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
@@ -309,26 +310,28 @@
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

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.pyi` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,18 @@
     StandardUnitType,
     StateValueType,
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
+    DimensionOutputTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -289,24 +291,24 @@
     state_reason: str
     state_reason_data: str
     state_updated_timestamp: datetime
     metric_name: str
     namespace: str
     statistic: StatisticType
     extended_statistic: str
-    dimensions: List[DimensionTypeDef]
+    dimensions: List[DimensionOutputTypeDef]
     period: int
     unit: StandardUnitType
     evaluation_periods: int
     datapoints_to_alarm: int
     threshold: float
     comparison_operator: ComparisonOperatorType
     treat_missing_data: str
     evaluate_low_sample_count_percentile: str
-    metrics: List[MetricDataQueryTypeDef]
+    metrics: List[MetricDataQueryOutputTypeDef]
     threshold_metric_id: str
     evaluation_state: Literal["PARTIAL_DATA"]
     state_transitioned_timestamp: datetime
     name: str
     metric: "Metric"
 
     def delete(self) -> None:
@@ -394,15 +396,15 @@
 class Metric(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Metric)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/service_resource/#metric)
     """
 
     metric_name: str
-    dimensions: List[DimensionTypeDef]
+    dimensions: List[DimensionOutputTypeDef]
     namespace: str
     name: str
     alarms: MetricAlarmsCollection
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.pyi` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,18 @@
     StandardUnitType,
     StateValueType,
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
+    DimensionOutputTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -263,24 +265,24 @@
     state_reason: str
     state_reason_data: str
     state_updated_timestamp: datetime
     metric_name: str
     namespace: str
     statistic: StatisticType
     extended_statistic: str
-    dimensions: List[DimensionTypeDef]
+    dimensions: List[DimensionOutputTypeDef]
     period: int
     unit: StandardUnitType
     evaluation_periods: int
     datapoints_to_alarm: int
     threshold: float
     comparison_operator: ComparisonOperatorType
     treat_missing_data: str
     evaluate_low_sample_count_percentile: str
-    metrics: List[MetricDataQueryTypeDef]
+    metrics: List[MetricDataQueryOutputTypeDef]
     threshold_metric_id: str
     evaluation_state: Literal["PARTIAL_DATA"]
     state_transitioned_timestamp: datetime
     name: str
     metric: "Metric"
 
     def delete(self) -> None:
@@ -359,15 +361,15 @@
 class Metric(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Metric)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/service_resource/#metric)
     """
 
     metric_name: str
-    dimensions: List[DimensionTypeDef]
+    dimensions: List[DimensionOutputTypeDef]
     namespace: str
     name: str
     alarms: MetricAlarmsCollection
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,23 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
+    "RangeOutputTypeDef",
     "RangeTypeDef",
-    "DimensionTypeDef",
+    "DimensionOutputTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
+    "DimensionTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
@@ -70,82 +72,92 @@
     "GetDashboardInputRequestTypeDef",
     "GetDashboardOutputTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
-    "MetricStreamFilterTypeDef",
+    "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
     "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
     "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ManagedRuleStateTypeDef",
+    "TagTypeDef",
     "StatisticSetTypeDef",
+    "MetricStreamFilterTypeDef",
+    "MetricStreamStatisticsMetricOutputTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
     "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
     "PutMetricStreamOutputTypeDef",
     "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "DescribeAlarmHistoryOutputTypeDef",
+    "AnomalyDetectorConfigurationOutputTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
+    "MetricOutputTypeDef",
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
     "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
     "MetricTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
     "DeleteInsightRulesOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
     "EnableInsightRulesOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
     "ListMetricStreamsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "ManagedRuleDescriptionTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
+    "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
-    "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
+    "PutManagedInsightRulesInputRequestTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
     "PutMetricStreamInputRequestTypeDef",
+    "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
+    "MetricAlarmTypeDef",
+    "MetricMathAnomalyDetectorOutputTypeDef",
     "GetMetricDataInputGetMetricDataPaginateTypeDef",
     "GetMetricDataInputRequestTypeDef",
-    "MetricAlarmTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
     "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
     "AnomalyDetectorTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
@@ -162,24 +174,32 @@
         "HistoryItemType": HistoryItemTypeType,
         "HistorySummary": str,
         "HistoryData": str,
     },
     total=False,
 )
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
+RangeOutputTypeDef = TypedDict(
+    "RangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
-DimensionTypeDef = TypedDict(
-    "DimensionTypeDef",
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+
+DimensionOutputTypeDef = TypedDict(
+    "DimensionOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 CompositeAlarmTypeDef = TypedDict(
@@ -246,14 +266,22 @@
 DeleteAlarmsInputRequestTypeDef = TypedDict(
     "DeleteAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
+DimensionTypeDef = TypedDict(
+    "DimensionTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 DeleteDashboardsInputRequestTypeDef = TypedDict(
     "DeleteDashboardsInputRequestTypeDef",
     {
         "DashboardNames": Sequence[str],
     },
 )
 
@@ -541,16 +569,16 @@
 GetMetricStreamInputRequestTypeDef = TypedDict(
     "GetMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-MetricStreamFilterTypeDef = TypedDict(
-    "MetricStreamFilterTypeDef",
+MetricStreamFilterOutputTypeDef = TypedDict(
+    "MetricStreamFilterOutputTypeDef",
     {
         "Namespace": str,
         "MetricNames": List[str],
     },
     total=False,
 )
 
@@ -659,40 +687,65 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ManagedRuleStateTypeDef = TypedDict(
     "ManagedRuleStateTypeDef",
     {
         "RuleName": str,
         "State": str,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 StatisticSetTypeDef = TypedDict(
     "StatisticSetTypeDef",
     {
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
 )
 
+MetricStreamFilterTypeDef = TypedDict(
+    "MetricStreamFilterTypeDef",
+    {
+        "Namespace": str,
+        "MetricNames": Sequence[str],
+    },
+    total=False,
+)
+
+MetricStreamStatisticsMetricOutputTypeDef = TypedDict(
+    "MetricStreamStatisticsMetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+    },
+)
+
 MetricStreamStatisticsMetricTypeDef = TypedDict(
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -806,23 +859,79 @@
     {
         "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationOutputTypeDef",
+    {
+        "ExcludedTimeRanges": List[RangeOutputTypeDef],
+        "MetricTimezone": str,
+    },
+    total=False,
+)
+
 AnomalyDetectorConfigurationTypeDef = TypedDict(
     "AnomalyDetectorConfigurationTypeDef",
     {
-        "ExcludedTimeRanges": List[RangeTypeDef],
+        "ExcludedTimeRanges": Sequence[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
+MetricOutputTypeDef = TypedDict(
+    "MetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionOutputTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
+    {
+        "DashboardEntries": List[DashboardEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
+    {
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetMetricStatisticsOutputTypeDef = TypedDict(
+    "GetMetricStatisticsOutputTypeDef",
+    {
+        "Label": str,
+        "Datapoints": List[DatapointTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
     },
 )
@@ -943,40 +1052,14 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
     },
     total=False,
 )
 
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
-    {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
-    {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMetricStatisticsOutputTypeDef = TypedDict(
-    "GetMetricStatisticsOutputTypeDef",
-    {
-        "Label": str,
-        "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInsightRulesOutputTypeDef = TypedDict(
     "DeleteInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1106,19 +1189,29 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ManagedRuleDescriptionTypeDef = TypedDict(
+    "ManagedRuleDescriptionTypeDef",
+    {
+        "TemplateName": str,
+        "ResourceARN": str,
+        "RuleState": ManagedRuleStateTypeDef,
+    },
+    total=False,
+)
+
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
         "ResourceARN": str,
     },
 )
@@ -1192,24 +1285,14 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ManagedRuleDescriptionTypeDef = TypedDict(
-    "ManagedRuleDescriptionTypeDef",
-    {
-        "TemplateName": str,
-        "ResourceARN": str,
-        "RuleState": ManagedRuleStateTypeDef,
-    },
-    total=False,
-)
-
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
@@ -1228,32 +1311,61 @@
 )
 
 
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
 
+MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
+    {
+        "IncludeMetrics": List[MetricStreamStatisticsMetricOutputTypeDef],
+        "AdditionalStatistics": List[str],
+    },
+)
+
 MetricStreamStatisticsConfigurationTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationTypeDef",
     {
-        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
-        "AdditionalStatistics": List[str],
+        "IncludeMetrics": Sequence[MetricStreamStatisticsMetricTypeDef],
+        "AdditionalStatistics": Sequence[str],
     },
 )
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
-        "Metrics": List[MetricTypeDef],
+        "Metrics": List[MetricOutputTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Period": int,
+        "Stat": str,
+    },
+)
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
+    {
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
+
+
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Period": int,
         "Stat": str,
     },
@@ -1290,52 +1402,52 @@
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutManagedInsightRulesInputRequestTypeDef = TypedDict(
-    "PutManagedInsightRulesInputRequestTypeDef",
-    {
-        "ManagedRules": Sequence[ManagedRuleTypeDef],
-    },
-)
-
 ListManagedInsightRulesOutputTypeDef = TypedDict(
     "ListManagedInsightRulesOutputTypeDef",
     {
         "ManagedRules": List[ManagedRuleDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutManagedInsightRulesInputRequestTypeDef = TypedDict(
+    "PutManagedInsightRulesInputRequestTypeDef",
+    {
+        "ManagedRules": Sequence[ManagedRuleTypeDef],
+    },
+)
+
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricData": Sequence[MetricDatumTypeDef],
     },
 )
 
 GetMetricStreamOutputTypeDef = TypedDict(
     "GetMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
-        "IncludeFilters": List[MetricStreamFilterTypeDef],
-        "ExcludeFilters": List[MetricStreamFilterTypeDef],
+        "IncludeFilters": List[MetricStreamFilterOutputTypeDef],
+        "ExcludeFilters": List[MetricStreamFilterOutputTypeDef],
         "FirehoseArn": str,
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
-        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
+        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricStreamInputRequestTypeDef",
@@ -1361,14 +1473,40 @@
 
 class PutMetricStreamInputRequestTypeDef(
     _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
 ):
     pass
 
 
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
+    {
+        "MetricStat": MetricStatOutputTypeDef,
+        "Expression": str,
+        "Label": str,
+        "ReturnData": bool,
+        "Period": int,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+):
+    pass
+
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -1385,14 +1523,58 @@
 )
 
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
 
+MetricAlarmTypeDef = TypedDict(
+    "MetricAlarmTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmArn": str,
+        "AlarmDescription": str,
+        "AlarmConfigurationUpdatedTimestamp": datetime,
+        "ActionsEnabled": bool,
+        "OKActions": List[str],
+        "AlarmActions": List[str],
+        "InsufficientDataActions": List[str],
+        "StateValue": StateValueType,
+        "StateReason": str,
+        "StateReasonData": str,
+        "StateUpdatedTimestamp": datetime,
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": StatisticType,
+        "ExtendedStatistic": str,
+        "Dimensions": List[DimensionOutputTypeDef],
+        "Period": int,
+        "Unit": StandardUnitType,
+        "EvaluationPeriods": int,
+        "DatapointsToAlarm": int,
+        "Threshold": float,
+        "ComparisonOperator": ComparisonOperatorType,
+        "TreatMissingData": str,
+        "EvaluateLowSampleCountPercentile": str,
+        "Metrics": List[MetricDataQueryOutputTypeDef],
+        "ThresholdMetricId": str,
+        "EvaluationState": Literal["PARTIAL_DATA"],
+        "StateTransitionedTimestamp": datetime,
+    },
+    total=False,
+)
+
+MetricMathAnomalyDetectorOutputTypeDef = TypedDict(
+    "MetricMathAnomalyDetectorOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
     "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
@@ -1437,50 +1619,14 @@
 
 class GetMetricDataInputRequestTypeDef(
     _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
 ):
     pass
 
 
-MetricAlarmTypeDef = TypedDict(
-    "MetricAlarmTypeDef",
-    {
-        "AlarmName": str,
-        "AlarmArn": str,
-        "AlarmDescription": str,
-        "AlarmConfigurationUpdatedTimestamp": datetime,
-        "ActionsEnabled": bool,
-        "OKActions": List[str],
-        "AlarmActions": List[str],
-        "InsufficientDataActions": List[str],
-        "StateValue": StateValueType,
-        "StateReason": str,
-        "StateReasonData": str,
-        "StateUpdatedTimestamp": datetime,
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": StatisticType,
-        "ExtendedStatistic": str,
-        "Dimensions": List[DimensionTypeDef],
-        "Period": int,
-        "Unit": StandardUnitType,
-        "EvaluationPeriods": int,
-        "DatapointsToAlarm": int,
-        "Threshold": float,
-        "ComparisonOperator": ComparisonOperatorType,
-        "TreatMissingData": str,
-        "EvaluateLowSampleCountPercentile": str,
-        "Metrics": List[MetricDataQueryTypeDef],
-        "ThresholdMetricId": str,
-        "EvaluationState": Literal["PARTIAL_DATA"],
-        "StateTransitionedTimestamp": datetime,
-    },
-    total=False,
-)
-
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1585,20 +1731,20 @@
 )
 
 AnomalyDetectorTypeDef = TypedDict(
     "AnomalyDetectorTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
+        "Dimensions": List[DimensionOutputTypeDef],
         "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationTypeDef,
+        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
         "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
     },
     total=False,
 )
 
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.pyi` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,23 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
+    "RangeOutputTypeDef",
     "RangeTypeDef",
-    "DimensionTypeDef",
+    "DimensionOutputTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
+    "DimensionTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
@@ -69,82 +71,92 @@
     "GetDashboardInputRequestTypeDef",
     "GetDashboardOutputTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
-    "MetricStreamFilterTypeDef",
+    "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
     "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
     "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ManagedRuleStateTypeDef",
+    "TagTypeDef",
     "StatisticSetTypeDef",
+    "MetricStreamFilterTypeDef",
+    "MetricStreamStatisticsMetricOutputTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
     "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
     "PutMetricStreamOutputTypeDef",
     "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "DescribeAlarmHistoryOutputTypeDef",
+    "AnomalyDetectorConfigurationOutputTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
+    "MetricOutputTypeDef",
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
     "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
     "MetricTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
     "DeleteInsightRulesOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
     "EnableInsightRulesOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
     "ListMetricStreamsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "ManagedRuleDescriptionTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
+    "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
-    "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
+    "PutManagedInsightRulesInputRequestTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
     "PutMetricStreamInputRequestTypeDef",
+    "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
+    "MetricAlarmTypeDef",
+    "MetricMathAnomalyDetectorOutputTypeDef",
     "GetMetricDataInputGetMetricDataPaginateTypeDef",
     "GetMetricDataInputRequestTypeDef",
-    "MetricAlarmTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
     "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
     "AnomalyDetectorTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
@@ -161,24 +173,32 @@
         "HistoryItemType": HistoryItemTypeType,
         "HistorySummary": str,
         "HistoryData": str,
     },
     total=False,
 )
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
+RangeOutputTypeDef = TypedDict(
+    "RangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
-DimensionTypeDef = TypedDict(
-    "DimensionTypeDef",
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+
+DimensionOutputTypeDef = TypedDict(
+    "DimensionOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 CompositeAlarmTypeDef = TypedDict(
@@ -245,14 +265,22 @@
 DeleteAlarmsInputRequestTypeDef = TypedDict(
     "DeleteAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
+DimensionTypeDef = TypedDict(
+    "DimensionTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 DeleteDashboardsInputRequestTypeDef = TypedDict(
     "DeleteDashboardsInputRequestTypeDef",
     {
         "DashboardNames": Sequence[str],
     },
 )
 
@@ -532,16 +560,16 @@
 GetMetricStreamInputRequestTypeDef = TypedDict(
     "GetMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-MetricStreamFilterTypeDef = TypedDict(
-    "MetricStreamFilterTypeDef",
+MetricStreamFilterOutputTypeDef = TypedDict(
+    "MetricStreamFilterOutputTypeDef",
     {
         "Namespace": str,
         "MetricNames": List[str],
     },
     total=False,
 )
 
@@ -646,40 +674,65 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ManagedRuleStateTypeDef = TypedDict(
     "ManagedRuleStateTypeDef",
     {
         "RuleName": str,
         "State": str,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 StatisticSetTypeDef = TypedDict(
     "StatisticSetTypeDef",
     {
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
 )
 
+MetricStreamFilterTypeDef = TypedDict(
+    "MetricStreamFilterTypeDef",
+    {
+        "Namespace": str,
+        "MetricNames": Sequence[str],
+    },
+    total=False,
+)
+
+MetricStreamStatisticsMetricOutputTypeDef = TypedDict(
+    "MetricStreamStatisticsMetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+    },
+)
+
 MetricStreamStatisticsMetricTypeDef = TypedDict(
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -789,23 +842,79 @@
     {
         "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationOutputTypeDef",
+    {
+        "ExcludedTimeRanges": List[RangeOutputTypeDef],
+        "MetricTimezone": str,
+    },
+    total=False,
+)
+
 AnomalyDetectorConfigurationTypeDef = TypedDict(
     "AnomalyDetectorConfigurationTypeDef",
     {
-        "ExcludedTimeRanges": List[RangeTypeDef],
+        "ExcludedTimeRanges": Sequence[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
+MetricOutputTypeDef = TypedDict(
+    "MetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionOutputTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
+    {
+        "DashboardEntries": List[DashboardEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
+    {
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetMetricStatisticsOutputTypeDef = TypedDict(
+    "GetMetricStatisticsOutputTypeDef",
+    {
+        "Label": str,
+        "Datapoints": List[DatapointTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
     },
 )
@@ -920,40 +1029,14 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
     },
     total=False,
 )
 
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
-    {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
-    {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMetricStatisticsOutputTypeDef = TypedDict(
-    "GetMetricStatisticsOutputTypeDef",
-    {
-        "Label": str,
-        "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInsightRulesOutputTypeDef = TypedDict(
     "DeleteInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1083,19 +1166,29 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ManagedRuleDescriptionTypeDef = TypedDict(
+    "ManagedRuleDescriptionTypeDef",
+    {
+        "TemplateName": str,
+        "ResourceARN": str,
+        "RuleState": ManagedRuleStateTypeDef,
+    },
+    total=False,
+)
+
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
         "ResourceARN": str,
     },
 )
@@ -1163,24 +1256,14 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ManagedRuleDescriptionTypeDef = TypedDict(
-    "ManagedRuleDescriptionTypeDef",
-    {
-        "TemplateName": str,
-        "ResourceARN": str,
-        "RuleState": ManagedRuleStateTypeDef,
-    },
-    total=False,
-)
-
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
@@ -1197,32 +1280,59 @@
     },
     total=False,
 )
 
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
+MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
+    {
+        "IncludeMetrics": List[MetricStreamStatisticsMetricOutputTypeDef],
+        "AdditionalStatistics": List[str],
+    },
+)
+
 MetricStreamStatisticsConfigurationTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationTypeDef",
     {
-        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
-        "AdditionalStatistics": List[str],
+        "IncludeMetrics": Sequence[MetricStreamStatisticsMetricTypeDef],
+        "AdditionalStatistics": Sequence[str],
     },
 )
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
-        "Metrics": List[MetricTypeDef],
+        "Metrics": List[MetricOutputTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Period": int,
+        "Stat": str,
+    },
+)
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
+    {
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
+
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Period": int,
         "Stat": str,
     },
@@ -1257,52 +1367,52 @@
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutManagedInsightRulesInputRequestTypeDef = TypedDict(
-    "PutManagedInsightRulesInputRequestTypeDef",
-    {
-        "ManagedRules": Sequence[ManagedRuleTypeDef],
-    },
-)
-
 ListManagedInsightRulesOutputTypeDef = TypedDict(
     "ListManagedInsightRulesOutputTypeDef",
     {
         "ManagedRules": List[ManagedRuleDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutManagedInsightRulesInputRequestTypeDef = TypedDict(
+    "PutManagedInsightRulesInputRequestTypeDef",
+    {
+        "ManagedRules": Sequence[ManagedRuleTypeDef],
+    },
+)
+
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricData": Sequence[MetricDatumTypeDef],
     },
 )
 
 GetMetricStreamOutputTypeDef = TypedDict(
     "GetMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
-        "IncludeFilters": List[MetricStreamFilterTypeDef],
-        "ExcludeFilters": List[MetricStreamFilterTypeDef],
+        "IncludeFilters": List[MetricStreamFilterOutputTypeDef],
+        "ExcludeFilters": List[MetricStreamFilterOutputTypeDef],
         "FirehoseArn": str,
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
-        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
+        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricStreamInputRequestTypeDef",
@@ -1326,14 +1436,38 @@
 )
 
 class PutMetricStreamInputRequestTypeDef(
     _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
 ):
     pass
 
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
+    {
+        "MetricStat": MetricStatOutputTypeDef,
+        "Expression": str,
+        "Label": str,
+        "ReturnData": bool,
+        "Period": int,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+):
+    pass
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -1348,14 +1482,58 @@
     },
     total=False,
 )
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
+MetricAlarmTypeDef = TypedDict(
+    "MetricAlarmTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmArn": str,
+        "AlarmDescription": str,
+        "AlarmConfigurationUpdatedTimestamp": datetime,
+        "ActionsEnabled": bool,
+        "OKActions": List[str],
+        "AlarmActions": List[str],
+        "InsufficientDataActions": List[str],
+        "StateValue": StateValueType,
+        "StateReason": str,
+        "StateReasonData": str,
+        "StateUpdatedTimestamp": datetime,
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": StatisticType,
+        "ExtendedStatistic": str,
+        "Dimensions": List[DimensionOutputTypeDef],
+        "Period": int,
+        "Unit": StandardUnitType,
+        "EvaluationPeriods": int,
+        "DatapointsToAlarm": int,
+        "Threshold": float,
+        "ComparisonOperator": ComparisonOperatorType,
+        "TreatMissingData": str,
+        "EvaluateLowSampleCountPercentile": str,
+        "Metrics": List[MetricDataQueryOutputTypeDef],
+        "ThresholdMetricId": str,
+        "EvaluationState": Literal["PARTIAL_DATA"],
+        "StateTransitionedTimestamp": datetime,
+    },
+    total=False,
+)
+
+MetricMathAnomalyDetectorOutputTypeDef = TypedDict(
+    "MetricMathAnomalyDetectorOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
     "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
@@ -1396,50 +1574,14 @@
 )
 
 class GetMetricDataInputRequestTypeDef(
     _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
 ):
     pass
 
-MetricAlarmTypeDef = TypedDict(
-    "MetricAlarmTypeDef",
-    {
-        "AlarmName": str,
-        "AlarmArn": str,
-        "AlarmDescription": str,
-        "AlarmConfigurationUpdatedTimestamp": datetime,
-        "ActionsEnabled": bool,
-        "OKActions": List[str],
-        "AlarmActions": List[str],
-        "InsufficientDataActions": List[str],
-        "StateValue": StateValueType,
-        "StateReason": str,
-        "StateReasonData": str,
-        "StateUpdatedTimestamp": datetime,
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": StatisticType,
-        "ExtendedStatistic": str,
-        "Dimensions": List[DimensionTypeDef],
-        "Period": int,
-        "Unit": StandardUnitType,
-        "EvaluationPeriods": int,
-        "DatapointsToAlarm": int,
-        "Threshold": float,
-        "ComparisonOperator": ComparisonOperatorType,
-        "TreatMissingData": str,
-        "EvaluateLowSampleCountPercentile": str,
-        "Metrics": List[MetricDataQueryTypeDef],
-        "ThresholdMetricId": str,
-        "EvaluationState": Literal["PARTIAL_DATA"],
-        "StateTransitionedTimestamp": datetime,
-    },
-    total=False,
-)
-
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1540,20 +1682,20 @@
 )
 
 AnomalyDetectorTypeDef = TypedDict(
     "AnomalyDetectorTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
+        "Dimensions": List[DimensionOutputTypeDef],
         "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationTypeDef,
+        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
         "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
     },
     total=False,
 )
 
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.py` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.pyi` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatch 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatch 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudwatch"></a>
 
 # mypy-boto3-cloudwatch
 
 [![PyPI - mypy-boto3-cloudwatch](https://img.shields.io/pypi/v/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -446,21 +446,23 @@
 
 `mypy_boto3_cloudwatch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
+    RangeOutputTypeDef,
     RangeTypeDef,
-    DimensionTypeDef,
+    DimensionOutputTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
+    DimensionTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
     DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
@@ -478,82 +480,92 @@
     GetDashboardInputRequestTypeDef,
     GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
-    MetricStreamFilterTypeDef,
+    MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
     GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
     ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ManagedRuleStateTypeDef,
+    TagTypeDef,
     StatisticSetTypeDef,
+    MetricStreamFilterTypeDef,
+    MetricStreamStatisticsMetricOutputTypeDef,
     MetricStreamStatisticsMetricTypeDef,
     PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
     PutMetricStreamOutputTypeDef,
     ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
+    AnomalyDetectorConfigurationOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
+    MetricOutputTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
     DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
     EnableInsightRulesOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    ManagedRuleDescriptionTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
+    MetricStatOutputTypeDef,
     MetricStatTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
-    PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
+    PutManagedInsightRulesInputRequestTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
     PutMetricStreamInputRequestTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
+    MetricAlarmTypeDef,
+    MetricMathAnomalyDetectorOutputTypeDef,
     GetMetricDataInputGetMetricDataPaginateTypeDef,
     GetMetricDataInputRequestTypeDef,
-    MetricAlarmTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
     PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt` & `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.0/setup.py` & `mypy-boto3-cloudwatch-1.28.12/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudwatch",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatch 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudWatch 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

