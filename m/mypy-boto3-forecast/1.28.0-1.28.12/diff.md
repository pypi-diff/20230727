# Comparing `tmp/mypy-boto3-forecast-1.28.0.tar.gz` & `tmp/mypy-boto3-forecast-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-forecast-1.28.0.tar", last modified: Thu Jul  6 20:59:37 2023, max compression
+gzip compressed data, was "mypy-boto3-forecast-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
```

## Comparing `mypy-boto3-forecast-1.28.0.tar` & `mypy-boto3-forecast-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.098307 mypy-boto3-forecast-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-06 20:59:37.098307 mypy-boto3-forecast-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.098307 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51565 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51481 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-07-06 20:41:16.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65458 2023-07-06 20:41:19.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65405 2023-07-06 20:41:16.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:15.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.098307 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-06 20:59:36.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 20:59:36.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:36.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:36.000000 mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:37.098307 mypy-boto3-forecast-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:41:14.000000 mypy-boto3-forecast-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51565 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51481 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-27 05:22:25.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-27 05:22:25.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75342 2023-07-27 05:22:27.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75270 2023-07-27 05:22:26.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:22:23.000000 mypy-boto3-forecast-1.28.12/setup.py
```

### Comparing `mypy-boto3-forecast-1.28.0/LICENSE` & `mypy-boto3-forecast-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/PKG-INFO` & `mypy-boto3-forecast-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.28.0
-Summary: Type annotations for boto3.ForecastService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ForecastService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-forecast?color=blue)](https://pypistats.org/packages/mypy-boto3-forecast)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,19 +396,24 @@
 ### Typed dictionaries
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
+    ActionOutputTypeDef,
     ActionTypeDef,
+    AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
+    AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
+    CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
+    ContinuousParameterRangeOutputTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
     CreateAutoPredictorResponseTypeDef,
     CreateDatasetGroupResponseTypeDef,
@@ -422,14 +427,15 @@
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -440,73 +446,86 @@
     DeletePredictorBacktestExportJobRequestRequestTypeDef,
     DeletePredictorRequestRequestTypeDef,
     DeleteResourceTreeRequestRequestTypeDef,
     DeleteWhatIfAnalysisRequestRequestTypeDef,
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
+    TimeAlignmentBoundaryOutputTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
+    ExplainabilityConfigOutputTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
+    EvaluationParametersOutputTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
+    FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
+    SupplementaryFeatureOutputTypeDef,
     SupplementaryFeatureTypeDef,
+    IntegerParameterRangeOutputTypeDef,
     IntegerParameterRangeTypeDef,
     ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
     PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
     ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
+    SchemaAttributeOutputTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
+    TimeSeriesConditionOutputTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExplainabilitySummaryTypeDef,
+    DataDestinationOutputTypeDef,
+    DataSourceOutputTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
+    ExplainabilitySummaryTypeDef,
+    FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
     ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
     ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
     ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
@@ -525,76 +544,86 @@
     ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
     ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
     ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
     ListMonitorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
-    CreateAutoPredictorRequestRequestTypeDef,
     DescribeAutoPredictorResponseTypeDef,
+    CreateAutoPredictorRequestRequestTypeDef,
     BaselineTypeDef,
-    ListExplainabilitiesResponseTypeDef,
-    CreateExplainabilityExportRequestRequestTypeDef,
-    CreateForecastExportJobRequestRequestTypeDef,
-    CreatePredictorBacktestExportJobRequestRequestTypeDef,
-    CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
     DescribeForecastExportJobResponseTypeDef,
     DescribePredictorBacktestExportJobResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     ExplainabilityExportSummaryTypeDef,
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
-    CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
+    CreateExplainabilityExportRequestRequestTypeDef,
+    CreateForecastExportJobRequestRequestTypeDef,
+    CreatePredictorBacktestExportJobRequestRequestTypeDef,
+    CreateWhatIfForecastExportRequestRequestTypeDef,
+    CreateDatasetImportJobRequestRequestTypeDef,
     ListPredictorsResponseTypeDef,
+    ListExplainabilitiesResponseTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    CreateExplainabilityRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
+    TimeSeriesIdentifiersOutputTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    CreateExplainabilityRequestRequestTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     CreatePredictorRequestRequestTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
+    DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
-    DescribeWhatIfForecastResponseTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    CreateForecastRequestRequestTypeDef,
-    CreateWhatIfAnalysisRequestRequestTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
+    CreateForecastRequestRequestTypeDef,
+    CreateWhatIfAnalysisRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_structure() -> ActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.0/README.md` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-forecast
+Version: 1.28.12
+Summary: Type annotations for boto3.ForecastService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 forecast type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-forecast?color=blue)](https://pypistats.org/packages/mypy-boto3-forecast)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,19 +396,24 @@
 ### Typed dictionaries
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
+    ActionOutputTypeDef,
     ActionTypeDef,
+    AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
+    AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
+    CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
+    ContinuousParameterRangeOutputTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
     CreateAutoPredictorResponseTypeDef,
     CreateDatasetGroupResponseTypeDef,
@@ -390,14 +427,15 @@
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -408,73 +446,86 @@
     DeletePredictorBacktestExportJobRequestRequestTypeDef,
     DeletePredictorRequestRequestTypeDef,
     DeleteResourceTreeRequestRequestTypeDef,
     DeleteWhatIfAnalysisRequestRequestTypeDef,
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
+    TimeAlignmentBoundaryOutputTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
+    ExplainabilityConfigOutputTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
+    EvaluationParametersOutputTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
+    FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
+    SupplementaryFeatureOutputTypeDef,
     SupplementaryFeatureTypeDef,
+    IntegerParameterRangeOutputTypeDef,
     IntegerParameterRangeTypeDef,
     ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
     PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
     ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
+    SchemaAttributeOutputTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
+    TimeSeriesConditionOutputTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExplainabilitySummaryTypeDef,
+    DataDestinationOutputTypeDef,
+    DataSourceOutputTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
+    ExplainabilitySummaryTypeDef,
+    FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
     ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
     ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
     ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
@@ -493,76 +544,86 @@
     ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
     ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
     ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
     ListMonitorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
-    CreateAutoPredictorRequestRequestTypeDef,
     DescribeAutoPredictorResponseTypeDef,
+    CreateAutoPredictorRequestRequestTypeDef,
     BaselineTypeDef,
-    ListExplainabilitiesResponseTypeDef,
-    CreateExplainabilityExportRequestRequestTypeDef,
-    CreateForecastExportJobRequestRequestTypeDef,
-    CreatePredictorBacktestExportJobRequestRequestTypeDef,
-    CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
     DescribeForecastExportJobResponseTypeDef,
     DescribePredictorBacktestExportJobResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     ExplainabilityExportSummaryTypeDef,
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
-    CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
+    CreateExplainabilityExportRequestRequestTypeDef,
+    CreateForecastExportJobRequestRequestTypeDef,
+    CreatePredictorBacktestExportJobRequestRequestTypeDef,
+    CreateWhatIfForecastExportRequestRequestTypeDef,
+    CreateDatasetImportJobRequestRequestTypeDef,
     ListPredictorsResponseTypeDef,
+    ListExplainabilitiesResponseTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    CreateExplainabilityRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
+    TimeSeriesIdentifiersOutputTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    CreateExplainabilityRequestRequestTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     CreatePredictorRequestRequestTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
+    DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
-    DescribeWhatIfForecastResponseTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    CreateForecastRequestRequestTypeDef,
-    CreateWhatIfAnalysisRequestRequestTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
+    CreateForecastRequestRequestTypeDef,
+    CreateWhatIfAnalysisRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_structure() -> ActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/__init__.py` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/__init__.pyi` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/__main__.py` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ForecastService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ForecastService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
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

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/client.py` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/client.pyi` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/literals.py` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.py`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/literals.pyi` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,15 @@
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
@@ -307,26 +308,28 @@
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

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/paginator.py` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/paginator.pyi` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/type_defs.py` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for forecast service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_forecast.type_defs import ActionTypeDef
+    from mypy_boto3_forecast.type_defs import ActionOutputTypeDef
 
-    data: ActionTypeDef = {...}
+    data: ActionOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -39,21 +39,25 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
+    "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
+    "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
+    "ContinuousParameterRangeOutputTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
     "CreateAutoPredictorResponseTypeDef",
     "CreateDatasetGroupResponseTypeDef",
@@ -67,14 +71,15 @@
     "CreateMonitorResponseTypeDef",
     "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
     "CreatePredictorResponseTypeDef",
     "CreateWhatIfAnalysisResponseTypeDef",
     "CreateWhatIfForecastExportResponseTypeDef",
     "CreateWhatIfForecastResponseTypeDef",
+    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -85,73 +90,86 @@
     "DeletePredictorBacktestExportJobRequestRequestTypeDef",
     "DeletePredictorRequestRequestTypeDef",
     "DeleteResourceTreeRequestRequestTypeDef",
     "DeleteWhatIfAnalysisRequestRequestTypeDef",
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
+    "TimeAlignmentBoundaryOutputTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
+    "ExplainabilityConfigOutputTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
+    "EvaluationParametersOutputTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
+    "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
+    "SupplementaryFeatureOutputTypeDef",
     "SupplementaryFeatureTypeDef",
+    "IntegerParameterRangeOutputTypeDef",
     "IntegerParameterRangeTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
     "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
+    "SchemaAttributeOutputTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
+    "TimeSeriesConditionOutputTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
+    "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ExplainabilitySummaryTypeDef",
+    "DataDestinationOutputTypeDef",
+    "DataSourceOutputTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
+    "ExplainabilitySummaryTypeDef",
+    "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
     "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
     "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
@@ -170,103 +188,147 @@
     "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
     "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
     "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
+    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
     "ListMonitorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
+    "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
-    "CreateAutoPredictorRequestRequestTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
+    "CreateAutoPredictorRequestRequestTypeDef",
     "BaselineTypeDef",
-    "ListExplainabilitiesResponseTypeDef",
-    "CreateExplainabilityExportRequestRequestTypeDef",
-    "CreateForecastExportJobRequestRequestTypeDef",
-    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
-    "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
     "DescribeForecastExportJobResponseTypeDef",
     "DescribePredictorBacktestExportJobResponseTypeDef",
     "DescribeWhatIfForecastExportResponseTypeDef",
     "ExplainabilityExportSummaryTypeDef",
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
-    "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
+    "CreateExplainabilityExportRequestRequestTypeDef",
+    "CreateForecastExportJobRequestRequestTypeDef",
+    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
+    "CreateWhatIfForecastExportRequestRequestTypeDef",
+    "CreateDatasetImportJobRequestRequestTypeDef",
     "ListPredictorsResponseTypeDef",
+    "ListExplainabilitiesResponseTypeDef",
+    "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
+    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "CreateExplainabilityRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DescribeExplainabilityResponseTypeDef",
+    "TimeSeriesIdentifiersOutputTypeDef",
+    "TimeSeriesReplacementsDataSourceOutputTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "CreateExplainabilityRequestRequestTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "CreatePredictorRequestRequestTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
+    "TimeSeriesSelectorOutputTypeDef",
+    "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
-    "DescribeWhatIfForecastResponseTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
-    "CreateForecastRequestRequestTypeDef",
-    "CreateWhatIfAnalysisRequestRequestTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
+    "CreateForecastRequestRequestTypeDef",
+    "CreateWhatIfAnalysisRequestRequestTypeDef",
+)
+
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Operation": OperationType,
+        "Value": float,
+    },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
 )
 
