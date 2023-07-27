# Comparing `tmp/mypy-boto3-frauddetector-1.28.0.tar.gz` & `tmp/mypy-boto3-frauddetector-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-frauddetector-1.28.0.tar", last modified: Thu Jul  6 20:59:37 2023, max compression
+gzip compressed data, was "mypy-boto3-frauddetector-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
```

## Comparing `mypy-boto3-frauddetector-1.28.0.tar` & `mypy-boto3-frauddetector-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.394307 mypy-boto3-frauddetector-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-07-06 20:59:37.394307 mypy-boto3-frauddetector-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17364 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.378307 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46336 2023-07-06 20:41:22.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-07-06 20:41:22.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-06 20:41:22.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-06 20:41:22.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59398 2023-07-06 20:41:24.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59331 2023-07-06 20:41:23.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.394307 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-07-06 20:59:37.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 20:59:37.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:37.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:37.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:37.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:37.000000 mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:37.394307 mypy-boto3-frauddetector-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-06 20:41:21.000000 mypy-boto3-frauddetector-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.968506 mypy-boto3-frauddetector-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-27 05:34:42.964506 mypy-boto3-frauddetector-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.964506 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46336 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63313 2023-07-27 05:22:30.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63238 2023-07-27 05:22:30.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.964506 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.968506 mypy-boto3-frauddetector-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/setup.py
```

### Comparing `mypy-boto3-frauddetector-1.28.0/LICENSE` & `mypy-boto3-frauddetector-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.0/PKG-INFO` & `mypy-boto3-frauddetector-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.0
-Summary: Type annotations for boto3.FraudDetector 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.FraudDetector 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-frauddetector"></a>
 
 # mypy-boto3-frauddetector
 
 [![PyPI - mypy-boto3-frauddetector](https://img.shields.io/pypi/v/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,14 +332,15 @@
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
     CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
     CreateModelVersionResultTypeDef,
+    RuleOutputTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
@@ -354,31 +355,35 @@
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
+    EntityOutputTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
+    EventOrchestrationOutputTypeDef,
     EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
+    ExternalEventsDetailOutputTypeDef,
     ExternalModelSummaryTypeDef,
-    ModelInputConfigurationTypeDef,
-    ModelOutputConfigurationTypeDef,
+    ModelInputConfigurationOutputTypeDef,
+    ModelOutputConfigurationOutputTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
+    ModelVersionOutputTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
@@ -393,20 +398,25 @@
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
     GetVariablesRequestRequestTypeDef,
+    IngestedEventsTimeWindowOutputTypeDef,
     IngestedEventsTimeWindowTypeDef,
+    LabelSchemaOutputTypeDef,
     LabelSchemaTypeDef,
     PredictionTimeRangeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
+    ModelInputConfigurationTypeDef,
+    ModelOutputConfigurationTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -424,67 +434,69 @@
     BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
-    ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
-    CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
     UpdateRuleVersionRequestRequestTypeDef,
+    CreateRuleResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    PutExternalModelRequestRequestTypeDef,
+    GetDetectorVersionResultTypeDef,
+    ModelScoresTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
+    IngestedEventsDetailOutputTypeDef,
     IngestedEventsDetailTypeDef,
+    TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
+    PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
-    GetEventPredictionResultTypeDef,
     GetExternalModelsResultTypeDef,
+    GetEventPredictionResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
-    CreateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
+    CreateModelVersionRequestRequestTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
     TrainingMetricsV2TypeDef,
     EvaluatedModelVersionTypeDef,
     TrainingResultV2TypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.28.0/README.md` & `mypy-boto3-frauddetector-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-frauddetector"></a>
 
 # mypy-boto3-frauddetector
 
 [![PyPI - mypy-boto3-frauddetector](https://img.shields.io/pypi/v/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,14 +300,15 @@
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
     CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
     CreateModelVersionResultTypeDef,
+    RuleOutputTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
@@ -322,31 +323,35 @@
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
+    EntityOutputTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
+    EventOrchestrationOutputTypeDef,
     EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
+    ExternalEventsDetailOutputTypeDef,
     ExternalModelSummaryTypeDef,
-    ModelInputConfigurationTypeDef,
-    ModelOutputConfigurationTypeDef,
+    ModelInputConfigurationOutputTypeDef,
+    ModelOutputConfigurationOutputTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
+    ModelVersionOutputTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
@@ -361,20 +366,25 @@
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
     GetVariablesRequestRequestTypeDef,
+    IngestedEventsTimeWindowOutputTypeDef,
     IngestedEventsTimeWindowTypeDef,
+    LabelSchemaOutputTypeDef,
     LabelSchemaTypeDef,
     PredictionTimeRangeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
+    ModelInputConfigurationTypeDef,
+    ModelOutputConfigurationTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -392,67 +402,69 @@
     BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
-    ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
-    CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
     UpdateRuleVersionRequestRequestTypeDef,
+    CreateRuleResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    PutExternalModelRequestRequestTypeDef,
+    GetDetectorVersionResultTypeDef,
+    ModelScoresTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
+    IngestedEventsDetailOutputTypeDef,
     IngestedEventsDetailTypeDef,
+    TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
+    PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
-    GetEventPredictionResultTypeDef,
     GetExternalModelsResultTypeDef,
+    GetEventPredictionResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
-    CreateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
+    CreateModelVersionRequestRequestTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
     TrainingMetricsV2TypeDef,
     EvaluatedModelVersionTypeDef,
     TrainingResultV2TypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/__main__.py` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FraudDetector 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.FraudDetector 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
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

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/client.py` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/client.pyi` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/literals.py` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,15 @@
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
@@ -270,26 +271,28 @@
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

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/literals.pyi` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
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
@@ -268,26 +269,28 @@
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

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/type_defs.py` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
     "CreateDetectorVersionResultTypeDef",
     "ExternalEventsDetailTypeDef",
     "CreateModelVersionResultTypeDef",
+    "RuleOutputTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
     "DeleteBatchImportJobRequestRequestTypeDef",
     "DeleteBatchPredictionJobRequestRequestTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
@@ -82,31 +83,35 @@
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
     "DescribeDetectorRequestRequestTypeDef",
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
     "DetectorTypeDef",
+    "EntityOutputTypeDef",
     "EntityTypeDef",
     "EntityTypeTypeDef",
     "EvaluatedExternalModelTypeDef",
     "EvaluatedRuleTypeDef",
+    "EventOrchestrationOutputTypeDef",
     "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
+    "ExternalEventsDetailOutputTypeDef",
     "ExternalModelSummaryTypeDef",
-    "ModelInputConfigurationTypeDef",
-    "ModelOutputConfigurationTypeDef",
+    "ModelInputConfigurationOutputTypeDef",
+    "ModelOutputConfigurationOutputTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusResultTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
+    "ModelVersionOutputTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
     "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
@@ -121,20 +126,25 @@
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
     "GetVariablesRequestRequestTypeDef",
+    "IngestedEventsTimeWindowOutputTypeDef",
     "IngestedEventsTimeWindowTypeDef",
+    "LabelSchemaOutputTypeDef",
     "LabelSchemaTypeDef",
     "PredictionTimeRangeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
+    "ModelInputConfigurationTypeDef",
+    "ModelOutputConfigurationTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -152,67 +162,69 @@
     "BatchCreateVariableResultTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
     "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
     "PutOutcomeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
-    "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
-    "CreateRuleResultTypeDef",
     "DeleteRuleRequestRequestTypeDef",
-    "GetDetectorVersionResultTypeDef",
     "UpdateDetectorVersionRequestRequestTypeDef",
     "UpdateRuleMetadataRequestRequestTypeDef",
     "UpdateRuleVersionRequestRequestTypeDef",
+    "CreateRuleResultTypeDef",
     "UpdateRuleVersionResultTypeDef",
     "DataValidationMetricsTypeDef",
     "DescribeDetectorResultTypeDef",
     "GetDetectorsResultTypeDef",
     "EventTypeDef",
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
-    "PutExternalModelRequestRequestTypeDef",
+    "GetDetectorVersionResultTypeDef",
+    "ModelScoresTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
+    "IngestedEventsDetailOutputTypeDef",
     "IngestedEventsDetailTypeDef",
+    "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
+    "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
-    "GetEventPredictionResultTypeDef",
     "GetExternalModelsResultTypeDef",
+    "GetEventPredictionResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
-    "CreateModelVersionRequestRequestTypeDef",
     "GetModelVersionResultTypeDef",
+    "CreateModelVersionRequestRequestTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
     "TrainingMetricsV2TypeDef",
     "EvaluatedModelVersionTypeDef",
     "TrainingResultV2TypeDef",
@@ -456,14 +468,23 @@
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "detectorId": str,
+        "ruleId": str,
+        "ruleVersion": str,
+    },
+)
+
 FieldValidationMessageTypeDef = TypedDict(
     "FieldValidationMessageTypeDef",
     {
         "fieldName": str,
         "identifier": str,
         "title": str,
         "content": str,
@@ -669,14 +690,22 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
+EntityOutputTypeDef = TypedDict(
+    "EntityOutputTypeDef",
+    {
+        "entityType": str,
+        "entityId": str,
+    },
+)
+
 EntityTypeDef = TypedDict(
     "EntityTypeDef",
     {
         "entityType": str,
         "entityId": str,
     },
 )
@@ -714,14 +743,21 @@
         "outcomes": List[str],
         "evaluated": bool,
         "matched": bool,
     },
     total=False,
 )
 
+EventOrchestrationOutputTypeDef = TypedDict(
+    "EventOrchestrationOutputTypeDef",
+    {
+        "eventBridgeEnabled": bool,
+    },
+)
+
 EventOrchestrationTypeDef = TypedDict(
     "EventOrchestrationTypeDef",
     {
         "eventBridgeEnabled": bool,
     },
 )
 
@@ -756,65 +792,73 @@
         "name": str,
         "value": str,
         "source": str,
     },
     total=False,
 )
 
