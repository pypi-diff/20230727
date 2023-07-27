# Comparing `tmp/mypy-boto3-drs-1.28.0.tar.gz` & `tmp/mypy-boto3-drs-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-drs-1.28.0.tar", last modified: Thu Jul  6 20:59:26 2023, max compression
+gzip compressed data, was "mypy-boto3-drs-1.28.12.tar", last modified: Thu Jul 27 05:34:35 2023, max compression
```

## Comparing `mypy-boto3-drs-1.28.0.tar` & `mypy-boto3-drs-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.406283 mypy-boto3-drs-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-07-06 20:59:26.402283 mypy-boto3-drs-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.394283 mypy-boto3-drs-1.28.0/mypy_boto3_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-07-06 20:38:15.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39630 2023-07-06 20:38:14.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-06 20:38:15.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-07-06 20:38:15.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-06 20:38:15.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-06 20:38:15.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56958 2023-07-06 20:38:17.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56911 2023-07-06 20:38:16.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.402283 mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-07-06 20:59:26.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:26.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:26.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:26.000000 mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:26.406283 mypy-boto3-drs-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:38:13.000000 mypy-boto3-drs-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20420 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/mypy_boto3_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39630 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58187 2023-07-27 05:20:31.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58138 2023-07-27 05:20:31.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/setup.py
```

### Comparing `mypy-boto3-drs-1.28.0/LICENSE` & `mypy-boto3-drs-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/PKG-INFO` & `mypy-boto3-drs-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.0
-Summary: Type annotations for boto3.drs 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.drs 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-drs"></a>
 
 # mypy-boto3-drs
 
 [![PyPI - mypy-boto3-drs](https://img.shields.io/pypi/v/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,32 +438,35 @@
     ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
     GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
+    LicensingOutputTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
     ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
     ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PITPolicyRuleOutputTypeDef,
     PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
+    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
     ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
@@ -477,53 +480,53 @@
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     ListStagingAccountsResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
-    LaunchConfigurationTemplateTypeDef,
-    LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
     DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     EventResourceDataTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
+    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateTypeDef,
     ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
     SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestRequestTypeDef,
+    DataReplicationInfoTypeDef,
+    JobLogEventDataTypeDef,
     CreateLaunchConfigurationTemplateResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     UpdateLaunchConfigurationTemplateResponseTypeDef,
-    DescribeReplicationConfigurationTemplatesResponseTypeDef,
-    DataReplicationInfoTypeDef,
-    JobLogEventDataTypeDef,
     LifeCycleTypeDef,
+    DescribeReplicationConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
     SourceServerResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-drs-1.28.0/README.md` & `mypy-boto3-drs-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-drs"></a>
 
 # mypy-boto3-drs
 
 [![PyPI - mypy-boto3-drs](https://img.shields.io/pypi/v/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,32 +406,35 @@
     ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
     GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
+    LicensingOutputTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
     ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
     ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PITPolicyRuleOutputTypeDef,
     PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
+    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
     ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
@@ -445,53 +448,53 @@
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     ListStagingAccountsResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
-    LaunchConfigurationTemplateTypeDef,
-    LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
     DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     EventResourceDataTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
+    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateTypeDef,
     ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
     SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestRequestTypeDef,
+    DataReplicationInfoTypeDef,
+    JobLogEventDataTypeDef,
     CreateLaunchConfigurationTemplateResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     UpdateLaunchConfigurationTemplateResponseTypeDef,
-    DescribeReplicationConfigurationTemplatesResponseTypeDef,
-    DataReplicationInfoTypeDef,
-    JobLogEventDataTypeDef,
     LifeCycleTypeDef,
+    DescribeReplicationConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
     SourceServerResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/__init__.py` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/__init__.pyi` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/__main__.py` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.drs 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.drs 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/client.py` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/client.pyi` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/literals.py` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,15 @@
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
@@ -470,26 +471,28 @@
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

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/literals.pyi` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,15 @@
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
@@ -468,26 +469,28 @@
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

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/paginator.py` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/paginator.pyi` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/type_defs.py` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,32 +95,35 @@
     "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
+    "LicensingOutputTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
     "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
     "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PITPolicyRuleOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
     "RecoveryLifeCycleTypeDef",
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
     "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
     "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
@@ -134,53 +137,53 @@
     "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
     "ListStagingAccountsResponseTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    "LaunchConfigurationTemplateTypeDef",
-    "LaunchConfigurationTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     "DescribeSourceNetworksRequestRequestTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "EventResourceDataTypeDef",
+    "LaunchConfigurationTemplateTypeDef",
+    "LaunchConfigurationTypeDef",
     "LifeCycleLastLaunchTypeDef",
     "ListExtensibleSourceServersResponseTypeDef",
     "SourcePropertiesTypeDef",
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ReplicationConfigurationTemplateTypeDef",
     "ParticipatingResourceTypeDef",
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     "RecoveryInstancePropertiesTypeDef",
     "SourceNetworkTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "StartRecoveryRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestRequestTypeDef",
+    "DataReplicationInfoTypeDef",
+    "JobLogEventDataTypeDef",
     "CreateLaunchConfigurationTemplateResponseTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
-    "DataReplicationInfoTypeDef",
-    "JobLogEventDataTypeDef",
     "LifeCycleTypeDef",
+    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
     "DescribeSourceNetworksResponseTypeDef",
     "StartSourceNetworkReplicationResponseTypeDef",
     "StopSourceNetworkReplicationResponseTypeDef",
     "JobLogTypeDef",
     "SourceServerResponseMetadataTypeDef",
@@ -651,14 +654,22 @@
         "launchStatus": LaunchStatusType,
         "recoveryInstanceID": str,
         "sourceServerID": str,
     },
     total=False,
 )
 
+LicensingOutputTypeDef = TypedDict(
+    "LicensingOutputTypeDef",
+    {
+        "osByol": bool,
+    },
+    total=False,
+)
+
 LifeCycleLastLaunchInitiatedTypeDef = TypedDict(
     "LifeCycleLastLaunchInitiatedTypeDef",
     {
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
@@ -766,14 +777,38 @@
     "OSTypeDef",
     {
         "fullString": str,
     },
     total=False,
 )
 
+_RequiredPITPolicyRuleOutputTypeDef = TypedDict(
+    "_RequiredPITPolicyRuleOutputTypeDef",
+    {
+        "interval": int,
+        "retentionDuration": int,
+        "units": PITPolicyRuleUnitsType,
+    },
+)
+_OptionalPITPolicyRuleOutputTypeDef = TypedDict(
+    "_OptionalPITPolicyRuleOutputTypeDef",
+    {
+        "enabled": bool,
+        "ruleID": int,
+    },
+    total=False,
+)
+
+
+class PITPolicyRuleOutputTypeDef(
+    _RequiredPITPolicyRuleOutputTypeDef, _OptionalPITPolicyRuleOutputTypeDef
+):
+    pass
+
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -851,14 +886,27 @@
         "apiCallDateTime": datetime,
         "jobID": str,
         "lastRecoveryResult": RecoveryResultType,
     },
     total=False,
 )
 
+ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
+    {
+        "deviceName": str,
+        "iops": int,
+        "isBootDisk": bool,
+        "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
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
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
@@ -1089,45 +1137,14 @@
         "licensing": LicensingTypeDef,
         "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-LaunchConfigurationTemplateTypeDef = TypedDict(
-    "LaunchConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "exportBucketArn": str,
-        "launchConfigurationTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "tags": Dict[str, str],
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-    },
-    total=False,
-)
-
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
-    {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "name": str,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
@@ -1209,75 +1226,14 @@
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleTypeDef],
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredReplicationConfigurationTemplateTypeDef",
-    {
-        "replicationConfigurationTemplateID": str,
-    },
-)
-_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalReplicationConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-    },
-    total=False,
-)
-
-
-class ReplicationConfigurationTemplateTypeDef(
-    _RequiredReplicationConfigurationTemplateTypeDef,
-    _OptionalReplicationConfigurationTemplateTypeDef,
-):
-    pass
-
-
 _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