+_RequiredAdditionalDatasetOutputTypeDef = TypedDict(
+    "_RequiredAdditionalDatasetOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAdditionalDatasetOutputTypeDef = TypedDict(
+    "_OptionalAdditionalDatasetOutputTypeDef",
+    {
+        "Configuration": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+class AdditionalDatasetOutputTypeDef(
+    _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
+):
+    pass
+
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
     "_OptionalAdditionalDatasetTypeDef",
     {
         "Configuration": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
+AttributeConfigOutputTypeDef = TypedDict(
+    "AttributeConfigOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Transformations": Dict[str, str],
+    },
+)
 
 AttributeConfigTypeDef = TypedDict(
     "AttributeConfigTypeDef",
     {
         "AttributeName": str,
         "Transformations": Mapping[str, str],
     },
@@ -277,22 +339,51 @@
     {
         "Name": str,
         "Value": float,
     },
     total=False,
 )
 
+CategoricalParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
+
 CategoricalParameterRangeTypeDef = TypedDict(
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+_RequiredContinuousParameterRangeOutputTypeDef = TypedDict(
+    "_RequiredContinuousParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "MaxValue": float,
+        "MinValue": float,
+    },
+)
+_OptionalContinuousParameterRangeOutputTypeDef = TypedDict(
+    "_OptionalContinuousParameterRangeOutputTypeDef",
+    {
+        "ScalingType": ScalingTypeType,
+    },
+    total=False,
+)
+
+class ContinuousParameterRangeOutputTypeDef(
+    _RequiredContinuousParameterRangeOutputTypeDef, _OptionalContinuousParameterRangeOutputTypeDef
+):
+    pass
+
 _RequiredContinuousParameterRangeTypeDef = TypedDict(
     "_RequiredContinuousParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": float,
         "MinValue": float,
     },
@@ -301,21 +392,19 @@
     "_OptionalContinuousParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
-
 class ContinuousParameterRangeTypeDef(
     _RequiredContinuousParameterRangeTypeDef, _OptionalContinuousParameterRangeTypeDef
 ):
     pass
 
-
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "RoleArn": str,
         "KMSKeyArn": str,
     },
 )
@@ -471,14 +560,32 @@
     "CreateWhatIfForecastResponseTypeDef",
     {
         "WhatIfForecastArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3ConfigOutputTypeDef = TypedDict(
+    "_RequiredS3ConfigOutputTypeDef",
+    {
+        "Path": str,
+        "RoleArn": str,
+    },
+)
+_OptionalS3ConfigOutputTypeDef = TypedDict(
+    "_OptionalS3ConfigOutputTypeDef",
+    {
+        "KMSKeyArn": str,
+    },
+    total=False,
+)
+
+class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
+    pass
+
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -486,19 +593,17 @@
     "_OptionalS3ConfigTypeDef",
     {
         "KMSKeyArn": str,
     },
     total=False,
 )
 
-
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
-
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetGroupName": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
@@ -620,14 +725,22 @@
 DescribeAutoPredictorRequestRequestTypeDef = TypedDict(
     "DescribeAutoPredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "KMSKeyArn": str,
+    },
+)
+
 ExplainabilityInfoTypeDef = TypedDict(
     "ExplainabilityInfoTypeDef",
     {
         "ExplainabilityArn": str,
         "Status": str,
     },
     total=False,
@@ -647,14 +760,25 @@
     {
         "Arn": str,
         "State": StateType,
     },
     total=False,
 )
 
+TimeAlignmentBoundaryOutputTypeDef = TypedDict(
+    "TimeAlignmentBoundaryOutputTypeDef",
+    {
+        "Month": MonthType,
+        "DayOfMonth": int,
+        "DayOfWeek": DayOfWeekType,
+        "Hour": int,
+    },
+    total=False,
+)
+
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
@@ -715,14 +839,22 @@
 DescribeExplainabilityRequestRequestTypeDef = TypedDict(
     "DescribeExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityArn": str,
     },
 )
 
+ExplainabilityConfigOutputTypeDef = TypedDict(
+    "ExplainabilityConfigOutputTypeDef",
+    {
+        "TimeSeriesGranularity": TimeSeriesGranularityType,
+        "TimePointGranularity": TimePointGranularityType,
+    },
+)
+
 DescribeForecastExportJobRequestRequestTypeDef = TypedDict(
     "DescribeForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobArn": str,
     },
 )
 
@@ -750,14 +882,23 @@
 DescribePredictorRequestRequestTypeDef = TypedDict(
     "DescribePredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
+EvaluationParametersOutputTypeDef = TypedDict(
+    "EvaluationParametersOutputTypeDef",
+    {
+        "NumberOfBacktestWindows": int,
+        "BackTestWindowOffset": int,
+    },
+    total=False,
+)
+
 DescribeWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisArn": str,
     },
 )
 
@@ -790,35 +931,52 @@
         "RMSE": float,
         "MASE": float,
         "MAPE": float,
     },
     total=False,
 )
 
+_RequiredFeaturizationMethodOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodName": Literal["filling"],
+    },
+)
+_OptionalFeaturizationMethodOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodParameters": Dict[str, str],
+    },
+    total=False,
+)
+
+class FeaturizationMethodOutputTypeDef(
+    _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
+):
+    pass
+
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
     "_OptionalFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodParameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class FeaturizationMethodTypeDef(
     _RequiredFeaturizationMethodTypeDef, _OptionalFeaturizationMethodTypeDef
 ):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Condition": FilterConditionStringType,
     },
@@ -843,22 +1001,51 @@
 GetAccuracyMetricsRequestRequestTypeDef = TypedDict(
     "GetAccuracyMetricsRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
+SupplementaryFeatureOutputTypeDef = TypedDict(
+    "SupplementaryFeatureOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 SupplementaryFeatureTypeDef = TypedDict(
     "SupplementaryFeatureTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+_RequiredIntegerParameterRangeOutputTypeDef = TypedDict(
+    "_RequiredIntegerParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "MaxValue": int,
+        "MinValue": int,
+    },
+)
+_OptionalIntegerParameterRangeOutputTypeDef = TypedDict(
+    "_OptionalIntegerParameterRangeOutputTypeDef",
+    {
+        "ScalingType": ScalingTypeType,
+    },
+    total=False,
+)
+
+class IntegerParameterRangeOutputTypeDef(
+    _RequiredIntegerParameterRangeOutputTypeDef, _OptionalIntegerParameterRangeOutputTypeDef
+):
+    pass
+
 _RequiredIntegerParameterRangeTypeDef = TypedDict(
     "_RequiredIntegerParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": int,
         "MinValue": int,
     },
@@ -867,21 +1054,19 @@
     "_OptionalIntegerParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
-
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
-
 ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -928,14 +1113,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 WhatIfAnalysisSummaryTypeDef = TypedDict(
     "WhatIfAnalysisSummaryTypeDef",
     {
         "WhatIfAnalysisArn": str,
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
         "Status": str,
@@ -1032,14 +1225,23 @@
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+SchemaAttributeOutputTypeDef = TypedDict(
+    "SchemaAttributeOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": AttributeTypeType,
+    },
+    total=False,
+)
+
 SchemaAttributeTypeDef = TypedDict(
     "SchemaAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeType": AttributeTypeType,
     },
     total=False,
@@ -1048,14 +1250,23 @@
 StopResourceRequestRequestTypeDef = TypedDict(
     "StopResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TimeSeriesConditionOutputTypeDef = TypedDict(
+    "TimeSeriesConditionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeValue": str,
+        "Condition": ConditionType,
+    },
+)
+
 TimeSeriesConditionTypeDef = TypedDict(
     "TimeSeriesConditionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
         "Condition": ConditionType,
     },
@@ -1073,14 +1284,32 @@
     "UpdateDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetArns": Sequence[str],
     },
 )
 
+_RequiredDataConfigOutputTypeDef = TypedDict(
+    "_RequiredDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalDataConfigOutputTypeDef = TypedDict(
+    "_OptionalDataConfigOutputTypeDef",
+    {
+        "AttributeConfigs": List[AttributeConfigOutputTypeDef],
+        "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
+    },
+    total=False,
+)
+
+class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
+    pass
+
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1088,19 +1317,17 @@
     {
         "AttributeConfigs": Sequence[AttributeConfigTypeDef],
         "AdditionalDatasets": Sequence[AdditionalDatasetTypeDef],
     },
     total=False,
 )
 
-
 class DataConfigTypeDef(_RequiredDataConfigTypeDef, _OptionalDataConfigTypeDef):
     pass
 
-
 PredictorBaselineTypeDef = TypedDict(
     "PredictorBaselineTypeDef",
     {
         "BaselineMetrics": List[BaselineMetricTypeDef],
     },
     total=False,
 )
@@ -1117,22 +1344,20 @@
     {
         "DatasetArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
         "ResourceArn": str,
     },
 )
@@ -1140,50 +1365,39 @@
     "_OptionalCreateMonitorRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ExplainabilitySummaryTypeDef = TypedDict(
-    "ExplainabilitySummaryTypeDef",
+DataDestinationOutputTypeDef = TypedDict(
+    "DataDestinationOutputTypeDef",
     {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
+        "S3Config": S3ConfigOutputTypeDef,
+    },
+)
+
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "S3Config": S3ConfigOutputTypeDef,
     },
