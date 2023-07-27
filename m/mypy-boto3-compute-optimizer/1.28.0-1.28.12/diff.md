# Comparing `tmp/mypy-boto3-compute-optimizer-1.28.0.tar.gz` & `tmp/mypy-boto3-compute-optimizer-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-compute-optimizer-1.28.0.tar", last modified: Thu Jul  6 20:59:19 2023, max compression
+gzip compressed data, was "mypy-boto3-compute-optimizer-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
```

## Comparing `mypy-boto3-compute-optimizer-1.28.0.tar` & `mypy-boto3-compute-optimizer-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.170266 mypy-boto3-compute-optimizer-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-07-06 20:59:19.170266 mypy-boto3-compute-optimizer-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.150266 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-07-06 20:36:41.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-07-06 20:36:41.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23909 2023-07-06 20:36:41.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-06 20:36:41.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-06 20:36:41.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42033 2023-07-06 20:36:42.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42010 2023-07-06 20:36:42.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.170266 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-07-06 20:59:18.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 20:59:18.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:18.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:18.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:18.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:18.000000 mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:19.170266 mypy-boto3-compute-optimizer-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:36:40.000000 mypy-boto3-compute-optimizer-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-07-27 05:19:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-07-27 05:19:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42449 2023-07-27 05:19:31.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-07-27 05:19:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/setup.py
```

### Comparing `mypy-boto3-compute-optimizer-1.28.0/LICENSE` & `mypy-boto3-compute-optimizer-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/PKG-INFO` & `mypy-boto3-compute-optimizer-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.28.0
-Summary: Type annotations for boto3.ComputeOptimizer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ComputeOptimizer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-compute-optimizer"></a>
 
 # mypy-boto3-compute-optimizer
 
 [![PyPI - mypy-boto3-compute-optimizer](https://img.shields.io/pypi/v/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,35 +406,37 @@
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
-    ExternalMetricsPreferenceTypeDef,
+    ExternalMetricsPreferenceOutputTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
+    ExternalMetricsPreferenceTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
     GetEnrollmentStatusResponseTypeDef,
     GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
     PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
+    ScopeOutputTypeDef,
     ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
     UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
     GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
@@ -444,16 +446,14 @@
     DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
-    PutRecommendationPreferencesRequestRequestTypeDef,
-    RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
@@ -466,27 +466,29 @@
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
+    RecommendationPreferencesDetailTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
-    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
     InstanceRecommendationOptionTypeDef,
     LambdaFunctionMemoryRecommendationOptionTypeDef,
     VolumeRecommendationOptionTypeDef,
     RecommendationExportJobTypeDef,
     GetEC2RecommendationProjectedMetricsResponseTypeDef,
     RecommendationSummaryTypeDef,
+    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationTypeDef,
     ECSServiceRecommendationTypeDef,
     InstanceRecommendationTypeDef,
     LambdaFunctionRecommendationTypeDef,
     VolumeRecommendationTypeDef,
     DescribeRecommendationExportJobsResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.0/README.md` & `mypy-boto3-compute-optimizer-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-compute-optimizer"></a>
 
 # mypy-boto3-compute-optimizer
 
 [![PyPI - mypy-boto3-compute-optimizer](https://img.shields.io/pypi/v/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,35 +374,37 @@
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
-    ExternalMetricsPreferenceTypeDef,
+    ExternalMetricsPreferenceOutputTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
+    ExternalMetricsPreferenceTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
     GetEnrollmentStatusResponseTypeDef,
     GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
     PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
+    ScopeOutputTypeDef,
     ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
     UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
     GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
@@ -412,16 +414,14 @@
     DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
-    PutRecommendationPreferencesRequestRequestTypeDef,
-    RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
@@ -434,27 +434,29 @@
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
+    RecommendationPreferencesDetailTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
-    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
     InstanceRecommendationOptionTypeDef,
     LambdaFunctionMemoryRecommendationOptionTypeDef,
     VolumeRecommendationOptionTypeDef,
     RecommendationExportJobTypeDef,
     GetEC2RecommendationProjectedMetricsResponseTypeDef,
     RecommendationSummaryTypeDef,
+    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationTypeDef,
     ECSServiceRecommendationTypeDef,
     InstanceRecommendationTypeDef,
     LambdaFunctionRecommendationTypeDef,
     VolumeRecommendationTypeDef,
     DescribeRecommendationExportJobsResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/__init__.py` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/__init__.pyi` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/__main__.py` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComputeOptimizer 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ComputeOptimizer 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
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

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/client.py` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/client.pyi` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/literals.py` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,15 @@
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
@@ -614,26 +615,28 @@
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

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/literals.pyi` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -526,14 +526,15 @@
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
@@ -612,26 +613,28 @@
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

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/paginator.py` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/paginator.pyi` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/type_defs.py` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,35 +83,37 @@
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
     "TagTypeDef",
-    "ExternalMetricsPreferenceTypeDef",
+    "ExternalMetricsPreferenceOutputTypeDef",
     "EnrollmentFilterTypeDef",
     "EstimatedMonthlySavingsTypeDef",
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
+    "ExternalMetricsPreferenceTypeDef",
     "GetRecommendationErrorTypeDef",
     "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     "GetEnrollmentStatusResponseTypeDef",
     "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
     "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
+    "ScopeOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
     "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
     "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
@@ -121,16 +123,14 @@
     "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     "DescribeRecommendationExportJobsRequestRequestTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
-    "PutRecommendationPreferencesRequestRequestTypeDef",
-    "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
     "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
@@ -143,27 +143,29 @@
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
+    "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
+    "RecommendationPreferencesDetailTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
-    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
     "InstanceRecommendationOptionTypeDef",
     "LambdaFunctionMemoryRecommendationOptionTypeDef",
     "VolumeRecommendationOptionTypeDef",
     "RecommendationExportJobTypeDef",
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     "RecommendationSummaryTypeDef",
+    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationTypeDef",
     "ECSServiceRecommendationTypeDef",
     "InstanceRecommendationTypeDef",
     "LambdaFunctionRecommendationTypeDef",
     "VolumeRecommendationTypeDef",
     "DescribeRecommendationExportJobsResponseTypeDef",
     "GetRecommendationSummariesResponseTypeDef",
@@ -309,16 +311,16 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-ExternalMetricsPreferenceTypeDef = TypedDict(
-    "ExternalMetricsPreferenceTypeDef",
+ExternalMetricsPreferenceOutputTypeDef = TypedDict(
+    "ExternalMetricsPreferenceOutputTypeDef",
     {
         "source": ExternalMetricsSourceType,
     },
     total=False,
 )
 
 EnrollmentFilterTypeDef = TypedDict(
@@ -389,14 +391,22 @@
     {
         "statusCode": ExternalMetricStatusCodeType,
         "statusReason": str,
     },
     total=False,
 )
 
+ExternalMetricsPreferenceTypeDef = TypedDict(
+    "ExternalMetricsPreferenceTypeDef",
+    {
+        "source": ExternalMetricsSourceType,
+    },
+    total=False,
+)
+
 GetRecommendationErrorTypeDef = TypedDict(
     "GetRecommendationErrorTypeDef",
     {
         "identifier": str,
         "code": str,
         "message": str,
     },
@@ -506,14 +516,23 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
     },
     total=False,
 )
 
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "name": ScopeNameType,
+        "value": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -722,65 +741,28 @@
 
 EffectiveRecommendationPreferencesTypeDef = TypedDict(
     "EffectiveRecommendationPreferencesTypeDef",
     {
         "cpuVendorArchitectures": List[CpuVendorArchitectureType],
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
     },
     total=False,
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-    },
-    total=False,
-)
-
-
-class PutRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
-):
-    pass
-
-
-RecommendationPreferencesDetailTypeDef = TypedDict(
-    "RecommendationPreferencesDetailTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "resourceType": ResourceTypeType,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-    },
-    total=False,
-)
-
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1070,14 +1052,39 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+    },
+    total=False,
+)
+
+
+class PutRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
+):
+    pass
+
+
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
@@ -1090,14 +1097,26 @@
         "name": FindingType,
         "value": float,
         "reasonCodeSummaries": List[ReasonCodeSummaryTypeDef],
     },
     total=False,
 )
 
