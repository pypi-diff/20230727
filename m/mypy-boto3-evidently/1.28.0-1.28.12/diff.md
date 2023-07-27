# Comparing `tmp/mypy-boto3-evidently-1.28.0.tar.gz` & `tmp/mypy-boto3-evidently-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-evidently-1.28.0.tar", last modified: Thu Jul  6 20:59:34 2023, max compression
+gzip compressed data, was "mypy-boto3-evidently-1.28.12.tar", last modified: Thu Jul 27 05:34:41 2023, max compression
```

## Comparing `mypy-boto3-evidently-1.28.0.tar` & `mypy-boto3-evidently-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:34.962302 mypy-boto3-evidently-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-06 20:59:34.962302 mypy-boto3-evidently-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:34.950302 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-07-06 20:40:54.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-06 20:40:54.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-06 20:40:54.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-06 20:40:54.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-06 20:40:54.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-06 20:40:54.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45527 2023-07-06 20:40:55.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45442 2023-07-06 20:40:55.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:34.962302 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-06 20:59:34.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 20:59:34.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:34.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:34.000000 mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:34.962302 mypy-boto3-evidently-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-06 20:40:53.000000 mypy-boto3-evidently-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.216512 mypy-boto3-evidently-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-07-27 05:34:41.212512 mypy-boto3-evidently-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16911 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.204512 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46024 2023-07-27 05:22:13.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45939 2023-07-27 05:22:13.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.212512 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:41.216512 mypy-boto3-evidently-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-27 05:22:10.000000 mypy-boto3-evidently-1.28.12/setup.py
```

### Comparing `mypy-boto3-evidently-1.28.0/LICENSE` & `mypy-boto3-evidently-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/PKG-INFO` & `mypy-boto3-evidently-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatchEvidently 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchEvidently 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-evidently"></a>
 
 # mypy-boto3-evidently
 
 [![PyPI - mypy-boto3-evidently](https://img.shields.io/pypi/v/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-evidently?color=blue)](https://pypistats.org/packages/mypy-boto3-evidently)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,15 +370,15 @@
     SegmentTypeDef,
     DeleteExperimentRequestRequestTypeDef,
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
-    VariableValueTypeDef,
+    VariableValueOutputTypeDef,
     EvaluationRuleTypeDef,
     EventTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
@@ -412,33 +412,34 @@
     PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
     ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
+    SegmentOverrideOutputTypeDef,
     StartExperimentRequestRequestTypeDef,
     StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
     StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
     TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    VariableValueTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
-    VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
@@ -447,26 +448,27 @@
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
     UpdateProjectDataDeliveryRequestRequestTypeDef,
     ProjectDataDeliveryTypeDef,
     PutProjectEventsResponseTypeDef,
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
+    VariationConfigTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
-    CreateFeatureRequestRequestTypeDef,
-    UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
+    CreateFeatureRequestRequestTypeDef,
+    UpdateFeatureRequestRequestTypeDef,
     CreateFeatureResponseTypeDef,
     GetFeatureResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     CreateExperimentResponseTypeDef,
     GetExperimentResponseTypeDef,
     ListExperimentsResponseTypeDef,
     UpdateExperimentResponseTypeDef,
```

### Comparing `mypy-boto3-evidently-1.28.0/README.md` & `mypy-boto3-evidently-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-evidently"></a>
 
 # mypy-boto3-evidently
 
 [![PyPI - mypy-boto3-evidently](https://img.shields.io/pypi/v/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-evidently?color=blue)](https://pypistats.org/packages/mypy-boto3-evidently)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,15 +338,15 @@
     SegmentTypeDef,
     DeleteExperimentRequestRequestTypeDef,
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
-    VariableValueTypeDef,
+    VariableValueOutputTypeDef,
     EvaluationRuleTypeDef,
     EventTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
@@ -380,33 +380,34 @@
     PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
     ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
+    SegmentOverrideOutputTypeDef,
     StartExperimentRequestRequestTypeDef,
     StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
     StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
     TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    VariableValueTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
-    VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
@@ -415,26 +416,27 @@
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
     UpdateProjectDataDeliveryRequestRequestTypeDef,
     ProjectDataDeliveryTypeDef,
     PutProjectEventsResponseTypeDef,
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
+    VariationConfigTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
-    CreateFeatureRequestRequestTypeDef,
-    UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
+    CreateFeatureRequestRequestTypeDef,
+    UpdateFeatureRequestRequestTypeDef,
     CreateFeatureResponseTypeDef,
     GetFeatureResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     CreateExperimentResponseTypeDef,
     GetExperimentResponseTypeDef,
     ListExperimentsResponseTypeDef,
     UpdateExperimentResponseTypeDef,
```

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/__init__.py` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/__init__.pyi` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/client.py` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/client.pyi` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/literals.py` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.pyi`

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
     "ChangeDirectionEnumType",
     "EventTypeType",
     "ExperimentBaseStatType",
     "ExperimentReportNameType",
     "ExperimentResultRequestTypeType",
     "ExperimentResultResponseTypeType",
@@ -46,15 +45,14 @@
     "CloudWatchEvidentlyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ChangeDirectionEnumType = Literal["DECREASE", "INCREASE"]
 EventTypeType = Literal["aws.evidently.custom", "aws.evidently.evaluation"]
 ExperimentBaseStatType = Literal["Mean"]
 ExperimentReportNameType = Literal["BayesianInference"]
 ExperimentResultRequestTypeType = Literal[
     "BaseStat", "ConfidenceInterval", "PValue", "TreatmentEffect"
 ]
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

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/literals.pyi` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.py`

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
     "ChangeDirectionEnumType",
     "EventTypeType",
     "ExperimentBaseStatType",
     "ExperimentReportNameType",
     "ExperimentResultRequestTypeType",
     "ExperimentResultResponseTypeType",
@@ -45,14 +46,15 @@
     "CloudWatchEvidentlyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ChangeDirectionEnumType = Literal["DECREASE", "INCREASE"]
 EventTypeType = Literal["aws.evidently.custom", "aws.evidently.evaluation"]
 ExperimentBaseStatType = Literal["Mean"]
 ExperimentReportNameType = Literal["BayesianInference"]
 ExperimentResultRequestTypeType = Literal[
     "BaseStat", "ConfidenceInterval", "PValue", "TreatmentEffect"
 ]
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

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/paginator.py` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/paginator.pyi` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/type_defs.py` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     "SegmentTypeDef",
     "DeleteExperimentRequestRequestTypeDef",
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
-    "VariableValueTypeDef",
+    "VariableValueOutputTypeDef",
     "EvaluationRuleTypeDef",
     "EventTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
@@ -95,33 +95,34 @@
     "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
     "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
+    "SegmentOverrideOutputTypeDef",
     "StartExperimentRequestRequestTypeDef",
     "StartExperimentResponseTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
     "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
     "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "VariableValueTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
-    "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
     "PutProjectEventsRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
@@ -130,26 +131,27 @@
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
     "UpdateProjectDataDeliveryRequestRequestTypeDef",
     "ProjectDataDeliveryTypeDef",
     "PutProjectEventsResponseTypeDef",
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
+    "VariationConfigTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
-    "CreateFeatureRequestRequestTypeDef",
-    "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
+    "CreateFeatureRequestRequestTypeDef",
+    "UpdateFeatureRequestRequestTypeDef",
     "CreateFeatureResponseTypeDef",
     "GetFeatureResponseTypeDef",
     "UpdateFeatureResponseTypeDef",
     "CreateExperimentResponseTypeDef",
     "GetExperimentResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "UpdateExperimentResponseTypeDef",
@@ -373,16 +375,16 @@
 
 class EvaluateFeatureRequestRequestTypeDef(
     _RequiredEvaluateFeatureRequestRequestTypeDef, _OptionalEvaluateFeatureRequestRequestTypeDef
 ):
     pass
 
 
-VariableValueTypeDef = TypedDict(
-    "VariableValueTypeDef",
+VariableValueOutputTypeDef = TypedDict(
+    "VariableValueOutputTypeDef",
     {
         "boolValue": bool,
         "doubleValue": float,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
@@ -965,14 +967,23 @@
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
 )
 
+SegmentOverrideOutputTypeDef = TypedDict(
+    "SegmentOverrideOutputTypeDef",
+    {
+        "evaluationOrder": int,
+        "segment": str,
+        "weights": Dict[str, int],
+    },
+)
+
 StartExperimentRequestRequestTypeDef = TypedDict(
     "StartExperimentRequestRequestTypeDef",
     {
         "analysisCompleteTime": Union[datetime, str],
         "experiment": str,
         "project": str,
     },
@@ -1084,14 +1095,25 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+VariableValueTypeDef = TypedDict(
+    "VariableValueTypeDef",
+    {
+        "boolValue": bool,
+        "doubleValue": float,
+        "longValue": int,
+        "stringValue": str,
+    },
+    total=False,
+)
+
 BatchEvaluateFeatureRequestRequestTypeDef = TypedDict(
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
@@ -1144,15 +1166,15 @@
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
-        "value": VariableValueTypeDef,
+        "value": VariableValueOutputTypeDef,
         "variation": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
@@ -1163,38 +1185,30 @@
 )
 _OptionalEvaluationResultTypeDef = TypedDict(
     "_OptionalEvaluationResultTypeDef",
     {
         "details": str,
         "project": str,
         "reason": str,
-        "value": VariableValueTypeDef,
+        "value": VariableValueOutputTypeDef,
         "variation": str,
     },
     total=False,
 )
 
 
 class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
     pass
 
 
-VariationConfigTypeDef = TypedDict(
-    "VariationConfigTypeDef",
-    {
-        "name": str,
-        "value": VariableValueTypeDef,
-    },
-)
-
 VariationTypeDef = TypedDict(
     "VariationTypeDef",
     {
         "name": str,
-        "value": VariableValueTypeDef,
+        "value": VariableValueOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredFeatureSummaryTypeDef = TypedDict(
     "_RequiredFeatureSummaryTypeDef",
     {
@@ -1389,86 +1403,40 @@
         "startTime": datetime,
     },
 )
 _OptionalScheduledSplitTypeDef = TypedDict(
     "_OptionalScheduledSplitTypeDef",
     {
         "groupWeights": Dict[str, int],
-        "segmentOverrides": List[SegmentOverrideTypeDef],
+        "segmentOverrides": List[SegmentOverrideOutputTypeDef],
     },
     total=False,
 )
 
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
 
 
-BatchEvaluateFeatureResponseTypeDef = TypedDict(
-    "BatchEvaluateFeatureResponseTypeDef",
-    {
-        "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFeatureRequestRequestTypeDef",
+VariationConfigTypeDef = TypedDict(
+    "VariationConfigTypeDef",
     {
         "name": str,
-        "project": str,
-        "variations": Sequence[VariationConfigTypeDef],
-    },
-)
-_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFeatureRequestRequestTypeDef",
-    {
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "tags": Mapping[str, str],
+        "value": VariableValueTypeDef,
     },
-    total=False,
 )
 
-
-class CreateFeatureRequestRequestTypeDef(
-    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFeatureRequestRequestTypeDef",
-    {
-        "feature": str,
-        "project": str,
-    },
-)
-_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFeatureRequestRequestTypeDef",
+BatchEvaluateFeatureResponseTypeDef = TypedDict(
+    "BatchEvaluateFeatureResponseTypeDef",
     {
-        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "removeVariations": Sequence[str],
+        "results": List[EvaluationResultTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class UpdateFeatureRequestRequestTypeDef(
-    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredFeatureTypeDef = TypedDict(
     "_RequiredFeatureTypeDef",
     {
         "arn": str,
         "createdTime": datetime,
         "evaluationStrategy": FeatureEvaluationStrategyType,
         "lastUpdatedTime": datetime,
@@ -1664,14 +1632,68 @@
     "ScheduledSplitsLaunchDefinitionTypeDef",
     {
         "steps": List[ScheduledSplitTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFeatureRequestRequestTypeDef",
+    {
+        "name": str,
+        "project": str,
+        "variations": Sequence[VariationConfigTypeDef],
+    },
+)
+_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFeatureRequestRequestTypeDef",
+    {
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateFeatureRequestRequestTypeDef(
+    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeatureRequestRequestTypeDef",
+    {
+        "feature": str,
+        "project": str,
+    },
+)
+_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeatureRequestRequestTypeDef",
+    {
+        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "removeVariations": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateFeatureRequestRequestTypeDef(
+    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
+):
+    pass
+
+
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently/type_defs.pyi` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "SegmentTypeDef",
     "DeleteExperimentRequestRequestTypeDef",
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
-    "VariableValueTypeDef",
+    "VariableValueOutputTypeDef",
     "EvaluationRuleTypeDef",
     "EventTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
@@ -94,33 +94,34 @@
     "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
     "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
+    "SegmentOverrideOutputTypeDef",
     "StartExperimentRequestRequestTypeDef",
     "StartExperimentResponseTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
     "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
     "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "VariableValueTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
-    "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
     "PutProjectEventsRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
@@ -129,26 +130,27 @@
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
     "UpdateProjectDataDeliveryRequestRequestTypeDef",
     "ProjectDataDeliveryTypeDef",
     "PutProjectEventsResponseTypeDef",
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
+    "VariationConfigTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
-    "CreateFeatureRequestRequestTypeDef",
-    "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
+    "CreateFeatureRequestRequestTypeDef",
+    "UpdateFeatureRequestRequestTypeDef",
     "CreateFeatureResponseTypeDef",
     "GetFeatureResponseTypeDef",
     "UpdateFeatureResponseTypeDef",
     "CreateExperimentResponseTypeDef",
     "GetExperimentResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "UpdateExperimentResponseTypeDef",
@@ -360,16 +362,16 @@
 )
 
 class EvaluateFeatureRequestRequestTypeDef(
     _RequiredEvaluateFeatureRequestRequestTypeDef, _OptionalEvaluateFeatureRequestRequestTypeDef
 ):
     pass
 
-VariableValueTypeDef = TypedDict(
-    "VariableValueTypeDef",
+VariableValueOutputTypeDef = TypedDict(
+    "VariableValueOutputTypeDef",
     {
         "boolValue": bool,
         "doubleValue": float,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
@@ -922,14 +924,23 @@
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
 )
 
+SegmentOverrideOutputTypeDef = TypedDict(
+    "SegmentOverrideOutputTypeDef",
+    {
+        "evaluationOrder": int,
+        "segment": str,
+        "weights": Dict[str, int],
+    },
+)
+
 StartExperimentRequestRequestTypeDef = TypedDict(
     "StartExperimentRequestRequestTypeDef",
     {
         "analysisCompleteTime": Union[datetime, str],
         "experiment": str,
         "project": str,
     },
@@ -1037,14 +1048,25 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+VariableValueTypeDef = TypedDict(
+    "VariableValueTypeDef",
+    {
+        "boolValue": bool,
+        "doubleValue": float,
+        "longValue": int,
+        "stringValue": str,
+    },
+    total=False,
+)
+
 BatchEvaluateFeatureRequestRequestTypeDef = TypedDict(
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
@@ -1095,15 +1117,15 @@
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
-        "value": VariableValueTypeDef,
+        "value": VariableValueOutputTypeDef,
         "variation": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
@@ -1114,36 +1136,28 @@
 )
 _OptionalEvaluationResultTypeDef = TypedDict(
     "_OptionalEvaluationResultTypeDef",
     {
         "details": str,
         "project": str,
         "reason": str,
-        "value": VariableValueTypeDef,
+        "value": VariableValueOutputTypeDef,
         "variation": str,
     },
     total=False,
 )
 
 class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
     pass
 
-VariationConfigTypeDef = TypedDict(
-    "VariationConfigTypeDef",
-    {
-        "name": str,
-        "value": VariableValueTypeDef,
-    },
-)
-
 VariationTypeDef = TypedDict(
     "VariationTypeDef",
     {
         "name": str,
-        "value": VariableValueTypeDef,
+        "value": VariableValueOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredFeatureSummaryTypeDef = TypedDict(
     "_RequiredFeatureSummaryTypeDef",
     {
@@ -1328,80 +1342,38 @@
         "startTime": datetime,
     },
 )
 _OptionalScheduledSplitTypeDef = TypedDict(
     "_OptionalScheduledSplitTypeDef",
     {
         "groupWeights": Dict[str, int],
-        "segmentOverrides": List[SegmentOverrideTypeDef],
+        "segmentOverrides": List[SegmentOverrideOutputTypeDef],
     },
     total=False,
 )
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
 
-BatchEvaluateFeatureResponseTypeDef = TypedDict(
-    "BatchEvaluateFeatureResponseTypeDef",
-    {
-        "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFeatureRequestRequestTypeDef",
+VariationConfigTypeDef = TypedDict(
+    "VariationConfigTypeDef",
     {
         "name": str,
-        "project": str,
-        "variations": Sequence[VariationConfigTypeDef],
-    },
-)
-_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFeatureRequestRequestTypeDef",
-    {
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "tags": Mapping[str, str],
+        "value": VariableValueTypeDef,
     },
-    total=False,
 )
 
-class CreateFeatureRequestRequestTypeDef(
-    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFeatureRequestRequestTypeDef",
-    {
-        "feature": str,
-        "project": str,
-    },
-)
-_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFeatureRequestRequestTypeDef",
+BatchEvaluateFeatureResponseTypeDef = TypedDict(
+    "BatchEvaluateFeatureResponseTypeDef",
     {
-        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "removeVariations": Sequence[str],
+        "results": List[EvaluationResultTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class UpdateFeatureRequestRequestTypeDef(
-    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
-):
-    pass
-
 _RequiredFeatureTypeDef = TypedDict(
     "_RequiredFeatureTypeDef",
     {
         "arn": str,
         "createdTime": datetime,
         "evaluationStrategy": FeatureEvaluationStrategyType,
         "lastUpdatedTime": datetime,
@@ -1585,14 +1557,64 @@
     "ScheduledSplitsLaunchDefinitionTypeDef",
     {
         "steps": List[ScheduledSplitTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFeatureRequestRequestTypeDef",
+    {
+        "name": str,
+        "project": str,
+        "variations": Sequence[VariationConfigTypeDef],
+    },
+)
+_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFeatureRequestRequestTypeDef",
+    {
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateFeatureRequestRequestTypeDef(
+    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeatureRequestRequestTypeDef",
+    {
+        "feature": str,
+        "project": str,
+    },
+)
+_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeatureRequestRequestTypeDef",
+    {
+        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "removeVariations": Sequence[str],
+    },
+    total=False,
+)
+
+class UpdateFeatureRequestRequestTypeDef(
+    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
+):
+    pass
+
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/PKG-INFO` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatchEvidently 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchEvidently 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-evidently"></a>
 
 # mypy-boto3-evidently
 
 [![PyPI - mypy-boto3-evidently](https://img.shields.io/pypi/v/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-evidently?color=blue)](https://pypistats.org/packages/mypy-boto3-evidently)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,15 +370,15 @@
     SegmentTypeDef,
     DeleteExperimentRequestRequestTypeDef,
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
-    VariableValueTypeDef,
+    VariableValueOutputTypeDef,
     EvaluationRuleTypeDef,
     EventTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
@@ -412,33 +412,34 @@
     PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
     ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
+    SegmentOverrideOutputTypeDef,
     StartExperimentRequestRequestTypeDef,
     StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
     StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
     TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    VariableValueTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
-    VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
@@ -447,26 +448,27 @@
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
     UpdateProjectDataDeliveryRequestRequestTypeDef,
     ProjectDataDeliveryTypeDef,
     PutProjectEventsResponseTypeDef,
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
+    VariationConfigTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
-    CreateFeatureRequestRequestTypeDef,
-    UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
+    CreateFeatureRequestRequestTypeDef,
+    UpdateFeatureRequestRequestTypeDef,
     CreateFeatureResponseTypeDef,
     GetFeatureResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     CreateExperimentResponseTypeDef,
     GetExperimentResponseTypeDef,
     ListExperimentsResponseTypeDef,
     UpdateExperimentResponseTypeDef,
```

### Comparing `mypy-boto3-evidently-1.28.0/mypy_boto3_evidently.egg-info/SOURCES.txt` & `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.0/setup.py` & `mypy-boto3-evidently-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-evidently",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchEvidently 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CloudWatchEvidently 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

