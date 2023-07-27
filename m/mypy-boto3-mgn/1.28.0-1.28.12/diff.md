# Comparing `tmp/mypy-boto3-mgn-1.28.0.tar.gz` & `tmp/mypy-boto3-mgn-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgn-1.28.0.tar", last modified: Thu Jul  6 21:00:08 2023, max compression
+gzip compressed data, was "mypy-boto3-mgn-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
```

## Comparing `mypy-boto3-mgn-1.28.0.tar` & `mypy-boto3-mgn-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.914373 mypy-boto3-mgn-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-07-06 21:00:08.914373 mypy-boto3-mgn-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.898373 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51946 2023-07-06 20:47:39.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51859 2023-07-06 20:47:39.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-06 20:47:40.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-07-06 20:47:39.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-06 20:47:39.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-06 20:47:39.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80103 2023-07-06 20:47:44.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79988 2023-07-06 20:47:41.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.914373 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-07-06 21:00:08.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:08.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:08.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:08.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:08.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:08.000000 mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:08.914373 mypy-boto3-mgn-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:47:38.000000 mypy-boto3-mgn-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.928434 mypy-boto3-mgn-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23791 2023-07-27 05:35:02.924434 mypy-boto3-mgn-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22320 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.920434 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51946 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51859 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-27 05:26:37.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    82975 2023-07-27 05:26:39.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82856 2023-07-27 05:26:38.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.924434 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23791 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.928434 mypy-boto3-mgn-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/setup.py
```

### Comparing `mypy-boto3-mgn-1.28.0/LICENSE` & `mypy-boto3-mgn-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/PKG-INFO` & `mypy-boto3-mgn-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.28.0
-Summary: Type annotations for boto3.mgn 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.mgn 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -459,16 +459,18 @@
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
     ImportTaskSummaryApplicationsTypeDef,
     ImportTaskSummaryServersTypeDef,
     ImportTaskSummaryWavesTypeDef,
-    S3BucketSourceTypeDef,
+    S3BucketSourceOutputTypeDef,
     JobLogEventDataTypeDef,
+    LaunchTemplateDiskConfOutputTypeDef,
+    LicensingOutputTypeDef,
     LaunchedInstanceTypeDef,
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
@@ -492,19 +494,23 @@
     OSTypeDef,
     PaginatorConfigTypeDef,
     PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
+    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ResponseMetadataTypeDef,
     ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
+    S3BucketSourceTypeDef,
+    SsmExternalParameterOutputTypeDef,
+    SsmParameterStoreParameterOutputTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -526,15 +532,14 @@
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
     ExportTaskTypeDef,
     ImportTaskErrorTypeDef,
     ImportTaskSummaryTypeDef,
-    StartImportRequestRequestTypeDef,
     JobLogTypeDef,
     LifeCycleLastCutoverTypeDef,
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
@@ -546,48 +551,51 @@
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
     PutSourceServerActionRequestRequestTypeDef,
     PutTemplateActionRequestRequestTypeDef,
+    SsmDocumentTypeDef,
+    ReplicationConfigurationTypeDef,
+    UpdateReplicationConfigurationRequestRequestTypeDef,
+    StartImportRequestRequestTypeDef,
     SourceServerActionDocumentResponseMetadataTypeDef,
     SourceServerActionDocumentTypeDef,
-    SsmDocumentTypeDef,
+    SsmDocumentOutputTypeDef,
     TemplateActionDocumentResponseMetadataTypeDef,
     TemplateActionDocumentTypeDef,
-    ReplicationConfigurationTypeDef,
-    UpdateReplicationConfigurationRequestRequestTypeDef,
     WaveResponseMetadataTypeDef,
     WaveTypeDef,
     ListApplicationsResponseTypeDef,
     DataReplicationInfoTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsResponseTypeDef,
     StartExportResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ImportTaskTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     LifeCycleTypeDef,
+    PostLaunchActionsTypeDef,
     ListSourceServerActionsResponseTypeDef,
     JobPostLaunchActionsLaunchStatusTypeDef,
-    PostLaunchActionsTypeDef,
+    PostLaunchActionsOutputTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesResponseTypeDef,
     ListImportsResponseTypeDef,
     StartImportResponseTypeDef,
     SourceServerResponseMetadataTypeDef,
     SourceServerTypeDef,
-    PostLaunchActionsStatusTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    PostLaunchActionsStatusTypeDef,
     LaunchConfigurationTemplateResponseMetadataTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
-    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     DescribeSourceServersResponseTypeDef,
     ParticipatingServerTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     DescribeJobsResponseTypeDef,
     StartCutoverResponseTypeDef,
     StartTestResponseTypeDef,
```

### Comparing `mypy-boto3-mgn-1.28.0/README.md` & `mypy-boto3-mgn-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -427,16 +427,18 @@
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
     ImportTaskSummaryApplicationsTypeDef,
     ImportTaskSummaryServersTypeDef,
     ImportTaskSummaryWavesTypeDef,
-    S3BucketSourceTypeDef,
+    S3BucketSourceOutputTypeDef,
     JobLogEventDataTypeDef,