+RecommendationPreferencesDetailTypeDef = TypedDict(
+    "RecommendationPreferencesDetailTypeDef",
+    {
+        "scope": ScopeOutputTypeDef,
+        "resourceType": ResourceTypeType,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 ServiceConfigurationTypeDef = TypedDict(
     "ServiceConfigurationTypeDef",
     {
         "memory": int,
         "cpu": int,
         "containerConfigurations": List[ContainerConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationType,
@@ -1112,23 +1131,14 @@
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRecommendationPreferencesResponseTypeDef = TypedDict(
-    "GetRecommendationPreferencesResponseTypeDef",
-    {
-        "nextToken": str,
-        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
         "projectedUtilizationMetrics": List[UtilizationMetricTypeDef],
         "performanceRisk": float,
         "rank": int,
@@ -1217,14 +1227,23 @@
         "savingsOpportunity": SavingsOpportunityTypeDef,
         "currentPerformanceRiskRatings": CurrentPerformanceRiskRatingsTypeDef,
         "inferredWorkloadSavings": List[InferredWorkloadSavingTypeDef],
     },
     total=False,
 )
 
+GetRecommendationPreferencesResponseTypeDef = TypedDict(
+    "GetRecommendationPreferencesResponseTypeDef",
+    {
+        "nextToken": str,
+        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AutoScalingGroupRecommendationTypeDef = TypedDict(
     "AutoScalingGroupRecommendationTypeDef",
     {
         "accountId": str,
         "autoScalingGroupArn": str,
         "autoScalingGroupName": str,
         "finding": FindingType,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer/type_defs.pyi` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,35 +82,37 @@
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
     "TagTypeDef",
-    "ExternalMetricsPreferenceTypeDef",
+    "ExternalMetricsPreferenceOutputTypeDef",
     "EnrollmentFilterTypeDef",
     "EstimatedMonthlySavingsTypeDef",
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
+    "ExternalMetricsPreferenceTypeDef",
     "GetRecommendationErrorTypeDef",
     "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     "GetEnrollmentStatusResponseTypeDef",
     "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
     "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
+    "ScopeOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
     "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
     "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
@@ -120,16 +122,14 @@
     "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     "DescribeRecommendationExportJobsRequestRequestTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
-    "PutRecommendationPreferencesRequestRequestTypeDef",
-    "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
     "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
@@ -142,27 +142,29 @@
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
+    "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
+    "RecommendationPreferencesDetailTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
-    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
     "InstanceRecommendationOptionTypeDef",
     "LambdaFunctionMemoryRecommendationOptionTypeDef",
     "VolumeRecommendationOptionTypeDef",
     "RecommendationExportJobTypeDef",
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     "RecommendationSummaryTypeDef",
+    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationTypeDef",
     "ECSServiceRecommendationTypeDef",
     "InstanceRecommendationTypeDef",
     "LambdaFunctionRecommendationTypeDef",
     "VolumeRecommendationTypeDef",
     "DescribeRecommendationExportJobsResponseTypeDef",
     "GetRecommendationSummariesResponseTypeDef",
@@ -308,16 +310,16 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-ExternalMetricsPreferenceTypeDef = TypedDict(
-    "ExternalMetricsPreferenceTypeDef",
+ExternalMetricsPreferenceOutputTypeDef = TypedDict(
+    "ExternalMetricsPreferenceOutputTypeDef",
     {
         "source": ExternalMetricsSourceType,
     },
     total=False,
 )
 
 EnrollmentFilterTypeDef = TypedDict(
@@ -388,14 +390,22 @@
     {
         "statusCode": ExternalMetricStatusCodeType,
         "statusReason": str,
     },
     total=False,
 )
 
+ExternalMetricsPreferenceTypeDef = TypedDict(
+    "ExternalMetricsPreferenceTypeDef",
+    {
+        "source": ExternalMetricsSourceType,
+    },
+    total=False,
+)
+
 GetRecommendationErrorTypeDef = TypedDict(
     "GetRecommendationErrorTypeDef",
     {
         "identifier": str,
         "code": str,
         "message": str,
     },
@@ -505,14 +515,23 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
     },
     total=False,
 )
 
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "name": ScopeNameType,
+        "value": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -713,63 +732,28 @@
 
 EffectiveRecommendationPreferencesTypeDef = TypedDict(
     "EffectiveRecommendationPreferencesTypeDef",
     {
         "cpuVendorArchitectures": List[CpuVendorArchitectureType],
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
     },
     total=False,
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-    },
-    total=False,
-)
-
-class PutRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
-):
-    pass
-
-RecommendationPreferencesDetailTypeDef = TypedDict(
-    "RecommendationPreferencesDetailTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "resourceType": ResourceTypeType,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-    },
-    total=False,
-)
-
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1047,14 +1031,37 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+    },
+    total=False,
+)
+
+class PutRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
+):
+    pass
+
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
@@ -1067,14 +1074,26 @@
         "name": FindingType,
         "value": float,
         "reasonCodeSummaries": List[ReasonCodeSummaryTypeDef],
     },
     total=False,
 )
 
+RecommendationPreferencesDetailTypeDef = TypedDict(
+    "RecommendationPreferencesDetailTypeDef",
+    {
+        "scope": ScopeOutputTypeDef,
+        "resourceType": ResourceTypeType,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 ServiceConfigurationTypeDef = TypedDict(
     "ServiceConfigurationTypeDef",
     {
         "memory": int,
         "cpu": int,
         "containerConfigurations": List[ContainerConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationType,
@@ -1089,23 +1108,14 @@
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRecommendationPreferencesResponseTypeDef = TypedDict(
-    "GetRecommendationPreferencesResponseTypeDef",
-    {
-        "nextToken": str,
-        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
         "projectedUtilizationMetrics": List[UtilizationMetricTypeDef],
         "performanceRisk": float,
         "rank": int,
@@ -1194,14 +1204,23 @@
         "savingsOpportunity": SavingsOpportunityTypeDef,
         "currentPerformanceRiskRatings": CurrentPerformanceRiskRatingsTypeDef,
         "inferredWorkloadSavings": List[InferredWorkloadSavingTypeDef],
     },
     total=False,
 )
 
+GetRecommendationPreferencesResponseTypeDef = TypedDict(
+    "GetRecommendationPreferencesResponseTypeDef",
+    {
+        "nextToken": str,
+        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AutoScalingGroupRecommendationTypeDef = TypedDict(
     "AutoScalingGroupRecommendationTypeDef",
     {
         "accountId": str,
         "autoScalingGroupArn": str,
         "autoScalingGroupName": str,
         "finding": FindingType,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/PKG-INFO` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.28.0
-Summary: Type annotations for boto3.ComputeOptimizer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ComputeOptimizer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-compute-optimizer"></a>
 
 # mypy-boto3-compute-optimizer
 
 [![PyPI - mypy-boto3-compute-optimizer](https://img.shields.io/pypi/v/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,35 +406,37 @@
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
-    ExternalMetricsPreferenceTypeDef,
+    ExternalMetricsPreferenceOutputTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
+    ExternalMetricsPreferenceTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
     GetEnrollmentStatusResponseTypeDef,
     GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
     PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
+    ScopeOutputTypeDef,
     ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
     UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
     GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
@@ -444,16 +446,14 @@
     DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
-    PutRecommendationPreferencesRequestRequestTypeDef,
-    RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
@@ -466,27 +466,29 @@
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
+    RecommendationPreferencesDetailTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
-    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
     InstanceRecommendationOptionTypeDef,
     LambdaFunctionMemoryRecommendationOptionTypeDef,
     VolumeRecommendationOptionTypeDef,
     RecommendationExportJobTypeDef,
     GetEC2RecommendationProjectedMetricsResponseTypeDef,
     RecommendationSummaryTypeDef,
+    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationTypeDef,
     ECSServiceRecommendationTypeDef,
     InstanceRecommendationTypeDef,
     LambdaFunctionRecommendationTypeDef,
     VolumeRecommendationTypeDef,
     DescribeRecommendationExportJobsResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.0/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt` & `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.0/setup.py` & `mypy-boto3-compute-optimizer-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-compute-optimizer",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComputeOptimizer 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ComputeOptimizer 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

