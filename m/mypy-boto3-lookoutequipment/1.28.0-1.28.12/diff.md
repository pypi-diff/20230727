# Comparing `tmp/mypy-boto3-lookoutequipment-1.28.0.tar.gz` & `tmp/mypy-boto3-lookoutequipment-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutequipment-1.28.0.tar", last modified: Thu Jul  6 21:00:01 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutequipment-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
```

## Comparing `mypy-boto3-lookoutequipment-1.28.0.tar` & `mypy-boto3-lookoutequipment-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.242357 mypy-boto3-lookoutequipment-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-07-06 21:00:01.234357 mypy-boto3-lookoutequipment-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.234357 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-07-06 20:46:11.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35915 2023-07-06 20:46:11.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:10.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.234357 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-07-06 21:00:00.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-06 21:00:01.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:00.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 21:00:00.000000 mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:01.242357 mypy-boto3-lookoutequipment-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:46:07.000000 mypy-boto3-lookoutequipment-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-27 05:25:35.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-07-27 05:25:37.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40437 2023-07-27 05:25:36.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/setup.py
```

### Comparing `mypy-boto3-lookoutequipment-1.28.0/LICENSE` & `mypy-boto3-lookoutequipment-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.0/PKG-INFO` & `mypy-boto3-lookoutequipment-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutequipment
-Version: 1.28.0
-Summary: Type annotations for boto3.LookoutEquipment 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LookoutEquipment 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lookoutequipment"></a>
 
 # mypy-boto3-lookoutequipment
 
 [![PyPI - mypy-boto3-lookoutequipment](https://img.shields.io/pypi/v/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutequipment?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutequipment)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutequipment)](https://pepy.tech/project/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,14 +319,15 @@
     CreateDatasetResponseTypeDef,
     CreateInferenceSchedulerResponseTypeDef,
     CreateLabelGroupResponseTypeDef,
     CreateLabelRequestRequestTypeDef,
     CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
     CreateModelResponseTypeDef,
+    DataPreProcessingConfigurationOutputTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
@@ -340,72 +341,82 @@
     DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
     DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
+    InferenceInputNameConfigurationOutputTypeDef,
+    InferenceS3InputConfigurationOutputTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
+    InferenceS3OutputConfigurationOutputTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
+    IngestionS3InputConfigurationOutputTypeDef,
     IngestionS3InputConfigurationTypeDef,
     MissingCompleteSensorDataTypeDef,
     SensorsWithShortDateRangeTypeDef,
     LabelGroupSummaryTypeDef,
     LabelSummaryTypeDef,
+    LabelsS3InputConfigurationOutputTypeDef,
     LabelsS3InputConfigurationTypeDef,
     LargeTimestampGapsTypeDef,
     ListDataIngestionJobsRequestRequestTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListInferenceEventsRequestRequestTypeDef,
     ListInferenceExecutionsRequestRequestTypeDef,
     ListInferenceSchedulersRequestRequestTypeDef,
     ListLabelGroupsRequestRequestTypeDef,
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
     ResponseMetadataTypeDef,
     StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
     StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
     StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
+    InferenceInputConfigurationOutputTypeDef,
     InferenceInputConfigurationTypeDef,
+    InferenceOutputConfigurationOutputTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
+    IngestionInputConfigurationOutputTypeDef,
     IngestionInputConfigurationTypeDef,
     InsufficientSensorDataTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
+    LabelsInputConfigurationOutputTypeDef,
     LabelsInputConfigurationTypeDef,
     ListModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SensorStatisticsSummaryTypeDef,
-    CreateInferenceSchedulerRequestRequestTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     InferenceExecutionSummaryTypeDef,
+    CreateInferenceSchedulerRequestRequestTypeDef,
     UpdateInferenceSchedulerRequestRequestTypeDef,
     DataIngestionJobSummaryTypeDef,
     StartDataIngestionJobRequestRequestTypeDef,
     DataQualitySummaryTypeDef,
-    CreateModelRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
+    CreateModelRequestRequestTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.0/README.md` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-lookoutequipment
+Version: 1.28.12
+Summary: Type annotations for boto3.LookoutEquipment 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 lookoutequipment type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-lookoutequipment"></a>
 
 # mypy-boto3-lookoutequipment
 
 [![PyPI - mypy-boto3-lookoutequipment](https://img.shields.io/pypi/v/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutequipment?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutequipment)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutequipment)](https://pepy.tech/project/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,14 +319,15 @@
     CreateDatasetResponseTypeDef,
     CreateInferenceSchedulerResponseTypeDef,
     CreateLabelGroupResponseTypeDef,
     CreateLabelRequestRequestTypeDef,
     CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
     CreateModelResponseTypeDef,
+    DataPreProcessingConfigurationOutputTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
@@ -308,72 +341,82 @@
     DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
     DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
+    InferenceInputNameConfigurationOutputTypeDef,
+    InferenceS3InputConfigurationOutputTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
+    InferenceS3OutputConfigurationOutputTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
+    IngestionS3InputConfigurationOutputTypeDef,
     IngestionS3InputConfigurationTypeDef,
     MissingCompleteSensorDataTypeDef,
     SensorsWithShortDateRangeTypeDef,
     LabelGroupSummaryTypeDef,
     LabelSummaryTypeDef,
+    LabelsS3InputConfigurationOutputTypeDef,
     LabelsS3InputConfigurationTypeDef,
     LargeTimestampGapsTypeDef,
     ListDataIngestionJobsRequestRequestTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListInferenceEventsRequestRequestTypeDef,
     ListInferenceExecutionsRequestRequestTypeDef,
     ListInferenceSchedulersRequestRequestTypeDef,
     ListLabelGroupsRequestRequestTypeDef,
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
     ResponseMetadataTypeDef,
     StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
     StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
     StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
+    InferenceInputConfigurationOutputTypeDef,
     InferenceInputConfigurationTypeDef,
+    InferenceOutputConfigurationOutputTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
+    IngestionInputConfigurationOutputTypeDef,
     IngestionInputConfigurationTypeDef,
     InsufficientSensorDataTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
+    LabelsInputConfigurationOutputTypeDef,
     LabelsInputConfigurationTypeDef,
     ListModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SensorStatisticsSummaryTypeDef,
-    CreateInferenceSchedulerRequestRequestTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     InferenceExecutionSummaryTypeDef,
+    CreateInferenceSchedulerRequestRequestTypeDef,
     UpdateInferenceSchedulerRequestRequestTypeDef,
     DataIngestionJobSummaryTypeDef,
     StartDataIngestionJobRequestRequestTypeDef,
     DataQualitySummaryTypeDef,
-    CreateModelRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
+    CreateModelRequestRequestTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/__main__.py` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutEquipment 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LookoutEquipment 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment\nOther"
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

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/client.py` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/client.pyi` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/literals.py` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.pyi`

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
     "DataUploadFrequencyType",
     "DatasetStatusType",
     "InferenceExecutionStatusType",
     "InferenceSchedulerStatusType",
     "IngestionJobStatusType",
     "LabelRatingType",
@@ -33,15 +32,14 @@
     "TargetSamplingRateType",
     "LookoutEquipmentServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DataUploadFrequencyType = Literal["PT10M", "PT15M", "PT1H", "PT30M", "PT5M"]
 DatasetStatusType = Literal["ACTIVE", "CREATED", "INGESTION_IN_PROGRESS"]
 InferenceExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 InferenceSchedulerStatusType = Literal["PENDING", "RUNNING", "STOPPED", "STOPPING"]
 IngestionJobStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 LabelRatingType = Literal["ANOMALY", "NEUTRAL", "NO_ANOMALY"]
 LatestInferenceResultType = Literal["ANOMALOUS", "NORMAL"]
@@ -167,14 +165,15 @@
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
@@ -253,26 +252,28 @@
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

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/literals.pyi` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DataUploadFrequencyType",
     "DatasetStatusType",
     "InferenceExecutionStatusType",
     "InferenceSchedulerStatusType",
     "IngestionJobStatusType",
     "LabelRatingType",
@@ -32,14 +33,15 @@
     "TargetSamplingRateType",
     "LookoutEquipmentServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 DataUploadFrequencyType = Literal["PT10M", "PT15M", "PT1H", "PT30M", "PT5M"]
 DatasetStatusType = Literal["ACTIVE", "CREATED", "INGESTION_IN_PROGRESS"]
 InferenceExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 InferenceSchedulerStatusType = Literal["PENDING", "RUNNING", "STOPPED", "STOPPING"]
 IngestionJobStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 LabelRatingType = Literal["ANOMALY", "NEUTRAL", "NO_ANOMALY"]
 LatestInferenceResultType = Literal["ANOMALOUS", "NORMAL"]
@@ -165,14 +167,15 @@
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
@@ -251,26 +254,28 @@
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

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/type_defs.py` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "CreateDatasetResponseTypeDef",
     "CreateInferenceSchedulerResponseTypeDef",
     "CreateLabelGroupResponseTypeDef",
     "CreateLabelRequestRequestTypeDef",
     "CreateLabelResponseTypeDef",
     "DataPreProcessingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
+    "DataPreProcessingConfigurationOutputTypeDef",
     "DuplicateTimestampsTypeDef",
     "InvalidSensorDataTypeDef",
     "MissingSensorDataTypeDef",
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
@@ -64,72 +65,82 @@
     "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelRequestRequestTypeDef",
     "DescribeLabelResponseTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
+    "InferenceInputNameConfigurationOutputTypeDef",
+    "InferenceS3InputConfigurationOutputTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
+    "InferenceS3OutputConfigurationOutputTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
+    "IngestionS3InputConfigurationOutputTypeDef",
     "IngestionS3InputConfigurationTypeDef",
     "MissingCompleteSensorDataTypeDef",
     "SensorsWithShortDateRangeTypeDef",
     "LabelGroupSummaryTypeDef",
     "LabelSummaryTypeDef",
+    "LabelsS3InputConfigurationOutputTypeDef",
     "LabelsS3InputConfigurationTypeDef",
     "LargeTimestampGapsTypeDef",
     "ListDataIngestionJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListInferenceEventsRequestRequestTypeDef",
     "ListInferenceExecutionsRequestRequestTypeDef",
     "ListInferenceSchedulersRequestRequestTypeDef",
     "ListLabelGroupsRequestRequestTypeDef",
     "ListLabelsRequestRequestTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
     "ResponseMetadataTypeDef",
     "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
     "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
     "StopInferenceSchedulerResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
+    "InferenceInputConfigurationOutputTypeDef",
     "InferenceInputConfigurationTypeDef",
+    "InferenceOutputConfigurationOutputTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
+    "IngestionInputConfigurationOutputTypeDef",
     "IngestionInputConfigurationTypeDef",
     "InsufficientSensorDataTypeDef",
     "ListLabelGroupsResponseTypeDef",
     "ListLabelsResponseTypeDef",
+    "LabelsInputConfigurationOutputTypeDef",
     "LabelsInputConfigurationTypeDef",
     "ListModelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SensorStatisticsSummaryTypeDef",
-    "CreateInferenceSchedulerRequestRequestTypeDef",
     "DescribeInferenceSchedulerResponseTypeDef",
     "InferenceExecutionSummaryTypeDef",
+    "CreateInferenceSchedulerRequestRequestTypeDef",
     "UpdateInferenceSchedulerRequestRequestTypeDef",
     "DataIngestionJobSummaryTypeDef",
     "StartDataIngestionJobRequestRequestTypeDef",
     "DataQualitySummaryTypeDef",
-    "CreateModelRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
+    "CreateModelRequestRequestTypeDef",
     "ListSensorStatisticsResponseTypeDef",
     "ListInferenceExecutionsResponseTypeDef",
     "ListDataIngestionJobsResponseTypeDef",
     "DescribeDataIngestionJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
@@ -255,14 +266,22 @@
     {
         "ModelArn": str,
         "Status": ModelStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataPreProcessingConfigurationOutputTypeDef = TypedDict(
+    "DataPreProcessingConfigurationOutputTypeDef",
+    {
+        "TargetSamplingRate": TargetSamplingRateType,
+    },
+    total=False,
+)
+
 DuplicateTimestampsTypeDef = TypedDict(
     "DuplicateTimestampsTypeDef",
     {
         "TotalNumberOfDuplicateTimestamps": int,
     },
 )
 
@@ -432,14 +451,45 @@
     "S3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
+InferenceInputNameConfigurationOutputTypeDef = TypedDict(
+    "InferenceInputNameConfigurationOutputTypeDef",
+    {
+        "TimestampFormat": str,
+        "ComponentTimestampDelimiter": str,
+    },
+    total=False,
+)
+
+_RequiredInferenceS3InputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredInferenceS3InputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalInferenceS3InputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalInferenceS3InputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+
+class InferenceS3InputConfigurationOutputTypeDef(
+    _RequiredInferenceS3InputConfigurationOutputTypeDef,
+    _OptionalInferenceS3InputConfigurationOutputTypeDef,
+):
+    pass
+
+
 InferenceInputNameConfigurationTypeDef = TypedDict(
     "InferenceInputNameConfigurationTypeDef",
     {
         "TimestampFormat": str,
         "ComponentTimestampDelimiter": str,
     },
     total=False,
@@ -462,14 +512,36 @@
 
 class InferenceS3InputConfigurationTypeDef(
     _RequiredInferenceS3InputConfigurationTypeDef, _OptionalInferenceS3InputConfigurationTypeDef
 ):
     pass
 
 
+_RequiredInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredInferenceS3OutputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalInferenceS3OutputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+
+class InferenceS3OutputConfigurationOutputTypeDef(
+    _RequiredInferenceS3OutputConfigurationOutputTypeDef,
+    _OptionalInferenceS3OutputConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredInferenceS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceS3OutputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalInferenceS3OutputConfigurationTypeDef = TypedDict(
@@ -498,14 +570,37 @@
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "LatestInferenceResult": LatestInferenceResultType,
     },
     total=False,
 )
 
+_RequiredIngestionS3InputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredIngestionS3InputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalIngestionS3InputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalIngestionS3InputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+        "KeyPattern": str,
+    },
+    total=False,
+)
+
+
+class IngestionS3InputConfigurationOutputTypeDef(
+    _RequiredIngestionS3InputConfigurationOutputTypeDef,
+    _OptionalIngestionS3InputConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredIngestionS3InputConfigurationTypeDef = TypedDict(
     "_RequiredIngestionS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalIngestionS3InputConfigurationTypeDef = TypedDict(
@@ -561,14 +656,36 @@
         "FaultCode": str,
         "Equipment": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
+_RequiredLabelsS3InputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLabelsS3InputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalLabelsS3InputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLabelsS3InputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+
+class LabelsS3InputConfigurationOutputTypeDef(
+    _RequiredLabelsS3InputConfigurationOutputTypeDef,
+    _OptionalLabelsS3InputConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredLabelsS3InputConfigurationTypeDef = TypedDict(
     "_RequiredLabelsS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalLabelsS3InputConfigurationTypeDef = TypedDict(
@@ -780,14 +897,22 @@
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
 _RequiredMonotonicValuesTypeDef = TypedDict(
     "_RequiredMonotonicValuesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
     },
 )
 _OptionalMonotonicValuesTypeDef = TypedDict(
@@ -940,22 +1065,14 @@
 
 class CreateLabelGroupRequestRequestTypeDef(
     _RequiredCreateLabelGroupRequestRequestTypeDef, _OptionalCreateLabelGroupRequestRequestTypeDef
 ):
     pass
 
 
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
@@ -996,24 +1113,56 @@
 
 class IngestedFilesSummaryTypeDef(
     _RequiredIngestedFilesSummaryTypeDef, _OptionalIngestedFilesSummaryTypeDef
 ):
     pass
 
 
+InferenceInputConfigurationOutputTypeDef = TypedDict(
+    "InferenceInputConfigurationOutputTypeDef",
+    {
+        "S3InputConfiguration": InferenceS3InputConfigurationOutputTypeDef,
+        "InputTimeZoneOffset": str,
+        "InferenceInputNameConfiguration": InferenceInputNameConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 InferenceInputConfigurationTypeDef = TypedDict(
     "InferenceInputConfigurationTypeDef",
     {
         "S3InputConfiguration": InferenceS3InputConfigurationTypeDef,
         "InputTimeZoneOffset": str,
         "InferenceInputNameConfiguration": InferenceInputNameConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredInferenceOutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredInferenceOutputConfigurationOutputTypeDef",
+    {
+        "S3OutputConfiguration": InferenceS3OutputConfigurationOutputTypeDef,
+    },
+)
+_OptionalInferenceOutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalInferenceOutputConfigurationOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class InferenceOutputConfigurationOutputTypeDef(
+    _RequiredInferenceOutputConfigurationOutputTypeDef,
+    _OptionalInferenceOutputConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredInferenceOutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceOutputConfigurationTypeDef",
     {
         "S3OutputConfiguration": InferenceS3OutputConfigurationTypeDef,
     },
 )
 _OptionalInferenceOutputConfigurationTypeDef = TypedDict(
@@ -1036,14 +1185,21 @@
     {
         "NextToken": str,
         "InferenceSchedulerSummaries": List[InferenceSchedulerSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IngestionInputConfigurationOutputTypeDef = TypedDict(
+    "IngestionInputConfigurationOutputTypeDef",
+    {
+        "S3InputConfiguration": IngestionS3InputConfigurationOutputTypeDef,
+    },
+)
+
 IngestionInputConfigurationTypeDef = TypedDict(
     "IngestionInputConfigurationTypeDef",
     {
         "S3InputConfiguration": IngestionS3InputConfigurationTypeDef,
     },
 )
 
@@ -1069,14 +1225,23 @@
     {
         "NextToken": str,
         "LabelSummaries": List[LabelSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LabelsInputConfigurationOutputTypeDef = TypedDict(
+    "LabelsInputConfigurationOutputTypeDef",
+    {
+        "S3InputConfiguration": LabelsS3InputConfigurationOutputTypeDef,
+        "LabelGroupName": str,
+    },
+    total=False,
+)
+
 LabelsInputConfigurationTypeDef = TypedDict(
     "LabelsInputConfigurationTypeDef",
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
         "LabelGroupName": str,
     },
     total=False,
@@ -1087,14 +1252,22 @@
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
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
 SensorStatisticsSummaryTypeDef = TypedDict(
     "SensorStatisticsSummaryTypeDef",
     {
         "ComponentName": str,
         "SensorName": str,
         "DataExists": bool,
         "MissingValues": CountPercentTypeDef,
@@ -1107,58 +1280,28 @@
         "MonotonicValues": MonotonicValuesTypeDef,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "DataUploadFrequency": DataUploadFrequencyType,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
-        "RoleArn": str,
-        "ClientToken": str,
-    },
-)
-_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "DataDelayOffsetInMinutes": int,
-        "ServerSideKmsKeyId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateInferenceSchedulerRequestRequestTypeDef(
-    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
-    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeInferenceSchedulerResponseTypeDef = TypedDict(
     "DescribeInferenceSchedulerResponseTypeDef",
     {
         "ModelArn": str,
         "ModelName": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "Status": InferenceSchedulerStatusType,
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
         "RoleArn": str,
         "ServerSideKmsKeyId": str,
         "LatestInferenceResult": LatestInferenceResultType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1168,23 +1311,53 @@
         "ModelName": str,
         "ModelArn": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "ScheduledStartTime": datetime,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
         "CustomerResultObject": S3ObjectTypeDef,
         "Status": InferenceExecutionStatusType,
         "FailedReason": str,
     },
     total=False,
 )
 
+_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "DataUploadFrequency": DataUploadFrequencyType,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "RoleArn": str,
+        "ClientToken": str,
+    },
+)
+_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "DataDelayOffsetInMinutes": int,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateInferenceSchedulerRequestRequestTypeDef(
+    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
+    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 _OptionalUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
@@ -1209,15 +1382,15 @@
 
 DataIngestionJobSummaryTypeDef = TypedDict(
     "DataIngestionJobSummaryTypeDef",
     {
         "JobId": str,
         "DatasetName": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
         "Status": IngestionJobStatusType,
     },
     total=False,
 )
 
 StartDataIngestionJobRequestRequestTypeDef = TypedDict(
     "StartDataIngestionJobRequestRequestTypeDef",
@@ -1236,14 +1409,42 @@
         "MissingSensorData": MissingSensorDataTypeDef,
         "InvalidSensorData": InvalidSensorDataTypeDef,
         "UnsupportedTimestamps": UnsupportedTimestampsTypeDef,
         "DuplicateTimestamps": DuplicateTimestampsTypeDef,
     },
 )
 
+DescribeModelResponseTypeDef = TypedDict(
+    "DescribeModelResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Schema": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationOutputTypeDef,
+        "TrainingDataStartTime": datetime,
+        "TrainingDataEndTime": datetime,
+        "EvaluationDataStartTime": datetime,
+        "EvaluationDataEndTime": datetime,
+        "RoleArn": str,
+        "DataPreProcessingConfiguration": DataPreProcessingConfigurationOutputTypeDef,
+        "Status": ModelStatusType,
+        "TrainingExecutionStartTime": datetime,
+        "TrainingExecutionEndTime": datetime,
+        "FailedReason": str,
+        "ModelMetrics": str,
+        "LastUpdatedTime": datetime,
+        "CreatedAt": datetime,
+        "ServerSideKmsKeyId": str,
+        "OffCondition": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ModelName": str,
         "DatasetName": str,
         "ClientToken": str,
     },
@@ -1269,42 +1470,14 @@
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
 
-DescribeModelResponseTypeDef = TypedDict(
-    "DescribeModelResponseTypeDef",
-    {
-        "ModelName": str,
-        "ModelArn": str,
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Schema": str,
-        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
-        "TrainingDataStartTime": datetime,
-        "TrainingDataEndTime": datetime,
-        "EvaluationDataStartTime": datetime,
-        "EvaluationDataEndTime": datetime,
-        "RoleArn": str,
-        "DataPreProcessingConfiguration": DataPreProcessingConfigurationTypeDef,
-        "Status": ModelStatusType,
-        "TrainingExecutionStartTime": datetime,
-        "TrainingExecutionEndTime": datetime,
-        "FailedReason": str,
-        "ModelMetrics": str,
-        "LastUpdatedTime": datetime,
-        "CreatedAt": datetime,
-        "ServerSideKmsKeyId": str,
-        "OffCondition": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1329,15 +1502,15 @@
 )
 
 DescribeDataIngestionJobResponseTypeDef = TypedDict(
     "DescribeDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
         "RoleArn": str,
         "CreatedAt": datetime,
         "Status": IngestionJobStatusType,
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
@@ -1354,15 +1527,15 @@
         "DatasetName": str,
         "DatasetArn": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Status": DatasetStatusType,
         "Schema": str,
         "ServerSideKmsKeyId": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment/type_defs.pyi` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     "CreateDatasetResponseTypeDef",
     "CreateInferenceSchedulerResponseTypeDef",
     "CreateLabelGroupResponseTypeDef",
     "CreateLabelRequestRequestTypeDef",
     "CreateLabelResponseTypeDef",
     "DataPreProcessingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
+    "DataPreProcessingConfigurationOutputTypeDef",
     "DuplicateTimestampsTypeDef",
     "InvalidSensorDataTypeDef",
     "MissingSensorDataTypeDef",
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
@@ -63,72 +64,82 @@
     "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelRequestRequestTypeDef",
     "DescribeLabelResponseTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
+    "InferenceInputNameConfigurationOutputTypeDef",
+    "InferenceS3InputConfigurationOutputTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
+    "InferenceS3OutputConfigurationOutputTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
+    "IngestionS3InputConfigurationOutputTypeDef",
     "IngestionS3InputConfigurationTypeDef",
     "MissingCompleteSensorDataTypeDef",
     "SensorsWithShortDateRangeTypeDef",
     "LabelGroupSummaryTypeDef",
     "LabelSummaryTypeDef",
+    "LabelsS3InputConfigurationOutputTypeDef",
     "LabelsS3InputConfigurationTypeDef",
     "LargeTimestampGapsTypeDef",
     "ListDataIngestionJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListInferenceEventsRequestRequestTypeDef",
     "ListInferenceExecutionsRequestRequestTypeDef",
     "ListInferenceSchedulersRequestRequestTypeDef",
     "ListLabelGroupsRequestRequestTypeDef",
     "ListLabelsRequestRequestTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
     "ResponseMetadataTypeDef",
     "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
     "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
     "StopInferenceSchedulerResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
+    "InferenceInputConfigurationOutputTypeDef",
     "InferenceInputConfigurationTypeDef",
+    "InferenceOutputConfigurationOutputTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
+    "IngestionInputConfigurationOutputTypeDef",
     "IngestionInputConfigurationTypeDef",
     "InsufficientSensorDataTypeDef",
     "ListLabelGroupsResponseTypeDef",
     "ListLabelsResponseTypeDef",
+    "LabelsInputConfigurationOutputTypeDef",
     "LabelsInputConfigurationTypeDef",
     "ListModelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SensorStatisticsSummaryTypeDef",
-    "CreateInferenceSchedulerRequestRequestTypeDef",
     "DescribeInferenceSchedulerResponseTypeDef",
     "InferenceExecutionSummaryTypeDef",
+    "CreateInferenceSchedulerRequestRequestTypeDef",
     "UpdateInferenceSchedulerRequestRequestTypeDef",
     "DataIngestionJobSummaryTypeDef",
     "StartDataIngestionJobRequestRequestTypeDef",
     "DataQualitySummaryTypeDef",
-    "CreateModelRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
+    "CreateModelRequestRequestTypeDef",
     "ListSensorStatisticsResponseTypeDef",
     "ListInferenceExecutionsResponseTypeDef",
     "ListDataIngestionJobsResponseTypeDef",
     "DescribeDataIngestionJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
@@ -250,14 +261,22 @@
     {
         "ModelArn": str,
         "Status": ModelStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataPreProcessingConfigurationOutputTypeDef = TypedDict(
+    "DataPreProcessingConfigurationOutputTypeDef",
+    {
+        "TargetSamplingRate": TargetSamplingRateType,
+    },
+    total=False,
+)
+
 DuplicateTimestampsTypeDef = TypedDict(
     "DuplicateTimestampsTypeDef",
     {
         "TotalNumberOfDuplicateTimestamps": int,
     },
 )
 
@@ -427,14 +446,43 @@
     "S3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
+InferenceInputNameConfigurationOutputTypeDef = TypedDict(
+    "InferenceInputNameConfigurationOutputTypeDef",
+    {
+        "TimestampFormat": str,
+        "ComponentTimestampDelimiter": str,
+    },
+    total=False,
+)
+
+_RequiredInferenceS3InputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredInferenceS3InputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalInferenceS3InputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalInferenceS3InputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+class InferenceS3InputConfigurationOutputTypeDef(
+    _RequiredInferenceS3InputConfigurationOutputTypeDef,
+    _OptionalInferenceS3InputConfigurationOutputTypeDef,
+):
+    pass
+
 InferenceInputNameConfigurationTypeDef = TypedDict(
     "InferenceInputNameConfigurationTypeDef",
     {
         "TimestampFormat": str,
         "ComponentTimestampDelimiter": str,
     },
     total=False,
@@ -455,14 +503,34 @@
 )
 
 class InferenceS3InputConfigurationTypeDef(
     _RequiredInferenceS3InputConfigurationTypeDef, _OptionalInferenceS3InputConfigurationTypeDef
 ):
     pass
 
+_RequiredInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredInferenceS3OutputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalInferenceS3OutputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+class InferenceS3OutputConfigurationOutputTypeDef(
+    _RequiredInferenceS3OutputConfigurationOutputTypeDef,
+    _OptionalInferenceS3OutputConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredInferenceS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceS3OutputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalInferenceS3OutputConfigurationTypeDef = TypedDict(
@@ -489,14 +557,35 @@
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "LatestInferenceResult": LatestInferenceResultType,
     },
     total=False,
 )
 
+_RequiredIngestionS3InputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredIngestionS3InputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalIngestionS3InputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalIngestionS3InputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+        "KeyPattern": str,
+    },
+    total=False,
+)
+
+class IngestionS3InputConfigurationOutputTypeDef(
+    _RequiredIngestionS3InputConfigurationOutputTypeDef,
+    _OptionalIngestionS3InputConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredIngestionS3InputConfigurationTypeDef = TypedDict(
     "_RequiredIngestionS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalIngestionS3InputConfigurationTypeDef = TypedDict(
@@ -550,14 +639,34 @@
         "FaultCode": str,
         "Equipment": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
+_RequiredLabelsS3InputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLabelsS3InputConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalLabelsS3InputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLabelsS3InputConfigurationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+class LabelsS3InputConfigurationOutputTypeDef(
+    _RequiredLabelsS3InputConfigurationOutputTypeDef,
+    _OptionalLabelsS3InputConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredLabelsS3InputConfigurationTypeDef = TypedDict(
     "_RequiredLabelsS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalLabelsS3InputConfigurationTypeDef = TypedDict(
@@ -757,14 +866,22 @@
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
 _RequiredMonotonicValuesTypeDef = TypedDict(
     "_RequiredMonotonicValuesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
     },
 )
 _OptionalMonotonicValuesTypeDef = TypedDict(
@@ -909,22 +1026,14 @@
 )
 
 class CreateLabelGroupRequestRequestTypeDef(
     _RequiredCreateLabelGroupRequestRequestTypeDef, _OptionalCreateLabelGroupRequestRequestTypeDef
 ):
     pass
 
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
@@ -963,24 +1072,54 @@
 )
 
 class IngestedFilesSummaryTypeDef(
     _RequiredIngestedFilesSummaryTypeDef, _OptionalIngestedFilesSummaryTypeDef
 ):
     pass
 
+InferenceInputConfigurationOutputTypeDef = TypedDict(
+    "InferenceInputConfigurationOutputTypeDef",
+    {
+        "S3InputConfiguration": InferenceS3InputConfigurationOutputTypeDef,
+        "InputTimeZoneOffset": str,
+        "InferenceInputNameConfiguration": InferenceInputNameConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 InferenceInputConfigurationTypeDef = TypedDict(
     "InferenceInputConfigurationTypeDef",
     {
         "S3InputConfiguration": InferenceS3InputConfigurationTypeDef,
         "InputTimeZoneOffset": str,
         "InferenceInputNameConfiguration": InferenceInputNameConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredInferenceOutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredInferenceOutputConfigurationOutputTypeDef",
+    {
+        "S3OutputConfiguration": InferenceS3OutputConfigurationOutputTypeDef,
+    },
+)
+_OptionalInferenceOutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalInferenceOutputConfigurationOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class InferenceOutputConfigurationOutputTypeDef(
+    _RequiredInferenceOutputConfigurationOutputTypeDef,
+    _OptionalInferenceOutputConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredInferenceOutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceOutputConfigurationTypeDef",
     {
         "S3OutputConfiguration": InferenceS3OutputConfigurationTypeDef,
     },
 )
 _OptionalInferenceOutputConfigurationTypeDef = TypedDict(
@@ -1001,14 +1140,21 @@
     {
         "NextToken": str,
         "InferenceSchedulerSummaries": List[InferenceSchedulerSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IngestionInputConfigurationOutputTypeDef = TypedDict(
+    "IngestionInputConfigurationOutputTypeDef",
+    {
+        "S3InputConfiguration": IngestionS3InputConfigurationOutputTypeDef,
+    },
+)
+
 IngestionInputConfigurationTypeDef = TypedDict(
     "IngestionInputConfigurationTypeDef",
     {
         "S3InputConfiguration": IngestionS3InputConfigurationTypeDef,
     },
 )
 
@@ -1034,14 +1180,23 @@
     {
         "NextToken": str,
         "LabelSummaries": List[LabelSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LabelsInputConfigurationOutputTypeDef = TypedDict(
+    "LabelsInputConfigurationOutputTypeDef",
+    {
+        "S3InputConfiguration": LabelsS3InputConfigurationOutputTypeDef,
+        "LabelGroupName": str,
+    },
+    total=False,
+)
+
 LabelsInputConfigurationTypeDef = TypedDict(
     "LabelsInputConfigurationTypeDef",
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
         "LabelGroupName": str,
     },
     total=False,
@@ -1052,14 +1207,22 @@
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
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
 SensorStatisticsSummaryTypeDef = TypedDict(
     "SensorStatisticsSummaryTypeDef",
     {
         "ComponentName": str,
         "SensorName": str,
         "DataExists": bool,
         "MissingValues": CountPercentTypeDef,
@@ -1072,56 +1235,28 @@
         "MonotonicValues": MonotonicValuesTypeDef,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "DataUploadFrequency": DataUploadFrequencyType,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
-        "RoleArn": str,
-        "ClientToken": str,
-    },
-)
-_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "DataDelayOffsetInMinutes": int,
-        "ServerSideKmsKeyId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateInferenceSchedulerRequestRequestTypeDef(
-    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
-    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
-):
-    pass
-
 DescribeInferenceSchedulerResponseTypeDef = TypedDict(
     "DescribeInferenceSchedulerResponseTypeDef",
     {
         "ModelArn": str,
         "ModelName": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "Status": InferenceSchedulerStatusType,
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
         "RoleArn": str,
         "ServerSideKmsKeyId": str,
         "LatestInferenceResult": LatestInferenceResultType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1131,23 +1266,51 @@
         "ModelName": str,
         "ModelArn": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "ScheduledStartTime": datetime,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
         "CustomerResultObject": S3ObjectTypeDef,
         "Status": InferenceExecutionStatusType,
         "FailedReason": str,
     },
     total=False,
 )
 
+_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "DataUploadFrequency": DataUploadFrequencyType,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "RoleArn": str,
+        "ClientToken": str,
+    },
+)
+_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "DataDelayOffsetInMinutes": int,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateInferenceSchedulerRequestRequestTypeDef(
+    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
+    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 _OptionalUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
@@ -1170,15 +1333,15 @@
 
 DataIngestionJobSummaryTypeDef = TypedDict(
     "DataIngestionJobSummaryTypeDef",
     {
         "JobId": str,
         "DatasetName": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
         "Status": IngestionJobStatusType,
     },
     total=False,
 )
 
 StartDataIngestionJobRequestRequestTypeDef = TypedDict(
     "StartDataIngestionJobRequestRequestTypeDef",
@@ -1197,14 +1360,42 @@
         "MissingSensorData": MissingSensorDataTypeDef,
         "InvalidSensorData": InvalidSensorDataTypeDef,
         "UnsupportedTimestamps": UnsupportedTimestampsTypeDef,
         "DuplicateTimestamps": DuplicateTimestampsTypeDef,
     },
 )
 
+DescribeModelResponseTypeDef = TypedDict(
+    "DescribeModelResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Schema": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationOutputTypeDef,
+        "TrainingDataStartTime": datetime,
+        "TrainingDataEndTime": datetime,
+        "EvaluationDataStartTime": datetime,
+        "EvaluationDataEndTime": datetime,
+        "RoleArn": str,
+        "DataPreProcessingConfiguration": DataPreProcessingConfigurationOutputTypeDef,
+        "Status": ModelStatusType,
+        "TrainingExecutionStartTime": datetime,
+        "TrainingExecutionEndTime": datetime,
+        "FailedReason": str,
+        "ModelMetrics": str,
+        "LastUpdatedTime": datetime,
+        "CreatedAt": datetime,
+        "ServerSideKmsKeyId": str,
+        "OffCondition": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ModelName": str,
         "DatasetName": str,
         "ClientToken": str,
     },
@@ -1228,42 +1419,14 @@
 )
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-DescribeModelResponseTypeDef = TypedDict(
-    "DescribeModelResponseTypeDef",
-    {
-        "ModelName": str,
-        "ModelArn": str,
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Schema": str,
-        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
-        "TrainingDataStartTime": datetime,
-        "TrainingDataEndTime": datetime,
-        "EvaluationDataStartTime": datetime,
-        "EvaluationDataEndTime": datetime,
-        "RoleArn": str,
-        "DataPreProcessingConfiguration": DataPreProcessingConfigurationTypeDef,
-        "Status": ModelStatusType,
-        "TrainingExecutionStartTime": datetime,
-        "TrainingExecutionEndTime": datetime,
-        "FailedReason": str,
-        "ModelMetrics": str,
-        "LastUpdatedTime": datetime,
-        "CreatedAt": datetime,
-        "ServerSideKmsKeyId": str,
-        "OffCondition": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1288,15 +1451,15 @@
 )
 
 DescribeDataIngestionJobResponseTypeDef = TypedDict(
     "DescribeDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
         "RoleArn": str,
         "CreatedAt": datetime,
         "Status": IngestionJobStatusType,
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
@@ -1313,15 +1476,15 @@
         "DatasetName": str,
         "DatasetArn": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Status": DatasetStatusType,
         "Schema": str,
         "ServerSideKmsKeyId": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/PKG-INFO` & `mypy-boto3-lookoutequipment-1.28.12/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-lookoutequipment
-Version: 1.28.0
-Summary: Type annotations for boto3.LookoutEquipment 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lookoutequipment type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-lookoutequipment"></a>
 
 # mypy-boto3-lookoutequipment
 
 [![PyPI - mypy-boto3-lookoutequipment](https://img.shields.io/pypi/v/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutequipment?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutequipment)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutequipment)](https://pepy.tech/project/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,14 +287,15 @@
     CreateDatasetResponseTypeDef,
     CreateInferenceSchedulerResponseTypeDef,
     CreateLabelGroupResponseTypeDef,
     CreateLabelRequestRequestTypeDef,
     CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
     CreateModelResponseTypeDef,
+    DataPreProcessingConfigurationOutputTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
@@ -340,72 +309,82 @@
     DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
     DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
+    InferenceInputNameConfigurationOutputTypeDef,
+    InferenceS3InputConfigurationOutputTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
+    InferenceS3OutputConfigurationOutputTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
+    IngestionS3InputConfigurationOutputTypeDef,
     IngestionS3InputConfigurationTypeDef,
     MissingCompleteSensorDataTypeDef,
     SensorsWithShortDateRangeTypeDef,
     LabelGroupSummaryTypeDef,
     LabelSummaryTypeDef,
+    LabelsS3InputConfigurationOutputTypeDef,
     LabelsS3InputConfigurationTypeDef,
     LargeTimestampGapsTypeDef,
     ListDataIngestionJobsRequestRequestTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListInferenceEventsRequestRequestTypeDef,
     ListInferenceExecutionsRequestRequestTypeDef,
     ListInferenceSchedulersRequestRequestTypeDef,
     ListLabelGroupsRequestRequestTypeDef,
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
     ResponseMetadataTypeDef,
     StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
     StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
     StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
+    InferenceInputConfigurationOutputTypeDef,
     InferenceInputConfigurationTypeDef,
+    InferenceOutputConfigurationOutputTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
+    IngestionInputConfigurationOutputTypeDef,
     IngestionInputConfigurationTypeDef,
     InsufficientSensorDataTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
+    LabelsInputConfigurationOutputTypeDef,
     LabelsInputConfigurationTypeDef,
     ListModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SensorStatisticsSummaryTypeDef,
-    CreateInferenceSchedulerRequestRequestTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     InferenceExecutionSummaryTypeDef,
+    CreateInferenceSchedulerRequestRequestTypeDef,
     UpdateInferenceSchedulerRequestRequestTypeDef,
     DataIngestionJobSummaryTypeDef,
     StartDataIngestionJobRequestRequestTypeDef,
     DataQualitySummaryTypeDef,
-    CreateModelRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
+    CreateModelRequestRequestTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.0/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt` & `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.0/setup.py` & `mypy-boto3-lookoutequipment-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutequipment",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_lookoutequipment"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutEquipment 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.LookoutEquipment 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

