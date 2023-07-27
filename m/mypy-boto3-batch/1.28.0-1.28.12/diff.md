# Comparing `tmp/mypy-boto3-batch-1.28.0.tar.gz` & `tmp/mypy-boto3-batch-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-batch-1.28.0.tar", last modified: Thu Jul  6 20:59:04 2023, max compression
+gzip compressed data, was "mypy-boto3-batch-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
```

## Comparing `mypy-boto3-batch-1.28.0.tar` & `mypy-boto3-batch-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:04.106232 mypy-boto3-batch-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-06 20:59:04.106232 mypy-boto3-batch-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:04.070232 mypy-boto3-batch-1.28.0/mypy_boto3_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20489 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-06 20:34:14.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44362 2023-07-06 20:34:15.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44305 2023-07-06 20:34:14.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:04.106232 mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-06 20:59:03.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 20:59:03.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:03.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:03.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:03.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 20:59:03.000000 mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:04.106232 mypy-boto3-batch-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:34:13.000000 mypy-boto3-batch-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.140569 mypy-boto3-batch-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-27 05:34:22.132569 mypy-boto3-batch-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17885 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.132569 mypy-boto3-batch-1.28.12/mypy_boto3_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20489 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59854 2023-07-27 05:17:59.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59771 2023-07-27 05:17:58.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.132569 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:22.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.140569 mypy-boto3-batch-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/setup.py
```

### Comparing `mypy-boto3-batch-1.28.0/LICENSE` & `mypy-boto3-batch-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/PKG-INFO` & `mypy-boto3-batch-1.28.12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.0
-Summary: Type annotations for boto3.Batch 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Batch 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-batch"></a>
 
 # mypy-boto3-batch
 
 [![PyPI - mypy-boto3-batch](https://img.shields.io/pypi/v/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-batch?color=blue)](https://pypistats.org/packages/mypy-boto3-batch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,29 +365,42 @@
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
     CancelJobRequestRequestTypeDef,
-    EksConfigurationTypeDef,
-    UpdatePolicyTypeDef,
+    EksConfigurationOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
+    ComputeEnvironmentOrderOutputTypeDef,
     ComputeEnvironmentOrderTypeDef,
+    Ec2ConfigurationOutputTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     Ec2ConfigurationTypeDef,
     LaunchTemplateSpecificationTypeDef,
+    EphemeralStorageOutputTypeDef,
+    FargatePlatformConfigurationOutputTypeDef,
+    KeyValuePairOutputTypeDef,
+    MountPointOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
+    ResourceRequirementOutputTypeDef,
+    RuntimePlatformOutputTypeDef,
+    SecretOutputTypeDef,
+    UlimitOutputTypeDef,
+    KeyValuePairTypeDef,
+    ResourceRequirementTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
-    KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
-    ResourceRequirementTypeDef,
     RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
+    EksConfigurationTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
@@ -395,93 +408,124 @@
     DescribeComputeEnvironmentsRequestRequestTypeDef,
     DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
     DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
+    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
+    EksContainerEnvironmentVariableOutputTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
+    EksContainerSecurityContextOutputTypeDef,
+    EksContainerVolumeMountOutputTypeDef,
     EksContainerEnvironmentVariableTypeDef,
     EksContainerResourceRequirementsTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
+    EksEmptyDirOutputTypeDef,
     EksEmptyDirTypeDef,
+    EksHostPathOutputTypeDef,
     EksHostPathTypeDef,
+    EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
+    EksSecretOutputTypeDef,
     EksSecretTypeDef,
+    EvaluateOnExitOutputTypeDef,
     EvaluateOnExitTypeDef,
+    ShareAttributesOutputTypeDef,
     ShareAttributesTypeDef,
+    HostOutputTypeDef,
     HostTypeDef,
-    JobTimeoutTypeDef,
+    JobTimeoutOutputTypeDef,
+    JobDependencyOutputTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
+    JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
     ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     RegisterJobDefinitionResponseTypeDef,
     ResponseMetadataTypeDef,
     SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdatePolicyTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
-    CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
+    CreateJobQueueRequestRequestTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
+    LogConfigurationOutputTypeDef,
     ContainerOverridesTypeDef,
     LogConfigurationTypeDef,
+    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
-    EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
+    EksContainerOutputTypeDef,
+    EksContainerOverrideTypeDef,
     EksContainerTypeDef,
+    EksVolumeOutputTypeDef,
     EksVolumeTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
+    EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
-    CreateSchedulingPolicyRequestRequestTypeDef,
     SchedulingPolicyDetailTypeDef,
+    CreateSchedulingPolicyRequestRequestTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
+    NodeRangePropertyOutputTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-batch-1.28.0/README.md` & `mypy-boto3-batch-1.28.12/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-batch"></a>
 
 # mypy-boto3-batch
 
 [![PyPI - mypy-boto3-batch](https://img.shields.io/pypi/v/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-batch?color=blue)](https://pypistats.org/packages/mypy-boto3-batch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,42 @@
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
     CancelJobRequestRequestTypeDef,
-    EksConfigurationTypeDef,
-    UpdatePolicyTypeDef,
+    EksConfigurationOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
+    ComputeEnvironmentOrderOutputTypeDef,
     ComputeEnvironmentOrderTypeDef,
+    Ec2ConfigurationOutputTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     Ec2ConfigurationTypeDef,
     LaunchTemplateSpecificationTypeDef,
+    EphemeralStorageOutputTypeDef,
+    FargatePlatformConfigurationOutputTypeDef,
+    KeyValuePairOutputTypeDef,
+    MountPointOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
+    ResourceRequirementOutputTypeDef,
+    RuntimePlatformOutputTypeDef,
+    SecretOutputTypeDef,
+    UlimitOutputTypeDef,
+    KeyValuePairTypeDef,
+    ResourceRequirementTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
-    KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
-    ResourceRequirementTypeDef,
     RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
+    EksConfigurationTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
@@ -363,93 +376,124 @@
     DescribeComputeEnvironmentsRequestRequestTypeDef,
     DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
     DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
+    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
+    EksContainerEnvironmentVariableOutputTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
+    EksContainerSecurityContextOutputTypeDef,
+    EksContainerVolumeMountOutputTypeDef,
     EksContainerEnvironmentVariableTypeDef,
     EksContainerResourceRequirementsTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
+    EksEmptyDirOutputTypeDef,
     EksEmptyDirTypeDef,
+    EksHostPathOutputTypeDef,
     EksHostPathTypeDef,
+    EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
+    EksSecretOutputTypeDef,
     EksSecretTypeDef,
+    EvaluateOnExitOutputTypeDef,
     EvaluateOnExitTypeDef,
+    ShareAttributesOutputTypeDef,
     ShareAttributesTypeDef,
+    HostOutputTypeDef,
     HostTypeDef,
-    JobTimeoutTypeDef,
+    JobTimeoutOutputTypeDef,
+    JobDependencyOutputTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
+    JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
     ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     RegisterJobDefinitionResponseTypeDef,
     ResponseMetadataTypeDef,
     SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdatePolicyTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
-    CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
+    CreateJobQueueRequestRequestTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
+    LogConfigurationOutputTypeDef,
     ContainerOverridesTypeDef,
     LogConfigurationTypeDef,
+    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
-    EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
+    EksContainerOutputTypeDef,
+    EksContainerOverrideTypeDef,
     EksContainerTypeDef,
+    EksVolumeOutputTypeDef,
     EksVolumeTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
+    EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
-    CreateSchedulingPolicyRequestRequestTypeDef,
     SchedulingPolicyDetailTypeDef,
+    CreateSchedulingPolicyRequestRequestTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
+    NodeRangePropertyOutputTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/__init__.py` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/__init__.pyi` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/__main__.py` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Batch 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Batch 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/client.py` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/client.pyi` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/literals.py` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.pyi`

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
     "ArrayJobDependencyType",
     "AssignPublicIpType",
     "CEStateType",
     "CEStatusType",
     "CETypeType",
     "CRAllocationStrategyType",
@@ -48,15 +47,14 @@
     "BatchServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ArrayJobDependencyType = Literal["N_TO_N", "SEQUENTIAL"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CEStateType = Literal["DISABLED", "ENABLED"]
 CEStatusType = Literal["CREATING", "DELETED", "DELETING", "INVALID", "UPDATING", "VALID"]
 CETypeType = Literal["MANAGED", "UNMANAGED"]
 CRAllocationStrategyType = Literal["BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
 CRTypeType = Literal["EC2", "FARGATE", "FARGATE_SPOT", "SPOT"]
@@ -196,14 +194,15 @@
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
@@ -282,26 +281,28 @@
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

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/literals.pyi` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.py`

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
     "ArrayJobDependencyType",
     "AssignPublicIpType",
     "CEStateType",
     "CEStatusType",
     "CETypeType",
     "CRAllocationStrategyType",
@@ -47,14 +48,15 @@
     "BatchServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ArrayJobDependencyType = Literal["N_TO_N", "SEQUENTIAL"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CEStateType = Literal["DISABLED", "ENABLED"]
 CEStatusType = Literal["CREATING", "DELETED", "DELETING", "INVALID", "UPDATING", "VALID"]
 CETypeType = Literal["MANAGED", "UNMANAGED"]
 CRAllocationStrategyType = Literal["BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
 CRTypeType = Literal["EC2", "FARGATE", "FARGATE_SPOT", "SPOT"]
@@ -194,14 +196,15 @@
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
@@ -280,26 +283,28 @@
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

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/paginator.py` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/paginator.pyi` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch/type_defs.pyi` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch/type_defs.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -44,29 +44,42 @@
 
 __all__ = (
     "ArrayPropertiesDetailTypeDef",
     "ArrayPropertiesSummaryTypeDef",
     "ArrayPropertiesTypeDef",
     "NetworkInterfaceTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "EksConfigurationTypeDef",
-    "UpdatePolicyTypeDef",
+    "EksConfigurationOutputTypeDef",
+    "UpdatePolicyOutputTypeDef",
+    "ComputeEnvironmentOrderOutputTypeDef",
     "ComputeEnvironmentOrderTypeDef",
+    "Ec2ConfigurationOutputTypeDef",
+    "LaunchTemplateSpecificationOutputTypeDef",
     "Ec2ConfigurationTypeDef",
     "LaunchTemplateSpecificationTypeDef",
+    "EphemeralStorageOutputTypeDef",
+    "FargatePlatformConfigurationOutputTypeDef",
+    "KeyValuePairOutputTypeDef",
+    "MountPointOutputTypeDef",
+    "NetworkConfigurationOutputTypeDef",
+    "ResourceRequirementOutputTypeDef",
+    "RuntimePlatformOutputTypeDef",
+    "SecretOutputTypeDef",
+    "UlimitOutputTypeDef",
+    "KeyValuePairTypeDef",
+    "ResourceRequirementTypeDef",
     "EphemeralStorageTypeDef",
     "FargatePlatformConfigurationTypeDef",
-    "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
-    "ResourceRequirementTypeDef",
     "RuntimePlatformTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
+    "EksConfigurationTypeDef",
     "CreateComputeEnvironmentResponseTypeDef",
     "CreateJobQueueResponseTypeDef",
     "CreateSchedulingPolicyResponseTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
     "DeregisterJobDefinitionRequestRequestTypeDef",
@@ -74,93 +87,124 @@
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
     "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
+    "DeviceOutputTypeDef",
     "DeviceTypeDef",
+    "EFSAuthorizationConfigOutputTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
+    "EksContainerEnvironmentVariableOutputTypeDef",
+    "EksContainerResourceRequirementsOutputTypeDef",
+    "EksContainerSecurityContextOutputTypeDef",
+    "EksContainerVolumeMountOutputTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
     "EksContainerResourceRequirementsTypeDef",
     "EksContainerSecurityContextTypeDef",
     "EksContainerVolumeMountTypeDef",
+    "EksEmptyDirOutputTypeDef",
     "EksEmptyDirTypeDef",
+    "EksHostPathOutputTypeDef",
     "EksHostPathTypeDef",
+    "EksMetadataOutputTypeDef",
     "EksMetadataTypeDef",
+    "EksSecretOutputTypeDef",
     "EksSecretTypeDef",
+    "EvaluateOnExitOutputTypeDef",
     "EvaluateOnExitTypeDef",
+    "ShareAttributesOutputTypeDef",
     "ShareAttributesTypeDef",
+    "HostOutputTypeDef",
     "HostTypeDef",
-    "JobTimeoutTypeDef",
+    "JobTimeoutOutputTypeDef",
+    "JobDependencyOutputTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
+    "JobTimeoutTypeDef",
     "KeyValuesPairTypeDef",
+    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
     "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "RegisterJobDefinitionResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SubmitJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdatePolicyTypeDef",
     "UpdateComputeEnvironmentResponseTypeDef",
     "UpdateJobQueueResponseTypeDef",
     "AttemptContainerDetailTypeDef",
-    "CreateJobQueueRequestRequestTypeDef",
     "JobQueueDetailTypeDef",
+    "CreateJobQueueRequestRequestTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
+    "ComputeResourceOutputTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
+    "LogConfigurationOutputTypeDef",
     "ContainerOverridesTypeDef",
     "LogConfigurationTypeDef",
+    "EFSVolumeConfigurationOutputTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
-    "EksContainerOverrideTypeDef",
     "EksContainerDetailTypeDef",
+    "EksContainerOutputTypeDef",
+    "EksContainerOverrideTypeDef",
     "EksContainerTypeDef",
+    "EksVolumeOutputTypeDef",
     "EksVolumeTypeDef",
+    "RetryStrategyOutputTypeDef",
     "RetryStrategyTypeDef",
+    "FairsharePolicyOutputTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
+    "VolumeOutputTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
+    "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
-    "CreateSchedulingPolicyRequestRequestTypeDef",
     "SchedulingPolicyDetailTypeDef",
+    "CreateSchedulingPolicyRequestRequestTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "NodeOverridesTypeDef",
     "ContainerDetailTypeDef",
+    "ContainerPropertiesOutputTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
+    "EksPropertiesOutputTypeDef",
     "EksPropertiesTypeDef",
     "DescribeSchedulingPoliciesResponseTypeDef",
+    "NodeRangePropertyOutputTypeDef",
     "NodeRangePropertyTypeDef",
     "SubmitJobRequestRequestTypeDef",
+    "NodePropertiesOutputTypeDef",
     "NodePropertiesTypeDef",
     "JobDefinitionTypeDef",
     "JobDetailTypeDef",
     "RegisterJobDefinitionRequestRequestTypeDef",
     "DescribeJobDefinitionsResponseTypeDef",
     "DescribeJobsResponseTypeDef",
 )
@@ -206,39 +250,77 @@
     "CancelJobRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
 
-EksConfigurationTypeDef = TypedDict(
-    "EksConfigurationTypeDef",
+EksConfigurationOutputTypeDef = TypedDict(
+    "EksConfigurationOutputTypeDef",
     {
         "eksClusterArn": str,
         "kubernetesNamespace": str,
     },
 )
 
-UpdatePolicyTypeDef = TypedDict(
-    "UpdatePolicyTypeDef",
+UpdatePolicyOutputTypeDef = TypedDict(
+    "UpdatePolicyOutputTypeDef",
     {
         "terminateJobsOnUpdate": bool,
         "jobExecutionTimeoutMinutes": int,
     },
     total=False,
 )
 
+ComputeEnvironmentOrderOutputTypeDef = TypedDict(
+    "ComputeEnvironmentOrderOutputTypeDef",
+    {
+        "order": int,
+        "computeEnvironment": str,
+    },
+)
+
 ComputeEnvironmentOrderTypeDef = TypedDict(
     "ComputeEnvironmentOrderTypeDef",
     {
         "order": int,
         "computeEnvironment": str,
     },
 )
 
+_RequiredEc2ConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEc2ConfigurationOutputTypeDef",
+    {
+        "imageType": str,
+    },
+)
+_OptionalEc2ConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEc2ConfigurationOutputTypeDef",
+    {
+        "imageIdOverride": str,
+        "imageKubernetesVersion": str,
+    },
+    total=False,
+)
+
+class Ec2ConfigurationOutputTypeDef(
+    _RequiredEc2ConfigurationOutputTypeDef, _OptionalEc2ConfigurationOutputTypeDef
+):
+    pass
+
+LaunchTemplateSpecificationOutputTypeDef = TypedDict(
+    "LaunchTemplateSpecificationOutputTypeDef",
+    {
+        "launchTemplateId": str,
+        "launchTemplateName": str,
+        "version": str,
+    },
+    total=False,
+)
+
 _RequiredEc2ConfigurationTypeDef = TypedDict(
     "_RequiredEc2ConfigurationTypeDef",
     {
         "imageType": str,
     },
 )
 _OptionalEc2ConfigurationTypeDef = TypedDict(
@@ -259,64 +341,140 @@
         "launchTemplateId": str,
         "launchTemplateName": str,
         "version": str,
     },
     total=False,
 )
 
-EphemeralStorageTypeDef = TypedDict(
-    "EphemeralStorageTypeDef",
+EphemeralStorageOutputTypeDef = TypedDict(
+    "EphemeralStorageOutputTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
-FargatePlatformConfigurationTypeDef = TypedDict(
-    "FargatePlatformConfigurationTypeDef",
+FargatePlatformConfigurationOutputTypeDef = TypedDict(
+    "FargatePlatformConfigurationOutputTypeDef",
     {
         "platformVersion": str,
     },
     total=False,
 )
 
-KeyValuePairTypeDef = TypedDict(
-    "KeyValuePairTypeDef",
+KeyValuePairOutputTypeDef = TypedDict(
+    "KeyValuePairOutputTypeDef",
     {
         "name": str,
         "value": str,
     },
     total=False,
 )
 
-MountPointTypeDef = TypedDict(
-    "MountPointTypeDef",
+MountPointOutputTypeDef = TypedDict(
+    "MountPointOutputTypeDef",
     {
         "containerPath": str,
         "readOnly": bool,
         "sourceVolume": str,
     },
     total=False,
 )
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
     {
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
+ResourceRequirementOutputTypeDef = TypedDict(
+    "ResourceRequirementOutputTypeDef",
+    {
+        "value": str,
+        "type": ResourceTypeType,
+    },
+)
+
+RuntimePlatformOutputTypeDef = TypedDict(
+    "RuntimePlatformOutputTypeDef",
+    {
+        "operatingSystemFamily": str,
+        "cpuArchitecture": str,
+    },
+    total=False,
+)
+
+SecretOutputTypeDef = TypedDict(
+    "SecretOutputTypeDef",
+    {
+        "name": str,
+        "valueFrom": str,
+    },
+)
+
+UlimitOutputTypeDef = TypedDict(
+    "UlimitOutputTypeDef",
+    {
+        "hardLimit": int,
+        "name": str,
+        "softLimit": int,
+    },
+)
+
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
+    {
+        "name": str,
+        "value": str,
+    },
+    total=False,
+)
+
 ResourceRequirementTypeDef = TypedDict(
     "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
+EphemeralStorageTypeDef = TypedDict(
+    "EphemeralStorageTypeDef",
+    {
+        "sizeInGiB": int,
+    },
+)
+
+FargatePlatformConfigurationTypeDef = TypedDict(
+    "FargatePlatformConfigurationTypeDef",
+    {
+        "platformVersion": str,
+    },
+    total=False,
+)
+
+MountPointTypeDef = TypedDict(
+    "MountPointTypeDef",
+    {
+        "containerPath": str,
+        "readOnly": bool,
+        "sourceVolume": str,
+    },
+    total=False,
+)
+
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
+    {
+        "assignPublicIp": AssignPublicIpType,
+    },
+    total=False,
+)
+
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "operatingSystemFamily": str,
         "cpuArchitecture": str,
     },
     total=False,
@@ -344,14 +502,22 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
+EksConfigurationTypeDef = TypedDict(
+    "EksConfigurationTypeDef",
+    {
+        "eksClusterArn": str,
+        "kubernetesNamespace": str,
+    },
+)
+
 CreateComputeEnvironmentResponseTypeDef = TypedDict(
     "CreateComputeEnvironmentResponseTypeDef",
     {
         "computeEnvironmentName": str,
         "computeEnvironmentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -474,32 +640,59 @@
 DescribeSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
 
+_RequiredDeviceOutputTypeDef = TypedDict(
+    "_RequiredDeviceOutputTypeDef",
+    {
+        "hostPath": str,
+    },
+)
+_OptionalDeviceOutputTypeDef = TypedDict(
+    "_OptionalDeviceOutputTypeDef",
+    {
+        "containerPath": str,
+        "permissions": List[DeviceCgroupPermissionType],
+    },
+    total=False,
+)
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
     "_OptionalDeviceTypeDef",
     {
         "containerPath": str,
-        "permissions": List[DeviceCgroupPermissionType],
+        "permissions": Sequence[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
+EFSAuthorizationConfigOutputTypeDef = TypedDict(
+    "EFSAuthorizationConfigOutputTypeDef",
+    {
+        "accessPointId": str,
+        "iam": EFSAuthorizationConfigIAMType,
+    },
+    total=False,
+)
+
 EFSAuthorizationConfigTypeDef = TypedDict(
     "EFSAuthorizationConfigTypeDef",
     {
         "accessPointId": str,
         "iam": EFSAuthorizationConfigIAMType,
     },
     total=False,
@@ -510,14 +703,65 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
+_RequiredEksContainerEnvironmentVariableOutputTypeDef = TypedDict(
+    "_RequiredEksContainerEnvironmentVariableOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalEksContainerEnvironmentVariableOutputTypeDef = TypedDict(
+    "_OptionalEksContainerEnvironmentVariableOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class EksContainerEnvironmentVariableOutputTypeDef(
+    _RequiredEksContainerEnvironmentVariableOutputTypeDef,
+    _OptionalEksContainerEnvironmentVariableOutputTypeDef,
+):
+    pass
+
+EksContainerResourceRequirementsOutputTypeDef = TypedDict(
+    "EksContainerResourceRequirementsOutputTypeDef",
+    {
+        "limits": Dict[str, str],
+        "requests": Dict[str, str],
+    },
+    total=False,
+)
+
+EksContainerSecurityContextOutputTypeDef = TypedDict(
+    "EksContainerSecurityContextOutputTypeDef",
+    {
+        "runAsUser": int,
+        "runAsGroup": int,
+        "privileged": bool,
+        "readOnlyRootFilesystem": bool,
+        "runAsNonRoot": bool,
+    },
+    total=False,
+)
+
+EksContainerVolumeMountOutputTypeDef = TypedDict(
+    "EksContainerVolumeMountOutputTypeDef",
+    {
+        "name": str,
+        "mountPath": str,
+        "readOnly": bool,
+    },
+    total=False,
+)
+
 _RequiredEksContainerEnvironmentVariableTypeDef = TypedDict(
     "_RequiredEksContainerEnvironmentVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalEksContainerEnvironmentVariableTypeDef = TypedDict(
@@ -532,16 +776,16 @@
     _RequiredEksContainerEnvironmentVariableTypeDef, _OptionalEksContainerEnvironmentVariableTypeDef
 ):
     pass
 
 EksContainerResourceRequirementsTypeDef = TypedDict(
     "EksContainerResourceRequirementsTypeDef",
     {
-        "limits": Dict[str, str],
-        "requests": Dict[str, str],
+        "limits": Mapping[str, str],
+        "requests": Mapping[str, str],
     },
     total=False,
 )
 
 EksContainerSecurityContextTypeDef = TypedDict(
     "EksContainerSecurityContextTypeDef",
     {
@@ -560,39 +804,81 @@
         "name": str,
         "mountPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
+EksEmptyDirOutputTypeDef = TypedDict(
+    "EksEmptyDirOutputTypeDef",
+    {
+        "medium": str,
+        "sizeLimit": str,
+    },
+    total=False,
+)
+
 EksEmptyDirTypeDef = TypedDict(
     "EksEmptyDirTypeDef",
     {
         "medium": str,
         "sizeLimit": str,
     },
     total=False,
 )
 
+EksHostPathOutputTypeDef = TypedDict(
+    "EksHostPathOutputTypeDef",
+    {
+        "path": str,
+    },
+    total=False,
+)
+
 EksHostPathTypeDef = TypedDict(
     "EksHostPathTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
+EksMetadataOutputTypeDef = TypedDict(
+    "EksMetadataOutputTypeDef",
+    {
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
 EksMetadataTypeDef = TypedDict(
     "EksMetadataTypeDef",
     {
-        "labels": Dict[str, str],
+        "labels": Mapping[str, str],
     },
     total=False,
 )
 
+_RequiredEksSecretOutputTypeDef = TypedDict(
+    "_RequiredEksSecretOutputTypeDef",
+    {
+        "secretName": str,
+    },
+)
+_OptionalEksSecretOutputTypeDef = TypedDict(
+    "_OptionalEksSecretOutputTypeDef",
+    {
+        "optional": bool,
+    },
+    total=False,
+)
+
+class EksSecretOutputTypeDef(_RequiredEksSecretOutputTypeDef, _OptionalEksSecretOutputTypeDef):
+    pass
+
 _RequiredEksSecretTypeDef = TypedDict(
     "_RequiredEksSecretTypeDef",
     {
         "secretName": str,
     },
 )
 _OptionalEksSecretTypeDef = TypedDict(
@@ -602,14 +888,35 @@
     },
     total=False,
 )
 
 class EksSecretTypeDef(_RequiredEksSecretTypeDef, _OptionalEksSecretTypeDef):
     pass
 
+_RequiredEvaluateOnExitOutputTypeDef = TypedDict(
+    "_RequiredEvaluateOnExitOutputTypeDef",
+    {
+        "action": RetryActionType,
+    },
+)
+_OptionalEvaluateOnExitOutputTypeDef = TypedDict(
+    "_OptionalEvaluateOnExitOutputTypeDef",
+    {
+        "onStatusReason": str,
+        "onReason": str,
+        "onExitCode": str,
+    },
+    total=False,
+)
+
+class EvaluateOnExitOutputTypeDef(
+    _RequiredEvaluateOnExitOutputTypeDef, _OptionalEvaluateOnExitOutputTypeDef
+):
+    pass
+
 _RequiredEvaluateOnExitTypeDef = TypedDict(
     "_RequiredEvaluateOnExitTypeDef",
     {
         "action": RetryActionType,
     },
 )
 _OptionalEvaluateOnExitTypeDef = TypedDict(
@@ -621,14 +928,33 @@
     },
     total=False,
 )
 
 class EvaluateOnExitTypeDef(_RequiredEvaluateOnExitTypeDef, _OptionalEvaluateOnExitTypeDef):
     pass
 
+_RequiredShareAttributesOutputTypeDef = TypedDict(
+    "_RequiredShareAttributesOutputTypeDef",
+    {
+        "shareIdentifier": str,
+    },
+)
+_OptionalShareAttributesOutputTypeDef = TypedDict(
+    "_OptionalShareAttributesOutputTypeDef",
+    {
+        "weightFactor": float,
+    },
+    total=False,
+)
+
+class ShareAttributesOutputTypeDef(
+    _RequiredShareAttributesOutputTypeDef, _OptionalShareAttributesOutputTypeDef
+):
+    pass
+
 _RequiredShareAttributesTypeDef = TypedDict(
     "_RequiredShareAttributesTypeDef",
     {
         "shareIdentifier": str,
     },
 )
 _OptionalShareAttributesTypeDef = TypedDict(
@@ -638,30 +964,47 @@
     },
     total=False,
 )
 
 class ShareAttributesTypeDef(_RequiredShareAttributesTypeDef, _OptionalShareAttributesTypeDef):
     pass
 
+HostOutputTypeDef = TypedDict(
+    "HostOutputTypeDef",
+    {
+        "sourcePath": str,
+    },
+    total=False,
+)
+
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "sourcePath": str,
     },
     total=False,
 )
 
-JobTimeoutTypeDef = TypedDict(
-    "JobTimeoutTypeDef",
+JobTimeoutOutputTypeDef = TypedDict(
+    "JobTimeoutOutputTypeDef",
     {
         "attemptDurationSeconds": int,
     },
     total=False,
 )
 
+JobDependencyOutputTypeDef = TypedDict(
+    "JobDependencyOutputTypeDef",
+    {
+        "jobId": str,
+        "type": ArrayJobDependencyType,
+    },
+    total=False,
+)
+
 JobDependencyTypeDef = TypedDict(
     "JobDependencyTypeDef",
     {
         "jobId": str,
         "type": ArrayJobDependencyType,
     },
     total=False,
@@ -682,34 +1025,60 @@
         "isMainNode": bool,
         "numNodes": int,
         "nodeIndex": int,
     },
     total=False,
 )
 
+JobTimeoutTypeDef = TypedDict(
+    "JobTimeoutTypeDef",
+    {
+        "attemptDurationSeconds": int,
+    },
+    total=False,
+)
+
 KeyValuesPairTypeDef = TypedDict(
     "KeyValuesPairTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
+_RequiredTmpfsOutputTypeDef = TypedDict(
+    "_RequiredTmpfsOutputTypeDef",
+    {
+        "containerPath": str,
+        "size": int,
+    },
+)
+_OptionalTmpfsOutputTypeDef = TypedDict(
+    "_OptionalTmpfsOutputTypeDef",
+    {
+        "mountOptions": List[str],
+    },
+    total=False,
+)
+
+class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
+    pass
+
 _RequiredTmpfsTypeDef = TypedDict(
     "_RequiredTmpfsTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
 _OptionalTmpfsTypeDef = TypedDict(
     "_OptionalTmpfsTypeDef",
     {
-        "mountOptions": List[str],
+        "mountOptions": Sequence[str],
     },
     total=False,
 )
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
@@ -813,14 +1182,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdatePolicyTypeDef = TypedDict(
+    "UpdatePolicyTypeDef",
+    {
+        "terminateJobsOnUpdate": bool,
+        "jobExecutionTimeoutMinutes": int,
+    },
+    total=False,
+)
+
 UpdateComputeEnvironmentResponseTypeDef = TypedDict(
     "UpdateComputeEnvironmentResponseTypeDef",
     {
         "computeEnvironmentName": str,
         "computeEnvironmentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -844,59 +1222,59 @@
         "reason": str,
         "logStreamName": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateJobQueueRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobQueueRequestRequestTypeDef",
+_RequiredJobQueueDetailTypeDef = TypedDict(
+    "_RequiredJobQueueDetailTypeDef",
     {
         "jobQueueName": str,
+        "jobQueueArn": str,
+        "state": JQStateType,
         "priority": int,
-        "computeEnvironmentOrder": Sequence[ComputeEnvironmentOrderTypeDef],
+        "computeEnvironmentOrder": List[ComputeEnvironmentOrderOutputTypeDef],
     },
 )
-_OptionalCreateJobQueueRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobQueueRequestRequestTypeDef",
+_OptionalJobQueueDetailTypeDef = TypedDict(
+    "_OptionalJobQueueDetailTypeDef",
     {
-        "state": JQStateType,
         "schedulingPolicyArn": str,
-        "tags": Mapping[str, str],
+        "status": JQStatusType,
+        "statusReason": str,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateJobQueueRequestRequestTypeDef(
-    _RequiredCreateJobQueueRequestRequestTypeDef, _OptionalCreateJobQueueRequestRequestTypeDef
-):
+class JobQueueDetailTypeDef(_RequiredJobQueueDetailTypeDef, _OptionalJobQueueDetailTypeDef):
     pass
 
-_RequiredJobQueueDetailTypeDef = TypedDict(
-    "_RequiredJobQueueDetailTypeDef",
+_RequiredCreateJobQueueRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobQueueRequestRequestTypeDef",
     {
         "jobQueueName": str,
-        "jobQueueArn": str,
-        "state": JQStateType,
         "priority": int,
-        "computeEnvironmentOrder": List[ComputeEnvironmentOrderTypeDef],
+        "computeEnvironmentOrder": Sequence[ComputeEnvironmentOrderTypeDef],
     },
 )
-_OptionalJobQueueDetailTypeDef = TypedDict(
-    "_OptionalJobQueueDetailTypeDef",
+_OptionalCreateJobQueueRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobQueueRequestRequestTypeDef",
     {
+        "state": JQStateType,
         "schedulingPolicyArn": str,
-        "status": JQStatusType,
-        "statusReason": str,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class JobQueueDetailTypeDef(_RequiredJobQueueDetailTypeDef, _OptionalJobQueueDetailTypeDef):
+class CreateJobQueueRequestRequestTypeDef(
+    _RequiredCreateJobQueueRequestRequestTypeDef, _OptionalCreateJobQueueRequestRequestTypeDef
+):
     pass
 
 _RequiredUpdateJobQueueRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobQueueRequestRequestTypeDef",
     {
         "jobQueue": str,
     },
@@ -913,14 +1291,48 @@
 )
 
 class UpdateJobQueueRequestRequestTypeDef(
     _RequiredUpdateJobQueueRequestRequestTypeDef, _OptionalUpdateJobQueueRequestRequestTypeDef
 ):
     pass
 
+_RequiredComputeResourceOutputTypeDef = TypedDict(
+    "_RequiredComputeResourceOutputTypeDef",
+    {
+        "type": CRTypeType,
+        "maxvCpus": int,
+        "subnets": List[str],
+    },
+)
+_OptionalComputeResourceOutputTypeDef = TypedDict(
+    "_OptionalComputeResourceOutputTypeDef",
+    {
+        "allocationStrategy": CRAllocationStrategyType,
+        "minvCpus": int,
+        "desiredvCpus": int,
+        "instanceTypes": List[str],
+        "imageId": str,
+        "securityGroupIds": List[str],
+        "ec2KeyPair": str,
+        "instanceRole": str,
+        "tags": Dict[str, str],
+        "placementGroup": str,
+        "bidPercentage": int,
+        "spotIamFleetRole": str,
+        "launchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "ec2Configuration": List[Ec2ConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+class ComputeResourceOutputTypeDef(
+    _RequiredComputeResourceOutputTypeDef, _OptionalComputeResourceOutputTypeDef
+):
+    pass
+
 _RequiredComputeResourceTypeDef = TypedDict(
     "_RequiredComputeResourceTypeDef",
     {
         "type": CRTypeType,
         "maxvCpus": int,
         "subnets": Sequence[str],
     },
@@ -969,14 +1381,34 @@
         "updateToLatestImageVersion": bool,
         "type": CRTypeType,
         "imageId": str,
     },
     total=False,
 )
 
+_RequiredLogConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLogConfigurationOutputTypeDef",
+    {
+        "logDriver": LogDriverType,
+    },
+)
+_OptionalLogConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLogConfigurationOutputTypeDef",
+    {
+        "options": Dict[str, str],
+        "secretOptions": List[SecretOutputTypeDef],
+    },
+    total=False,
+)
+
+class LogConfigurationOutputTypeDef(
+    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
+):
+    pass
+
 ContainerOverridesTypeDef = TypedDict(
     "ContainerOverridesTypeDef",
     {
         "vcpus": int,
         "memory": int,
         "command": Sequence[str],
         "instanceType": str,
@@ -991,23 +1423,45 @@
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
     "_OptionalLogConfigurationTypeDef",
     {
-        "options": Dict[str, str],
-        "secretOptions": List[SecretTypeDef],
+        "options": Mapping[str, str],
+        "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
+_RequiredEFSVolumeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEFSVolumeConfigurationOutputTypeDef",
+    {
+        "fileSystemId": str,
+    },
+)
+_OptionalEFSVolumeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEFSVolumeConfigurationOutputTypeDef",
+    {
+        "rootDirectory": str,
+        "transitEncryption": EFSTransitEncryptionType,
+        "transitEncryptionPort": int,
+        "authorizationConfig": EFSAuthorizationConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class EFSVolumeConfigurationOutputTypeDef(
+    _RequiredEFSVolumeConfigurationOutputTypeDef, _OptionalEFSVolumeConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -1035,40 +1489,66 @@
         "startedAt": int,
         "stoppedAt": int,
         "statusReason": str,
     },
     total=False,
 )
 
-EksContainerOverrideTypeDef = TypedDict(
-    "EksContainerOverrideTypeDef",
+EksContainerDetailTypeDef = TypedDict(
+    "EksContainerDetailTypeDef",
     {
+        "name": str,
         "image": str,
-        "command": Sequence[str],
-        "args": Sequence[str],
-        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsTypeDef,
+        "imagePullPolicy": str,
+        "command": List[str],
+        "args": List[str],
+        "env": List[EksContainerEnvironmentVariableOutputTypeDef],
+        "resources": EksContainerResourceRequirementsOutputTypeDef,
+        "exitCode": int,
+        "reason": str,
+        "volumeMounts": List[EksContainerVolumeMountOutputTypeDef],
+        "securityContext": EksContainerSecurityContextOutputTypeDef,
     },
     total=False,
 )
 
-EksContainerDetailTypeDef = TypedDict(
-    "EksContainerDetailTypeDef",
+_RequiredEksContainerOutputTypeDef = TypedDict(
+    "_RequiredEksContainerOutputTypeDef",
     {
-        "name": str,
         "image": str,
+    },
+)
+_OptionalEksContainerOutputTypeDef = TypedDict(
+    "_OptionalEksContainerOutputTypeDef",
+    {
+        "name": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
-        "env": List[EksContainerEnvironmentVariableTypeDef],
+        "env": List[EksContainerEnvironmentVariableOutputTypeDef],
+        "resources": EksContainerResourceRequirementsOutputTypeDef,
+        "volumeMounts": List[EksContainerVolumeMountOutputTypeDef],
+        "securityContext": EksContainerSecurityContextOutputTypeDef,
+    },
+    total=False,
+)
+
+class EksContainerOutputTypeDef(
+    _RequiredEksContainerOutputTypeDef, _OptionalEksContainerOutputTypeDef
+):
+    pass
+
+EksContainerOverrideTypeDef = TypedDict(
+    "EksContainerOverrideTypeDef",
+    {
+        "image": str,
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsTypeDef,
-        "exitCode": int,
-        "reason": str,
-        "volumeMounts": List[EksContainerVolumeMountTypeDef],
-        "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 _RequiredEksContainerTypeDef = TypedDict(
     "_RequiredEksContainerTypeDef",
     {
@@ -1076,27 +1556,46 @@
     },
 )
 _OptionalEksContainerTypeDef = TypedDict(
     "_OptionalEksContainerTypeDef",
     {
         "name": str,
         "imagePullPolicy": str,
-        "command": List[str],
-        "args": List[str],
-        "env": List[EksContainerEnvironmentVariableTypeDef],
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsTypeDef,
-        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "volumeMounts": Sequence[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 class EksContainerTypeDef(_RequiredEksContainerTypeDef, _OptionalEksContainerTypeDef):
     pass
 
+_RequiredEksVolumeOutputTypeDef = TypedDict(
+    "_RequiredEksVolumeOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalEksVolumeOutputTypeDef = TypedDict(
+    "_OptionalEksVolumeOutputTypeDef",
+    {
+        "hostPath": EksHostPathOutputTypeDef,
+        "emptyDir": EksEmptyDirOutputTypeDef,
+        "secret": EksSecretOutputTypeDef,
+    },
+    total=False,
+)
+
+class EksVolumeOutputTypeDef(_RequiredEksVolumeOutputTypeDef, _OptionalEksVolumeOutputTypeDef):
+    pass
+
 _RequiredEksVolumeTypeDef = TypedDict(
     "_RequiredEksVolumeTypeDef",
     {
         "name": str,
     },
 )
 _OptionalEksVolumeTypeDef = TypedDict(
@@ -1108,19 +1607,38 @@
     },
     total=False,
 )
 
 class EksVolumeTypeDef(_RequiredEksVolumeTypeDef, _OptionalEksVolumeTypeDef):
     pass
 
+RetryStrategyOutputTypeDef = TypedDict(
+    "RetryStrategyOutputTypeDef",
+    {
+        "attempts": int,
+        "evaluateOnExit": List[EvaluateOnExitOutputTypeDef],
+    },
+    total=False,
+)
+
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "attempts": int,
-        "evaluateOnExit": List[EvaluateOnExitTypeDef],
+        "evaluateOnExit": Sequence[EvaluateOnExitTypeDef],
+    },
+    total=False,
+)
+
+FairsharePolicyOutputTypeDef = TypedDict(
+    "FairsharePolicyOutputTypeDef",
+    {
+        "shareDecaySeconds": int,
+        "computeReservation": int,
+        "shareDistribution": List[ShareAttributesOutputTypeDef],
     },
     total=False,
 )
 
 FairsharePolicyTypeDef = TypedDict(
     "FairsharePolicyTypeDef",
     {
@@ -1181,21 +1699,34 @@
         "maxResults": int,
         "nextToken": str,
         "filters": Sequence[KeyValuesPairTypeDef],
     },
     total=False,
 )
 
+LinuxParametersOutputTypeDef = TypedDict(
+    "LinuxParametersOutputTypeDef",
+    {
+        "devices": List[DeviceOutputTypeDef],
+        "initProcessEnabled": bool,
+        "sharedMemorySize": int,
+        "tmpfs": List[TmpfsOutputTypeDef],
+        "maxSwap": int,
+        "swappiness": int,
+    },
+    total=False,
+)
+
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
-        "devices": List[DeviceTypeDef],
+        "devices": Sequence[DeviceTypeDef],
         "initProcessEnabled": bool,
         "sharedMemorySize": int,
-        "tmpfs": List[TmpfsTypeDef],
+        "tmpfs": Sequence[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
@@ -1240,18 +1771,18 @@
         "unmanagedvCpus": int,
         "ecsClusterArn": str,
         "tags": Dict[str, str],
         "type": CETypeType,
         "state": CEStateType,
         "status": CEStatusType,
         "statusReason": str,
-        "computeResources": ComputeResourceTypeDef,
+        "computeResources": ComputeResourceOutputTypeDef,
         "serviceRole": str,
-        "updatePolicy": UpdatePolicyTypeDef,
-        "eksConfiguration": EksConfigurationTypeDef,
+        "updatePolicy": UpdatePolicyOutputTypeDef,
+        "eksConfiguration": EksConfigurationOutputTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
         "uuid": str,
     },
     total=False,
 )
 
 class ComputeEnvironmentDetailTypeDef(
@@ -1324,14 +1855,24 @@
 )
 
 class NodePropertyOverrideTypeDef(
     _RequiredNodePropertyOverrideTypeDef, _OptionalNodePropertyOverrideTypeDef
 ):
     pass
 
+VolumeOutputTypeDef = TypedDict(
+    "VolumeOutputTypeDef",
+    {
+        "host": HostOutputTypeDef,
+        "name": str,
+        "efsVolumeConfiguration": EFSVolumeConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "host": HostTypeDef,
         "name": str,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
     },
@@ -1350,74 +1891,87 @@
 EksPodPropertiesDetailTypeDef = TypedDict(
     "EksPodPropertiesDetailTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
-        "volumes": List[EksVolumeTypeDef],
+        "volumes": List[EksVolumeOutputTypeDef],
         "podName": str,
         "nodeName": str,
-        "metadata": EksMetadataTypeDef,
+        "metadata": EksMetadataOutputTypeDef,
+    },
+    total=False,
+)
+
+EksPodPropertiesOutputTypeDef = TypedDict(
+    "EksPodPropertiesOutputTypeDef",
+    {
+        "serviceAccountName": str,
+        "hostNetwork": bool,
+        "dnsPolicy": str,
+        "containers": List[EksContainerOutputTypeDef],
+        "volumes": List[EksVolumeOutputTypeDef],
+        "metadata": EksMetadataOutputTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
-        "containers": List[EksContainerTypeDef],
-        "volumes": List[EksVolumeTypeDef],
+        "containers": Sequence[EksContainerTypeDef],
+        "volumes": Sequence[EksVolumeTypeDef],
         "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
+_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
+    "_RequiredSchedulingPolicyDetailTypeDef",
     {
         "name": str,
+        "arn": str,
     },
 )
-_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
+_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
+    "_OptionalSchedulingPolicyDetailTypeDef",
     {
-        "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Mapping[str, str],
+        "fairsharePolicy": FairsharePolicyOutputTypeDef,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateSchedulingPolicyRequestRequestTypeDef(
-    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
-    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
+class SchedulingPolicyDetailTypeDef(
+    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
 ):
     pass
 
-_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
-    "_RequiredSchedulingPolicyDetailTypeDef",
+_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "name": str,
-        "arn": str,
     },
 )
-_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
-    "_OptionalSchedulingPolicyDetailTypeDef",
+_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class SchedulingPolicyDetailTypeDef(
-    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
+class CreateSchedulingPolicyRequestRequestTypeDef(
+    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
+    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
 ):
     pass
 
 _RequiredUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchedulingPolicyRequestRequestTypeDef",
     {
         "arn": str,
@@ -1469,61 +2023,90 @@
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
-        "volumes": List[VolumeTypeDef],
-        "environment": List[KeyValuePairTypeDef],
-        "mountPoints": List[MountPointTypeDef],
+        "volumes": List[VolumeOutputTypeDef],
+        "environment": List[KeyValuePairOutputTypeDef],
+        "mountPoints": List[MountPointOutputTypeDef],
         "readonlyRootFilesystem": bool,
-        "ulimits": List[UlimitTypeDef],
+        "ulimits": List[UlimitOutputTypeDef],
         "privileged": bool,
         "user": str,
         "exitCode": int,
         "reason": str,
         "containerInstanceArn": str,
         "taskArn": str,
         "logStreamName": str,
         "instanceType": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
-        "resourceRequirements": List[ResourceRequirementTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
-        "logConfiguration": LogConfigurationTypeDef,
-        "secrets": List[SecretTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-        "runtimePlatform": RuntimePlatformTypeDef,
+        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "secrets": List[SecretOutputTypeDef],
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "runtimePlatform": RuntimePlatformOutputTypeDef,
+    },
+    total=False,
+)
+
+ContainerPropertiesOutputTypeDef = TypedDict(
+    "ContainerPropertiesOutputTypeDef",
+    {
+        "image": str,
+        "vcpus": int,
+        "memory": int,
+        "command": List[str],
+        "jobRoleArn": str,
+        "executionRoleArn": str,
+        "volumes": List[VolumeOutputTypeDef],
+        "environment": List[KeyValuePairOutputTypeDef],
+        "mountPoints": List[MountPointOutputTypeDef],
+        "readonlyRootFilesystem": bool,
+        "privileged": bool,
+        "ulimits": List[UlimitOutputTypeDef],
+        "user": str,
+        "instanceType": str,
+        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "secrets": List[SecretOutputTypeDef],
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "runtimePlatform": RuntimePlatformOutputTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesTypeDef = TypedDict(
     "ContainerPropertiesTypeDef",
     {
         "image": str,
         "vcpus": int,
         "memory": int,
-        "command": List[str],
+        "command": Sequence[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
-        "volumes": List[VolumeTypeDef],
-        "environment": List[KeyValuePairTypeDef],
-        "mountPoints": List[MountPointTypeDef],
+        "volumes": Sequence[VolumeTypeDef],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "mountPoints": Sequence[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
         "privileged": bool,
-        "ulimits": List[UlimitTypeDef],
+        "ulimits": Sequence[UlimitTypeDef],
         "user": str,
         "instanceType": str,
-        "resourceRequirements": List[ResourceRequirementTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
-        "secrets": List[SecretTypeDef],
+        "secrets": Sequence[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
         "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
@@ -1540,14 +2123,22 @@
     "EksPropertiesDetailTypeDef",
     {
         "podProperties": EksPodPropertiesDetailTypeDef,
     },
     total=False,
 )
 
+EksPropertiesOutputTypeDef = TypedDict(
+    "EksPropertiesOutputTypeDef",
+    {
+        "podProperties": EksPodPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 EksPropertiesTypeDef = TypedDict(
     "EksPropertiesTypeDef",
     {
         "podProperties": EksPodPropertiesTypeDef,
     },
     total=False,
 )
@@ -1556,14 +2147,33 @@
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredNodeRangePropertyOutputTypeDef = TypedDict(
+    "_RequiredNodeRangePropertyOutputTypeDef",
+    {
+        "targetNodes": str,
+    },
+)
+_OptionalNodeRangePropertyOutputTypeDef = TypedDict(
+    "_OptionalNodeRangePropertyOutputTypeDef",
+    {
+        "container": ContainerPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
+class NodeRangePropertyOutputTypeDef(
+    _RequiredNodeRangePropertyOutputTypeDef, _OptionalNodeRangePropertyOutputTypeDef
+):
+    pass
+
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
     },
 )
 _OptionalNodeRangePropertyTypeDef = TypedDict(
@@ -1607,20 +2217,29 @@
 )
 
 class SubmitJobRequestRequestTypeDef(
     _RequiredSubmitJobRequestRequestTypeDef, _OptionalSubmitJobRequestRequestTypeDef
 ):
     pass
 
+NodePropertiesOutputTypeDef = TypedDict(
+    "NodePropertiesOutputTypeDef",
+    {
+        "numNodes": int,
+        "mainNode": int,
+        "nodeRangeProperties": List[NodeRangePropertyOutputTypeDef],
+    },
+)
+
 NodePropertiesTypeDef = TypedDict(
     "NodePropertiesTypeDef",
     {
         "numNodes": int,
         "mainNode": int,
-        "nodeRangeProperties": List[NodeRangePropertyTypeDef],
+        "nodeRangeProperties": Sequence[NodeRangePropertyTypeDef],
     },
 )
 
 _RequiredJobDefinitionTypeDef = TypedDict(
     "_RequiredJobDefinitionTypeDef",
     {
         "jobDefinitionName": str,
@@ -1631,22 +2250,22 @@
 )
 _OptionalJobDefinitionTypeDef = TypedDict(
     "_OptionalJobDefinitionTypeDef",
     {
         "status": str,
         "schedulingPriority": int,
         "parameters": Dict[str, str],
-        "retryStrategy": RetryStrategyTypeDef,
-        "containerProperties": ContainerPropertiesTypeDef,
-        "timeout": JobTimeoutTypeDef,
-        "nodeProperties": NodePropertiesTypeDef,
+        "retryStrategy": RetryStrategyOutputTypeDef,
+        "containerProperties": ContainerPropertiesOutputTypeDef,
+        "timeout": JobTimeoutOutputTypeDef,
+        "nodeProperties": NodePropertiesOutputTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
-        "eksProperties": EksPropertiesTypeDef,
+        "eksProperties": EksPropertiesOutputTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
     },
     total=False,
 )
 
 class JobDefinitionTypeDef(_RequiredJobDefinitionTypeDef, _OptionalJobDefinitionTypeDef):
     pass
@@ -1667,23 +2286,23 @@
     {
         "jobArn": str,
         "shareIdentifier": str,
         "schedulingPriority": int,
         "attempts": List[AttemptDetailTypeDef],
         "statusReason": str,
         "createdAt": int,
-        "retryStrategy": RetryStrategyTypeDef,
+        "retryStrategy": RetryStrategyOutputTypeDef,
         "stoppedAt": int,
-        "dependsOn": List[JobDependencyTypeDef],
+        "dependsOn": List[JobDependencyOutputTypeDef],
         "parameters": Dict[str, str],
         "container": ContainerDetailTypeDef,
         "nodeDetails": NodeDetailsTypeDef,
-        "nodeProperties": NodePropertiesTypeDef,
+        "nodeProperties": NodePropertiesOutputTypeDef,
         "arrayProperties": ArrayPropertiesDetailTypeDef,
-        "timeout": JobTimeoutTypeDef,
+        "timeout": JobTimeoutOutputTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesDetailTypeDef,
         "eksAttempts": List[EksAttemptDetailTypeDef],
         "isCancelled": bool,
         "isTerminated": bool,
```

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/PKG-INFO` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.0
-Summary: Type annotations for boto3.Batch 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Batch 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-batch"></a>
 
 # mypy-boto3-batch
 
 [![PyPI - mypy-boto3-batch](https://img.shields.io/pypi/v/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-batch?color=blue)](https://pypistats.org/packages/mypy-boto3-batch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,29 +365,42 @@
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
     CancelJobRequestRequestTypeDef,
-    EksConfigurationTypeDef,
-    UpdatePolicyTypeDef,
+    EksConfigurationOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
+    ComputeEnvironmentOrderOutputTypeDef,
     ComputeEnvironmentOrderTypeDef,
+    Ec2ConfigurationOutputTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     Ec2ConfigurationTypeDef,
     LaunchTemplateSpecificationTypeDef,
+    EphemeralStorageOutputTypeDef,
+    FargatePlatformConfigurationOutputTypeDef,
+    KeyValuePairOutputTypeDef,
+    MountPointOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
+    ResourceRequirementOutputTypeDef,
+    RuntimePlatformOutputTypeDef,
+    SecretOutputTypeDef,
+    UlimitOutputTypeDef,
+    KeyValuePairTypeDef,
+    ResourceRequirementTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
-    KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
-    ResourceRequirementTypeDef,
     RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
+    EksConfigurationTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
@@ -395,93 +408,124 @@
     DescribeComputeEnvironmentsRequestRequestTypeDef,
     DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
     DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
+    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
+    EksContainerEnvironmentVariableOutputTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
+    EksContainerSecurityContextOutputTypeDef,
+    EksContainerVolumeMountOutputTypeDef,
     EksContainerEnvironmentVariableTypeDef,
     EksContainerResourceRequirementsTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
+    EksEmptyDirOutputTypeDef,
     EksEmptyDirTypeDef,
+    EksHostPathOutputTypeDef,
     EksHostPathTypeDef,
+    EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
+    EksSecretOutputTypeDef,
     EksSecretTypeDef,
+    EvaluateOnExitOutputTypeDef,
     EvaluateOnExitTypeDef,
+    ShareAttributesOutputTypeDef,
     ShareAttributesTypeDef,
+    HostOutputTypeDef,
     HostTypeDef,
-    JobTimeoutTypeDef,
+    JobTimeoutOutputTypeDef,
+    JobDependencyOutputTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
+    JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
     ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     RegisterJobDefinitionResponseTypeDef,
     ResponseMetadataTypeDef,
     SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdatePolicyTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
-    CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
+    CreateJobQueueRequestRequestTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
+    LogConfigurationOutputTypeDef,
     ContainerOverridesTypeDef,
     LogConfigurationTypeDef,
+    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
-    EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
+    EksContainerOutputTypeDef,
+    EksContainerOverrideTypeDef,
     EksContainerTypeDef,
+    EksVolumeOutputTypeDef,
     EksVolumeTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
+    EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
-    CreateSchedulingPolicyRequestRequestTypeDef,
     SchedulingPolicyDetailTypeDef,
+    CreateSchedulingPolicyRequestRequestTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
+    NodeRangePropertyOutputTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-batch-1.28.0/mypy_boto3_batch.egg-info/SOURCES.txt` & `mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.0/setup.py` & `mypy-boto3-batch-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-batch",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Batch 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Batch 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

