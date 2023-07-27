# Comparing `tmp/mypy-boto3-machinelearning-1.28.0.tar.gz` & `tmp/mypy-boto3-machinelearning-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-machinelearning-1.28.0.tar", last modified: Thu Jul  6 21:00:02 2023, max compression
+gzip compressed data, was "mypy-boto3-machinelearning-1.28.12.tar", last modified: Thu Jul 27 05:34:58 2023, max compression
```

## Comparing `mypy-boto3-machinelearning-1.28.0.tar` & `mypy-boto3-machinelearning-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.314360 mypy-boto3-machinelearning-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-06 21:00:02.314360 mypy-boto3-machinelearning-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.298359 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31699 2023-07-06 20:46:23.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-06 20:46:22.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.314360 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-06 21:00:02.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-06 21:00:02.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:02.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:02.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:02.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 21:00:02.000000 mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:02.314360 mypy-boto3-machinelearning-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 20:46:21.000000 mypy-boto3-machinelearning-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-27 05:25:44.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-07-27 05:25:44.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32223 2023-07-27 05:25:44.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/setup.py
```

### Comparing `mypy-boto3-machinelearning-1.28.0/LICENSE` & `mypy-boto3-machinelearning-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/PKG-INFO` & `mypy-boto3-machinelearning-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-machinelearning
-Version: 1.28.0
-Summary: Type annotations for boto3.MachineLearning 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MachineLearning 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-machinelearning"></a>
 
 # mypy-boto3-machinelearning
 
 [![PyPI - mypy-boto3-machinelearning](https://img.shields.io/pypi/v/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-machinelearning?color=blue)](https://pypistats.org/packages/mypy-boto3-machinelearning)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-machinelearning)](https://pepy.tech/project/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -420,48 +420,51 @@
     DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
     DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
     DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
+    TagOutputTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
     GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
     PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
+    RDSDatabaseOutputTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
+    RedshiftDatabaseOutputTypeDef,
     ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
     UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
     UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
     UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
     UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
+    DescribeTagsOutputTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
```

### Comparing `mypy-boto3-machinelearning-1.28.0/README.md` & `mypy-boto3-machinelearning-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-machinelearning"></a>
 
 # mypy-boto3-machinelearning
 
 [![PyPI - mypy-boto3-machinelearning](https://img.shields.io/pypi/v/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-machinelearning?color=blue)](https://pypistats.org/packages/mypy-boto3-machinelearning)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-machinelearning)](https://pepy.tech/project/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,48 +388,51 @@
     DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
     DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
     DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
+    TagOutputTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
     GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
     PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
+    RDSDatabaseOutputTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
+    RedshiftDatabaseOutputTypeDef,
     ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
     UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
     UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
     UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
     UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
+    DescribeTagsOutputTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
```

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/__init__.py` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/__init__.pyi` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/__main__.py` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MachineLearning 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MachineLearning 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning\nOther"
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

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/client.py` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/client.pyi` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/literals.py` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
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
@@ -300,26 +301,28 @@
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

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/literals.pyi` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -298,26 +299,28 @@
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

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/paginator.py` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/paginator.pyi` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/type_defs.py` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,48 +71,51 @@
     "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
     "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
     "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
+    "TagOutputTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
     "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
+    "RDSDatabaseOutputTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
+    "RedshiftDatabaseOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
     "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
     "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
     "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
     "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
-    "DescribeTagsOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
+    "DescribeTagsOutputTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -565,14 +568,23 @@
     "DescribeTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 PerformanceMetricsTypeDef = TypedDict(
     "PerformanceMetricsTypeDef",
     {
         "Properties": Dict[str, str],
     },
     total=False,
 )
@@ -699,14 +711,22 @@
     "RDSDatabaseTypeDef",
     {
         "InstanceIdentifier": str,
         "DatabaseName": str,
     },
 )
 
+RDSDatabaseOutputTypeDef = TypedDict(
+    "RDSDatabaseOutputTypeDef",
+    {
+        "InstanceIdentifier": str,
+        "DatabaseName": str,
+    },
+)
+
 RedshiftDatabaseCredentialsTypeDef = TypedDict(
     "RedshiftDatabaseCredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
     },
 )
@@ -715,14 +735,22 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
     },
 )
 
+RedshiftDatabaseOutputTypeDef = TypedDict(
+    "RedshiftDatabaseOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "ClusterIdentifier": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -813,24 +841,14 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1004,14 +1022,24 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
         "InputDataLocationS3": str,
@@ -1086,15 +1114,15 @@
 class RDSDataSpecTypeDef(_RequiredRDSDataSpecTypeDef, _OptionalRDSDataSpecTypeDef):
     pass
 
 
 RDSMetadataTypeDef = TypedDict(
     "RDSMetadataTypeDef",
     {
-        "Database": RDSDatabaseTypeDef,
+        "Database": RDSDatabaseOutputTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
         "ResourceRole": str,
         "ServiceRole": str,
         "DataPipelineId": str,
     },
     total=False,
@@ -1123,15 +1151,15 @@
 class RedshiftDataSpecTypeDef(_RequiredRedshiftDataSpecTypeDef, _OptionalRedshiftDataSpecTypeDef):
     pass
 
 
 RedshiftMetadataTypeDef = TypedDict(
     "RedshiftMetadataTypeDef",
     {
-        "RedshiftDatabase": RedshiftDatabaseTypeDef,
+        "RedshiftDatabase": RedshiftDatabaseOutputTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
     },
     total=False,
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
```

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/type_defs.pyi` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -70,48 +70,51 @@
     "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
     "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
     "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
+    "TagOutputTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
     "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
+    "RDSDatabaseOutputTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
+    "RedshiftDatabaseOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
     "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
     "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
     "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
     "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
-    "DescribeTagsOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
+    "DescribeTagsOutputTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -556,14 +559,23 @@
     "DescribeTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 PerformanceMetricsTypeDef = TypedDict(
     "PerformanceMetricsTypeDef",
     {
         "Properties": Dict[str, str],
     },
     total=False,
 )
@@ -686,14 +698,22 @@
     "RDSDatabaseTypeDef",
     {
         "InstanceIdentifier": str,
         "DatabaseName": str,
     },
 )
 
+RDSDatabaseOutputTypeDef = TypedDict(
+    "RDSDatabaseOutputTypeDef",
+    {
+        "InstanceIdentifier": str,
+        "DatabaseName": str,
+    },
+)
+
 RedshiftDatabaseCredentialsTypeDef = TypedDict(
     "RedshiftDatabaseCredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
     },
 )
@@ -702,14 +722,22 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
     },
 )
 
+RedshiftDatabaseOutputTypeDef = TypedDict(
+    "RedshiftDatabaseOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "ClusterIdentifier": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -798,24 +826,14 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -987,14 +1005,24 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
         "InputDataLocationS3": str,
@@ -1067,15 +1095,15 @@
 
 class RDSDataSpecTypeDef(_RequiredRDSDataSpecTypeDef, _OptionalRDSDataSpecTypeDef):
     pass
 
 RDSMetadataTypeDef = TypedDict(
     "RDSMetadataTypeDef",
     {
-        "Database": RDSDatabaseTypeDef,
+        "Database": RDSDatabaseOutputTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
         "ResourceRole": str,
         "ServiceRole": str,
         "DataPipelineId": str,
     },
     total=False,
@@ -1102,15 +1130,15 @@
 
 class RedshiftDataSpecTypeDef(_RequiredRedshiftDataSpecTypeDef, _OptionalRedshiftDataSpecTypeDef):
     pass
 
 RedshiftMetadataTypeDef = TypedDict(
     "RedshiftMetadataTypeDef",
     {
-        "RedshiftDatabase": RedshiftDatabaseTypeDef,
+        "RedshiftDatabase": RedshiftDatabaseOutputTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
     },
     total=False,
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
```

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/waiter.py` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning/waiter.pyi` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/PKG-INFO` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-machinelearning
-Version: 1.28.0
-Summary: Type annotations for boto3.MachineLearning 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MachineLearning 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-machinelearning"></a>
 
 # mypy-boto3-machinelearning
 
 [![PyPI - mypy-boto3-machinelearning](https://img.shields.io/pypi/v/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-machinelearning?color=blue)](https://pypistats.org/packages/mypy-boto3-machinelearning)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-machinelearning)](https://pepy.tech/project/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -420,48 +420,51 @@
     DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
     DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
     DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
+    TagOutputTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
     GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
     PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
+    RDSDatabaseOutputTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
+    RedshiftDatabaseOutputTypeDef,
     ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
     UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
     UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
     UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
     UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
+    DescribeTagsOutputTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
```

### Comparing `mypy-boto3-machinelearning-1.28.0/mypy_boto3_machinelearning.egg-info/SOURCES.txt` & `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.0/setup.py` & `mypy-boto3-machinelearning-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-machinelearning",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_machinelearning"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MachineLearning 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MachineLearning 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

