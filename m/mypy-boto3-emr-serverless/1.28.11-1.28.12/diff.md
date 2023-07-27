# Comparing `tmp/mypy-boto3-emr-serverless-1.28.11.tar.gz` & `tmp/mypy-boto3-emr-serverless-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-serverless-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.28.11.tar` & `mypy-boto3-emr-serverless-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-25 19:47:56.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-07-25 19:47:56.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23114 2023-07-25 19:47:56.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-07-27 05:22:04.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-07-27 05:22:03.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:40.000000 mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.304515 mypy-boto3-emr-serverless-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:22:02.000000 mypy-boto3-emr-serverless-1.28.12/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/LICENSE` & `mypy-boto3-emr-serverless-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.11/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.11
-Summary: Type annotations for boto3.EMRServerless 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.EMRServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,62 +334,62 @@
     AutoStopConfigOutputTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesOutputTypeDef,
     NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     CloudWatchLoggingConfigurationOutputTypeDef,
     CloudWatchLoggingConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveOutputTypeDef,
     HiveTypeDef,
     WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationTypeDef,
     WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/README.md` & `mypy-boto3-emr-serverless-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,62 +302,62 @@
     AutoStopConfigOutputTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesOutputTypeDef,
     NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     CloudWatchLoggingConfigurationOutputTypeDef,
     CloudWatchLoggingConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveOutputTypeDef,
     HiveTypeDef,
     WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationTypeDef,
     WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.py` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.pyi` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__main__.py` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.28.11\nVersion:         1.28.11\nBuilder"
-        " version: 7.15.1\nDocs:           "
+        "Type annotations for boto3.EMRServerless 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.11")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.py` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.pyi` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.py` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationStateType",
     "ArchitectureType",
     "JobRunStateType",
     "ListApplicationsPaginatorName",
     "ListJobRunsPaginatorName",
     "EMRServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStateType = Literal[
     "CREATED", "CREATING", "STARTED", "STARTING", "STOPPED", "STOPPING", "TERMINATED"
 ]
 ArchitectureType = Literal["ARM64", "X86_64"]
 JobRunStateType = Literal[
     "CANCELLED", "CANCELLING", "FAILED", "PENDING", "RUNNING", "SCHEDULED", "SUBMITTED", "SUCCESS"
 ]
@@ -158,14 +156,15 @@
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
@@ -244,14 +243,15 @@
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
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.pyi` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApplicationStateType",
     "ArchitectureType",
     "JobRunStateType",
     "ListApplicationsPaginatorName",
     "ListJobRunsPaginatorName",
     "EMRServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApplicationStateType = Literal[
     "CREATED", "CREATING", "STARTED", "STARTING", "STOPPED", "STOPPING", "TERMINATED"
 ]
 ArchitectureType = Literal["ARM64", "X86_64"]
 JobRunStateType = Literal[
     "CANCELLED", "CANCELLING", "FAILED", "PENDING", "RUNNING", "SCHEDULED", "SUBMITTED", "SUCCESS"
 ]
@@ -156,14 +158,15 @@
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
@@ -242,14 +245,15 @@
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
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.py` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 
@@ -73,13 +73,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.pyi` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 class ListJobRunsPaginator(Paginator):
@@ -69,13 +69,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.py` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -18,141 +18,176 @@
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigOutputTypeDef",
     "AutoStopConfigOutputTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesOutputTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobRunResponseTypeDef",
     "CloudWatchLoggingConfigurationOutputTypeDef",
     "CloudWatchLoggingConfigurationTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveOutputTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigOutputTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "WorkerTypeSpecificationTypeDef",
-    "CancelJobRunResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartJobRunResponseTypeDef",
+    "WorkerTypeSpecificationTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
     "InitialCapacityConfigOutputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
