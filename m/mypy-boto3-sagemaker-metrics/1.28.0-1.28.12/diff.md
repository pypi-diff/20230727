# Comparing `tmp/mypy-boto3-sagemaker-metrics-1.28.0.tar.gz` & `tmp/mypy-boto3-sagemaker-metrics-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-metrics-1.28.0.tar", last modified: Thu Jul  6 21:00:32 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-metrics-1.28.12.tar", last modified: Thu Jul 27 11:49:35 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-metrics-1.28.0.tar` & `mypy-boto3-sagemaker-metrics-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.898421 mypy-boto3-sagemaker-metrics-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-06 21:00:32.894421 mypy-boto3-sagemaker-metrics-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.874421 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 20:54:54.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.894421 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:32.898421 mypy-boto3-sagemaker-metrics-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-metrics-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.713264 mypy-boto3-sagemaker-metrics-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-07-27 11:49:35.713264 mypy-boto3-sagemaker-metrics-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.705264 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.713264 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:35.713264 mypy-boto3-sagemaker-metrics-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-metrics-1.28.12/setup.py
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/LICENSE` & `mypy-boto3-sagemaker-metrics-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/PKG-INFO` & `mypy-boto3-sagemaker-metrics-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-metrics
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakerMetrics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SageMakerMetrics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-metrics"></a>
 
 # mypy-boto3-sagemaker-metrics
 
 [![PyPI - mypy-boto3-sagemaker-metrics](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-metrics?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-metrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-metrics)](https://pepy.tech/project/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,16 +301,16 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
     RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsResponseTypeDef,
     BatchPutMetricsRequestRequestTypeDef,
+    BatchPutMetricsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/README.md` & `mypy-boto3-sagemaker-metrics-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-metrics"></a>
 
 # mypy-boto3-sagemaker-metrics
 
 [![PyPI - mypy-boto3-sagemaker-metrics](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-metrics?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-metrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-metrics)](https://pepy.tech/project/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,16 +269,16 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
     RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsResponseTypeDef,
     BatchPutMetricsRequestRequestTypeDef,
+    BatchPutMetricsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/__main__.py` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerMetrics 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SageMakerMetrics 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics\nOther"
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

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/client.py` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/client.pyi` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/literals.py` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "PutMetricsErrorCodeType",
     "SageMakerMetricsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 PutMetricsErrorCodeType = Literal[
     "CONFLICT_ERROR", "INTERNAL_ERROR", "METRIC_LIMIT_EXCEEDED", "VALIDATION_ERROR"
 ]
 SageMakerMetricsServiceName = Literal["sagemaker-metrics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -147,14 +145,15 @@
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
@@ -233,26 +232,28 @@
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

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/literals.pyi` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "PutMetricsErrorCodeType",
     "SageMakerMetricsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 PutMetricsErrorCodeType = Literal[
     "CONFLICT_ERROR", "INTERNAL_ERROR", "METRIC_LIMIT_EXCEEDED", "VALIDATION_ERROR"
 ]
 SageMakerMetricsServiceName = Literal["sagemaker-metrics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -145,14 +147,15 @@
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
@@ -231,26 +234,28 @@
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

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/type_defs.py` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchPutMetricsErrorTypeDef",
     "RawMetricDataTypeDef",
     "ResponseMetadataTypeDef",
-    "BatchPutMetricsResponseTypeDef",
     "BatchPutMetricsRequestRequestTypeDef",
+    "BatchPutMetricsResponseTypeDef",
 )
 
 BatchPutMetricsErrorTypeDef = TypedDict(
     "BatchPutMetricsErrorTypeDef",
     {
         "Code": PutMetricsErrorCodeType,
         "MetricIndex": int,
@@ -68,22 +68,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-BatchPutMetricsResponseTypeDef = TypedDict(
-    "BatchPutMetricsResponseTypeDef",
-    {
-        "Errors": List[BatchPutMetricsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchPutMetricsRequestRequestTypeDef = TypedDict(
     "BatchPutMetricsRequestRequestTypeDef",
     {
         "TrialComponentName": str,
         "MetricData": Sequence[RawMetricDataTypeDef],
     },
 )
+
+BatchPutMetricsResponseTypeDef = TypedDict(
+    "BatchPutMetricsResponseTypeDef",
+    {
+        "Errors": List[BatchPutMetricsErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics/type_defs.pyi` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchPutMetricsErrorTypeDef",
     "RawMetricDataTypeDef",
     "ResponseMetadataTypeDef",
-    "BatchPutMetricsResponseTypeDef",
     "BatchPutMetricsRequestRequestTypeDef",
+    "BatchPutMetricsResponseTypeDef",
 )
 
 BatchPutMetricsErrorTypeDef = TypedDict(
     "BatchPutMetricsErrorTypeDef",
     {
         "Code": PutMetricsErrorCodeType,
         "MetricIndex": int,
@@ -65,22 +65,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-BatchPutMetricsResponseTypeDef = TypedDict(
-    "BatchPutMetricsResponseTypeDef",
-    {
-        "Errors": List[BatchPutMetricsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchPutMetricsRequestRequestTypeDef = TypedDict(
     "BatchPutMetricsRequestRequestTypeDef",
     {
         "TrialComponentName": str,
         "MetricData": Sequence[RawMetricDataTypeDef],
     },
 )
+
+BatchPutMetricsResponseTypeDef = TypedDict(
+    "BatchPutMetricsResponseTypeDef",
+    {
+        "Errors": List[BatchPutMetricsErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-metrics
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakerMetrics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SageMakerMetrics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-metrics"></a>
 
 # mypy-boto3-sagemaker-metrics
 
 [![PyPI - mypy-boto3-sagemaker-metrics](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-metrics?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-metrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-metrics)](https://pepy.tech/project/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,16 +301,16 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
     RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsResponseTypeDef,
     BatchPutMetricsRequestRequestTypeDef,
+    BatchPutMetricsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-metrics-1.28.12/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.28.0/setup.py` & `mypy-boto3-sagemaker-metrics-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-metrics",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sagemaker_metrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerMetrics 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SageMakerMetrics 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