+    LaunchTemplateDiskConfOutputTypeDef,
+    LicensingOutputTypeDef,
     LaunchedInstanceTypeDef,
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
@@ -460,19 +462,23 @@
     OSTypeDef,
     PaginatorConfigTypeDef,
     PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
+    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ResponseMetadataTypeDef,
     ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
+    S3BucketSourceTypeDef,
+    SsmExternalParameterOutputTypeDef,
+    SsmParameterStoreParameterOutputTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -494,15 +500,14 @@
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
     ExportTaskTypeDef,
     ImportTaskErrorTypeDef,
     ImportTaskSummaryTypeDef,
-    StartImportRequestRequestTypeDef,
     JobLogTypeDef,
     LifeCycleLastCutoverTypeDef,
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
@@ -514,48 +519,51 @@
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
     PutSourceServerActionRequestRequestTypeDef,
     PutTemplateActionRequestRequestTypeDef,
+    SsmDocumentTypeDef,
+    ReplicationConfigurationTypeDef,
+    UpdateReplicationConfigurationRequestRequestTypeDef,
+    StartImportRequestRequestTypeDef,
     SourceServerActionDocumentResponseMetadataTypeDef,
     SourceServerActionDocumentTypeDef,
-    SsmDocumentTypeDef,
+    SsmDocumentOutputTypeDef,
     TemplateActionDocumentResponseMetadataTypeDef,
     TemplateActionDocumentTypeDef,
-    ReplicationConfigurationTypeDef,
-    UpdateReplicationConfigurationRequestRequestTypeDef,
     WaveResponseMetadataTypeDef,
     WaveTypeDef,
     ListApplicationsResponseTypeDef,
     DataReplicationInfoTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsResponseTypeDef,
     StartExportResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ImportTaskTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     LifeCycleTypeDef,
+    PostLaunchActionsTypeDef,
     ListSourceServerActionsResponseTypeDef,
     JobPostLaunchActionsLaunchStatusTypeDef,
-    PostLaunchActionsTypeDef,
+    PostLaunchActionsOutputTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesResponseTypeDef,
     ListImportsResponseTypeDef,
     StartImportResponseTypeDef,
     SourceServerResponseMetadataTypeDef,
     SourceServerTypeDef,
-    PostLaunchActionsStatusTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    PostLaunchActionsStatusTypeDef,
     LaunchConfigurationTemplateResponseMetadataTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
-    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     DescribeSourceServersResponseTypeDef,
     ParticipatingServerTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     DescribeJobsResponseTypeDef,
     StartCutoverResponseTypeDef,
     StartTestResponseTypeDef,