@@ -1458,14 +1414,45 @@
     "EventResourceDataTypeDef",
     {
         "sourceNetworkData": SourceNetworkDataTypeDef,
     },
     total=False,
 )
 
+LaunchConfigurationTemplateTypeDef = TypedDict(
+    "LaunchConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchConfigurationTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingOutputTypeDef,
+        "tags": Dict[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingOutputTypeDef,
+        "name": str,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
         "status": LaunchStatusType,
     },
     total=False,
@@ -1492,14 +1479,75 @@
         "ramBytes": int,
         "recommendedInstanceType": str,
         "supportsNitroInstances": bool,
     },
     total=False,
 )
 
+ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredReplicationConfigurationTemplateTypeDef",
+    {
+        "replicationConfigurationTemplateID": str,
+    },
+)
+_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalReplicationConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+    },
+    total=False,
+)
+
+
+class ReplicationConfigurationTemplateTypeDef(
+    _RequiredReplicationConfigurationTemplateTypeDef,
+    _OptionalReplicationConfigurationTemplateTypeDef,
+):
+    pass
+
+
 ParticipatingResourceTypeDef = TypedDict(
     "ParticipatingResourceTypeDef",
     {
         "launchStatus": LaunchStatusType,
         "participatingResourceID": ParticipatingResourceIDTypeDef,
     },
     total=False,
@@ -1554,16 +1602,16 @@
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
-        "pitPolicy": List[PITPolicyRuleTypeDef],
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
+        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1648,48 +1696,14 @@
 class StartSourceNetworkRecoveryRequestRequestTypeDef(
     _RequiredStartSourceNetworkRecoveryRequestRequestTypeDef,
     _OptionalStartSourceNetworkRecoveryRequestRequestTypeDef,
 ):
     pass
 
 
-CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[LaunchConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[ReplicationConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
         "dataReplicationInitiation": DataReplicationInitiationTypeDef,
         "dataReplicationState": DataReplicationStateType,
         "etaDateTime": str,
@@ -1709,26 +1723,60 @@
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
+CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[LaunchConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
         "elapsedReplicationDuration": str,
         "firstByteDateTime": str,
         "lastLaunch": LifeCycleLastLaunchTypeDef,
         "lastSeenByServiceDateTime": str,
     },
     total=False,
 )
 
+DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[ReplicationConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalJobTypeDef = TypedDict(
```

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs/type_defs.pyi` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -94,32 +94,35 @@
     "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
+    "LicensingOutputTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
     "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
     "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PITPolicyRuleOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
     "RecoveryLifeCycleTypeDef",
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
     "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
     "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
@@ -133,53 +136,53 @@
     "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
     "ListStagingAccountsResponseTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    "LaunchConfigurationTemplateTypeDef",
-    "LaunchConfigurationTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     "DescribeSourceNetworksRequestRequestTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "EventResourceDataTypeDef",
+    "LaunchConfigurationTemplateTypeDef",
+    "LaunchConfigurationTypeDef",
     "LifeCycleLastLaunchTypeDef",
     "ListExtensibleSourceServersResponseTypeDef",
     "SourcePropertiesTypeDef",
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ReplicationConfigurationTemplateTypeDef",
     "ParticipatingResourceTypeDef",
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     "RecoveryInstancePropertiesTypeDef",
     "SourceNetworkTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "StartRecoveryRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestRequestTypeDef",
+    "DataReplicationInfoTypeDef",
+    "JobLogEventDataTypeDef",
     "CreateLaunchConfigurationTemplateResponseTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
-    "DataReplicationInfoTypeDef",
-    "JobLogEventDataTypeDef",
     "LifeCycleTypeDef",
+    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
     "DescribeSourceNetworksResponseTypeDef",
     "StartSourceNetworkReplicationResponseTypeDef",
     "StopSourceNetworkReplicationResponseTypeDef",
     "JobLogTypeDef",
     "SourceServerResponseMetadataTypeDef",
@@ -638,14 +641,22 @@
         "launchStatus": LaunchStatusType,
         "recoveryInstanceID": str,
         "sourceServerID": str,
     },
     total=False,
 )
 
+LicensingOutputTypeDef = TypedDict(
+    "LicensingOutputTypeDef",
+    {
+        "osByol": bool,
+    },
+    total=False,
+)
+
 LifeCycleLastLaunchInitiatedTypeDef = TypedDict(
     "LifeCycleLastLaunchInitiatedTypeDef",
     {
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
@@ -749,14 +760,36 @@
     "OSTypeDef",
     {
         "fullString": str,
     },
     total=False,
 )
 
+_RequiredPITPolicyRuleOutputTypeDef = TypedDict(
+    "_RequiredPITPolicyRuleOutputTypeDef",
+    {
+        "interval": int,
+        "retentionDuration": int,
+        "units": PITPolicyRuleUnitsType,
+    },
+)
+_OptionalPITPolicyRuleOutputTypeDef = TypedDict(
+    "_OptionalPITPolicyRuleOutputTypeDef",
+    {
+        "enabled": bool,
+        "ruleID": int,
+    },
+    total=False,
+)
+
+class PITPolicyRuleOutputTypeDef(
+    _RequiredPITPolicyRuleOutputTypeDef, _OptionalPITPolicyRuleOutputTypeDef
+):
+    pass
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -834,14 +867,27 @@
         "apiCallDateTime": datetime,
         "jobID": str,
         "lastRecoveryResult": RecoveryResultType,
     },
     total=False,
 )
 
+ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
+    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
+    {
+        "deviceName": str,
+        "iops": int,
+        "isBootDisk": bool,
+        "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
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
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
@@ -1064,45 +1110,14 @@
         "licensing": LicensingTypeDef,
         "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-LaunchConfigurationTemplateTypeDef = TypedDict(
-    "LaunchConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "exportBucketArn": str,
-        "launchConfigurationTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "tags": Dict[str, str],
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-    },
-    total=False,
-)
-
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
-    {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "name": str,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
@@ -1178,73 +1193,14 @@
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleTypeDef],
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredReplicationConfigurationTemplateTypeDef",
-    {
-        "replicationConfigurationTemplateID": str,
-    },
-)
-_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalReplicationConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-    },
-    total=False,
-)
-
-class ReplicationConfigurationTemplateTypeDef(
-    _RequiredReplicationConfigurationTemplateTypeDef,
-    _OptionalReplicationConfigurationTemplateTypeDef,
-):
-    pass
-
 _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