-    total=False,
 )
 
 DataDestinationTypeDef = TypedDict(
     "DataDestinationTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
@@ -1226,33 +1440,65 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
+ExplainabilitySummaryTypeDef = TypedDict(
+    "ExplainabilitySummaryTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+    },
+    total=False,
+)
+
+_RequiredFeaturizationOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationOutputTypeDef",
+    {
+        "AttributeName": str,
+    },
+)
+_OptionalFeaturizationOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationOutputTypeDef",
+    {
+        "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
+    },
+    total=False,
+)
+
+class FeaturizationOutputTypeDef(
+    _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
+):
+    pass
+
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
     "_OptionalFeaturizationTypeDef",
     {
         "FeaturizationPipeline": Sequence[FeaturizationMethodTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
-
 ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1355,22 +1601,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
     _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
 )
 _OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
@@ -1379,22 +1623,20 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1510,32 +1752,59 @@
     {
         "Forecasts": List[ForecastSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "SupplementaryFeatures": List[SupplementaryFeatureOutputTypeDef],
+    },
+    total=False,
+)
+
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
+    pass
+
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
     "_OptionalInputDataConfigTypeDef",
     {
         "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
-
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
+ParameterRangesOutputTypeDef = TypedDict(
+    "ParameterRangesOutputTypeDef",
+    {
+        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
+        "ContinuousParameterRanges": List[ContinuousParameterRangeOutputTypeDef],
+        "IntegerParameterRanges": List[IntegerParameterRangeOutputTypeDef],
+    },
+    total=False,
+)
 
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
@@ -1548,14 +1817,22 @@
     {
         "Monitors": List[MonitorSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1604,214 +1881,120 @@
     {
         "AlgorithmArn": str,
         "TestWindows": List[TestWindowSummaryTypeDef],
     },
     total=False,
 )
 
-SchemaTypeDef = TypedDict(
-    "SchemaTypeDef",
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
     {
-        "Attributes": Sequence[SchemaAttributeTypeDef],
+        "Attributes": List[SchemaAttributeOutputTypeDef],
     },
     total=False,
 )
 
-TimeSeriesTransformationTypeDef = TypedDict(
-    "TimeSeriesTransformationTypeDef",
+SchemaTypeDef = TypedDict(
+    "SchemaTypeDef",
     {
-        "Action": ActionTypeDef,
-        "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
+        "Attributes": Sequence[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAutoPredictorRequestRequestTypeDef",
+TimeSeriesTransformationOutputTypeDef = TypedDict(
+    "TimeSeriesTransformationOutputTypeDef",
     {
-        "PredictorName": str,
+        "Action": ActionOutputTypeDef,
+        "TimeSeriesConditions": List[TimeSeriesConditionOutputTypeDef],
     },
+    total=False,
 )
-_OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAutoPredictorRequestRequestTypeDef",
+
+TimeSeriesTransformationTypeDef = TypedDict(
+    "TimeSeriesTransformationTypeDef",
     {
-        "ForecastHorizon": int,
-        "ForecastTypes": Sequence[str],
-        "ForecastDimensions": Sequence[str],
-        "ForecastFrequency": str,
-        "DataConfig": DataConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "ReferencePredictorArn": str,
-        "OptimizationMetric": OptimizationMetricType,
-        "ExplainPredictor": bool,
-        "Tags": Sequence[TagTypeDef],
-        "MonitorConfig": MonitorConfigTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "Action": ActionTypeDef,
+        "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
-
-class CreateAutoPredictorRequestRequestTypeDef(
-    _RequiredCreateAutoPredictorRequestRequestTypeDef,
-    _OptionalCreateAutoPredictorRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeAutoPredictorResponseTypeDef = TypedDict(
     "DescribeAutoPredictorResponseTypeDef",
     {
         "PredictorArn": str,
         "PredictorName": str,
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "ForecastFrequency": str,
         "ForecastDimensions": List[str],
         "DatasetImportJobArns": List[str],
-        "DataConfig": DataConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
+        "DataConfig": DataConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigOutputTypeDef,
         "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ExplainabilityInfo": ExplainabilityInfoTypeDef,
         "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BaselineTypeDef = TypedDict(
-    "BaselineTypeDef",
-    {
-        "PredictorBaseline": PredictorBaselineTypeDef,
-    },
-    total=False,
-)
-
-ListExplainabilitiesResponseTypeDef = TypedDict(
-    "ListExplainabilitiesResponseTypeDef",
-    {
-        "Explainabilities": List[ExplainabilitySummaryTypeDef],
-        "NextToken": str,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
-    {
-        "ExplainabilityExportName": str,
-        "ExplainabilityArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-
-class CreateExplainabilityExportRequestRequestTypeDef(
-    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
-    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "ForecastExportJobName": str,
-        "ForecastArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-
-class CreateForecastExportJobRequestRequestTypeDef(
-    _RequiredCreateForecastExportJobRequestRequestTypeDef,
-    _OptionalCreateForecastExportJobRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
+_RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
-        "PredictorBacktestExportJobName": str,
-        "PredictorArn": str,
-        "Destination": DataDestinationTypeDef,
+        "PredictorName": str,
     },
 )
-_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
+_OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutoPredictorRequestRequestTypeDef",
     {
+        "ForecastHorizon": int,
+        "ForecastTypes": Sequence[str],
+        "ForecastDimensions": Sequence[str],
+        "ForecastFrequency": str,
+        "DataConfig": DataConfigTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "ReferencePredictorArn": str,
+        "OptimizationMetric": OptimizationMetricType,
+        "ExplainPredictor": bool,
         "Tags": Sequence[TagTypeDef],
-        "Format": str,
+        "MonitorConfig": MonitorConfigTypeDef,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
     },
     total=False,
 )
 
-
-class CreatePredictorBacktestExportJobRequestRequestTypeDef(
-    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
-    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
+class CreateAutoPredictorRequestRequestTypeDef(
+    _RequiredCreateAutoPredictorRequestRequestTypeDef,
+    _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
-    {
-        "WhatIfForecastExportName": str,
-        "WhatIfForecastArns": Sequence[str],
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
+BaselineTypeDef = TypedDict(
+    "BaselineTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
+        "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
 
-
-class CreateWhatIfForecastExportRequestRequestTypeDef(
-    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
-    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1819,15 +2002,15 @@
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
         "ForecastArn": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1835,15 +2018,15 @@
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1851,15 +2034,15 @@
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": List[str],
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1867,102 +2050,72 @@
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 ForecastExportJobSummaryTypeDef = TypedDict(
     "ForecastExportJobSummaryTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 PredictorBacktestExportJobSummaryTypeDef = TypedDict(
     "PredictorBacktestExportJobSummaryTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 WhatIfForecastExportSummaryTypeDef = TypedDict(
     "WhatIfForecastExportSummaryTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastArns": List[str],
         "WhatIfForecastExportName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
-    {
-        "DatasetImportJobName": str,
-        "DatasetArn": str,
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
-    {
-        "TimestampFormat": str,
-        "TimeZone": str,
-        "UseGeolocationForTimeZone": bool,
-        "GeolocationFormat": str,
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-        "ImportMode": ImportModeType,
-    },
-    total=False,
-)
-
-
-class CreateDatasetImportJobRequestRequestTypeDef(
-    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
-    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
-):
-    pass
-
-
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
-        "DataSource": DataSourceTypeDef,
+        "DataSource": DataSourceOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "ImportMode": ImportModeType,
     },
     total=False,
@@ -1974,37 +2127,186 @@
         "DatasetImportJobName": str,
         "DatasetImportJobArn": str,
         "DatasetArn": str,
         "TimestampFormat": str,
         "TimeZone": str,
         "UseGeolocationForTimeZone": bool,
         "GeolocationFormat": str,
-        "DataSource": DataSourceTypeDef,
+        "DataSource": DataSourceOutputTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "FieldStatistics": Dict[str, StatisticsTypeDef],
         "DataSize": float,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "ExplainabilityExportName": str,
+        "ExplainabilityArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreateExplainabilityExportRequestRequestTypeDef(
+    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
+    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "ForecastExportJobName": str,
+        "ForecastArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreateForecastExportJobRequestRequestTypeDef(
+    _RequiredCreateForecastExportJobRequestRequestTypeDef,
+    _OptionalCreateForecastExportJobRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "PredictorBacktestExportJobName": str,
+        "PredictorArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreatePredictorBacktestExportJobRequestRequestTypeDef(
+    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
+    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "WhatIfForecastExportName": str,
+        "WhatIfForecastArns": Sequence[str],
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreateWhatIfForecastExportRequestRequestTypeDef(
+    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
+    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
+    {
+        "DatasetImportJobName": str,
+        "DatasetArn": str,
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
+    {
+        "TimestampFormat": str,
+        "TimeZone": str,
+        "UseGeolocationForTimeZone": bool,
+        "GeolocationFormat": str,
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+        "ImportMode": ImportModeType,
+    },
+    total=False,
+)
+
+class CreateDatasetImportJobRequestRequestTypeDef(
+    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
+    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
+):
+    pass
+
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListExplainabilitiesResponseTypeDef = TypedDict(
+    "ListExplainabilitiesResponseTypeDef",
+    {
+        "Explainabilities": List[ExplainabilitySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredFeaturizationConfigOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastFrequency": str,
+    },
+)
+_OptionalFeaturizationConfigOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastDimensions": List[str],
+        "Featurizations": List[FeaturizationOutputTypeDef],
+    },
+    total=False,
+)
+
+class FeaturizationConfigOutputTypeDef(
+    _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
+):
+    pass
+
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -2012,20 +2314,26 @@
     {
         "ForecastDimensions": Sequence[str],
         "Featurizations": Sequence[FeaturizationTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
+HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigOutputTypeDef",
+    {
+        "ParameterRanges": ParameterRangesOutputTypeDef,
+    },
+    total=False,
+)
 
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
     {
         "ParameterRanges": ParameterRangesTypeDef,
     },
     total=False,
@@ -2056,14 +2364,84 @@
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
     },
     total=False,
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": str,
+        "Domain": DomainType,
+        "DatasetType": DatasetTypeType,
+        "DataFrequency": str,
+        "Schema": SchemaOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeExplainabilityResponseTypeDef = TypedDict(
+    "DescribeExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
+        "EnableVisualization": bool,
+        "DataSource": DataSourceOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "StartDateTime": str,
+        "EndDateTime": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Message": str,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TimeSeriesIdentifiersOutputTypeDef = TypedDict(
+    "TimeSeriesIdentifiersOutputTypeDef",
+    {
+        "DataSource": DataSourceOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "Format": str,
+    },
+    total=False,
+)
+
+_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "S3Config": S3ConfigOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+)
+_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "Format": str,
+        "TimestampFormat": str,
+    },
+    total=False,
+)
+
+class TimeSeriesReplacementsDataSourceOutputTypeDef(
+    _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
+    _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
+):
+    pass
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2075,21 +2453,19 @@
         "DataFrequency": str,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateExplainabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
     },
@@ -2103,60 +2479,20 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "DatasetName": str,
-        "Domain": DomainType,
-        "DatasetType": DatasetTypeType,
-        "DataFrequency": str,
-        "Schema": SchemaTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeExplainabilityResponseTypeDef = TypedDict(
-    "DescribeExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "EnableVisualization": bool,
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaTypeDef,
-        "StartDateTime": str,
-        "EndDateTime": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Message": str,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2175,22 +2511,20 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
-
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
-
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2273,21 +2607,19 @@
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OptimizationMetric": OptimizationMetricType,
     },
     total=False,
 )
 
-
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
-
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2302,32 +2634,58 @@
         "AutoMLAlgorithmArns": List[str],
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
-        "EvaluationParameters": EvaluationParametersTypeDef,
-        "HPOConfig": HyperParameterTuningJobConfigTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "FeaturizationConfig": FeaturizationConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
+        "EvaluationParameters": EvaluationParametersOutputTypeDef,
+        "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigOutputTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TimeSeriesSelectorOutputTypeDef = TypedDict(
+    "TimeSeriesSelectorOutputTypeDef",
+    {
+        "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
+    },
+    total=False,
+)
+
+DescribeWhatIfForecastResponseTypeDef = TypedDict(
+    "DescribeWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastName": str,
+        "WhatIfForecastArn": str,
+        "WhatIfAnalysisArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
+        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
+        "ForecastTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
@@ -2345,47 +2703,61 @@
         "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
+GetAccuracyMetricsResponseTypeDef = TypedDict(
+    "GetAccuracyMetricsResponseTypeDef",
+    {
+        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
+        "IsAutoPredictor": bool,
+        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
+        "OptimizationMetric": OptimizationMetricType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-DescribeWhatIfForecastResponseTypeDef = TypedDict(
-    "DescribeWhatIfForecastResponseTypeDef",
+DescribeForecastResponseTypeDef = TypedDict(
+    "DescribeForecastResponseTypeDef",
     {
-        "WhatIfForecastName": str,
-        "WhatIfForecastArn": str,
-        "WhatIfAnalysisArn": str,
+        "ForecastArn": str,
+        "ForecastName": str,
+        "ForecastTypes": List[str],
+        "PredictorArn": str,
+        "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
-        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
-        "ForecastTypes": List[str],
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccuracyMetricsResponseTypeDef = TypedDict(
-    "GetAccuracyMetricsResponseTypeDef",
+DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
+    "DescribeWhatIfAnalysisResponseTypeDef",
     {
-        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
-        "IsAutoPredictor": bool,
-        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
-        "OptimizationMetric": OptimizationMetricType,
+        "WhatIfAnalysisName": str,
+        "WhatIfAnalysisArn": str,
+        "ForecastArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
@@ -2399,21 +2771,19 @@
         "ForecastTypes": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
     },
     total=False,
 )
 
-
 class CreateForecastRequestRequestTypeDef(
     _RequiredCreateForecastRequestRequestTypeDef, _OptionalCreateForecastRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
     },
 )
@@ -2422,48 +2792,12 @@
     {
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
-
-
-DescribeForecastResponseTypeDef = TypedDict(
-    "DescribeForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ForecastName": str,
-        "ForecastTypes": List[str],
-        "PredictorArn": str,
-        "DatasetGroupArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
-    "DescribeWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisName": str,
-        "WhatIfAnalysisArn": str,
-        "ForecastArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast/type_defs.pyi` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for forecast service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_forecast.type_defs import ActionTypeDef
+    from mypy_boto3_forecast.type_defs import ActionOutputTypeDef
 
-    data: ActionTypeDef = {...}
+    data: ActionOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -39,20 +39,26 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
+    "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
+    "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
+    "ContinuousParameterRangeOutputTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
     "CreateAutoPredictorResponseTypeDef",
     "CreateDatasetGroupResponseTypeDef",
@@ -66,14 +72,15 @@
     "CreateMonitorResponseTypeDef",
     "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
     "CreatePredictorResponseTypeDef",
     "CreateWhatIfAnalysisResponseTypeDef",
     "CreateWhatIfForecastExportResponseTypeDef",
     "CreateWhatIfForecastResponseTypeDef",
+    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -84,73 +91,86 @@
     "DeletePredictorBacktestExportJobRequestRequestTypeDef",
     "DeletePredictorRequestRequestTypeDef",
     "DeleteResourceTreeRequestRequestTypeDef",
     "DeleteWhatIfAnalysisRequestRequestTypeDef",
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
+    "TimeAlignmentBoundaryOutputTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
+    "ExplainabilityConfigOutputTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
+    "EvaluationParametersOutputTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
+    "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
+    "SupplementaryFeatureOutputTypeDef",
     "SupplementaryFeatureTypeDef",
+    "IntegerParameterRangeOutputTypeDef",
     "IntegerParameterRangeTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
     "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
+    "SchemaAttributeOutputTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
+    "TimeSeriesConditionOutputTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
+    "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ExplainabilitySummaryTypeDef",
+    "DataDestinationOutputTypeDef",
+    "DataSourceOutputTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
+    "ExplainabilitySummaryTypeDef",
+    "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
     "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
     "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
@@ -169,102 +189,152 @@
     "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
     "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
     "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
+    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
     "ListMonitorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
+    "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
-    "CreateAutoPredictorRequestRequestTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
+    "CreateAutoPredictorRequestRequestTypeDef",
     "BaselineTypeDef",
-    "ListExplainabilitiesResponseTypeDef",
-    "CreateExplainabilityExportRequestRequestTypeDef",
-    "CreateForecastExportJobRequestRequestTypeDef",
-    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
-    "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
     "DescribeForecastExportJobResponseTypeDef",
     "DescribePredictorBacktestExportJobResponseTypeDef",
     "DescribeWhatIfForecastExportResponseTypeDef",
     "ExplainabilityExportSummaryTypeDef",
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
-    "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
+    "CreateExplainabilityExportRequestRequestTypeDef",
+    "CreateForecastExportJobRequestRequestTypeDef",
+    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
+    "CreateWhatIfForecastExportRequestRequestTypeDef",
+    "CreateDatasetImportJobRequestRequestTypeDef",
     "ListPredictorsResponseTypeDef",
+    "ListExplainabilitiesResponseTypeDef",
+    "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
+    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "CreateExplainabilityRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DescribeExplainabilityResponseTypeDef",
+    "TimeSeriesIdentifiersOutputTypeDef",
+    "TimeSeriesReplacementsDataSourceOutputTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "CreateExplainabilityRequestRequestTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "CreatePredictorRequestRequestTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
+    "TimeSeriesSelectorOutputTypeDef",
+    "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
-    "DescribeWhatIfForecastResponseTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
-    "CreateForecastRequestRequestTypeDef",
-    "CreateWhatIfAnalysisRequestRequestTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
+    "CreateForecastRequestRequestTypeDef",
+    "CreateWhatIfAnalysisRequestRequestTypeDef",
+)
+
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Operation": OperationType,
+        "Value": float,
+    },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
 )
 
+_RequiredAdditionalDatasetOutputTypeDef = TypedDict(
+    "_RequiredAdditionalDatasetOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAdditionalDatasetOutputTypeDef = TypedDict(
+    "_OptionalAdditionalDatasetOutputTypeDef",
+    {
+        "Configuration": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+
+class AdditionalDatasetOutputTypeDef(
+    _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
+):
+    pass
+
+
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
     "_OptionalAdditionalDatasetTypeDef",
     {
         "Configuration": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
+
+AttributeConfigOutputTypeDef = TypedDict(
+    "AttributeConfigOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Transformations": Dict[str, str],
+    },
+)
+
 AttributeConfigTypeDef = TypedDict(
     "AttributeConfigTypeDef",
     {
         "AttributeName": str,
         "Transformations": Mapping[str, str],
     },
 )
@@ -274,22 +344,53 @@
     {
         "Name": str,
         "Value": float,
     },
     total=False,
 )
 
+CategoricalParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
+
 CategoricalParameterRangeTypeDef = TypedDict(
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+_RequiredContinuousParameterRangeOutputTypeDef = TypedDict(
+    "_RequiredContinuousParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "MaxValue": float,
+        "MinValue": float,
+    },
+)
+_OptionalContinuousParameterRangeOutputTypeDef = TypedDict(
+    "_OptionalContinuousParameterRangeOutputTypeDef",
+    {
+        "ScalingType": ScalingTypeType,
+    },
+    total=False,
+)
+
+
+class ContinuousParameterRangeOutputTypeDef(
+    _RequiredContinuousParameterRangeOutputTypeDef, _OptionalContinuousParameterRangeOutputTypeDef
+):
+    pass
+
+
 _RequiredContinuousParameterRangeTypeDef = TypedDict(
     "_RequiredContinuousParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": float,
         "MinValue": float,
     },
@@ -298,19 +399,21 @@
     "_OptionalContinuousParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
+
 class ContinuousParameterRangeTypeDef(
     _RequiredContinuousParameterRangeTypeDef, _OptionalContinuousParameterRangeTypeDef
 ):
     pass
 
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "RoleArn": str,
         "KMSKeyArn": str,
     },
 )
@@ -466,14 +569,34 @@
     "CreateWhatIfForecastResponseTypeDef",
     {
         "WhatIfForecastArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3ConfigOutputTypeDef = TypedDict(
+    "_RequiredS3ConfigOutputTypeDef",
+    {
+        "Path": str,
+        "RoleArn": str,
+    },
+)
+_OptionalS3ConfigOutputTypeDef = TypedDict(
+    "_OptionalS3ConfigOutputTypeDef",
+    {
+        "KMSKeyArn": str,
+    },
+    total=False,
+)
+
+
+class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
+    pass
+
+
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -481,17 +604,19 @@
     "_OptionalS3ConfigTypeDef",
     {
         "KMSKeyArn": str,
     },
     total=False,
 )
 
+
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
+
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetGroupName": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
@@ -613,14 +738,22 @@
 DescribeAutoPredictorRequestRequestTypeDef = TypedDict(
     "DescribeAutoPredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "KMSKeyArn": str,
+    },
+)
+
 ExplainabilityInfoTypeDef = TypedDict(
     "ExplainabilityInfoTypeDef",
     {
         "ExplainabilityArn": str,
         "Status": str,
     },
     total=False,
@@ -640,14 +773,25 @@
     {
         "Arn": str,
         "State": StateType,
     },
     total=False,
 )
 
+TimeAlignmentBoundaryOutputTypeDef = TypedDict(
+    "TimeAlignmentBoundaryOutputTypeDef",
+    {
+        "Month": MonthType,
+        "DayOfMonth": int,
+        "DayOfWeek": DayOfWeekType,
+        "Hour": int,
+    },
+    total=False,
+)
+
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
@@ -708,14 +852,22 @@
 DescribeExplainabilityRequestRequestTypeDef = TypedDict(
     "DescribeExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityArn": str,
     },
 )
 
+ExplainabilityConfigOutputTypeDef = TypedDict(
+    "ExplainabilityConfigOutputTypeDef",
+    {
+        "TimeSeriesGranularity": TimeSeriesGranularityType,
+        "TimePointGranularity": TimePointGranularityType,
+    },
+)
+
 DescribeForecastExportJobRequestRequestTypeDef = TypedDict(
     "DescribeForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobArn": str,
     },
 )
 
@@ -743,14 +895,23 @@
 DescribePredictorRequestRequestTypeDef = TypedDict(
     "DescribePredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
+EvaluationParametersOutputTypeDef = TypedDict(
+    "EvaluationParametersOutputTypeDef",
+    {
+        "NumberOfBacktestWindows": int,
+        "BackTestWindowOffset": int,
+    },
+    total=False,
+)
+
 DescribeWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisArn": str,
     },
 )
 
@@ -783,33 +944,56 @@
         "RMSE": float,
         "MASE": float,
         "MAPE": float,
     },
     total=False,
 )
 
+_RequiredFeaturizationMethodOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodName": Literal["filling"],
+    },
+)
+_OptionalFeaturizationMethodOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodParameters": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class FeaturizationMethodOutputTypeDef(
+    _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
+):
+    pass
+
+
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
     "_OptionalFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodParameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class FeaturizationMethodTypeDef(
     _RequiredFeaturizationMethodTypeDef, _OptionalFeaturizationMethodTypeDef
 ):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Condition": FilterConditionStringType,
     },
@@ -834,22 +1018,53 @@
 GetAccuracyMetricsRequestRequestTypeDef = TypedDict(
     "GetAccuracyMetricsRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
+SupplementaryFeatureOutputTypeDef = TypedDict(
+    "SupplementaryFeatureOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 SupplementaryFeatureTypeDef = TypedDict(
     "SupplementaryFeatureTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+_RequiredIntegerParameterRangeOutputTypeDef = TypedDict(
+    "_RequiredIntegerParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "MaxValue": int,
+        "MinValue": int,
+    },
+)
+_OptionalIntegerParameterRangeOutputTypeDef = TypedDict(
+    "_OptionalIntegerParameterRangeOutputTypeDef",
+    {
+        "ScalingType": ScalingTypeType,
+    },
+    total=False,
+)
+
+
+class IntegerParameterRangeOutputTypeDef(
+    _RequiredIntegerParameterRangeOutputTypeDef, _OptionalIntegerParameterRangeOutputTypeDef
+):
+    pass
+
+
 _RequiredIntegerParameterRangeTypeDef = TypedDict(
     "_RequiredIntegerParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": int,
         "MinValue": int,
     },
@@ -858,19 +1073,21 @@
     "_OptionalIntegerParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
+
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
+
 ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -917,14 +1134,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 WhatIfAnalysisSummaryTypeDef = TypedDict(
     "WhatIfAnalysisSummaryTypeDef",
     {
         "WhatIfAnalysisArn": str,
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
         "Status": str,
@@ -1021,14 +1246,23 @@
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+SchemaAttributeOutputTypeDef = TypedDict(
+    "SchemaAttributeOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": AttributeTypeType,
+    },
+    total=False,
+)
+
 SchemaAttributeTypeDef = TypedDict(
     "SchemaAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeType": AttributeTypeType,
     },
     total=False,
@@ -1037,14 +1271,23 @@
 StopResourceRequestRequestTypeDef = TypedDict(
     "StopResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TimeSeriesConditionOutputTypeDef = TypedDict(
+    "TimeSeriesConditionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeValue": str,
+        "Condition": ConditionType,
+    },
+)
+
 TimeSeriesConditionTypeDef = TypedDict(
     "TimeSeriesConditionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
         "Condition": ConditionType,
     },
@@ -1062,14 +1305,34 @@
     "UpdateDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetArns": Sequence[str],
     },
 )
 
+_RequiredDataConfigOutputTypeDef = TypedDict(
+    "_RequiredDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalDataConfigOutputTypeDef = TypedDict(
+    "_OptionalDataConfigOutputTypeDef",
+    {
+        "AttributeConfigs": List[AttributeConfigOutputTypeDef],
+        "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
+    pass
+
+
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1077,17 +1340,19 @@
     {
         "AttributeConfigs": Sequence[AttributeConfigTypeDef],
         "AdditionalDatasets": Sequence[AdditionalDatasetTypeDef],
     },
     total=False,
 )
 
+
 class DataConfigTypeDef(_RequiredDataConfigTypeDef, _OptionalDataConfigTypeDef):
     pass
 
+
 PredictorBaselineTypeDef = TypedDict(
     "PredictorBaselineTypeDef",
     {
         "BaselineMetrics": List[BaselineMetricTypeDef],
     },
     total=False,
 )
@@ -1104,20 +1369,22 @@
     {
         "DatasetArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
         "ResourceArn": str,
     },
 )
@@ -1125,48 +1392,41 @@
     "_OptionalCreateMonitorRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ExplainabilitySummaryTypeDef = TypedDict(
-    "ExplainabilitySummaryTypeDef",
+DataDestinationOutputTypeDef = TypedDict(
+    "DataDestinationOutputTypeDef",
     {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
+        "S3Config": S3ConfigOutputTypeDef,
+    },
+)
+
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "S3Config": S3ConfigOutputTypeDef,
     },