```

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/__init__.py` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/__init__.pyi` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/__main__.py` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mgn 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.mgn 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
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

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/client.py` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/client.pyi` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/literals.py` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,14 +331,15 @@
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
@@ -417,26 +418,28 @@
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

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/literals.pyi` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -329,14 +329,15 @@
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
@@ -415,26 +416,28 @@
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

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/paginator.py` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/paginator.pyi` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/type_defs.py` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,18 @@
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ImportErrorDataTypeDef",
     "ImportTaskSummaryApplicationsTypeDef",
     "ImportTaskSummaryServersTypeDef",
     "ImportTaskSummaryWavesTypeDef",
-    "S3BucketSourceTypeDef",
+    "S3BucketSourceOutputTypeDef",
     "JobLogEventDataTypeDef",
+    "LaunchTemplateDiskConfOutputTypeDef",
+    "LicensingOutputTypeDef",
     "LaunchedInstanceTypeDef",
     "LifeCycleLastCutoverFinalizedTypeDef",
     "LifeCycleLastCutoverInitiatedTypeDef",
     "LifeCycleLastCutoverRevertedTypeDef",
     "LifeCycleLastTestFinalizedTypeDef",
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
@@ -138,19 +140,23 @@
     "OSTypeDef",
     "PaginatorConfigTypeDef",
     "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
+    "S3BucketSourceTypeDef",
+    "SsmExternalParameterOutputTypeDef",
+    "SsmParameterStoreParameterOutputTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
@@ -172,15 +178,14 @@
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
     "ExportTaskTypeDef",
     "ImportTaskErrorTypeDef",
     "ImportTaskSummaryTypeDef",
-    "StartImportRequestRequestTypeDef",
     "JobLogTypeDef",
     "LifeCycleLastCutoverTypeDef",
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
@@ -192,48 +197,51 @@
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
     "PutSourceServerActionRequestRequestTypeDef",
     "PutTemplateActionRequestRequestTypeDef",
+    "SsmDocumentTypeDef",
+    "ReplicationConfigurationTypeDef",
+    "UpdateReplicationConfigurationRequestRequestTypeDef",
+    "StartImportRequestRequestTypeDef",
     "SourceServerActionDocumentResponseMetadataTypeDef",
     "SourceServerActionDocumentTypeDef",
-    "SsmDocumentTypeDef",
+    "SsmDocumentOutputTypeDef",
     "TemplateActionDocumentResponseMetadataTypeDef",
     "TemplateActionDocumentTypeDef",
-    "ReplicationConfigurationTypeDef",
-    "UpdateReplicationConfigurationRequestRequestTypeDef",
     "WaveResponseMetadataTypeDef",
     "WaveTypeDef",
     "ListApplicationsResponseTypeDef",
     "DataReplicationInfoTypeDef",
     "ListExportErrorsResponseTypeDef",
     "ListExportsResponseTypeDef",
     "StartExportResponseTypeDef",
     "ListImportErrorsResponseTypeDef",
     "ImportTaskTypeDef",
     "DescribeJobLogItemsResponseTypeDef",
     "LifeCycleTypeDef",
+    "PostLaunchActionsTypeDef",
     "ListSourceServerActionsResponseTypeDef",
     "JobPostLaunchActionsLaunchStatusTypeDef",
-    "PostLaunchActionsTypeDef",
+    "PostLaunchActionsOutputTypeDef",
     "ListTemplateActionsResponseTypeDef",
     "ListWavesResponseTypeDef",
     "ListImportsResponseTypeDef",
     "StartImportResponseTypeDef",
     "SourceServerResponseMetadataTypeDef",
     "SourceServerTypeDef",
-    "PostLaunchActionsStatusTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "PostLaunchActionsStatusTypeDef",
     "LaunchConfigurationTemplateResponseMetadataTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
-    "UpdateLaunchConfigurationRequestRequestTypeDef",
-    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "ParticipatingServerTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartCutoverResponseTypeDef",
     "StartTestResponseTypeDef",
@@ -981,45 +989,65 @@
     {
         "createdCount": int,
         "modifiedCount": int,
     },
     total=False,
 )
 
-_RequiredS3BucketSourceTypeDef = TypedDict(
-    "_RequiredS3BucketSourceTypeDef",
+_RequiredS3BucketSourceOutputTypeDef = TypedDict(
+    "_RequiredS3BucketSourceOutputTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
-_OptionalS3BucketSourceTypeDef = TypedDict(
-    "_OptionalS3BucketSourceTypeDef",
+_OptionalS3BucketSourceOutputTypeDef = TypedDict(
+    "_OptionalS3BucketSourceOutputTypeDef",
     {
         "s3BucketOwner": str,
     },
     total=False,
 )
 
 
-class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
+class S3BucketSourceOutputTypeDef(
+    _RequiredS3BucketSourceOutputTypeDef, _OptionalS3BucketSourceOutputTypeDef
+):
     pass
 
 
 JobLogEventDataTypeDef = TypedDict(
     "JobLogEventDataTypeDef",
     {
         "conversionServerID": str,
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
+LaunchTemplateDiskConfOutputTypeDef = TypedDict(
+    "LaunchTemplateDiskConfOutputTypeDef",
+    {
+        "iops": int,
+        "throughput": int,
+        "volumeType": VolumeTypeType,
+    },
+    total=False,
+)
+
+LicensingOutputTypeDef = TypedDict(
+    "LicensingOutputTypeDef",
+    {
+        "osByol": bool,
+    },
+    total=False,
+)
+
 LaunchedInstanceTypeDef = TypedDict(
     "LaunchedInstanceTypeDef",
     {
         "ec2InstanceID": str,
         "firstBoot": FirstBootType,
         "jobID": str,
     },
@@ -1368,14 +1396,26 @@
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
 )
 
+ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
+    {
+        "deviceName": str,
+        "iops": int,
+        "isBootDisk": bool,
+        "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
+        "throughput": int,
+    },
+    total=False,
+)
+
 ReplicationConfigurationReplicatedDiskTypeDef = TypedDict(
     "ReplicationConfigurationReplicatedDiskTypeDef",
     {
         "deviceName": str,
         "iops": int,
         "isBootDisk": bool,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
@@ -1457,14 +1497,50 @@
 class RetryDataReplicationRequestRequestTypeDef(
     _RequiredRetryDataReplicationRequestRequestTypeDef,
     _OptionalRetryDataReplicationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredS3BucketSourceTypeDef = TypedDict(
+    "_RequiredS3BucketSourceTypeDef",
+    {
+        "s3Bucket": str,
+        "s3Key": str,
+    },
+)
+_OptionalS3BucketSourceTypeDef = TypedDict(
+    "_OptionalS3BucketSourceTypeDef",
+    {
+        "s3BucketOwner": str,
+    },
+    total=False,
+)
+
+
+class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
+    pass
+
+
+SsmExternalParameterOutputTypeDef = TypedDict(
+    "SsmExternalParameterOutputTypeDef",
+    {
+        "dynamicPath": str,
+    },
+    total=False,
+)
+
+SsmParameterStoreParameterOutputTypeDef = TypedDict(
+    "SsmParameterStoreParameterOutputTypeDef",
+    {
+        "parameterName": str,
+        "parameterType": Literal["STRING"],
+    },
+)
+
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
@@ -1935,35 +2011,14 @@
         "applications": ImportTaskSummaryApplicationsTypeDef,
         "servers": ImportTaskSummaryServersTypeDef,
         "waves": ImportTaskSummaryWavesTypeDef,
     },
     total=False,
 )
 
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
-    {
-        "s3BucketSource": S3BucketSourceTypeDef,
-    },
-)
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
-    pass
-
-
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
@@ -2253,28 +2308,132 @@
 
 class PutTemplateActionRequestRequestTypeDef(
     _RequiredPutTemplateActionRequestRequestTypeDef, _OptionalPutTemplateActionRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredSsmDocumentTypeDef = TypedDict(
+    "_RequiredSsmDocumentTypeDef",
+    {
+        "actionName": str,
+        "ssmDocumentName": str,
+    },
+)
+_OptionalSsmDocumentTypeDef = TypedDict(
+    "_OptionalSsmDocumentTypeDef",
+    {
+        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
+        "mustSucceedForCutover": bool,
+        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
+        "timeoutSeconds": int,
+    },
+    total=False,
+)
+
+
+class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
+    pass
+
+
+ReplicationConfigurationTypeDef = TypedDict(
+    "ReplicationConfigurationTypeDef",
+    {
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "sourceServerID": str,
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": Sequence[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Mapping[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+    },
+    total=False,
+)
+
+
+class UpdateReplicationConfigurationRequestRequestTypeDef(
+    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
+    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "s3BucketSource": S3BucketSourceTypeDef,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
+
 SourceServerActionDocumentResponseMetadataTypeDef = TypedDict(
     "SourceServerActionDocumentResponseMetadataTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerActionDocumentTypeDef = TypedDict(
     "SourceServerActionDocumentTypeDef",
@@ -2282,61 +2441,63 @@
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-_RequiredSsmDocumentTypeDef = TypedDict(
-    "_RequiredSsmDocumentTypeDef",
+_RequiredSsmDocumentOutputTypeDef = TypedDict(
+    "_RequiredSsmDocumentOutputTypeDef",
     {
         "actionName": str,
         "ssmDocumentName": str,
     },
 )
-_OptionalSsmDocumentTypeDef = TypedDict(
-    "_OptionalSsmDocumentTypeDef",
+_OptionalSsmDocumentOutputTypeDef = TypedDict(
+    "_OptionalSsmDocumentOutputTypeDef",
     {
-        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
-        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
 
-class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
+class SsmDocumentOutputTypeDef(
+    _RequiredSsmDocumentOutputTypeDef, _OptionalSsmDocumentOutputTypeDef
+):
     pass
 
 
 TemplateActionDocumentResponseMetadataTypeDef = TypedDict(
     "TemplateActionDocumentResponseMetadataTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TemplateActionDocumentTypeDef = TypedDict(
     "TemplateActionDocumentTypeDef",
@@ -2344,84 +2505,24 @@
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-ReplicationConfigurationTypeDef = TypedDict(
-    "ReplicationConfigurationTypeDef",
-    {
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "sourceServerID": str,
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "sourceServerID": str,
-    },
-)
-_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "accountID": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": Sequence[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Mapping[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-    },
-    total=False,
-)
-
-
-class UpdateReplicationConfigurationRequestRequestTypeDef(
-    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
-    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 WaveResponseMetadataTypeDef = TypedDict(
     "WaveResponseMetadataTypeDef",
     {
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
@@ -2511,15 +2612,15 @@
 ImportTaskTypeDef = TypedDict(
     "ImportTaskTypeDef",
     {
         "creationDateTime": str,
         "endDateTime": str,
         "importID": str,
         "progressPercentage": float,
-        "s3BucketSource": S3BucketSourceTypeDef,
+        "s3BucketSource": S3BucketSourceOutputTypeDef,
         "status": ImportStatusType,
         "summary": ImportTaskSummaryTypeDef,
     },
     total=False,
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
@@ -2541,14 +2642,26 @@
         "lastSeenByServiceDateTime": str,
         "lastTest": LifeCycleLastTestTypeDef,
         "state": LifeCycleStateType,
     },
     total=False,
 )
 
+PostLaunchActionsTypeDef = TypedDict(
+    "PostLaunchActionsTypeDef",
+    {
+        "cloudWatchLogGroupName": str,
+        "deployment": PostLaunchActionsDeploymentTypeType,
+        "s3LogBucket": str,
+        "s3OutputKeyPrefix": str,
+        "ssmDocuments": Sequence[SsmDocumentTypeDef],
+    },
+    total=False,
+)
+
 ListSourceServerActionsResponseTypeDef = TypedDict(
     "ListSourceServerActionsResponseTypeDef",
     {
         "items": List[SourceServerActionDocumentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2556,28 +2669,28 @@
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
         "executionStatus": PostLaunchActionExecutionStatusType,
         "failureReason": str,
-        "ssmDocument": SsmDocumentTypeDef,
+        "ssmDocument": SsmDocumentOutputTypeDef,
         "ssmDocumentType": SsmDocumentTypeType,
     },
     total=False,
 )
 
-PostLaunchActionsTypeDef = TypedDict(
-    "PostLaunchActionsTypeDef",
+PostLaunchActionsOutputTypeDef = TypedDict(
+    "PostLaunchActionsOutputTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "deployment": PostLaunchActionsDeploymentTypeType,
         "s3LogBucket": str,
         "s3OutputKeyPrefix": str,
-        "ssmDocuments": Sequence[SsmDocumentTypeDef],
+        "ssmDocuments": List[SsmDocumentOutputTypeDef],
     },
     total=False,
 )
 
 ListTemplateActionsResponseTypeDef = TypedDict(
     "ListTemplateActionsResponseTypeDef",
     {
@@ -2649,23 +2762,14 @@
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
     },
     total=False,
 )
 
-PostLaunchActionsStatusTypeDef = TypedDict(
-    "PostLaunchActionsStatusTypeDef",
-    {
-        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
-        "ssmAgentDiscoveryDatetime": str,
-    },
-    total=False,
-)
-
 CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
@@ -2679,159 +2783,168 @@
         "smallVolumeMaxSize": int,
         "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-LaunchConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "LaunchConfigurationTemplateResponseMetadataTypeDef",
+_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
-        "associatePublicIpAddress": bool,
+        "sourceServerID": str,
+    },
+)
+_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
+        "name": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTemplateTypeDef",
+
+class UpdateLaunchConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
-_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTemplateTypeDef",
+_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
-        "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
 
-class LaunchConfigurationTemplateTypeDef(
-    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
+class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
+PostLaunchActionsStatusTypeDef = TypedDict(
+    "PostLaunchActionsStatusTypeDef",
+    {
+        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
+        "ssmAgentDiscoveryDatetime": str,
+    },
+    total=False,
+)
+
+LaunchConfigurationTemplateResponseMetadataTypeDef = TypedDict(
+    "LaunchConfigurationTemplateResponseMetadataTypeDef",
     {
+        "arn": str,
+        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
+        "licensing": LicensingOutputTypeDef,
         "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
-        "sourceServerID": str,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
+_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTemplateTypeDef",
     {
-        "sourceServerID": str,
+        "launchConfigurationTemplateID": str,
     },
 )
-_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
+_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTemplateTypeDef",
     {
-        "accountID": str,
+        "arn": str,
+        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
+        "licensing": LicensingOutputTypeDef,
         "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
 
-class UpdateLaunchConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+class LaunchConfigurationTemplateTypeDef(
+    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
 ):
     pass
 
 
-_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
-    {
-        "launchConfigurationTemplateID": str,
-    },
-)
-_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
     {
-        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
+        "licensing": LicensingOutputTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "smallVolumeMaxSize": int,
+        "name": str,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn/type_defs.pyi` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,18 @@
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ImportErrorDataTypeDef",
     "ImportTaskSummaryApplicationsTypeDef",
     "ImportTaskSummaryServersTypeDef",
     "ImportTaskSummaryWavesTypeDef",