@@ -1419,14 +1375,45 @@
     "EventResourceDataTypeDef",
     {
         "sourceNetworkData": SourceNetworkDataTypeDef,
     },
     total=False,
 )
 
+LaunchConfigurationTemplateTypeDef = TypedDict(
+    "LaunchConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchConfigurationTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingOutputTypeDef,
+        "tags": Dict[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingOutputTypeDef,
+        "name": str,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
         "status": LaunchStatusType,
     },
     total=False,
@@ -1453,14 +1440,73 @@
         "ramBytes": int,
         "recommendedInstanceType": str,
         "supportsNitroInstances": bool,
     },
     total=False,
 )
 
+ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredReplicationConfigurationTemplateTypeDef",
+    {
+        "replicationConfigurationTemplateID": str,
+    },
+)
+_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalReplicationConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+    },
+    total=False,
+)
+
+class ReplicationConfigurationTemplateTypeDef(
+    _RequiredReplicationConfigurationTemplateTypeDef,
+    _OptionalReplicationConfigurationTemplateTypeDef,
+):
+    pass
+
 ParticipatingResourceTypeDef = TypedDict(
     "ParticipatingResourceTypeDef",
     {
         "launchStatus": LaunchStatusType,
         "participatingResourceID": ParticipatingResourceIDTypeDef,
     },
     total=False,
@@ -1515,16 +1561,16 @@
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
-        "pitPolicy": List[PITPolicyRuleTypeDef],
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
+        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1603,48 +1649,14 @@
 
 class StartSourceNetworkRecoveryRequestRequestTypeDef(
     _RequiredStartSourceNetworkRecoveryRequestRequestTypeDef,
     _OptionalStartSourceNetworkRecoveryRequestRequestTypeDef,
 ):
     pass
 
-CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[LaunchConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[ReplicationConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
         "dataReplicationInitiation": DataReplicationInitiationTypeDef,
         "dataReplicationState": DataReplicationStateType,
         "etaDateTime": str,
@@ -1664,26 +1676,60 @@
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
+CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[LaunchConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
         "elapsedReplicationDuration": str,
         "firstByteDateTime": str,
         "lastLaunch": LifeCycleLastLaunchTypeDef,
         "lastSeenByServiceDateTime": str,
     },
     total=False,
 )
 
+DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[ReplicationConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalJobTypeDef = TypedDict(
```

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/PKG-INFO` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.0
-Summary: Type annotations for boto3.drs 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.drs 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-drs"></a>
 
 # mypy-boto3-drs
 
 [![PyPI - mypy-boto3-drs](https://img.shields.io/pypi/v/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,32 +438,35 @@
     ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
     GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
+    LicensingOutputTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
     ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
     ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PITPolicyRuleOutputTypeDef,
     PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
+    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
     ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
@@ -477,53 +480,53 @@
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     ListStagingAccountsResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
-    LaunchConfigurationTemplateTypeDef,
-    LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
     DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     EventResourceDataTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
+    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateTypeDef,
     ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
     SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestRequestTypeDef,
+    DataReplicationInfoTypeDef,
+    JobLogEventDataTypeDef,
     CreateLaunchConfigurationTemplateResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     UpdateLaunchConfigurationTemplateResponseTypeDef,
-    DescribeReplicationConfigurationTemplatesResponseTypeDef,
-    DataReplicationInfoTypeDef,
-    JobLogEventDataTypeDef,
     LifeCycleTypeDef,
+    DescribeReplicationConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
     SourceServerResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-drs-1.28.0/mypy_boto3_drs.egg-info/SOURCES.txt` & `mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.0/setup.py` & `mypy-boto3-drs-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-drs",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.drs 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.drs 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

