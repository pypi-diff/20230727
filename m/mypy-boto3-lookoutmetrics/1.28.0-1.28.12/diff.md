# Comparing `tmp/mypy-boto3-lookoutmetrics-1.28.0.tar.gz` & `tmp/mypy-boto3-lookoutmetrics-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.0.tar", last modified: Thu Jul  6 21:00:01 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
```

## Comparing `mypy-boto3-lookoutmetrics-1.28.0.tar` & `mypy-boto3-lookoutmetrics-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.322358 mypy-boto3-lookoutmetrics-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-06 21:00:01.322358 mypy-boto3-lookoutmetrics-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.310357 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-07-06 20:46:13.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36547 2023-07-06 20:46:14.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36514 2023-07-06 20:46:13.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.322358 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-06 21:00:01.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 21:00:01.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:01.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:01.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:01.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:01.000000 mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:01.322358 mypy-boto3-lookoutmetrics-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:46:12.000000 mypy-boto3-lookoutmetrics-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.888453 mypy-boto3-lookoutmetrics-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-27 05:34:57.884453 mypy-boto3-lookoutmetrics-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.884453 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42825 2023-07-27 05:25:38.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42788 2023-07-27 05:25:38.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.884453 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.888453 mypy-boto3-lookoutmetrics-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/setup.py
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/LICENSE` & `mypy-boto3-lookoutmetrics-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.12/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.28.0
-Summary: Type annotations for boto3.LookoutMetrics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LookoutMetrics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lookoutmetrics"></a>
 
 # mypy-boto3-lookoutmetrics
 
 [![PyPI - mypy-boto3-lookoutmetrics](https://img.shields.io/pypi/v/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutmetrics?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutmetrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,49 +311,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
+    LambdaConfigurationOutputTypeDef,
+    SNSConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
+    DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
+    AppFlowConfigOutputTypeDef,
     AppFlowConfigTypeDef,
+    BackTestConfigurationOutputTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
     CreateMetricSetResponseTypeDef,
+    CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     ExecutionStatusTypeDef,
     DescribeAnomalyDetectorRequestRequestTypeDef,
     DescribeMetricSetRequestRequestTypeDef,
+    MetricOutputTypeDef,
+    TimestampColumnOutputTypeDef,
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
+    JsonFormatDescriptorOutputTypeDef,
     JsonFormatDescriptorTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
     GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
@@ -361,77 +371,88 @@
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
     ListAlertsResponseTypeDef,
     DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
+    AthenaSourceConfigOutputTypeDef,
+    CloudWatchConfigOutputTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
+    FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
+    RDSSourceConfigOutputTypeDef,
+    RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
+    S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
-    CreateMetricSetRequestRequestTypeDef,
     DescribeMetricSetResponseTypeDef,
+    CreateMetricSetRequestRequestTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_structure() -> LambdaConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/README.md` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-lookoutmetrics
+Version: 1.28.12
+Summary: Type annotations for boto3.LookoutMetrics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-lookoutmetrics"></a>
 
 # mypy-boto3-lookoutmetrics
 
 [![PyPI - mypy-boto3-lookoutmetrics](https://img.shields.io/pypi/v/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutmetrics?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutmetrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,49 +311,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
+    LambdaConfigurationOutputTypeDef,
+    SNSConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
+    DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
+    AppFlowConfigOutputTypeDef,
     AppFlowConfigTypeDef,
+    BackTestConfigurationOutputTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
     CreateMetricSetResponseTypeDef,
+    CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     ExecutionStatusTypeDef,
     DescribeAnomalyDetectorRequestRequestTypeDef,
     DescribeMetricSetRequestRequestTypeDef,
+    MetricOutputTypeDef,
+    TimestampColumnOutputTypeDef,
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
+    JsonFormatDescriptorOutputTypeDef,
     JsonFormatDescriptorTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
     GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
@@ -329,77 +371,88 @@
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
     ListAlertsResponseTypeDef,
     DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
+    AthenaSourceConfigOutputTypeDef,
+    CloudWatchConfigOutputTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
+    FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
+    RDSSourceConfigOutputTypeDef,
+    RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
+    S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
-    CreateMetricSetRequestRequestTypeDef,
     DescribeMetricSetResponseTypeDef,
+    CreateMetricSetRequestRequestTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_structure() -> LambdaConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/__main__.py` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutMetrics 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LookoutMetrics 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/client.py` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/client.pyi` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/literals.py` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.pyi`

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
     "AggregationFunctionType",
     "AlertStatusType",
     "AlertTypeType",
     "AnomalyDetectionTaskStatusType",
     "AnomalyDetectorFailureTypeType",
     "AnomalyDetectorStatusType",
@@ -36,15 +35,14 @@
     "SnsFormatType",
     "LookoutMetricsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AggregationFunctionType = Literal["AVG", "SUM"]
 AlertStatusType = Literal["ACTIVE", "INACTIVE"]
 AlertTypeType = Literal["LAMBDA", "SNS"]
 AnomalyDetectionTaskStatusType = Literal[
     "COMPLETED", "FAILED", "FAILED_TO_SCHEDULE", "IN_PROGRESS", "PENDING"
 ]
 AnomalyDetectorFailureTypeType = Literal[
@@ -198,14 +196,15 @@
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
@@ -284,26 +283,28 @@
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

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/literals.pyi` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.py`

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
     "AggregationFunctionType",
     "AlertStatusType",
     "AlertTypeType",
     "AnomalyDetectionTaskStatusType",
     "AnomalyDetectorFailureTypeType",
     "AnomalyDetectorStatusType",
@@ -35,14 +36,15 @@
     "SnsFormatType",
     "LookoutMetricsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AggregationFunctionType = Literal["AVG", "SUM"]
 AlertStatusType = Literal["ACTIVE", "INACTIVE"]
 AlertTypeType = Literal["LAMBDA", "SNS"]
 AnomalyDetectionTaskStatusType = Literal[
     "COMPLETED", "FAILED", "FAILED_TO_SCHEDULE", "IN_PROGRESS", "PENDING"
 ]
 AnomalyDetectorFailureTypeType = Literal[
@@ -196,14 +198,15 @@
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
@@ -282,26 +285,28 @@
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

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/type_defs.py` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lookoutmetrics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
+    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationOutputTypeDef
 
-    data: LambdaConfigurationTypeDef = {...}
+    data: LambdaConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -38,49 +38,59 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "LambdaConfigurationOutputTypeDef",
+    "SNSConfigurationOutputTypeDef",
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
+    "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
+    "AppFlowConfigOutputTypeDef",
     "AppFlowConfigTypeDef",
+    "BackTestConfigurationOutputTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     "CreateAlertResponseTypeDef",
     "CreateAnomalyDetectorResponseTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
     "CreateMetricSetResponseTypeDef",
+    "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
     "ExecutionStatusTypeDef",
     "DescribeAnomalyDetectorRequestRequestTypeDef",
     "DescribeMetricSetRequestRequestTypeDef",
+    "MetricOutputTypeDef",
+    "TimestampColumnOutputTypeDef",
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
+    "JsonFormatDescriptorOutputTypeDef",
     "JsonFormatDescriptorTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
     "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
@@ -88,75 +98,116 @@
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAlertResponseTypeDef",
     "UpdateAnomalyDetectorResponseTypeDef",
     "UpdateMetricSetResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
     "ListAlertsResponseTypeDef",
     "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
     "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
+    "AthenaSourceConfigOutputTypeDef",
+    "CloudWatchConfigOutputTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
+    "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
+    "MetricSetDimensionFilterOutputTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
+    "RDSSourceConfigOutputTypeDef",
+    "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
+    "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
+    "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
-    "CreateMetricSetRequestRequestTypeDef",
     "DescribeMetricSetResponseTypeDef",
+    "CreateMetricSetRequestRequestTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
+LambdaConfigurationOutputTypeDef = TypedDict(
+    "LambdaConfigurationOutputTypeDef",
+    {
+        "RoleArn": str,
+        "LambdaArn": str,
+    },
+)
+
+_RequiredSNSConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSNSConfigurationOutputTypeDef",
+    {
+        "RoleArn": str,
+        "SnsTopicArn": str,
+    },
+)
+_OptionalSNSConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSNSConfigurationOutputTypeDef",
+    {
+        "SnsFormat": SnsFormatType,
+    },
+    total=False,
+)
+
+
+class SNSConfigurationOutputTypeDef(
+    _RequiredSNSConfigurationOutputTypeDef, _OptionalSNSConfigurationOutputTypeDef
+):
+    pass
+
+
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "RoleArn": str,
         "LambdaArn": str,
     },
 )
@@ -184,14 +235,23 @@
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
+DimensionFilterOutputTypeDef = TypedDict(
+    "DimensionFilterOutputTypeDef",
+    {
+        "DimensionName": str,
+        "DimensionValueList": List[str],
+    },
+    total=False,
+)
+
 DimensionFilterTypeDef = TypedDict(
     "DimensionFilterTypeDef",
     {
         "DimensionName": str,
         "DimensionValueList": Sequence[str],
     },
     total=False,
@@ -290,23 +350,39 @@
 
 class AnomalyGroupTimeSeriesTypeDef(
     _RequiredAnomalyGroupTimeSeriesTypeDef, _OptionalAnomalyGroupTimeSeriesTypeDef
 ):
     pass
 
 
+AppFlowConfigOutputTypeDef = TypedDict(
+    "AppFlowConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "FlowName": str,
+    },
+    total=False,
+)
+
 AppFlowConfigTypeDef = TypedDict(
     "AppFlowConfigTypeDef",
     {
         "RoleArn": str,
         "FlowName": str,
     },
     total=False,
 )
 
+BackTestConfigurationOutputTypeDef = TypedDict(
+    "BackTestConfigurationOutputTypeDef",
+    {
+        "RunBackTestMode": bool,
+    },
+)
+
 BackTestConfigurationTypeDef = TypedDict(
     "BackTestConfigurationTypeDef",
     {
         "RunBackTestMode": bool,
     },
 )
 
@@ -388,14 +464,27 @@
     "CreateMetricSetResponseTypeDef",
     {
         "MetricSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CsvFormatDescriptorOutputTypeDef = TypedDict(
+    "CsvFormatDescriptorOutputTypeDef",
+    {
+        "FileCompression": CSVFileCompressionType,
+        "Charset": str,
+        "ContainsHeader": bool,
+        "Delimiter": str,
+        "HeaderList": List[str],
+        "QuoteSymbol": str,
+    },
+    total=False,
+)
+
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -488,14 +577,43 @@
 DescribeMetricSetRequestRequestTypeDef = TypedDict(
     "DescribeMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "MetricName": str,
+        "AggregationFunction": AggregationFunctionType,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "Namespace": str,
+    },
+    total=False,
+)
+
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
+
+TimestampColumnOutputTypeDef = TypedDict(
+    "TimestampColumnOutputTypeDef",
+    {
+        "ColumnName": str,
+        "ColumnFormat": str,
+    },
+    total=False,
+)
+
 DimensionValueContributionTypeDef = TypedDict(
     "DimensionValueContributionTypeDef",
     {
         "DimensionValue": str,
         "ContributionScore": float,
     },
     total=False,
@@ -505,23 +623,41 @@
     "DimensionNameValueTypeDef",
     {
         "DimensionName": str,
         "DimensionValue": str,
     },
 )
 
+JsonFormatDescriptorOutputTypeDef = TypedDict(
+    "JsonFormatDescriptorOutputTypeDef",
+    {
+        "FileCompression": JsonFileCompressionType,
+        "Charset": str,
+    },
+    total=False,
+)
+
 JsonFormatDescriptorTypeDef = TypedDict(
     "JsonFormatDescriptorTypeDef",
     {
         "FileCompression": JsonFileCompressionType,
         "Charset": str,
     },
     total=False,
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "DimensionValue": str,
+        "FilterOperation": Literal["EQUALS"],
+    },
+    total=False,
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "DimensionValue": str,
         "FilterOperation": Literal["EQUALS"],
     },
     total=False,
@@ -714,14 +850,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "SubnetIdList": List[str],
+        "SecurityGroupIdList": List[str],
+    },
+)
+
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
     },
 )
@@ -773,23 +917,41 @@
     "UpdateMetricSetResponseTypeDef",
     {
         "MetricSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "SNSConfiguration": SNSConfigurationOutputTypeDef,
+        "LambdaConfiguration": LambdaConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
 )
 
+AlertFiltersOutputTypeDef = TypedDict(
+    "AlertFiltersOutputTypeDef",
+    {
+        "MetricList": List[str],
+        "DimensionFilterList": List[DimensionFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 AlertFiltersTypeDef = TypedDict(
     "AlertFiltersTypeDef",
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
@@ -916,14 +1078,37 @@
 
 class GetFeedbackRequestRequestTypeDef(
     _RequiredGetFeedbackRequestRequestTypeDef, _OptionalGetFeedbackRequestRequestTypeDef
 ):
     pass
 
 
+AthenaSourceConfigOutputTypeDef = TypedDict(
+    "AthenaSourceConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "DatabaseName": str,
+        "DataCatalog": str,
+        "TableName": str,
+        "WorkGroupName": str,
+        "S3ResultsPath": str,
+        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+CloudWatchConfigOutputTypeDef = TypedDict(
+    "CloudWatchConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AthenaSourceConfigTypeDef = TypedDict(
     "AthenaSourceConfigTypeDef",
     {
         "RoleArn": str,
         "DatabaseName": str,
         "DataCatalog": str,
         "TableName": str,
@@ -993,23 +1178,41 @@
     {
         "TimeSeriesId": str,
         "DimensionList": List[DimensionNameValueTypeDef],
         "MetricValueList": List[float],
     },
 )
 
+FileFormatDescriptorOutputTypeDef = TypedDict(
+    "FileFormatDescriptorOutputTypeDef",
+    {
+        "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
+        "JsonFormatDescriptor": JsonFormatDescriptorOutputTypeDef,
+    },
+    total=False,
+)
+
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorTypeDef,
         "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
+MetricSetDimensionFilterOutputTypeDef = TypedDict(
+    "MetricSetDimensionFilterOutputTypeDef",
+    {
+        "Name": str,
+        "FilterList": List[FilterOutputTypeDef],
+    },
+    total=False,
+)
+
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
         "Name": str,
         "FilterList": Sequence[FilterTypeDef],
     },
     total=False,
@@ -1038,14 +1241,44 @@
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RDSSourceConfigOutputTypeDef = TypedDict(
+    "RDSSourceConfigOutputTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+RedshiftSourceConfigOutputTypeDef = TypedDict(
+    "RedshiftSourceConfigOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DatabaseHost": str,
         "DatabasePort": int,
         "SecretManagerArn": str,
@@ -1071,25 +1304,25 @@
     },
     total=False,
 )
 
 AlertTypeDef = TypedDict(
     "AlertTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "AlertDescription": str,
         "AlertArn": str,
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
         "LastModificationTime": datetime,
         "CreationTime": datetime,
-        "AlertFilters": AlertFiltersTypeDef,
+        "AlertFilters": AlertFiltersOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
@@ -1205,14 +1438,25 @@
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3SourceConfigOutputTypeDef = TypedDict(
+    "S3SourceConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "TemplatedPathList": List[str],
+        "HistoricalDataPathList": List[str],
+        "FileFormatDescriptor": FileFormatDescriptorOutputTypeDef,
+    },
+    total=False,
+)
+
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
         "FileFormatDescriptor": FileFormatDescriptorTypeDef,
@@ -1274,14 +1518,27 @@
         "MetricName": str,
         "NumTimeSeries": int,
         "ContributionMatrix": ContributionMatrixTypeDef,
     },
     total=False,
 )
 
+MetricSourceOutputTypeDef = TypedDict(
+    "MetricSourceOutputTypeDef",
+    {
+        "S3SourceConfig": S3SourceConfigOutputTypeDef,
+        "AppFlowConfig": AppFlowConfigOutputTypeDef,
+        "CloudWatchConfig": CloudWatchConfigOutputTypeDef,
+        "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
+        "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
+        "AthenaSourceConfig": AthenaSourceConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
         "S3SourceConfig": S3SourceConfigTypeDef,
         "AppFlowConfig": AppFlowConfigTypeDef,
         "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigTypeDef,
@@ -1316,14 +1573,35 @@
         "AnomalyGroupScore": float,
         "PrimaryMetricName": str,
         "MetricLevelImpactList": List[MetricLevelImpactTypeDef],
     },
     total=False,
 )
 
+DescribeMetricSetResponseTypeDef = TypedDict(
+    "DescribeMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "AnomalyDetectorArn": str,
+        "MetricSetName": str,
+        "MetricSetDescription": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Offset": int,
+        "MetricList": List[MetricOutputTypeDef],
+        "TimestampColumn": TimestampColumnOutputTypeDef,
+        "DimensionList": List[str],
+        "MetricSetFrequency": FrequencyType,
+        "Timezone": str,
+        "MetricSource": MetricSourceOutputTypeDef,
+        "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricList": Sequence[MetricTypeDef],
         "MetricSource": MetricSourceTypeDef,
@@ -1347,35 +1625,14 @@
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
 
-DescribeMetricSetResponseTypeDef = TypedDict(
-    "DescribeMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "AnomalyDetectorArn": str,
-        "MetricSetName": str,
-        "MetricSetDescription": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Offset": int,
-        "MetricList": List[MetricTypeDef],
-        "TimestampColumn": TimestampColumnTypeDef,
-        "DimensionList": List[str],
-        "MetricSetFrequency": FrequencyType,
-        "Timezone": str,
-        "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics/type_defs.pyi` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lookoutmetrics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
+    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationOutputTypeDef
 
-    data: LambdaConfigurationTypeDef = {...}
+    data: LambdaConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,49 +37,59 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "LambdaConfigurationOutputTypeDef",
+    "SNSConfigurationOutputTypeDef",
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
+    "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
+    "AppFlowConfigOutputTypeDef",
     "AppFlowConfigTypeDef",
+    "BackTestConfigurationOutputTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     "CreateAlertResponseTypeDef",
     "CreateAnomalyDetectorResponseTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
     "CreateMetricSetResponseTypeDef",
+    "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
     "ExecutionStatusTypeDef",
     "DescribeAnomalyDetectorRequestRequestTypeDef",
     "DescribeMetricSetRequestRequestTypeDef",
+    "MetricOutputTypeDef",
+    "TimestampColumnOutputTypeDef",
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
+    "JsonFormatDescriptorOutputTypeDef",
     "JsonFormatDescriptorTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
     "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
@@ -87,75 +97,114 @@
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAlertResponseTypeDef",
     "UpdateAnomalyDetectorResponseTypeDef",
     "UpdateMetricSetResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
     "ListAlertsResponseTypeDef",
     "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
     "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
+    "AthenaSourceConfigOutputTypeDef",
+    "CloudWatchConfigOutputTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
+    "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
+    "MetricSetDimensionFilterOutputTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
+    "RDSSourceConfigOutputTypeDef",
+    "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
+    "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
+    "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
-    "CreateMetricSetRequestRequestTypeDef",
     "DescribeMetricSetResponseTypeDef",
+    "CreateMetricSetRequestRequestTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
+LambdaConfigurationOutputTypeDef = TypedDict(
+    "LambdaConfigurationOutputTypeDef",
+    {
+        "RoleArn": str,
+        "LambdaArn": str,
+    },
+)
+
+_RequiredSNSConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSNSConfigurationOutputTypeDef",
+    {
+        "RoleArn": str,
+        "SnsTopicArn": str,
+    },
+)
+_OptionalSNSConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSNSConfigurationOutputTypeDef",
+    {
+        "SnsFormat": SnsFormatType,
+    },
+    total=False,
+)
+
+class SNSConfigurationOutputTypeDef(
+    _RequiredSNSConfigurationOutputTypeDef, _OptionalSNSConfigurationOutputTypeDef
+):
+    pass
+
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "RoleArn": str,
         "LambdaArn": str,
     },
 )