-    "S3BucketSourceTypeDef",
+    "S3BucketSourceOutputTypeDef",
     "JobLogEventDataTypeDef",
+    "LaunchTemplateDiskConfOutputTypeDef",
+    "LicensingOutputTypeDef",
     "LaunchedInstanceTypeDef",
     "LifeCycleLastCutoverFinalizedTypeDef",
     "LifeCycleLastCutoverInitiatedTypeDef",
     "LifeCycleLastCutoverRevertedTypeDef",
     "LifeCycleLastTestFinalizedTypeDef",
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
@@ -137,19 +139,23 @@
     "OSTypeDef",
     "PaginatorConfigTypeDef",
     "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
     "ReplicationConfigurationTemplateResponseMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
+    "S3BucketSourceTypeDef",
+    "SsmExternalParameterOutputTypeDef",
+    "SsmParameterStoreParameterOutputTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
@@ -171,15 +177,14 @@
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
     "ExportTaskTypeDef",
     "ImportTaskErrorTypeDef",
     "ImportTaskSummaryTypeDef",
-    "StartImportRequestRequestTypeDef",
     "JobLogTypeDef",
     "LifeCycleLastCutoverTypeDef",
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
@@ -191,48 +196,51 @@
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
     "PutSourceServerActionRequestRequestTypeDef",
     "PutTemplateActionRequestRequestTypeDef",