+ExternalEventsDetailOutputTypeDef = TypedDict(
+    "ExternalEventsDetailOutputTypeDef",
+    {
+        "dataLocation": str,
+        "dataAccessRoleArn": str,
+    },
+)
+
 ExternalModelSummaryTypeDef = TypedDict(
     "ExternalModelSummaryTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
     },
     total=False,
 )
 
-_RequiredModelInputConfigurationTypeDef = TypedDict(
-    "_RequiredModelInputConfigurationTypeDef",
+_RequiredModelInputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredModelInputConfigurationOutputTypeDef",
     {
         "useEventVariables": bool,
     },
 )
-_OptionalModelInputConfigurationTypeDef = TypedDict(
-    "_OptionalModelInputConfigurationTypeDef",
+_OptionalModelInputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalModelInputConfigurationOutputTypeDef",
     {
         "eventTypeName": str,
         "format": ModelInputDataFormatType,
         "jsonInputTemplate": str,
         "csvInputTemplate": str,
     },
     total=False,
 )
 
 
-class ModelInputConfigurationTypeDef(
-    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
+class ModelInputConfigurationOutputTypeDef(
+    _RequiredModelInputConfigurationOutputTypeDef, _OptionalModelInputConfigurationOutputTypeDef
 ):
     pass
 
 
-_RequiredModelOutputConfigurationTypeDef = TypedDict(
-    "_RequiredModelOutputConfigurationTypeDef",
+_RequiredModelOutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredModelOutputConfigurationOutputTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
-_OptionalModelOutputConfigurationTypeDef = TypedDict(
-    "_OptionalModelOutputConfigurationTypeDef",
+_OptionalModelOutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalModelOutputConfigurationOutputTypeDef",
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
 
-class ModelOutputConfigurationTypeDef(
-    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
+class ModelOutputConfigurationOutputTypeDef(
+    _RequiredModelOutputConfigurationOutputTypeDef, _OptionalModelOutputConfigurationOutputTypeDef
 ):
     pass
 
 
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
@@ -863,14 +907,37 @@
     "GetDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
     },
 )
 
+_RequiredModelVersionOutputTypeDef = TypedDict(
+    "_RequiredModelVersionOutputTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+    },
+)
+_OptionalModelVersionOutputTypeDef = TypedDict(
+    "_OptionalModelVersionOutputTypeDef",
+    {
+        "arn": str,
+    },
+    total=False,
+)
+
+
+class ModelVersionOutputTypeDef(
+    _RequiredModelVersionOutputTypeDef, _OptionalModelVersionOutputTypeDef
+):
+    pass
+
+
 GetDetectorsRequestRequestTypeDef = TypedDict(
     "GetDetectorsRequestRequestTypeDef",
     {
         "detectorId": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1118,22 +1185,39 @@
         "name": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+IngestedEventsTimeWindowOutputTypeDef = TypedDict(
+    "IngestedEventsTimeWindowOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+    },
+)
+
 IngestedEventsTimeWindowTypeDef = TypedDict(
     "IngestedEventsTimeWindowTypeDef",
     {
         "startTime": str,
         "endTime": str,
     },
 )
 
+LabelSchemaOutputTypeDef = TypedDict(
+    "LabelSchemaOutputTypeDef",
+    {
+        "labelMapper": Dict[str, List[str]],
+        "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
+    },
+    total=False,
+)
+
 LabelSchemaTypeDef = TypedDict(
     "LabelSchemaTypeDef",
     {
         "labelMapper": Mapping[str, Sequence[str]],
         "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
     },
     total=False,
@@ -1166,14 +1250,22 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 LogOddsMetricTypeDef = TypedDict(
     "LogOddsMetricTypeDef",
     {
         "variableName": str,
         "variableType": str,
         "variableImportance": float,
     },
@@ -1186,14 +1278,60 @@
         "precision": float,
         "tpr": float,
         "threshold": float,
     },
     total=False,
 )
 
+_RequiredModelInputConfigurationTypeDef = TypedDict(
+    "_RequiredModelInputConfigurationTypeDef",
+    {
+        "useEventVariables": bool,
+    },
+)
+_OptionalModelInputConfigurationTypeDef = TypedDict(
+    "_OptionalModelInputConfigurationTypeDef",
+    {
+        "eventTypeName": str,
+        "format": ModelInputDataFormatType,
+        "jsonInputTemplate": str,
+        "csvInputTemplate": str,
+    },
+    total=False,
+)
+
+
+class ModelInputConfigurationTypeDef(
+    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
+):
+    pass
+
+
+_RequiredModelOutputConfigurationTypeDef = TypedDict(
+    "_RequiredModelOutputConfigurationTypeDef",
+    {
+        "format": ModelOutputDataFormatType,
+    },
+)
+_OptionalModelOutputConfigurationTypeDef = TypedDict(
+    "_OptionalModelOutputConfigurationTypeDef",
+    {
+        "jsonKeyToVariableMap": Mapping[str, str],
+        "csvIndexToVariableMap": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class ModelOutputConfigurationTypeDef(
+    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
+):
+    pass
+
+
 OFIMetricDataPointTypeDef = TypedDict(
     "OFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1558,23 +1696,14 @@
 
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1722,23 +1851,14 @@
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModelScoresTypeDef = TypedDict(
-    "ModelScoresTypeDef",
-    {
-        "modelVersion": ModelVersionTypeDef,
-        "scores": Dict[str, float],
-    },
-    total=False,
-)
-
 _RequiredCreateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "rules": Sequence[RuleTypeDef],
     },
 )
@@ -1758,47 +1878,21 @@
 class CreateDetectorVersionRequestRequestTypeDef(
     _RequiredCreateDetectorVersionRequestRequestTypeDef,
     _OptionalCreateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateRuleResultTypeDef = TypedDict(
-    "CreateRuleResultTypeDef",
-    {
-        "rule": RuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
     },
 )
 
-GetDetectorVersionResultTypeDef = TypedDict(
-    "GetDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "description": str,
-        "externalModelEndpoints": List[str],
-        "modelVersions": List[ModelVersionTypeDef],
-        "rules": List[RuleTypeDef],
-        "status": DetectorVersionStatusType,
-        "lastUpdatedTime": str,
-        "createdTime": str,
-        "ruleExecutionMode": RuleExecutionModeType,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
         "externalModelEndpoints": Sequence[str],
         "rules": Sequence[RuleTypeDef],
@@ -1851,18 +1945,26 @@
 
 class UpdateRuleVersionRequestRequestTypeDef(
     _RequiredUpdateRuleVersionRequestRequestTypeDef, _OptionalUpdateRuleVersionRequestRequestTypeDef
 ):
     pass
 
 
+CreateRuleResultTypeDef = TypedDict(
+    "CreateRuleResultTypeDef",
+    {
+        "rule": RuleOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
-        "rule": RuleTypeDef,
+        "rule": RuleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataValidationMetricsTypeDef = TypedDict(
     "DataValidationMetricsTypeDef",
     {
@@ -1897,15 +1999,15 @@
     {
         "eventId": str,
         "eventTypeName": str,
         "eventTimestamp": str,
         "eventVariables": Dict[str, str],
         "currentLabel": str,
         "labelTimestamp": str,
-        "entities": List[EntityTypeDef],
+        "entities": List[EntityOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
@@ -1986,15 +2088,15 @@
         "labels": List[str],
         "entityTypes": List[str],
         "eventIngestion": EventIngestionType,
         "ingestedEventStatistics": IngestedEventStatisticsTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
-        "eventOrchestration": EventOrchestrationTypeDef,
+        "eventOrchestration": EventOrchestrationOutputTypeDef,
     },
     total=False,
 )
 
 ExternalModelOutputsTypeDef = TypedDict(
     "ExternalModelOutputsTypeDef",
     {
@@ -2006,50 +2108,51 @@
 
 ExternalModelTypeDef = TypedDict(
     "ExternalModelTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationTypeDef,
+        "inputConfiguration": ModelInputConfigurationOutputTypeDef,
+        "outputConfiguration": ModelOutputConfigurationOutputTypeDef,
         "modelEndpointStatus": ModelEndpointStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_RequiredPutExternalModelRequestRequestTypeDef",
+GetDetectorVersionResultTypeDef = TypedDict(
+    "GetDetectorVersionResultTypeDef",
     {
-        "modelEndpoint": str,
-        "modelSource": Literal["SAGEMAKER"],
-        "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationTypeDef,
-        "modelEndpointStatus": ModelEndpointStatusType,
+        "detectorId": str,
+        "detectorVersionId": str,
+        "description": str,
+        "externalModelEndpoints": List[str],
+        "modelVersions": List[ModelVersionOutputTypeDef],
+        "rules": List[RuleOutputTypeDef],
+        "status": DetectorVersionStatusType,
+        "lastUpdatedTime": str,
+        "createdTime": str,
+        "ruleExecutionMode": RuleExecutionModeType,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_OptionalPutExternalModelRequestRequestTypeDef",
+
+ModelScoresTypeDef = TypedDict(
+    "ModelScoresTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "modelVersion": ModelVersionOutputTypeDef,
+        "scores": Dict[str, float],
     },
     total=False,
 )
 
-
-class PutExternalModelRequestRequestTypeDef(
-    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
     "_RequiredGetEventPredictionRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventId": str,
         "eventTypeName": str,
         "entities": Sequence[EntityTypeDef],
@@ -2114,21 +2217,49 @@
     {
         "ruleDetails": List[RuleDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IngestedEventsDetailOutputTypeDef = TypedDict(
+    "IngestedEventsDetailOutputTypeDef",
+    {
+        "ingestedEventsTimeWindow": IngestedEventsTimeWindowOutputTypeDef,
+    },
+)
+
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
     },
 )
 
+_RequiredTrainingDataSchemaOutputTypeDef = TypedDict(
+    "_RequiredTrainingDataSchemaOutputTypeDef",
+    {
+        "modelVariables": List[str],
+    },
+)
+_OptionalTrainingDataSchemaOutputTypeDef = TypedDict(
+    "_OptionalTrainingDataSchemaOutputTypeDef",
+    {
+        "labelSchema": LabelSchemaOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TrainingDataSchemaOutputTypeDef(
+    _RequiredTrainingDataSchemaOutputTypeDef, _OptionalTrainingDataSchemaOutputTypeDef
+):
+    pass
+
+
 _RequiredTrainingDataSchemaTypeDef = TypedDict(
     "_RequiredTrainingDataSchemaTypeDef",
     {
         "modelVariables": Sequence[str],
     },
 )
 _OptionalTrainingDataSchemaTypeDef = TypedDict(
@@ -2156,14 +2287,23 @@
         "predictionTimeRange": PredictionTimeRangeTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VariableImportanceMetricsTypeDef = TypedDict(
     "VariableImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[LogOddsMetricTypeDef],
     },
     total=False,
 )
@@ -2173,14 +2313,40 @@
     {
         "auc": float,
         "metricDataPoints": List[MetricDataPointTypeDef],
     },
     total=False,
 )
 
+_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_RequiredPutExternalModelRequestRequestTypeDef",
+    {
+        "modelEndpoint": str,
+        "modelSource": Literal["SAGEMAKER"],
+        "invokeModelEndpointRoleArn": str,
+        "inputConfiguration": ModelInputConfigurationTypeDef,
+        "outputConfiguration": ModelOutputConfigurationTypeDef,
+        "modelEndpointStatus": ModelEndpointStatusType,
+    },
+)
+_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_OptionalPutExternalModelRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutExternalModelRequestRequestTypeDef(
+    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
+):
+    pass
+
+
 OFIModelPerformanceTypeDef = TypedDict(
     "OFIModelPerformanceTypeDef",
     {
         "auc": float,
         "uncertaintyRange": UncertaintyRangeTypeDef,
     },
     total=False,
@@ -2217,29 +2383,29 @@
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEventPredictionResultTypeDef = TypedDict(
-    "GetEventPredictionResultTypeDef",
+GetExternalModelsResultTypeDef = TypedDict(
+    "GetExternalModelsResultTypeDef",
     {
-        "modelScores": List[ModelScoresTypeDef],
-        "ruleResults": List[RuleResultTypeDef],
-        "externalModelOutputs": List[ExternalModelOutputsTypeDef],
+        "externalModels": List[ExternalModelTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetExternalModelsResultTypeDef = TypedDict(
-    "GetExternalModelsResultTypeDef",
+GetEventPredictionResultTypeDef = TypedDict(
+    "GetEventPredictionResultTypeDef",
     {
-        "externalModels": List[ExternalModelTypeDef],
-        "nextToken": str,
+        "modelScores": List[ModelScoresTypeDef],
+        "ruleResults": List[RuleResultTypeDef],
+        "externalModelOutputs": List[ExternalModelOutputsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelVersionRequestRequestTypeDef",
     {
@@ -2262,14 +2428,30 @@
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
 
+GetModelVersionResultTypeDef = TypedDict(
+    "GetModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "trainingDataSource": TrainingDataSourceEnumType,
+        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
+        "status": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
@@ -2289,30 +2471,14 @@
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
 
-GetModelVersionResultTypeDef = TypedDict(
-    "GetModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaTypeDef,
-        "externalEventsDetail": ExternalEventsDetailTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
-        "status": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
@@ -2405,17 +2571,17 @@
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaTypeDef,
-        "externalEventsDetail": ExternalEventsDetailTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
+        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
         "trainingResult": TrainingResultTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
         "trainingResultV2": TrainingResultV2TypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector/type_defs.pyi` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
     "CreateDetectorVersionResultTypeDef",
     "ExternalEventsDetailTypeDef",
     "CreateModelVersionResultTypeDef",
+    "RuleOutputTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
     "DeleteBatchImportJobRequestRequestTypeDef",
     "DeleteBatchPredictionJobRequestRequestTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
@@ -81,31 +82,35 @@
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
     "DescribeDetectorRequestRequestTypeDef",
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
     "DetectorTypeDef",
+    "EntityOutputTypeDef",
     "EntityTypeDef",
     "EntityTypeTypeDef",
     "EvaluatedExternalModelTypeDef",
     "EvaluatedRuleTypeDef",
+    "EventOrchestrationOutputTypeDef",
     "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
+    "ExternalEventsDetailOutputTypeDef",
     "ExternalModelSummaryTypeDef",
-    "ModelInputConfigurationTypeDef",
-    "ModelOutputConfigurationTypeDef",
+    "ModelInputConfigurationOutputTypeDef",
+    "ModelOutputConfigurationOutputTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusResultTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
+    "ModelVersionOutputTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
     "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
@@ -120,20 +125,25 @@
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
     "GetVariablesRequestRequestTypeDef",
+    "IngestedEventsTimeWindowOutputTypeDef",
     "IngestedEventsTimeWindowTypeDef",
+    "LabelSchemaOutputTypeDef",
     "LabelSchemaTypeDef",
     "PredictionTimeRangeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
+    "ModelInputConfigurationTypeDef",
+    "ModelOutputConfigurationTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -151,67 +161,69 @@
     "BatchCreateVariableResultTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
     "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
     "PutOutcomeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
-    "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
-    "CreateRuleResultTypeDef",
     "DeleteRuleRequestRequestTypeDef",
-    "GetDetectorVersionResultTypeDef",
     "UpdateDetectorVersionRequestRequestTypeDef",
     "UpdateRuleMetadataRequestRequestTypeDef",
     "UpdateRuleVersionRequestRequestTypeDef",
+    "CreateRuleResultTypeDef",
     "UpdateRuleVersionResultTypeDef",
     "DataValidationMetricsTypeDef",
     "DescribeDetectorResultTypeDef",
     "GetDetectorsResultTypeDef",
     "EventTypeDef",
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
-    "PutExternalModelRequestRequestTypeDef",
+    "GetDetectorVersionResultTypeDef",
+    "ModelScoresTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
+    "IngestedEventsDetailOutputTypeDef",
     "IngestedEventsDetailTypeDef",
+    "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
+    "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
-    "GetEventPredictionResultTypeDef",
     "GetExternalModelsResultTypeDef",
+    "GetEventPredictionResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
-    "CreateModelVersionRequestRequestTypeDef",
     "GetModelVersionResultTypeDef",
+    "CreateModelVersionRequestRequestTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
     "TrainingMetricsV2TypeDef",
     "EvaluatedModelVersionTypeDef",
     "TrainingResultV2TypeDef",
@@ -451,14 +463,23 @@
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "detectorId": str,
+        "ruleId": str,
+        "ruleVersion": str,
+    },
+)
+
 FieldValidationMessageTypeDef = TypedDict(
     "FieldValidationMessageTypeDef",
     {
         "fieldName": str,
         "identifier": str,
         "title": str,
         "content": str,
@@ -660,14 +681,22 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
+EntityOutputTypeDef = TypedDict(
+    "EntityOutputTypeDef",
+    {
+        "entityType": str,
+        "entityId": str,
+    },
+)
+
 EntityTypeDef = TypedDict(
     "EntityTypeDef",
     {
         "entityType": str,
         "entityId": str,
     },
 )
@@ -705,14 +734,21 @@
         "outcomes": List[str],
         "evaluated": bool,
         "matched": bool,
     },
     total=False,
 )
 
+EventOrchestrationOutputTypeDef = TypedDict(
+    "EventOrchestrationOutputTypeDef",
+    {
+        "eventBridgeEnabled": bool,
+    },
+)
+
 EventOrchestrationTypeDef = TypedDict(
     "EventOrchestrationTypeDef",
     {
         "eventBridgeEnabled": bool,
     },
 )
 
@@ -747,62 +783,70 @@
         "name": str,
         "value": str,
         "source": str,
     },
     total=False,
 )
 
+ExternalEventsDetailOutputTypeDef = TypedDict(
+    "ExternalEventsDetailOutputTypeDef",
+    {
+        "dataLocation": str,
+        "dataAccessRoleArn": str,
+    },
+)
+
 ExternalModelSummaryTypeDef = TypedDict(
     "ExternalModelSummaryTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
     },
     total=False,
 )
 
-_RequiredModelInputConfigurationTypeDef = TypedDict(
-    "_RequiredModelInputConfigurationTypeDef",
+_RequiredModelInputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredModelInputConfigurationOutputTypeDef",
     {
         "useEventVariables": bool,
     },
 )
-_OptionalModelInputConfigurationTypeDef = TypedDict(
-    "_OptionalModelInputConfigurationTypeDef",
+_OptionalModelInputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalModelInputConfigurationOutputTypeDef",
     {
         "eventTypeName": str,
         "format": ModelInputDataFormatType,
         "jsonInputTemplate": str,
         "csvInputTemplate": str,
     },
     total=False,
 )
 
-class ModelInputConfigurationTypeDef(
-    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
+class ModelInputConfigurationOutputTypeDef(
+    _RequiredModelInputConfigurationOutputTypeDef, _OptionalModelInputConfigurationOutputTypeDef
 ):
     pass
 
-_RequiredModelOutputConfigurationTypeDef = TypedDict(
-    "_RequiredModelOutputConfigurationTypeDef",
+_RequiredModelOutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredModelOutputConfigurationOutputTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
-_OptionalModelOutputConfigurationTypeDef = TypedDict(
-    "_OptionalModelOutputConfigurationTypeDef",
+_OptionalModelOutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalModelOutputConfigurationOutputTypeDef",
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
-class ModelOutputConfigurationTypeDef(
-    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
+class ModelOutputConfigurationOutputTypeDef(
+    _RequiredModelOutputConfigurationOutputTypeDef, _OptionalModelOutputConfigurationOutputTypeDef
 ):
     pass
 
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "value": str,
@@ -850,14 +894,35 @@
     "GetDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
     },
 )
 
+_RequiredModelVersionOutputTypeDef = TypedDict(
+    "_RequiredModelVersionOutputTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+    },
+)
+_OptionalModelVersionOutputTypeDef = TypedDict(
+    "_OptionalModelVersionOutputTypeDef",
+    {
+        "arn": str,
+    },
+    total=False,
+)
+
+class ModelVersionOutputTypeDef(
+    _RequiredModelVersionOutputTypeDef, _OptionalModelVersionOutputTypeDef
+):
+    pass
+
 GetDetectorsRequestRequestTypeDef = TypedDict(
     "GetDetectorsRequestRequestTypeDef",
     {
         "detectorId": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1101,22 +1166,39 @@
         "name": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+IngestedEventsTimeWindowOutputTypeDef = TypedDict(
+    "IngestedEventsTimeWindowOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+    },
+)
+
 IngestedEventsTimeWindowTypeDef = TypedDict(
     "IngestedEventsTimeWindowTypeDef",
     {
         "startTime": str,
         "endTime": str,
     },
 )
 
+LabelSchemaOutputTypeDef = TypedDict(
+    "LabelSchemaOutputTypeDef",
+    {
+        "labelMapper": Dict[str, List[str]],
+        "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
+    },
+    total=False,
+)
+
 LabelSchemaTypeDef = TypedDict(
     "LabelSchemaTypeDef",
     {
         "labelMapper": Mapping[str, Sequence[str]],
         "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
     },
     total=False,
@@ -1147,14 +1229,22 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 LogOddsMetricTypeDef = TypedDict(
     "LogOddsMetricTypeDef",
     {
         "variableName": str,
         "variableType": str,
         "variableImportance": float,
     },
@@ -1167,14 +1257,56 @@
         "precision": float,
         "tpr": float,
         "threshold": float,
     },
     total=False,
 )
 
+_RequiredModelInputConfigurationTypeDef = TypedDict(
+    "_RequiredModelInputConfigurationTypeDef",
+    {
+        "useEventVariables": bool,
+    },
+)
+_OptionalModelInputConfigurationTypeDef = TypedDict(
+    "_OptionalModelInputConfigurationTypeDef",
+    {
+        "eventTypeName": str,
+        "format": ModelInputDataFormatType,
+        "jsonInputTemplate": str,
+        "csvInputTemplate": str,
+    },
+    total=False,
+)
+
+class ModelInputConfigurationTypeDef(
+    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
+):
+    pass
+
+_RequiredModelOutputConfigurationTypeDef = TypedDict(
+    "_RequiredModelOutputConfigurationTypeDef",
+    {
+        "format": ModelOutputDataFormatType,
+    },
+)
+_OptionalModelOutputConfigurationTypeDef = TypedDict(
+    "_OptionalModelOutputConfigurationTypeDef",
+    {
+        "jsonKeyToVariableMap": Mapping[str, str],
+        "csvIndexToVariableMap": Mapping[str, str],
+    },
+    total=False,
+)
+
+class ModelOutputConfigurationTypeDef(
+    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
+):
+    pass
+
 OFIMetricDataPointTypeDef = TypedDict(
     "OFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1521,23 +1653,14 @@
 )
 
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1675,23 +1798,14 @@
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModelScoresTypeDef = TypedDict(
-    "ModelScoresTypeDef",
-    {
-        "modelVersion": ModelVersionTypeDef,
-        "scores": Dict[str, float],
-    },
-    total=False,
-)
-
 _RequiredCreateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "rules": Sequence[RuleTypeDef],
     },
 )
@@ -1709,47 +1823,21 @@
 
 class CreateDetectorVersionRequestRequestTypeDef(
     _RequiredCreateDetectorVersionRequestRequestTypeDef,
     _OptionalCreateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
-CreateRuleResultTypeDef = TypedDict(
-    "CreateRuleResultTypeDef",
-    {
-        "rule": RuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
     },
 )
 
-GetDetectorVersionResultTypeDef = TypedDict(
-    "GetDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "description": str,
-        "externalModelEndpoints": List[str],
-        "modelVersions": List[ModelVersionTypeDef],
-        "rules": List[RuleTypeDef],
-        "status": DetectorVersionStatusType,
-        "lastUpdatedTime": str,
-        "createdTime": str,
-        "ruleExecutionMode": RuleExecutionModeType,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
         "externalModelEndpoints": Sequence[str],
         "rules": Sequence[RuleTypeDef],
@@ -1798,18 +1886,26 @@
 )
 
 class UpdateRuleVersionRequestRequestTypeDef(
     _RequiredUpdateRuleVersionRequestRequestTypeDef, _OptionalUpdateRuleVersionRequestRequestTypeDef
 ):
     pass
 
+CreateRuleResultTypeDef = TypedDict(
+    "CreateRuleResultTypeDef",
+    {
+        "rule": RuleOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
-        "rule": RuleTypeDef,
+        "rule": RuleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataValidationMetricsTypeDef = TypedDict(
     "DataValidationMetricsTypeDef",
     {
@@ -1844,15 +1940,15 @@
     {
         "eventId": str,
         "eventTypeName": str,
         "eventTimestamp": str,
         "eventVariables": Dict[str, str],
         "currentLabel": str,
         "labelTimestamp": str,
-        "entities": List[EntityTypeDef],
+        "entities": List[EntityOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
@@ -1929,15 +2025,15 @@
         "labels": List[str],
         "entityTypes": List[str],
         "eventIngestion": EventIngestionType,
         "ingestedEventStatistics": IngestedEventStatisticsTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
-        "eventOrchestration": EventOrchestrationTypeDef,
+        "eventOrchestration": EventOrchestrationOutputTypeDef,
     },
     total=False,
 )
 
 ExternalModelOutputsTypeDef = TypedDict(
     "ExternalModelOutputsTypeDef",
     {
@@ -1949,48 +2045,51 @@
 
 ExternalModelTypeDef = TypedDict(
     "ExternalModelTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationTypeDef,
+        "inputConfiguration": ModelInputConfigurationOutputTypeDef,
+        "outputConfiguration": ModelOutputConfigurationOutputTypeDef,
         "modelEndpointStatus": ModelEndpointStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_RequiredPutExternalModelRequestRequestTypeDef",
+GetDetectorVersionResultTypeDef = TypedDict(
+    "GetDetectorVersionResultTypeDef",
     {
-        "modelEndpoint": str,
-        "modelSource": Literal["SAGEMAKER"],
-        "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationTypeDef,
-        "modelEndpointStatus": ModelEndpointStatusType,
+        "detectorId": str,
+        "detectorVersionId": str,
+        "description": str,
+        "externalModelEndpoints": List[str],
+        "modelVersions": List[ModelVersionOutputTypeDef],
+        "rules": List[RuleOutputTypeDef],
+        "status": DetectorVersionStatusType,
+        "lastUpdatedTime": str,
+        "createdTime": str,
+        "ruleExecutionMode": RuleExecutionModeType,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_OptionalPutExternalModelRequestRequestTypeDef",
+
+ModelScoresTypeDef = TypedDict(
+    "ModelScoresTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "modelVersion": ModelVersionOutputTypeDef,
+        "scores": Dict[str, float],
     },
     total=False,
 )
 
-class PutExternalModelRequestRequestTypeDef(
-    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
-):
-    pass
-
 _RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
     "_RequiredGetEventPredictionRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventId": str,
         "eventTypeName": str,
         "entities": Sequence[EntityTypeDef],
@@ -2053,21 +2152,47 @@
     {
         "ruleDetails": List[RuleDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IngestedEventsDetailOutputTypeDef = TypedDict(
+    "IngestedEventsDetailOutputTypeDef",
+    {
+        "ingestedEventsTimeWindow": IngestedEventsTimeWindowOutputTypeDef,
+    },
+)
+
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
     },
 )
 
+_RequiredTrainingDataSchemaOutputTypeDef = TypedDict(
+    "_RequiredTrainingDataSchemaOutputTypeDef",
+    {
+        "modelVariables": List[str],
+    },
+)
+_OptionalTrainingDataSchemaOutputTypeDef = TypedDict(
+    "_OptionalTrainingDataSchemaOutputTypeDef",
+    {
+        "labelSchema": LabelSchemaOutputTypeDef,
+    },
+    total=False,
+)
+
+class TrainingDataSchemaOutputTypeDef(
+    _RequiredTrainingDataSchemaOutputTypeDef, _OptionalTrainingDataSchemaOutputTypeDef
+):
+    pass
+
 _RequiredTrainingDataSchemaTypeDef = TypedDict(
     "_RequiredTrainingDataSchemaTypeDef",
     {
         "modelVariables": Sequence[str],
     },
 )
 _OptionalTrainingDataSchemaTypeDef = TypedDict(
@@ -2093,14 +2218,23 @@
         "predictionTimeRange": PredictionTimeRangeTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VariableImportanceMetricsTypeDef = TypedDict(
     "VariableImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[LogOddsMetricTypeDef],
     },
     total=False,
 )
@@ -2110,14 +2244,38 @@
     {
         "auc": float,
         "metricDataPoints": List[MetricDataPointTypeDef],
     },
     total=False,
 )
 
+_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_RequiredPutExternalModelRequestRequestTypeDef",
+    {
+        "modelEndpoint": str,
+        "modelSource": Literal["SAGEMAKER"],
+        "invokeModelEndpointRoleArn": str,
+        "inputConfiguration": ModelInputConfigurationTypeDef,
+        "outputConfiguration": ModelOutputConfigurationTypeDef,
+        "modelEndpointStatus": ModelEndpointStatusType,
+    },
+)
+_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_OptionalPutExternalModelRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutExternalModelRequestRequestTypeDef(
+    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
+):
+    pass
+
 OFIModelPerformanceTypeDef = TypedDict(
     "OFIModelPerformanceTypeDef",
     {
         "auc": float,
         "uncertaintyRange": UncertaintyRangeTypeDef,
     },
     total=False,
@@ -2154,29 +2312,29 @@
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEventPredictionResultTypeDef = TypedDict(
-    "GetEventPredictionResultTypeDef",
+GetExternalModelsResultTypeDef = TypedDict(
+    "GetExternalModelsResultTypeDef",
     {
-        "modelScores": List[ModelScoresTypeDef],
-        "ruleResults": List[RuleResultTypeDef],
-        "externalModelOutputs": List[ExternalModelOutputsTypeDef],
+        "externalModels": List[ExternalModelTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetExternalModelsResultTypeDef = TypedDict(
-    "GetExternalModelsResultTypeDef",
+GetEventPredictionResultTypeDef = TypedDict(
+    "GetEventPredictionResultTypeDef",
     {
-        "externalModels": List[ExternalModelTypeDef],
-        "nextToken": str,
+        "modelScores": List[ModelScoresTypeDef],
+        "ruleResults": List[RuleResultTypeDef],
+        "externalModelOutputs": List[ExternalModelOutputsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelVersionRequestRequestTypeDef",
     {
@@ -2197,14 +2355,30 @@
 
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
+GetModelVersionResultTypeDef = TypedDict(
+    "GetModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "trainingDataSource": TrainingDataSourceEnumType,
+        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
+        "status": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
@@ -2222,30 +2396,14 @@
 
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
-GetModelVersionResultTypeDef = TypedDict(
-    "GetModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaTypeDef,
-        "externalEventsDetail": ExternalEventsDetailTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
-        "status": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
@@ -2338,17 +2496,17 @@
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaTypeDef,
-        "externalEventsDetail": ExternalEventsDetailTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
+        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
         "trainingResult": TrainingResultTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
         "trainingResultV2": TrainingResultV2TypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/PKG-INFO` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.0
-Summary: Type annotations for boto3.FraudDetector 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.FraudDetector 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-frauddetector"></a>
 
 # mypy-boto3-frauddetector
 
 [![PyPI - mypy-boto3-frauddetector](https://img.shields.io/pypi/v/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,14 +332,15 @@
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
     CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
     CreateModelVersionResultTypeDef,
+    RuleOutputTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
@@ -354,31 +355,35 @@
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
+    EntityOutputTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
+    EventOrchestrationOutputTypeDef,
     EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
+    ExternalEventsDetailOutputTypeDef,
     ExternalModelSummaryTypeDef,
-    ModelInputConfigurationTypeDef,
-    ModelOutputConfigurationTypeDef,
+    ModelInputConfigurationOutputTypeDef,
+    ModelOutputConfigurationOutputTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
+    ModelVersionOutputTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
@@ -393,20 +398,25 @@
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
     GetVariablesRequestRequestTypeDef,
+    IngestedEventsTimeWindowOutputTypeDef,
     IngestedEventsTimeWindowTypeDef,
+    LabelSchemaOutputTypeDef,
     LabelSchemaTypeDef,
     PredictionTimeRangeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
+    ModelInputConfigurationTypeDef,
+    ModelOutputConfigurationTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -424,67 +434,69 @@
     BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
-    ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
-    CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
     UpdateRuleVersionRequestRequestTypeDef,
+    CreateRuleResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    PutExternalModelRequestRequestTypeDef,
+    GetDetectorVersionResultTypeDef,
+    ModelScoresTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
+    IngestedEventsDetailOutputTypeDef,
     IngestedEventsDetailTypeDef,
+    TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
+    PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
-    GetEventPredictionResultTypeDef,
     GetExternalModelsResultTypeDef,
+    GetEventPredictionResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
-    CreateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
+    CreateModelVersionRequestRequestTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
     TrainingMetricsV2TypeDef,
     EvaluatedModelVersionTypeDef,
     TrainingResultV2TypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.28.0/mypy_boto3_frauddetector.egg-info/SOURCES.txt` & `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.0/setup.py` & `mypy-boto3-frauddetector-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-frauddetector",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FraudDetector 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.FraudDetector 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