@@ -181,14 +230,23 @@
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
+DimensionFilterOutputTypeDef = TypedDict(
+    "DimensionFilterOutputTypeDef",
+    {
+        "DimensionName": str,
+        "DimensionValueList": List[str],
+    },
+    total=False,
+)
+
 DimensionFilterTypeDef = TypedDict(
     "DimensionFilterTypeDef",
     {
         "DimensionName": str,
         "DimensionValueList": Sequence[str],
     },
     total=False,
@@ -285,23 +343,39 @@
 )
 
 class AnomalyGroupTimeSeriesTypeDef(
     _RequiredAnomalyGroupTimeSeriesTypeDef, _OptionalAnomalyGroupTimeSeriesTypeDef
 ):
     pass
 
+AppFlowConfigOutputTypeDef = TypedDict(
+    "AppFlowConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "FlowName": str,
+    },
+    total=False,
+)
+
 AppFlowConfigTypeDef = TypedDict(
     "AppFlowConfigTypeDef",
     {
         "RoleArn": str,
         "FlowName": str,
     },
     total=False,
 )
 
+BackTestConfigurationOutputTypeDef = TypedDict(
+    "BackTestConfigurationOutputTypeDef",
+    {
+        "RunBackTestMode": bool,
+    },
+)
+
 BackTestConfigurationTypeDef = TypedDict(
     "BackTestConfigurationTypeDef",
     {
         "RunBackTestMode": bool,
     },
 )
 