-    total=False,
 )
 
 DataDestinationTypeDef = TypedDict(
     "DataDestinationTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
@@ -1209,31 +1469,69 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
+ExplainabilitySummaryTypeDef = TypedDict(
+    "ExplainabilitySummaryTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+    },
+    total=False,
+)
+
+_RequiredFeaturizationOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationOutputTypeDef",
+    {
+        "AttributeName": str,
+    },
+)
+_OptionalFeaturizationOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationOutputTypeDef",
+    {
+        "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class FeaturizationOutputTypeDef(
+    _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
+):
+    pass
+
+
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
     "_OptionalFeaturizationTypeDef",
     {
         "FeaturizationPipeline": Sequence[FeaturizationMethodTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
+
 ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1336,20 +1634,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
     _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
 )
 _OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
@@ -1358,20 +1658,22 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1487,31 +1789,64 @@
     {
         "Forecasts": List[ForecastSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "SupplementaryFeatures": List[SupplementaryFeatureOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
     "_OptionalInputDataConfigTypeDef",
     {
         "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
+
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
+
+ParameterRangesOutputTypeDef = TypedDict(
+    "ParameterRangesOutputTypeDef",
+    {
+        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
+        "ContinuousParameterRanges": List[ContinuousParameterRangeOutputTypeDef],
+        "IntegerParameterRanges": List[IntegerParameterRangeOutputTypeDef],
+    },
+    total=False,
+)
+
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
@@ -1523,14 +1858,22 @@
     {
         "Monitors": List[MonitorSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1579,204 +1922,122 @@
     {
         "AlgorithmArn": str,
         "TestWindows": List[TestWindowSummaryTypeDef],
     },
     total=False,
 )
 
-SchemaTypeDef = TypedDict(
-    "SchemaTypeDef",
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
     {
-        "Attributes": Sequence[SchemaAttributeTypeDef],
+        "Attributes": List[SchemaAttributeOutputTypeDef],
     },
     total=False,
 )
 
-TimeSeriesTransformationTypeDef = TypedDict(
-    "TimeSeriesTransformationTypeDef",
+SchemaTypeDef = TypedDict(
+    "SchemaTypeDef",
     {
-        "Action": ActionTypeDef,
-        "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
+        "Attributes": Sequence[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAutoPredictorRequestRequestTypeDef",
+TimeSeriesTransformationOutputTypeDef = TypedDict(
+    "TimeSeriesTransformationOutputTypeDef",
     {
-        "PredictorName": str,
+        "Action": ActionOutputTypeDef,
+        "TimeSeriesConditions": List[TimeSeriesConditionOutputTypeDef],
     },
+    total=False,
 )
-_OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAutoPredictorRequestRequestTypeDef",
+
+TimeSeriesTransformationTypeDef = TypedDict(
+    "TimeSeriesTransformationTypeDef",
     {
-        "ForecastHorizon": int,
-        "ForecastTypes": Sequence[str],
-        "ForecastDimensions": Sequence[str],
-        "ForecastFrequency": str,
-        "DataConfig": DataConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "ReferencePredictorArn": str,
-        "OptimizationMetric": OptimizationMetricType,
-        "ExplainPredictor": bool,
-        "Tags": Sequence[TagTypeDef],
-        "MonitorConfig": MonitorConfigTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "Action": ActionTypeDef,
+        "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
-class CreateAutoPredictorRequestRequestTypeDef(
-    _RequiredCreateAutoPredictorRequestRequestTypeDef,
-    _OptionalCreateAutoPredictorRequestRequestTypeDef,
-):
-    pass
-
 DescribeAutoPredictorResponseTypeDef = TypedDict(
     "DescribeAutoPredictorResponseTypeDef",
     {
         "PredictorArn": str,
         "PredictorName": str,
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "ForecastFrequency": str,
         "ForecastDimensions": List[str],
         "DatasetImportJobArns": List[str],
-        "DataConfig": DataConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
+        "DataConfig": DataConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigOutputTypeDef,
         "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ExplainabilityInfo": ExplainabilityInfoTypeDef,
         "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BaselineTypeDef = TypedDict(
-    "BaselineTypeDef",
-    {
-        "PredictorBaseline": PredictorBaselineTypeDef,
-    },
-    total=False,
-)
-
-ListExplainabilitiesResponseTypeDef = TypedDict(
-    "ListExplainabilitiesResponseTypeDef",
-    {
-        "Explainabilities": List[ExplainabilitySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
+_RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
-        "ExplainabilityExportName": str,
-        "ExplainabilityArn": str,
-        "Destination": DataDestinationTypeDef,
+        "PredictorName": str,
     },
 )
-_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
+_OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutoPredictorRequestRequestTypeDef",
     {
+        "ForecastHorizon": int,
+        "ForecastTypes": Sequence[str],
+        "ForecastDimensions": Sequence[str],
+        "ForecastFrequency": str,
+        "DataConfig": DataConfigTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "ReferencePredictorArn": str,
+        "OptimizationMetric": OptimizationMetricType,
+        "ExplainPredictor": bool,
         "Tags": Sequence[TagTypeDef],
-        "Format": str,
+        "MonitorConfig": MonitorConfigTypeDef,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
     },
     total=False,
 )
 
-class CreateExplainabilityExportRequestRequestTypeDef(
-    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
-    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "ForecastExportJobName": str,
-        "ForecastArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
 
-class CreateForecastExportJobRequestRequestTypeDef(
-    _RequiredCreateForecastExportJobRequestRequestTypeDef,
-    _OptionalCreateForecastExportJobRequestRequestTypeDef,
+class CreateAutoPredictorRequestRequestTypeDef(
+    _RequiredCreateAutoPredictorRequestRequestTypeDef,
+    _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
-    {
-        "PredictorBacktestExportJobName": str,
-        "PredictorArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-class CreatePredictorBacktestExportJobRequestRequestTypeDef(
-    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
-    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
-):
-    pass
 
-_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
-    {
-        "WhatIfForecastExportName": str,
-        "WhatIfForecastArns": Sequence[str],
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
+BaselineTypeDef = TypedDict(
+    "BaselineTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
+        "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
 
-class CreateWhatIfForecastExportRequestRequestTypeDef(
-    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
-    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
-):
-    pass
-
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1784,15 +2045,15 @@
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
         "ForecastArn": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1800,15 +2061,15 @@
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1816,15 +2077,15 @@
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": List[str],
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1832,100 +2093,72 @@
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 ForecastExportJobSummaryTypeDef = TypedDict(
     "ForecastExportJobSummaryTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 PredictorBacktestExportJobSummaryTypeDef = TypedDict(
     "PredictorBacktestExportJobSummaryTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 WhatIfForecastExportSummaryTypeDef = TypedDict(
     "WhatIfForecastExportSummaryTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastArns": List[str],
         "WhatIfForecastExportName": str,
-        "Destination": DataDestinationTypeDef,
+        "Destination": DataDestinationOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
-    {
-        "DatasetImportJobName": str,
-        "DatasetArn": str,
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
-    {
-        "TimestampFormat": str,
-        "TimeZone": str,
-        "UseGeolocationForTimeZone": bool,
-        "GeolocationFormat": str,
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-        "ImportMode": ImportModeType,
-    },
-    total=False,
-)
-
-class CreateDatasetImportJobRequestRequestTypeDef(
-    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
-    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
-):
-    pass
-
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
-        "DataSource": DataSourceTypeDef,
+        "DataSource": DataSourceOutputTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "ImportMode": ImportModeType,
     },
     total=False,
@@ -1937,37 +2170,198 @@
         "DatasetImportJobName": str,
         "DatasetImportJobArn": str,
         "DatasetArn": str,
         "TimestampFormat": str,
         "TimeZone": str,
         "UseGeolocationForTimeZone": bool,
         "GeolocationFormat": str,
-        "DataSource": DataSourceTypeDef,
+        "DataSource": DataSourceOutputTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "FieldStatistics": Dict[str, StatisticsTypeDef],
         "DataSize": float,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "ExplainabilityExportName": str,
+        "ExplainabilityArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreateExplainabilityExportRequestRequestTypeDef(
+    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
+    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "ForecastExportJobName": str,
+        "ForecastArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreateForecastExportJobRequestRequestTypeDef(
+    _RequiredCreateForecastExportJobRequestRequestTypeDef,
+    _OptionalCreateForecastExportJobRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "PredictorBacktestExportJobName": str,
+        "PredictorArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreatePredictorBacktestExportJobRequestRequestTypeDef(
+    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
+    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "WhatIfForecastExportName": str,
+        "WhatIfForecastArns": Sequence[str],
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreateWhatIfForecastExportRequestRequestTypeDef(
+    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
+    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
+    {
+        "DatasetImportJobName": str,
+        "DatasetArn": str,
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
+    {
+        "TimestampFormat": str,
+        "TimeZone": str,
+        "UseGeolocationForTimeZone": bool,
+        "GeolocationFormat": str,
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+        "ImportMode": ImportModeType,
+    },
+    total=False,
+)
+
+
+class CreateDatasetImportJobRequestRequestTypeDef(
+    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
+    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
+):
+    pass
+
+
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListExplainabilitiesResponseTypeDef = TypedDict(
+    "ListExplainabilitiesResponseTypeDef",
+    {
+        "Explainabilities": List[ExplainabilitySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredFeaturizationConfigOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastFrequency": str,
+    },
+)
+_OptionalFeaturizationConfigOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastDimensions": List[str],
+        "Featurizations": List[FeaturizationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class FeaturizationConfigOutputTypeDef(
+    _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -1975,19 +2369,29 @@
     {
         "ForecastDimensions": Sequence[str],
         "Featurizations": Sequence[FeaturizationTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
+
+HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigOutputTypeDef",
+    {
+        "ParameterRanges": ParameterRangesOutputTypeDef,
+    },
+    total=False,
+)
+
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
     {
         "ParameterRanges": ParameterRangesTypeDef,
     },
     total=False,
 )
@@ -2017,14 +2421,86 @@
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
     },
     total=False,
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": str,
+        "Domain": DomainType,
+        "DatasetType": DatasetTypeType,
+        "DataFrequency": str,
+        "Schema": SchemaOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeExplainabilityResponseTypeDef = TypedDict(
+    "DescribeExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
+        "EnableVisualization": bool,
+        "DataSource": DataSourceOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "StartDateTime": str,
+        "EndDateTime": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Message": str,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TimeSeriesIdentifiersOutputTypeDef = TypedDict(
+    "TimeSeriesIdentifiersOutputTypeDef",
+    {
+        "DataSource": DataSourceOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "Format": str,
+    },
+    total=False,
+)
+
+_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "S3Config": S3ConfigOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+)
+_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "Format": str,
+        "TimestampFormat": str,
+    },
+    total=False,
+)
+
+
+class TimeSeriesReplacementsDataSourceOutputTypeDef(
+    _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
+    _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2036,19 +2512,21 @@
         "DataFrequency": str,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateExplainabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
     },
@@ -2062,57 +2540,21 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "DatasetName": str,
-        "Domain": DomainType,
-        "DatasetType": DatasetTypeType,
-        "DataFrequency": str,
-        "Schema": SchemaTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeExplainabilityResponseTypeDef = TypedDict(
-    "DescribeExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "EnableVisualization": bool,
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaTypeDef,
-        "StartDateTime": str,
-        "EndDateTime": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Message": str,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
@@ -2132,20 +2574,22 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
+
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
+
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2228,19 +2672,21 @@
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OptimizationMetric": OptimizationMetricType,
     },
     total=False,
 )
 
+
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
+
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2255,32 +2701,58 @@
         "AutoMLAlgorithmArns": List[str],
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
-        "EvaluationParameters": EvaluationParametersTypeDef,
-        "HPOConfig": HyperParameterTuningJobConfigTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "FeaturizationConfig": FeaturizationConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
+        "EvaluationParameters": EvaluationParametersOutputTypeDef,
+        "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigOutputTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TimeSeriesSelectorOutputTypeDef = TypedDict(
+    "TimeSeriesSelectorOutputTypeDef",
+    {
+        "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
+    },
+    total=False,
+)
+
+DescribeWhatIfForecastResponseTypeDef = TypedDict(
+    "DescribeWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastName": str,
+        "WhatIfForecastArn": str,
+        "WhatIfAnalysisArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
+        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
+        "ForecastTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
@@ -2298,45 +2770,63 @@
         "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
-DescribeWhatIfForecastResponseTypeDef = TypedDict(
-    "DescribeWhatIfForecastResponseTypeDef",
+
+GetAccuracyMetricsResponseTypeDef = TypedDict(
+    "GetAccuracyMetricsResponseTypeDef",
     {
-        "WhatIfForecastName": str,
-        "WhatIfForecastArn": str,
-        "WhatIfAnalysisArn": str,
+        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
+        "IsAutoPredictor": bool,
+        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
+        "OptimizationMetric": OptimizationMetricType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeForecastResponseTypeDef = TypedDict(
+    "DescribeForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ForecastName": str,
+        "ForecastTypes": List[str],
+        "PredictorArn": str,
+        "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
-        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
-        "ForecastTypes": List[str],
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccuracyMetricsResponseTypeDef = TypedDict(
-    "GetAccuracyMetricsResponseTypeDef",
+DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
+    "DescribeWhatIfAnalysisResponseTypeDef",
     {
-        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
-        "IsAutoPredictor": bool,
-        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
-        "OptimizationMetric": OptimizationMetricType,
+        "WhatIfAnalysisName": str,
+        "WhatIfAnalysisArn": str,
+        "ForecastArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
@@ -2350,19 +2840,21 @@
         "ForecastTypes": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
     },
     total=False,
 )
 
+
 class CreateForecastRequestRequestTypeDef(
     _RequiredCreateForecastRequestRequestTypeDef, _OptionalCreateForecastRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
     },
 )
@@ -2371,46 +2863,13 @@
     {
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
-
-DescribeForecastResponseTypeDef = TypedDict(
-    "DescribeForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ForecastName": str,
-        "ForecastTypes": List[str],
-        "PredictorArn": str,
-        "DatasetGroupArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
-    "DescribeWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisName": str,
-        "WhatIfAnalysisArn": str,
-        "ForecastArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/PKG-INFO` & `mypy-boto3-forecast-1.28.12/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-forecast
-Version: 1.28.0
-Summary: Type annotations for boto3.ForecastService 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 forecast type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-forecast?color=blue)](https://pypistats.org/packages/mypy-boto3-forecast)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,19 +364,24 @@
 ### Typed dictionaries
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
+    ActionOutputTypeDef,
     ActionTypeDef,
+    AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
+    AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
+    CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
+    ContinuousParameterRangeOutputTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
     CreateAutoPredictorResponseTypeDef,
     CreateDatasetGroupResponseTypeDef,
@@ -422,14 +395,15 @@
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -440,73 +414,86 @@
     DeletePredictorBacktestExportJobRequestRequestTypeDef,
     DeletePredictorRequestRequestTypeDef,
     DeleteResourceTreeRequestRequestTypeDef,
     DeleteWhatIfAnalysisRequestRequestTypeDef,
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
+    TimeAlignmentBoundaryOutputTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
+    ExplainabilityConfigOutputTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
+    EvaluationParametersOutputTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
+    FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
+    SupplementaryFeatureOutputTypeDef,
     SupplementaryFeatureTypeDef,
+    IntegerParameterRangeOutputTypeDef,
     IntegerParameterRangeTypeDef,
     ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
     PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
     ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
+    SchemaAttributeOutputTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
+    TimeSeriesConditionOutputTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExplainabilitySummaryTypeDef,
+    DataDestinationOutputTypeDef,
+    DataSourceOutputTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
+    ExplainabilitySummaryTypeDef,
+    FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
     ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
     ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
     ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
@@ -525,76 +512,86 @@
     ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
     ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
     ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
     ListMonitorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
-    CreateAutoPredictorRequestRequestTypeDef,
     DescribeAutoPredictorResponseTypeDef,
+    CreateAutoPredictorRequestRequestTypeDef,
     BaselineTypeDef,
-    ListExplainabilitiesResponseTypeDef,
-    CreateExplainabilityExportRequestRequestTypeDef,
-    CreateForecastExportJobRequestRequestTypeDef,
-    CreatePredictorBacktestExportJobRequestRequestTypeDef,
-    CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
     DescribeForecastExportJobResponseTypeDef,
     DescribePredictorBacktestExportJobResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     ExplainabilityExportSummaryTypeDef,
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
-    CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
+    CreateExplainabilityExportRequestRequestTypeDef,
+    CreateForecastExportJobRequestRequestTypeDef,
+    CreatePredictorBacktestExportJobRequestRequestTypeDef,
+    CreateWhatIfForecastExportRequestRequestTypeDef,
+    CreateDatasetImportJobRequestRequestTypeDef,
     ListPredictorsResponseTypeDef,
+    ListExplainabilitiesResponseTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    CreateExplainabilityRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
+    TimeSeriesIdentifiersOutputTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    CreateExplainabilityRequestRequestTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     CreatePredictorRequestRequestTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
+    DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
-    DescribeWhatIfForecastResponseTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    CreateForecastRequestRequestTypeDef,
-    CreateWhatIfAnalysisRequestRequestTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
+    CreateForecastRequestRequestTypeDef,
+    CreateWhatIfAnalysisRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_structure() -> ActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.0/mypy_boto3_forecast.egg-info/SOURCES.txt` & `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.0/setup.py` & `mypy-boto3-forecast-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-forecast",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ForecastService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ForecastService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