-ApplicationSummaryTypeDef = TypedDict(
-    "ApplicationSummaryTypeDef",
+_RequiredApplicationSummaryTypeDef = TypedDict(
+    "_RequiredApplicationSummaryTypeDef",
     {
         "id": str,
-        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
-        "stateDetails": str,
         "createdAt": datetime,
         "updatedAt": datetime,
+    },
+)
+_OptionalApplicationSummaryTypeDef = TypedDict(
+    "_OptionalApplicationSummaryTypeDef",
+    {
+        "name": str,
+        "stateDetails": str,
         "architecture": ArchitectureType,
     },
+    total=False,
 )
 
+class ApplicationSummaryTypeDef(
+    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
+):
+    pass
+
 AutoStartConfigOutputTypeDef = TypedDict(
     "AutoStartConfigOutputTypeDef",
     {
         "enabled": bool,
     },
+    total=False,
 )
 
 AutoStopConfigOutputTypeDef = TypedDict(
     "AutoStopConfigOutputTypeDef",
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
+    total=False,
 )
 
-ImageConfigurationTypeDef = TypedDict(
-    "ImageConfigurationTypeDef",
+_RequiredImageConfigurationTypeDef = TypedDict(
+    "_RequiredImageConfigurationTypeDef",
     {
         "imageUri": str,
+    },
+)
+_OptionalImageConfigurationTypeDef = TypedDict(
+    "_OptionalImageConfigurationTypeDef",
+    {
         "resolvedImageDigest": str,
     },
+    total=False,
 )
 
-MaximumAllowedResourcesOutputTypeDef = TypedDict(
-    "MaximumAllowedResourcesOutputTypeDef",
+class ImageConfigurationTypeDef(
+    _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
+):
+    pass
+
+_RequiredMaximumAllowedResourcesOutputTypeDef = TypedDict(
+    "_RequiredMaximumAllowedResourcesOutputTypeDef",
     {
         "cpu": str,
         "memory": str,
+    },
+)
+_OptionalMaximumAllowedResourcesOutputTypeDef = TypedDict(
+    "_OptionalMaximumAllowedResourcesOutputTypeDef",
+    {
         "disk": str,
     },
+    total=False,
 )
 
+class MaximumAllowedResourcesOutputTypeDef(
+    _RequiredMaximumAllowedResourcesOutputTypeDef, _OptionalMaximumAllowedResourcesOutputTypeDef
+):
+    pass
+
 NetworkConfigurationOutputTypeDef = TypedDict(
     "NetworkConfigurationOutputTypeDef",
     {
         "subnetIds": List[str],
         "securityGroupIds": List[str],
     },
+    total=False,
 )
 
 AutoStartConfigTypeDef = TypedDict(
     "AutoStartConfigTypeDef",
     {
         "enabled": bool,
     },
@@ -172,36 +207,46 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchLoggingConfigurationOutputTypeDef",
+_RequiredCloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLoggingConfigurationOutputTypeDef",
     {
         "enabled": bool,
+    },
+)
+_OptionalCloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLoggingConfigurationOutputTypeDef",
+    {
         "logGroupName": str,
         "logStreamNamePrefix": str,
         "encryptionKeyArn": str,
         "logTypes": Dict[str, List[str]],
     },
+    total=False,
 )
 
+class CloudWatchLoggingConfigurationOutputTypeDef(
+    _RequiredCloudWatchLoggingConfigurationOutputTypeDef,
+    _OptionalCloudWatchLoggingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredCloudWatchLoggingConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchLoggingConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalCloudWatchLoggingConfigurationTypeDef = TypedDict(
@@ -211,30 +256,39 @@
         "logStreamNamePrefix": str,
         "encryptionKeyArn": str,
         "logTypes": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class CloudWatchLoggingConfigurationTypeDef(
     _RequiredCloudWatchLoggingConfigurationTypeDef, _OptionalCloudWatchLoggingConfigurationTypeDef
 ):
     pass
 
-
-ConfigurationOutputTypeDef = TypedDict(
-    "ConfigurationOutputTypeDef",
+_RequiredConfigurationOutputTypeDef = TypedDict(
+    "_RequiredConfigurationOutputTypeDef",
     {
         "classification": str,
+    },
+)
+_OptionalConfigurationOutputTypeDef = TypedDict(
+    "_OptionalConfigurationOutputTypeDef",
+    {
         "properties": Dict[str, str],
         "configurations": List[Dict[str, Any]],
     },
+    total=False,
 )
 
+class ConfigurationOutputTypeDef(
+    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -242,19 +296,17 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
-
 ImageConfigurationInputTypeDef = TypedDict(
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
@@ -270,30 +322,38 @@
     "_OptionalMaximumAllowedResourcesTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
-
 class MaximumAllowedResourcesTypeDef(
     _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "subnetIds": Sequence[str],
         "securityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -308,31 +368,48 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-HiveOutputTypeDef = TypedDict(
-    "HiveOutputTypeDef",
+_RequiredHiveOutputTypeDef = TypedDict(
+    "_RequiredHiveOutputTypeDef",
     {
         "query": str,
+    },
+)
+_OptionalHiveOutputTypeDef = TypedDict(
+    "_OptionalHiveOutputTypeDef",
+    {
         "initQueryFile": str,
         "parameters": str,
     },
+    total=False,
 )
 
+class HiveOutputTypeDef(_RequiredHiveOutputTypeDef, _OptionalHiveOutputTypeDef):
+    pass
+
 _RequiredHiveTypeDef = TypedDict(
     "_RequiredHiveTypeDef",
     {
         "query": str,
     },
 )
 _OptionalHiveTypeDef = TypedDict(
@@ -340,28 +417,37 @@
     {
         "initQueryFile": str,
         "parameters": str,
     },
     total=False,
 )
 
-
 class HiveTypeDef(_RequiredHiveTypeDef, _OptionalHiveTypeDef):
     pass
 
-
-WorkerResourceConfigOutputTypeDef = TypedDict(
-    "WorkerResourceConfigOutputTypeDef",
+_RequiredWorkerResourceConfigOutputTypeDef = TypedDict(
+    "_RequiredWorkerResourceConfigOutputTypeDef",
     {
         "cpu": str,
         "memory": str,
+    },
+)
+_OptionalWorkerResourceConfigOutputTypeDef = TypedDict(
+    "_OptionalWorkerResourceConfigOutputTypeDef",
+    {
         "disk": str,
     },
+    total=False,
 )
 
+class WorkerResourceConfigOutputTypeDef(
+    _RequiredWorkerResourceConfigOutputTypeDef, _OptionalWorkerResourceConfigOutputTypeDef
+):
+    pass
+
 _RequiredWorkerResourceConfigTypeDef = TypedDict(
     "_RequiredWorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
@@ -369,30 +455,39 @@
     "_OptionalWorkerResourceConfigTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
-
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
-
-SparkSubmitOutputTypeDef = TypedDict(
-    "SparkSubmitOutputTypeDef",
+_RequiredSparkSubmitOutputTypeDef = TypedDict(
+    "_RequiredSparkSubmitOutputTypeDef",
     {
         "entryPoint": str,
+    },
+)
+_OptionalSparkSubmitOutputTypeDef = TypedDict(
+    "_OptionalSparkSubmitOutputTypeDef",
+    {
         "entryPointArguments": List[str],
         "sparkSubmitParameters": str,
     },
+    total=False,
 )
 
+class SparkSubmitOutputTypeDef(
+    _RequiredSparkSubmitOutputTypeDef, _OptionalSparkSubmitOutputTypeDef
+):
+    pass
+
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
@@ -400,75 +495,106 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
-
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
     pass
 
-
-JobRunSummaryTypeDef = TypedDict(
-    "JobRunSummaryTypeDef",
+_RequiredJobRunSummaryTypeDef = TypedDict(
+    "_RequiredJobRunSummaryTypeDef",
     {
         "applicationId": str,
         "id": str,
-        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
+    },
+)
+_OptionalJobRunSummaryTypeDef = TypedDict(
+    "_OptionalJobRunSummaryTypeDef",
+    {
+        "name": str,
         "type": str,
     },
+    total=False,
 )
 
+class JobRunSummaryTypeDef(_RequiredJobRunSummaryTypeDef, _OptionalJobRunSummaryTypeDef):
+    pass
+
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
+    total=False,
 )
 
 TotalResourceUtilizationTypeDef = TypedDict(
     "TotalResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -479,34 +605,41 @@
         "createdAtAfter": Union[datetime, str],
         "createdAtBefore": Union[datetime, str],
         "states": Sequence[JobRunStateType],
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ManagedPersistenceMonitoringConfigurationOutputTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
+    total=False,
 )
 
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
@@ -516,32 +649,64 @@
 
 S3MonitoringConfigurationOutputTypeDef = TypedDict(
     "S3MonitoringConfigurationOutputTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
+    total=False,
 )
 
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -557,118 +722,84 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
-    {
-        "imageConfiguration": ImageConfigurationTypeDef,
-    },
-)
-
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "imageConfiguration": ImageConfigurationTypeDef,
     },
+    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
-InitialCapacityConfigOutputTypeDef = TypedDict(
-    "InitialCapacityConfigOutputTypeDef",
+_RequiredInitialCapacityConfigOutputTypeDef = TypedDict(
+    "_RequiredInitialCapacityConfigOutputTypeDef",
     {
         "workerCount": int,
+    },
+)
+_OptionalInitialCapacityConfigOutputTypeDef = TypedDict(
+    "_OptionalInitialCapacityConfigOutputTypeDef",
+    {
         "workerConfiguration": WorkerResourceConfigOutputTypeDef,
     },
+    total=False,
 )
 
+class InitialCapacityConfigOutputTypeDef(
+    _RequiredInitialCapacityConfigOutputTypeDef, _OptionalInitialCapacityConfigOutputTypeDef
+):
+    pass
+
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
     "_OptionalInitialCapacityConfigTypeDef",
     {
         "workerConfiguration": WorkerResourceConfigTypeDef,
     },
     total=False,
 )
 
-
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
-
 JobDriverOutputTypeDef = TypedDict(
     "JobDriverOutputTypeDef",
     {
         "sparkSubmit": SparkSubmitOutputTypeDef,
         "hive": HiveOutputTypeDef,
     },
+    total=False,
 )
 
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
@@ -677,99 +808,75 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-
 MonitoringConfigurationOutputTypeDef = TypedDict(
     "MonitoringConfigurationOutputTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationOutputTypeDef
         ),
         "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
         "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+_RequiredApplicationTypeDef = TypedDict(
+    "_RequiredApplicationTypeDef",
     {
         "applicationId": str,
-        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+    },
+)
+_OptionalApplicationTypeDef = TypedDict(
+    "_OptionalApplicationTypeDef",
+    {
+        "name": str,
         "stateDetails": str,
         "initialCapacity": Dict[str, InitialCapacityConfigOutputTypeDef],
         "maximumCapacity": MaximumAllowedResourcesOutputTypeDef,
-        "createdAt": datetime,
-        "updatedAt": datetime,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigOutputTypeDef,
         "autoStopConfiguration": AutoStopConfigOutputTypeDef,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
+    total=False,
 )
 
+class ApplicationTypeDef(_RequiredApplicationTypeDef, _OptionalApplicationTypeDef):
+    pass
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "releaseLabel": str,
         "type": str,
         "clientToken": str,
     },
@@ -787,21 +894,19 @@
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
     },
 )
@@ -817,27 +922,26 @@
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
         "releaseLabel": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
@@ -845,51 +949,60 @@
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-JobRunTypeDef = TypedDict(
-    "JobRunTypeDef",
+_RequiredJobRunTypeDef = TypedDict(
+    "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
-        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "jobDriver": JobDriverOutputTypeDef,
+    },
+)
+_OptionalJobRunTypeDef = TypedDict(
+    "_OptionalJobRunTypeDef",
+    {
+        "name": str,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
+    total=False,
 )
 
+class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
+    pass
+
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
@@ -902,21 +1015,19 @@
         "tags": Mapping[str, str],
         "executionTimeoutMinutes": int,
         "name": str,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,140 +18,183 @@
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigOutputTypeDef",
     "AutoStopConfigOutputTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesOutputTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobRunResponseTypeDef",
     "CloudWatchLoggingConfigurationOutputTypeDef",
     "CloudWatchLoggingConfigurationTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveOutputTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigOutputTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "WorkerTypeSpecificationTypeDef",
-    "CancelJobRunResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartJobRunResponseTypeDef",
+    "WorkerTypeSpecificationTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
     "InitialCapacityConfigOutputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
-ApplicationSummaryTypeDef = TypedDict(
-    "ApplicationSummaryTypeDef",
+_RequiredApplicationSummaryTypeDef = TypedDict(
+    "_RequiredApplicationSummaryTypeDef",
     {
         "id": str,
-        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
-        "stateDetails": str,
         "createdAt": datetime,
         "updatedAt": datetime,
+    },
+)
+_OptionalApplicationSummaryTypeDef = TypedDict(
+    "_OptionalApplicationSummaryTypeDef",
+    {
+        "name": str,
+        "stateDetails": str,
         "architecture": ArchitectureType,
     },
+    total=False,
 )
 
+
+class ApplicationSummaryTypeDef(
+    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
+):
+    pass
+
+
 AutoStartConfigOutputTypeDef = TypedDict(
     "AutoStartConfigOutputTypeDef",
     {
         "enabled": bool,
     },
+    total=False,
 )
 
 AutoStopConfigOutputTypeDef = TypedDict(
     "AutoStopConfigOutputTypeDef",
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
+    total=False,
 )
 
-ImageConfigurationTypeDef = TypedDict(
-    "ImageConfigurationTypeDef",
+_RequiredImageConfigurationTypeDef = TypedDict(
+    "_RequiredImageConfigurationTypeDef",
     {
         "imageUri": str,
+    },
+)
+_OptionalImageConfigurationTypeDef = TypedDict(
+    "_OptionalImageConfigurationTypeDef",
+    {
         "resolvedImageDigest": str,
     },
+    total=False,
 )
 
-MaximumAllowedResourcesOutputTypeDef = TypedDict(
-    "MaximumAllowedResourcesOutputTypeDef",
+
+class ImageConfigurationTypeDef(
+    _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
+):
+    pass
+
+
+_RequiredMaximumAllowedResourcesOutputTypeDef = TypedDict(
+    "_RequiredMaximumAllowedResourcesOutputTypeDef",
     {
         "cpu": str,
         "memory": str,
+    },
+)
+_OptionalMaximumAllowedResourcesOutputTypeDef = TypedDict(
+    "_OptionalMaximumAllowedResourcesOutputTypeDef",
+    {
         "disk": str,
     },
+    total=False,
 )
 
+
+class MaximumAllowedResourcesOutputTypeDef(
+    _RequiredMaximumAllowedResourcesOutputTypeDef, _OptionalMaximumAllowedResourcesOutputTypeDef
+):
+    pass
+
+
 NetworkConfigurationOutputTypeDef = TypedDict(
     "NetworkConfigurationOutputTypeDef",
     {
         "subnetIds": List[str],
         "securityGroupIds": List[str],
     },
+    total=False,
 )
 
 AutoStartConfigTypeDef = TypedDict(
     "AutoStartConfigTypeDef",
     {
         "enabled": bool,
     },
@@ -171,36 +214,48 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchLoggingConfigurationOutputTypeDef",
+_RequiredCloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLoggingConfigurationOutputTypeDef",
     {
         "enabled": bool,
+    },
+)
+_OptionalCloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLoggingConfigurationOutputTypeDef",
+    {
         "logGroupName": str,
         "logStreamNamePrefix": str,
         "encryptionKeyArn": str,
         "logTypes": Dict[str, List[str]],
     },
+    total=False,
 )
 
+
+class CloudWatchLoggingConfigurationOutputTypeDef(
+    _RequiredCloudWatchLoggingConfigurationOutputTypeDef,
+    _OptionalCloudWatchLoggingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCloudWatchLoggingConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchLoggingConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalCloudWatchLoggingConfigurationTypeDef = TypedDict(
@@ -210,28 +265,43 @@
         "logStreamNamePrefix": str,
         "encryptionKeyArn": str,
         "logTypes": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class CloudWatchLoggingConfigurationTypeDef(
     _RequiredCloudWatchLoggingConfigurationTypeDef, _OptionalCloudWatchLoggingConfigurationTypeDef
 ):
     pass
 
-ConfigurationOutputTypeDef = TypedDict(
-    "ConfigurationOutputTypeDef",
+
+_RequiredConfigurationOutputTypeDef = TypedDict(
+    "_RequiredConfigurationOutputTypeDef",
     {
         "classification": str,
+    },
+)
+_OptionalConfigurationOutputTypeDef = TypedDict(
+    "_OptionalConfigurationOutputTypeDef",
+    {
         "properties": Dict[str, str],
         "configurations": List[Dict[str, Any]],
     },
+    total=False,
 )
 
+
+class ConfigurationOutputTypeDef(
+    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -239,17 +309,19 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+
 ImageConfigurationInputTypeDef = TypedDict(
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
@@ -265,28 +337,40 @@
     "_OptionalMaximumAllowedResourcesTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
+
 class MaximumAllowedResourcesTypeDef(
     _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "subnetIds": Sequence[str],
         "securityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -301,31 +385,50 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-HiveOutputTypeDef = TypedDict(
-    "HiveOutputTypeDef",
+_RequiredHiveOutputTypeDef = TypedDict(
+    "_RequiredHiveOutputTypeDef",
     {
         "query": str,
+    },
+)
+_OptionalHiveOutputTypeDef = TypedDict(
+    "_OptionalHiveOutputTypeDef",
+    {
         "initQueryFile": str,
         "parameters": str,
     },
+    total=False,
 )
 
+
+class HiveOutputTypeDef(_RequiredHiveOutputTypeDef, _OptionalHiveOutputTypeDef):
+    pass
+
+
 _RequiredHiveTypeDef = TypedDict(
     "_RequiredHiveTypeDef",
     {
         "query": str,
     },
 )
 _OptionalHiveTypeDef = TypedDict(
@@ -333,26 +436,41 @@
     {
         "initQueryFile": str,
         "parameters": str,
     },
     total=False,
 )
 
+
 class HiveTypeDef(_RequiredHiveTypeDef, _OptionalHiveTypeDef):
     pass
 
-WorkerResourceConfigOutputTypeDef = TypedDict(
-    "WorkerResourceConfigOutputTypeDef",
+
+_RequiredWorkerResourceConfigOutputTypeDef = TypedDict(
+    "_RequiredWorkerResourceConfigOutputTypeDef",
     {
         "cpu": str,
         "memory": str,
+    },
+)
+_OptionalWorkerResourceConfigOutputTypeDef = TypedDict(
+    "_OptionalWorkerResourceConfigOutputTypeDef",
+    {
         "disk": str,
     },
+    total=False,
 )
 
+
+class WorkerResourceConfigOutputTypeDef(
+    _RequiredWorkerResourceConfigOutputTypeDef, _OptionalWorkerResourceConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredWorkerResourceConfigTypeDef = TypedDict(
     "_RequiredWorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
@@ -360,28 +478,43 @@
     "_OptionalWorkerResourceConfigTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
+
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
-SparkSubmitOutputTypeDef = TypedDict(
-    "SparkSubmitOutputTypeDef",
+
+_RequiredSparkSubmitOutputTypeDef = TypedDict(
+    "_RequiredSparkSubmitOutputTypeDef",
     {
         "entryPoint": str,
+    },
+)
+_OptionalSparkSubmitOutputTypeDef = TypedDict(
+    "_OptionalSparkSubmitOutputTypeDef",
+    {
         "entryPointArguments": List[str],
         "sparkSubmitParameters": str,
     },
+    total=False,
 )
 
+
+class SparkSubmitOutputTypeDef(
+    _RequiredSparkSubmitOutputTypeDef, _OptionalSparkSubmitOutputTypeDef
+):
+    pass
+
+
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
@@ -389,73 +522,112 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
+
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
     pass
 
-JobRunSummaryTypeDef = TypedDict(
-    "JobRunSummaryTypeDef",
+
+_RequiredJobRunSummaryTypeDef = TypedDict(
+    "_RequiredJobRunSummaryTypeDef",
     {
         "applicationId": str,
         "id": str,
-        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
+    },
+)
+_OptionalJobRunSummaryTypeDef = TypedDict(
+    "_OptionalJobRunSummaryTypeDef",
+    {
+        "name": str,
         "type": str,
     },
+    total=False,
 )
 
+
+class JobRunSummaryTypeDef(_RequiredJobRunSummaryTypeDef, _OptionalJobRunSummaryTypeDef):
+    pass
+
+
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
+    total=False,
 )
 
 TotalResourceUtilizationTypeDef = TypedDict(
     "TotalResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -466,32 +638,43 @@
         "createdAtAfter": Union[datetime, str],
         "createdAtBefore": Union[datetime, str],
         "states": Sequence[JobRunStateType],
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ManagedPersistenceMonitoringConfigurationOutputTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
+    total=False,
 )
 
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
@@ -501,32 +684,64 @@
 
 S3MonitoringConfigurationOutputTypeDef = TypedDict(
     "S3MonitoringConfigurationOutputTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
+    total=False,
 )
 
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -542,116 +757,88 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
-    {
-        "imageConfiguration": ImageConfigurationTypeDef,
-    },
-)
-
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "imageConfiguration": ImageConfigurationTypeDef,
     },
+    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
-InitialCapacityConfigOutputTypeDef = TypedDict(
-    "InitialCapacityConfigOutputTypeDef",
+_RequiredInitialCapacityConfigOutputTypeDef = TypedDict(
+    "_RequiredInitialCapacityConfigOutputTypeDef",
     {
         "workerCount": int,
+    },
+)
+_OptionalInitialCapacityConfigOutputTypeDef = TypedDict(
+    "_OptionalInitialCapacityConfigOutputTypeDef",
+    {
         "workerConfiguration": WorkerResourceConfigOutputTypeDef,
     },
+    total=False,
 )
 
+
+class InitialCapacityConfigOutputTypeDef(
+    _RequiredInitialCapacityConfigOutputTypeDef, _OptionalInitialCapacityConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
     "_OptionalInitialCapacityConfigTypeDef",
     {
         "workerConfiguration": WorkerResourceConfigTypeDef,
     },
     total=False,
 )
 
+
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
+
 JobDriverOutputTypeDef = TypedDict(
     "JobDriverOutputTypeDef",
     {
         "sparkSubmit": SparkSubmitOutputTypeDef,
         "hive": HiveOutputTypeDef,
     },
+    total=False,
 )
 
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
@@ -660,97 +847,77 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
 MonitoringConfigurationOutputTypeDef = TypedDict(
     "MonitoringConfigurationOutputTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationOutputTypeDef
         ),
         "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
         "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+_RequiredApplicationTypeDef = TypedDict(
+    "_RequiredApplicationTypeDef",
     {
         "applicationId": str,
-        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+    },
+)
+_OptionalApplicationTypeDef = TypedDict(
+    "_OptionalApplicationTypeDef",
+    {
+        "name": str,
         "stateDetails": str,
         "initialCapacity": Dict[str, InitialCapacityConfigOutputTypeDef],
         "maximumCapacity": MaximumAllowedResourcesOutputTypeDef,
-        "createdAt": datetime,
-        "updatedAt": datetime,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigOutputTypeDef,
         "autoStopConfiguration": AutoStopConfigOutputTypeDef,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
+    total=False,
 )
 
+
+class ApplicationTypeDef(_RequiredApplicationTypeDef, _OptionalApplicationTypeDef):
+    pass
+
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "releaseLabel": str,
         "type": str,
         "clientToken": str,
     },
@@ -768,19 +935,21 @@
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
     },
 )
@@ -796,25 +965,28 @@
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
         "releaseLabel": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
@@ -822,51 +994,62 @@
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-JobRunTypeDef = TypedDict(
-    "JobRunTypeDef",
+_RequiredJobRunTypeDef = TypedDict(
+    "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
-        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "jobDriver": JobDriverOutputTypeDef,
+    },
+)
+_OptionalJobRunTypeDef = TypedDict(
+    "_OptionalJobRunTypeDef",
+    {
+        "name": str,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
+    total=False,
 )
 
+
+class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
+    pass
+
+
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
@@ -879,19 +1062,21 @@
         "tags": Mapping[str, str],
         "executionTimeoutMinutes": int,
         "name": str,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.11
-Summary: Type annotations for boto3.EMRServerless 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.EMRServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,62 +334,62 @@
     AutoStopConfigOutputTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesOutputTypeDef,
     NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     CloudWatchLoggingConfigurationOutputTypeDef,
     CloudWatchLoggingConfigurationTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveOutputTypeDef,
     HiveTypeDef,
     WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationTypeDef,
     WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy-boto3-emr-serverless-1.28.12/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.11/setup.py` & `mypy-boto3-emr-serverless-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRServerless 1.28.11 service generated with mypy-boto3-builder"
-        " 7.15.1"
+        "Type annotations for boto3.EMRServerless 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