@@ -381,14 +455,27 @@
     "CreateMetricSetResponseTypeDef",
     {
         "MetricSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CsvFormatDescriptorOutputTypeDef = TypedDict(
+    "CsvFormatDescriptorOutputTypeDef",
+    {
+        "FileCompression": CSVFileCompressionType,
+        "Charset": str,
+        "ContainsHeader": bool,
+        "Delimiter": str,
+        "HeaderList": List[str],
+        "QuoteSymbol": str,
+    },
+    total=False,
+)
+
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -479,14 +566,41 @@
 DescribeMetricSetRequestRequestTypeDef = TypedDict(
     "DescribeMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "MetricName": str,
+        "AggregationFunction": AggregationFunctionType,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "Namespace": str,
+    },
+    total=False,
+)
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
+TimestampColumnOutputTypeDef = TypedDict(
+    "TimestampColumnOutputTypeDef",
+    {
+        "ColumnName": str,
+        "ColumnFormat": str,
+    },
+    total=False,
+)
+
 DimensionValueContributionTypeDef = TypedDict(
     "DimensionValueContributionTypeDef",
     {
         "DimensionValue": str,
         "ContributionScore": float,
     },
     total=False,
@@ -496,23 +610,41 @@
     "DimensionNameValueTypeDef",
     {
         "DimensionName": str,
         "DimensionValue": str,
     },
 )
 