+    "SsmDocumentTypeDef",
+    "ReplicationConfigurationTypeDef",
+    "UpdateReplicationConfigurationRequestRequestTypeDef",
+    "StartImportRequestRequestTypeDef",
     "SourceServerActionDocumentResponseMetadataTypeDef",
     "SourceServerActionDocumentTypeDef",
-    "SsmDocumentTypeDef",
+    "SsmDocumentOutputTypeDef",
     "TemplateActionDocumentResponseMetadataTypeDef",
     "TemplateActionDocumentTypeDef",
-    "ReplicationConfigurationTypeDef",
-    "UpdateReplicationConfigurationRequestRequestTypeDef",
     "WaveResponseMetadataTypeDef",
     "WaveTypeDef",
     "ListApplicationsResponseTypeDef",
     "DataReplicationInfoTypeDef",
     "ListExportErrorsResponseTypeDef",
     "ListExportsResponseTypeDef",
     "StartExportResponseTypeDef",
     "ListImportErrorsResponseTypeDef",
     "ImportTaskTypeDef",
     "DescribeJobLogItemsResponseTypeDef",
     "LifeCycleTypeDef",
+    "PostLaunchActionsTypeDef",
     "ListSourceServerActionsResponseTypeDef",
     "JobPostLaunchActionsLaunchStatusTypeDef",
-    "PostLaunchActionsTypeDef",
+    "PostLaunchActionsOutputTypeDef",
     "ListTemplateActionsResponseTypeDef",
     "ListWavesResponseTypeDef",
     "ListImportsResponseTypeDef",
     "StartImportResponseTypeDef",
     "SourceServerResponseMetadataTypeDef",
     "SourceServerTypeDef",
-    "PostLaunchActionsStatusTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "PostLaunchActionsStatusTypeDef",
     "LaunchConfigurationTemplateResponseMetadataTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
-    "UpdateLaunchConfigurationRequestRequestTypeDef",
-    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "ParticipatingServerTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartCutoverResponseTypeDef",
     "StartTestResponseTypeDef",
@@ -940,43 +948,63 @@
     {
         "createdCount": int,
         "modifiedCount": int,
     },
     total=False,
 )
 
-_RequiredS3BucketSourceTypeDef = TypedDict(
-    "_RequiredS3BucketSourceTypeDef",
+_RequiredS3BucketSourceOutputTypeDef = TypedDict(
+    "_RequiredS3BucketSourceOutputTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
-_OptionalS3BucketSourceTypeDef = TypedDict(
-    "_OptionalS3BucketSourceTypeDef",
+_OptionalS3BucketSourceOutputTypeDef = TypedDict(
+    "_OptionalS3BucketSourceOutputTypeDef",
     {
         "s3BucketOwner": str,
     },
     total=False,
 )
 
-class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
+class S3BucketSourceOutputTypeDef(
+    _RequiredS3BucketSourceOutputTypeDef, _OptionalS3BucketSourceOutputTypeDef
+):
     pass
 
 JobLogEventDataTypeDef = TypedDict(
     "JobLogEventDataTypeDef",
     {
         "conversionServerID": str,
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
+LaunchTemplateDiskConfOutputTypeDef = TypedDict(
+    "LaunchTemplateDiskConfOutputTypeDef",
+    {
+        "iops": int,
+        "throughput": int,
+        "volumeType": VolumeTypeType,
+    },
+    total=False,
+)
+
+LicensingOutputTypeDef = TypedDict(
+    "LicensingOutputTypeDef",
+    {
+        "osByol": bool,
+    },
+    total=False,
+)
+
 LaunchedInstanceTypeDef = TypedDict(
     "LaunchedInstanceTypeDef",
     {
         "ec2InstanceID": str,
         "firstBoot": FirstBootType,
         "jobID": str,
     },
@@ -1311,14 +1339,26 @@
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
 )
 
+ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
+    {
+        "deviceName": str,
+        "iops": int,
+        "isBootDisk": bool,
+        "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
+        "throughput": int,
+    },
+    total=False,
+)
+
 ReplicationConfigurationReplicatedDiskTypeDef = TypedDict(
     "ReplicationConfigurationReplicatedDiskTypeDef",
     {
         "deviceName": str,
         "iops": int,
         "isBootDisk": bool,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
@@ -1396,14 +1436,48 @@
 
 class RetryDataReplicationRequestRequestTypeDef(
     _RequiredRetryDataReplicationRequestRequestTypeDef,
     _OptionalRetryDataReplicationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredS3BucketSourceTypeDef = TypedDict(
+    "_RequiredS3BucketSourceTypeDef",
+    {
+        "s3Bucket": str,
+        "s3Key": str,
+    },
+)
+_OptionalS3BucketSourceTypeDef = TypedDict(
+    "_OptionalS3BucketSourceTypeDef",
+    {
+        "s3BucketOwner": str,
+    },
+    total=False,
+)
+
+class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
+    pass
+
+SsmExternalParameterOutputTypeDef = TypedDict(
+    "SsmExternalParameterOutputTypeDef",
+    {
+        "dynamicPath": str,
+    },
+    total=False,
+)
+
+SsmParameterStoreParameterOutputTypeDef = TypedDict(
+    "SsmParameterStoreParameterOutputTypeDef",
+    {
+        "parameterName": str,
+        "parameterType": Literal["STRING"],
+    },
+)
+
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
@@ -1848,33 +1922,14 @@
         "applications": ImportTaskSummaryApplicationsTypeDef,
         "servers": ImportTaskSummaryServersTypeDef,
         "waves": ImportTaskSummaryWavesTypeDef,
     },
     total=False,
 )
 
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
-    {
-        "s3BucketSource": S3BucketSourceTypeDef,
-    },
-)
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
-    pass
-
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
@@ -2152,28 +2207,126 @@
 )
 
 class PutTemplateActionRequestRequestTypeDef(
     _RequiredPutTemplateActionRequestRequestTypeDef, _OptionalPutTemplateActionRequestRequestTypeDef
 ):
     pass
 
+_RequiredSsmDocumentTypeDef = TypedDict(
+    "_RequiredSsmDocumentTypeDef",
+    {
+        "actionName": str,
+        "ssmDocumentName": str,
+    },
+)
+_OptionalSsmDocumentTypeDef = TypedDict(
+    "_OptionalSsmDocumentTypeDef",
+    {
+        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
+        "mustSucceedForCutover": bool,
+        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
+        "timeoutSeconds": int,
+    },
+    total=False,
+)
+
+class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
+    pass
+
+ReplicationConfigurationTypeDef = TypedDict(
+    "ReplicationConfigurationTypeDef",
+    {
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "sourceServerID": str,
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": Sequence[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Mapping[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+    },
+    total=False,
+)
+
+class UpdateReplicationConfigurationRequestRequestTypeDef(
+    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
+    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "s3BucketSource": S3BucketSourceTypeDef,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
 SourceServerActionDocumentResponseMetadataTypeDef = TypedDict(
     "SourceServerActionDocumentResponseMetadataTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerActionDocumentTypeDef = TypedDict(
     "SourceServerActionDocumentTypeDef",
@@ -2181,59 +2334,61 @@
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-_RequiredSsmDocumentTypeDef = TypedDict(
-    "_RequiredSsmDocumentTypeDef",
+_RequiredSsmDocumentOutputTypeDef = TypedDict(
+    "_RequiredSsmDocumentOutputTypeDef",
     {
         "actionName": str,
         "ssmDocumentName": str,
     },
 )
-_OptionalSsmDocumentTypeDef = TypedDict(
-    "_OptionalSsmDocumentTypeDef",
+_OptionalSsmDocumentOutputTypeDef = TypedDict(
+    "_OptionalSsmDocumentOutputTypeDef",
     {
-        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
-        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
+class SsmDocumentOutputTypeDef(
+    _RequiredSsmDocumentOutputTypeDef, _OptionalSsmDocumentOutputTypeDef
+):
     pass
 
 TemplateActionDocumentResponseMetadataTypeDef = TypedDict(
     "TemplateActionDocumentResponseMetadataTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TemplateActionDocumentTypeDef = TypedDict(
     "TemplateActionDocumentTypeDef",
@@ -2241,82 +2396,24 @@
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-ReplicationConfigurationTypeDef = TypedDict(
-    "ReplicationConfigurationTypeDef",
-    {
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "sourceServerID": str,
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "sourceServerID": str,
-    },
-)
-_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "accountID": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": Sequence[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Mapping[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-    },
-    total=False,
-)
-
-class UpdateReplicationConfigurationRequestRequestTypeDef(
-    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
-    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
-):
-    pass
-
 WaveResponseMetadataTypeDef = TypedDict(
     "WaveResponseMetadataTypeDef",
     {
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
@@ -2406,15 +2503,15 @@
 ImportTaskTypeDef = TypedDict(
     "ImportTaskTypeDef",
     {
         "creationDateTime": str,
         "endDateTime": str,
         "importID": str,
         "progressPercentage": float,
-        "s3BucketSource": S3BucketSourceTypeDef,
+        "s3BucketSource": S3BucketSourceOutputTypeDef,
         "status": ImportStatusType,
         "summary": ImportTaskSummaryTypeDef,
     },
     total=False,
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
@@ -2436,14 +2533,26 @@
         "lastSeenByServiceDateTime": str,
         "lastTest": LifeCycleLastTestTypeDef,
         "state": LifeCycleStateType,
     },
     total=False,
 )
 
+PostLaunchActionsTypeDef = TypedDict(
+    "PostLaunchActionsTypeDef",
+    {
+        "cloudWatchLogGroupName": str,
+        "deployment": PostLaunchActionsDeploymentTypeType,
+        "s3LogBucket": str,
+        "s3OutputKeyPrefix": str,
+        "ssmDocuments": Sequence[SsmDocumentTypeDef],
+    },
+    total=False,
+)
+
 ListSourceServerActionsResponseTypeDef = TypedDict(
     "ListSourceServerActionsResponseTypeDef",
     {
         "items": List[SourceServerActionDocumentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2451,28 +2560,28 @@
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
         "executionStatus": PostLaunchActionExecutionStatusType,
         "failureReason": str,
-        "ssmDocument": SsmDocumentTypeDef,
+        "ssmDocument": SsmDocumentOutputTypeDef,
         "ssmDocumentType": SsmDocumentTypeType,
     },
     total=False,
 )
 
-PostLaunchActionsTypeDef = TypedDict(
-    "PostLaunchActionsTypeDef",
+PostLaunchActionsOutputTypeDef = TypedDict(
+    "PostLaunchActionsOutputTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "deployment": PostLaunchActionsDeploymentTypeType,
         "s3LogBucket": str,
         "s3OutputKeyPrefix": str,
-        "ssmDocuments": Sequence[SsmDocumentTypeDef],
+        "ssmDocuments": List[SsmDocumentOutputTypeDef],
     },
     total=False,
 )
 
 ListTemplateActionsResponseTypeDef = TypedDict(
     "ListTemplateActionsResponseTypeDef",
     {
@@ -2544,23 +2653,14 @@
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
     },
     total=False,
 )
 
-PostLaunchActionsStatusTypeDef = TypedDict(
-    "PostLaunchActionsStatusTypeDef",
-    {
-        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
-        "ssmAgentDiscoveryDatetime": str,
-    },
-    total=False,
-)
-
 CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
@@ -2574,153 +2674,162 @@
         "smallVolumeMaxSize": int,
         "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-LaunchConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "LaunchConfigurationTemplateResponseMetadataTypeDef",
+_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
-        "associatePublicIpAddress": bool,
+        "sourceServerID": str,
+    },
+)
+_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
+        "name": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTemplateTypeDef",
+class UpdateLaunchConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
-_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTemplateTypeDef",
+_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
-        "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-class LaunchConfigurationTemplateTypeDef(
-    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
+class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
+PostLaunchActionsStatusTypeDef = TypedDict(
+    "PostLaunchActionsStatusTypeDef",
     {
+        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
+        "ssmAgentDiscoveryDatetime": str,
+    },
+    total=False,
+)
+
+LaunchConfigurationTemplateResponseMetadataTypeDef = TypedDict(
+    "LaunchConfigurationTemplateResponseMetadataTypeDef",
+    {
+        "arn": str,
+        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
+        "licensing": LicensingOutputTypeDef,
         "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
-        "sourceServerID": str,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
+_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTemplateTypeDef",
     {
-        "sourceServerID": str,
+        "launchConfigurationTemplateID": str,
     },
 )
-_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
+_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTemplateTypeDef",
     {
-        "accountID": str,
+        "arn": str,
+        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
+        "licensing": LicensingOutputTypeDef,
         "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-class UpdateLaunchConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+class LaunchConfigurationTemplateTypeDef(
+    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
 ):
     pass
 
-_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
-    {
-        "launchConfigurationTemplateID": str,
-    },
-)
-_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
     {
-        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
+        "licensing": LicensingOutputTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "smallVolumeMaxSize": int,
+        "name": str,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-):
-    pass
-
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/PKG-INFO` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.28.0
-Summary: Type annotations for boto3.mgn 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.mgn 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -459,16 +459,18 @@
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
     ImportTaskSummaryApplicationsTypeDef,
     ImportTaskSummaryServersTypeDef,
     ImportTaskSummaryWavesTypeDef,
-    S3BucketSourceTypeDef,
+    S3BucketSourceOutputTypeDef,
     JobLogEventDataTypeDef,
+    LaunchTemplateDiskConfOutputTypeDef,
+    LicensingOutputTypeDef,
     LaunchedInstanceTypeDef,
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
@@ -492,19 +494,23 @@
     OSTypeDef,
     PaginatorConfigTypeDef,
     PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
+    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseMetadataTypeDef,
     ResponseMetadataTypeDef,
     ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
+    S3BucketSourceTypeDef,
+    SsmExternalParameterOutputTypeDef,
+    SsmParameterStoreParameterOutputTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -526,15 +532,14 @@
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
     ExportTaskTypeDef,
     ImportTaskErrorTypeDef,
     ImportTaskSummaryTypeDef,
-    StartImportRequestRequestTypeDef,
     JobLogTypeDef,
     LifeCycleLastCutoverTypeDef,
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
@@ -546,48 +551,51 @@
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
     PutSourceServerActionRequestRequestTypeDef,
     PutTemplateActionRequestRequestTypeDef,
+    SsmDocumentTypeDef,
+    ReplicationConfigurationTypeDef,
+    UpdateReplicationConfigurationRequestRequestTypeDef,
+    StartImportRequestRequestTypeDef,
     SourceServerActionDocumentResponseMetadataTypeDef,
     SourceServerActionDocumentTypeDef,
-    SsmDocumentTypeDef,
+    SsmDocumentOutputTypeDef,
     TemplateActionDocumentResponseMetadataTypeDef,
     TemplateActionDocumentTypeDef,
-    ReplicationConfigurationTypeDef,
-    UpdateReplicationConfigurationRequestRequestTypeDef,
     WaveResponseMetadataTypeDef,
     WaveTypeDef,
     ListApplicationsResponseTypeDef,
     DataReplicationInfoTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsResponseTypeDef,
     StartExportResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ImportTaskTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     LifeCycleTypeDef,
+    PostLaunchActionsTypeDef,
     ListSourceServerActionsResponseTypeDef,
     JobPostLaunchActionsLaunchStatusTypeDef,
-    PostLaunchActionsTypeDef,
+    PostLaunchActionsOutputTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesResponseTypeDef,
     ListImportsResponseTypeDef,
     StartImportResponseTypeDef,
     SourceServerResponseMetadataTypeDef,
     SourceServerTypeDef,
-    PostLaunchActionsStatusTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    PostLaunchActionsStatusTypeDef,
     LaunchConfigurationTemplateResponseMetadataTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
-    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     DescribeSourceServersResponseTypeDef,
     ParticipatingServerTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     DescribeJobsResponseTypeDef,
     StartCutoverResponseTypeDef,
     StartTestResponseTypeDef,
```

### Comparing `mypy-boto3-mgn-1.28.0/mypy_boto3_mgn.egg-info/SOURCES.txt` & `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.0/setup.py` & `mypy-boto3-mgn-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgn",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mgn 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.mgn 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