+JsonFormatDescriptorOutputTypeDef = TypedDict(
+    "JsonFormatDescriptorOutputTypeDef",
+    {
+        "FileCompression": JsonFileCompressionType,
+        "Charset": str,
+    },
+    total=False,
+)
+
 JsonFormatDescriptorTypeDef = TypedDict(
     "JsonFormatDescriptorTypeDef",
     {
         "FileCompression": JsonFileCompressionType,
         "Charset": str,
     },
     total=False,
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "DimensionValue": str,
+        "FilterOperation": Literal["EQUALS"],
+    },
+    total=False,
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "DimensionValue": str,
         "FilterOperation": Literal["EQUALS"],
     },
     total=False,
@@ -697,14 +829,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "SubnetIdList": List[str],
+        "SecurityGroupIdList": List[str],
+    },
+)
+
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
     },
 )
@@ -756,23 +896,41 @@
     "UpdateMetricSetResponseTypeDef",
     {
         "MetricSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "SNSConfiguration": SNSConfigurationOutputTypeDef,
+        "LambdaConfiguration": LambdaConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
 )
 
+AlertFiltersOutputTypeDef = TypedDict(
+    "AlertFiltersOutputTypeDef",
+    {
+        "MetricList": List[str],
+        "DimensionFilterList": List[DimensionFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 AlertFiltersTypeDef = TypedDict(
     "AlertFiltersTypeDef",
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
@@ -893,14 +1051,37 @@
 )
 
 class GetFeedbackRequestRequestTypeDef(
     _RequiredGetFeedbackRequestRequestTypeDef, _OptionalGetFeedbackRequestRequestTypeDef
 ):
     pass
 
+AthenaSourceConfigOutputTypeDef = TypedDict(
+    "AthenaSourceConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "DatabaseName": str,
+        "DataCatalog": str,
+        "TableName": str,
+        "WorkGroupName": str,
+        "S3ResultsPath": str,
+        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+CloudWatchConfigOutputTypeDef = TypedDict(
+    "CloudWatchConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AthenaSourceConfigTypeDef = TypedDict(
     "AthenaSourceConfigTypeDef",
     {
         "RoleArn": str,
         "DatabaseName": str,
         "DataCatalog": str,
         "TableName": str,
@@ -970,23 +1151,41 @@
     {
         "TimeSeriesId": str,
         "DimensionList": List[DimensionNameValueTypeDef],
         "MetricValueList": List[float],
     },
 )
 
+FileFormatDescriptorOutputTypeDef = TypedDict(
+    "FileFormatDescriptorOutputTypeDef",
+    {
+        "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
+        "JsonFormatDescriptor": JsonFormatDescriptorOutputTypeDef,
+    },
+    total=False,
+)
+
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorTypeDef,
         "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
+MetricSetDimensionFilterOutputTypeDef = TypedDict(
+    "MetricSetDimensionFilterOutputTypeDef",
+    {
+        "Name": str,
+        "FilterList": List[FilterOutputTypeDef],
+    },
+    total=False,
+)
+
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
         "Name": str,
         "FilterList": Sequence[FilterTypeDef],
     },
     total=False,
@@ -1015,14 +1214,44 @@
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RDSSourceConfigOutputTypeDef = TypedDict(
+    "RDSSourceConfigOutputTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+RedshiftSourceConfigOutputTypeDef = TypedDict(
+    "RedshiftSourceConfigOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DatabaseHost": str,
         "DatabasePort": int,
         "SecretManagerArn": str,
@@ -1048,25 +1277,25 @@
     },
     total=False,
 )
 
 AlertTypeDef = TypedDict(
     "AlertTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "AlertDescription": str,
         "AlertArn": str,
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
         "LastModificationTime": datetime,
         "CreationTime": datetime,
-        "AlertFilters": AlertFiltersTypeDef,
+        "AlertFilters": AlertFiltersOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
@@ -1178,14 +1407,25 @@
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3SourceConfigOutputTypeDef = TypedDict(
+    "S3SourceConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "TemplatedPathList": List[str],
+        "HistoricalDataPathList": List[str],
+        "FileFormatDescriptor": FileFormatDescriptorOutputTypeDef,
+    },
+    total=False,
+)
+
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
         "FileFormatDescriptor": FileFormatDescriptorTypeDef,
@@ -1245,14 +1485,27 @@
         "MetricName": str,
         "NumTimeSeries": int,
         "ContributionMatrix": ContributionMatrixTypeDef,
     },
     total=False,
 )
 
+MetricSourceOutputTypeDef = TypedDict(
+    "MetricSourceOutputTypeDef",
+    {
+        "S3SourceConfig": S3SourceConfigOutputTypeDef,
+        "AppFlowConfig": AppFlowConfigOutputTypeDef,
+        "CloudWatchConfig": CloudWatchConfigOutputTypeDef,
+        "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
+        "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
+        "AthenaSourceConfig": AthenaSourceConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
         "S3SourceConfig": S3SourceConfigTypeDef,
         "AppFlowConfig": AppFlowConfigTypeDef,
         "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigTypeDef,
@@ -1287,14 +1540,35 @@
         "AnomalyGroupScore": float,
         "PrimaryMetricName": str,
         "MetricLevelImpactList": List[MetricLevelImpactTypeDef],
     },
     total=False,
 )
 
+DescribeMetricSetResponseTypeDef = TypedDict(
+    "DescribeMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "AnomalyDetectorArn": str,
+        "MetricSetName": str,
+        "MetricSetDescription": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Offset": int,
+        "MetricList": List[MetricOutputTypeDef],
+        "TimestampColumn": TimestampColumnOutputTypeDef,
+        "DimensionList": List[str],
+        "MetricSetFrequency": FrequencyType,
+        "Timezone": str,
+        "MetricSource": MetricSourceOutputTypeDef,
+        "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricList": Sequence[MetricTypeDef],
         "MetricSource": MetricSourceTypeDef,
@@ -1316,35 +1590,14 @@
 )
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
-DescribeMetricSetResponseTypeDef = TypedDict(
-    "DescribeMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "AnomalyDetectorArn": str,
-        "MetricSetName": str,
-        "MetricSetDescription": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Offset": int,
-        "MetricList": List[MetricTypeDef],
-        "TimestampColumn": TimestampColumnTypeDef,
-        "DimensionList": List[str],
-        "MetricSetFrequency": FrequencyType,
-        "Timezone": str,
-        "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.12/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-lookoutmetrics
-Version: 1.28.0
-Summary: Type annotations for boto3.LookoutMetrics 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-lookoutmetrics"></a>
 
 # mypy-boto3-lookoutmetrics
 
 [![PyPI - mypy-boto3-lookoutmetrics](https://img.shields.io/pypi/v/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutmetrics?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutmetrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,49 +279,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
+    LambdaConfigurationOutputTypeDef,
+    SNSConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
+    DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
+    AppFlowConfigOutputTypeDef,
     AppFlowConfigTypeDef,
+    BackTestConfigurationOutputTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
     CreateMetricSetResponseTypeDef,
+    CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     ExecutionStatusTypeDef,
     DescribeAnomalyDetectorRequestRequestTypeDef,
     DescribeMetricSetRequestRequestTypeDef,
+    MetricOutputTypeDef,
+    TimestampColumnOutputTypeDef,
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
+    JsonFormatDescriptorOutputTypeDef,
     JsonFormatDescriptorTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
     GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
@@ -361,77 +339,88 @@
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
     ListAlertsResponseTypeDef,
     DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
+    AthenaSourceConfigOutputTypeDef,
+    CloudWatchConfigOutputTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
+    FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
+    RDSSourceConfigOutputTypeDef,
+    RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
+    S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
-    CreateMetricSetRequestRequestTypeDef,
     DescribeMetricSetResponseTypeDef,
+    CreateMetricSetRequestRequestTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_structure() -> LambdaConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt` & `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.0/setup.py` & `mypy-boto3-lookoutmetrics-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutmetrics",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutMetrics 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.LookoutMetrics 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

