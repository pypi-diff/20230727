# Comparing `tmp/mypy-boto3-ecs-1.28.0.tar.gz` & `tmp/mypy-boto3-ecs-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.28.0.tar", last modified: Thu Jul  6 20:59:29 2023, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
```

## Comparing `mypy-boto3-ecs-1.28.0.tar` & `mypy-boto3-ecs-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.826291 mypy-boto3-ecs-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24414 2023-07-06 20:59:29.822291 mypy-boto3-ecs-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22945 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.814291 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-07-06 20:39:57.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-07-06 20:39:57.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-06 20:39:58.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-07-06 20:39:57.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-06 20:39:57.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-06 20:39:57.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85580 2023-07-06 20:40:01.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85479 2023-07-06 20:39:59.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-06 20:39:57.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-06 20:39:57.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.822291 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24414 2023-07-06 20:59:29.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:59:29.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:29.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:29.000000 mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:29.826291 mypy-boto3-ecs-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:39:56.000000 mypy-boto3-ecs-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26619 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25148 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.072522 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   107340 2023-07-27 05:21:36.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107211 2023-07-27 05:21:35.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26619 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/setup.py
```

### Comparing `mypy-boto3-ecs-1.28.0/LICENSE` & `mypy-boto3-ecs-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/PKG-INFO` & `mypy-boto3-ecs-1.28.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.0
-Summary: Type annotations for boto3.ECS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ECS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ecs"></a>
 
 # mypy-boto3-ecs
 
 [![PyPI - mypy-boto3-ecs](https://img.shields.io/pypi/v/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -445,85 +445,120 @@
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
-    KeyValuePairTypeDef,
+    KeyValuePairOutputTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
+    ManagedScalingOutputTypeDef,
     ManagedScalingTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
+    ClusterSettingOutputTypeDef,
     ClusterSettingTypeDef,
+    ContainerDependencyOutputTypeDef,
+    EnvironmentFileOutputTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
+    HostEntryOutputTypeDef,
+    MountPointOutputTypeDef,
+    PortMappingOutputTypeDef,
+    RepositoryCredentialsOutputTypeDef,
+    ResourceRequirementOutputTypeDef,
+    SecretOutputTypeDef,
+    SystemControlOutputTypeDef,
+    UlimitOutputTypeDef,
+    VolumeFromOutputTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
     FirelensConfigurationTypeDef,
     HealthCheckTypeDef,
     HostEntryTypeDef,
+    KeyValuePairTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
     InstanceHealthCheckResultTypeDef,
-    ResourceTypeDef,
-    VersionInfoTypeDef,
+    ResourceOutputTypeDef,
+    VersionInfoOutputTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
+    NetworkBindingOutputTypeDef,
     NetworkInterfaceTypeDef,
+    TagTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
+    DeploymentCircuitBreakerOutputTypeDef,
     DeploymentCircuitBreakerTypeDef,
+    DeploymentControllerOutputTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
     DiscoverPollEndpointResponseTypeDef,
+    DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
+    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
+    EphemeralStorageOutputTypeDef,
     EphemeralStorageTypeDef,
+    ExecuteCommandLogConfigurationOutputTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
+    FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
+    HostVolumePropertiesOutputTypeDef,
     HostVolumePropertiesTypeDef,
+    InferenceAcceleratorOutputTypeDef,
+    InferenceAcceleratorOverrideOutputTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
+    KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
     ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
     ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
@@ -543,109 +578,135 @@
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
     ListTasksResponseTypeDef,
+    LoadBalancerOutputTypeDef,
     ManagedAgentStateChangeTypeDef,
     PaginatorConfigTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
+    ResourceTypeDef,
+    VersionInfoTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
     ResponseMetadataTypeDef,
+    RuntimePlatformOutputTypeDef,
+    ScaleOutputTypeDef,
+    ServiceConnectClientAliasOutputTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
+    ServiceRegistryOutputTypeDef,
     StopTaskRequestRequestTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
+    TaskDefinitionPlacementConstraintOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
-    ProxyConfigurationTypeDef,
-    DeleteAttributesRequestRequestTypeDef,
+    ProxyConfigurationOutputTypeDef,
     DeleteAttributesResponseTypeDef,
     ListAttributesResponseTypeDef,
-    PutAttributesRequestRequestTypeDef,
     PutAttributesResponseTypeDef,
+    DeleteAttributesRequestRequestTypeDef,
+    PutAttributesRequestRequestTypeDef,
+    AutoScalingGroupProviderOutputTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
+    ContainerOverrideOutputTypeDef,
+    LogConfigurationOutputTypeDef,
+    ProxyConfigurationTypeDef,
     ContainerOverrideTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
+    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
+    ExecuteCommandConfigurationOutputTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
+    FSxWindowsFileServerVolumeConfigurationOutputTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
-    CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
+    CreateTaskSetRequestRequestTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    ClusterConfigurationOutputTypeDef,
     ClusterConfigurationTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
+    TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
-    TaskTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceRequestRequestTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
+    CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
```

### Comparing `mypy-boto3-ecs-1.28.0/README.md` & `mypy-boto3-ecs-1.28.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ecs"></a>
 
 # mypy-boto3-ecs
 
 [![PyPI - mypy-boto3-ecs](https://img.shields.io/pypi/v/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -413,85 +413,120 @@
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
-    KeyValuePairTypeDef,
+    KeyValuePairOutputTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
+    ManagedScalingOutputTypeDef,
     ManagedScalingTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
+    ClusterSettingOutputTypeDef,
     ClusterSettingTypeDef,
+    ContainerDependencyOutputTypeDef,
+    EnvironmentFileOutputTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
+    HostEntryOutputTypeDef,
+    MountPointOutputTypeDef,
+    PortMappingOutputTypeDef,
+    RepositoryCredentialsOutputTypeDef,
+    ResourceRequirementOutputTypeDef,
+    SecretOutputTypeDef,
+    SystemControlOutputTypeDef,
+    UlimitOutputTypeDef,
+    VolumeFromOutputTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
     FirelensConfigurationTypeDef,
     HealthCheckTypeDef,
     HostEntryTypeDef,
+    KeyValuePairTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
     InstanceHealthCheckResultTypeDef,
-    ResourceTypeDef,
-    VersionInfoTypeDef,
+    ResourceOutputTypeDef,
+    VersionInfoOutputTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
+    NetworkBindingOutputTypeDef,
     NetworkInterfaceTypeDef,
+    TagTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
+    DeploymentCircuitBreakerOutputTypeDef,
     DeploymentCircuitBreakerTypeDef,
+    DeploymentControllerOutputTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
     DiscoverPollEndpointResponseTypeDef,
+    DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
+    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
+    EphemeralStorageOutputTypeDef,
     EphemeralStorageTypeDef,
+    ExecuteCommandLogConfigurationOutputTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
+    FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
+    HostVolumePropertiesOutputTypeDef,
     HostVolumePropertiesTypeDef,
+    InferenceAcceleratorOutputTypeDef,
+    InferenceAcceleratorOverrideOutputTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
+    KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
     ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
     ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
@@ -511,109 +546,135 @@
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
     ListTasksResponseTypeDef,
+    LoadBalancerOutputTypeDef,
     ManagedAgentStateChangeTypeDef,
     PaginatorConfigTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
+    ResourceTypeDef,
+    VersionInfoTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
     ResponseMetadataTypeDef,
+    RuntimePlatformOutputTypeDef,
+    ScaleOutputTypeDef,
+    ServiceConnectClientAliasOutputTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
+    ServiceRegistryOutputTypeDef,
     StopTaskRequestRequestTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
+    TaskDefinitionPlacementConstraintOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
-    ProxyConfigurationTypeDef,
-    DeleteAttributesRequestRequestTypeDef,
+    ProxyConfigurationOutputTypeDef,
     DeleteAttributesResponseTypeDef,
     ListAttributesResponseTypeDef,
-    PutAttributesRequestRequestTypeDef,
     PutAttributesResponseTypeDef,
+    DeleteAttributesRequestRequestTypeDef,
+    PutAttributesRequestRequestTypeDef,
+    AutoScalingGroupProviderOutputTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
+    ContainerOverrideOutputTypeDef,
+    LogConfigurationOutputTypeDef,
+    ProxyConfigurationTypeDef,
     ContainerOverrideTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
+    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
+    ExecuteCommandConfigurationOutputTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
+    FSxWindowsFileServerVolumeConfigurationOutputTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
-    CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
+    CreateTaskSetRequestRequestTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    ClusterConfigurationOutputTypeDef,
     ClusterConfigurationTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
+    TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
-    TaskTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceRequestRequestTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
+    CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
```

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ECS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
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

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.pyi`

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
     "AgentUpdateStatusType",
     "ApplicationProtocolType",
     "AssignPublicIpType",
     "CPUArchitectureType",
     "CapacityProviderFieldType",
     "CapacityProviderStatusType",
@@ -95,15 +94,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgentUpdateStatusType = Literal["FAILED", "PENDING", "STAGED", "STAGING", "UPDATED", "UPDATING"]
 ApplicationProtocolType = Literal["grpc", "http", "http2"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CPUArchitectureType = Literal["ARM64", "X86_64"]
 CapacityProviderFieldType = Literal["TAGS"]
 CapacityProviderStatusType = Literal["ACTIVE", "INACTIVE"]
 CapacityProviderUpdateStatusType = Literal[
@@ -338,14 +336,15 @@
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
@@ -424,26 +423,28 @@
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

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.py`

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
     "AgentUpdateStatusType",
     "ApplicationProtocolType",
     "AssignPublicIpType",
     "CPUArchitectureType",
     "CapacityProviderFieldType",
     "CapacityProviderStatusType",
@@ -94,14 +95,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AgentUpdateStatusType = Literal["FAILED", "PENDING", "STAGED", "STAGING", "UPDATED", "UPDATING"]
 ApplicationProtocolType = Literal["grpc", "http", "http2"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CPUArchitectureType = Literal["ARM64", "X86_64"]
 CapacityProviderFieldType = Literal["TAGS"]
 CapacityProviderStatusType = Literal["ACTIVE", "INACTIVE"]
 CapacityProviderUpdateStatusType = Literal[
@@ -336,14 +338,15 @@
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
@@ -422,26 +425,28 @@
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

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,85 +70,120 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttachmentStateChangeTypeDef",
-    "KeyValuePairTypeDef",
+    "KeyValuePairOutputTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
+    "ManagedScalingOutputTypeDef",
     "ManagedScalingTypeDef",
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
+    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
+    "ClusterSettingOutputTypeDef",
     "ClusterSettingTypeDef",
+    "ContainerDependencyOutputTypeDef",
+    "EnvironmentFileOutputTypeDef",
+    "FirelensConfigurationOutputTypeDef",
+    "HealthCheckOutputTypeDef",
+    "HostEntryOutputTypeDef",
+    "MountPointOutputTypeDef",
+    "PortMappingOutputTypeDef",
+    "RepositoryCredentialsOutputTypeDef",
+    "ResourceRequirementOutputTypeDef",
+    "SecretOutputTypeDef",
+    "SystemControlOutputTypeDef",
+    "UlimitOutputTypeDef",
+    "VolumeFromOutputTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
     "FirelensConfigurationTypeDef",
     "HealthCheckTypeDef",
     "HostEntryTypeDef",
+    "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
     "InstanceHealthCheckResultTypeDef",
-    "ResourceTypeDef",
-    "VersionInfoTypeDef",
+    "ResourceOutputTypeDef",
+    "VersionInfoOutputTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
+    "NetworkBindingOutputTypeDef",
     "NetworkInterfaceTypeDef",
+    "TagTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
+    "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
+    "DeploymentCircuitBreakerOutputTypeDef",
     "DeploymentCircuitBreakerTypeDef",
+    "DeploymentControllerOutputTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
+    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
     "DiscoverPollEndpointResponseTypeDef",
+    "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
+    "EFSAuthorizationConfigOutputTypeDef",
     "EFSAuthorizationConfigTypeDef",
+    "EphemeralStorageOutputTypeDef",
     "EphemeralStorageTypeDef",
+    "ExecuteCommandLogConfigurationOutputTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
+    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
+    "HostVolumePropertiesOutputTypeDef",
     "HostVolumePropertiesTypeDef",
+    "InferenceAcceleratorOutputTypeDef",
+    "InferenceAcceleratorOverrideOutputTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
+    "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
+    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
     "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
     "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
@@ -168,109 +203,135 @@
     "ListTaskDefinitionFamiliesResponseTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
     "ListTaskDefinitionsResponseTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
     "ListTasksResponseTypeDef",
+    "LoadBalancerOutputTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PaginatorConfigTypeDef",
+    "PlacementConstraintOutputTypeDef",
+    "PlacementStrategyOutputTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
+    "ResourceTypeDef",
+    "VersionInfoTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
     "ResponseMetadataTypeDef",
+    "RuntimePlatformOutputTypeDef",
+    "ScaleOutputTypeDef",
+    "ServiceConnectClientAliasOutputTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
+    "ServiceRegistryOutputTypeDef",
     "StopTaskRequestRequestTypeDef",
     "SubmitAttachmentStateChangesResponseTypeDef",
     "SubmitContainerStateChangeResponseTypeDef",
     "SubmitTaskStateChangeResponseTypeDef",
+    "TaskDefinitionPlacementConstraintOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
-    "ProxyConfigurationTypeDef",
-    "DeleteAttributesRequestRequestTypeDef",
+    "ProxyConfigurationOutputTypeDef",
     "DeleteAttributesResponseTypeDef",
     "ListAttributesResponseTypeDef",
-    "PutAttributesRequestRequestTypeDef",
     "PutAttributesResponseTypeDef",
+    "DeleteAttributesRequestRequestTypeDef",
+    "PutAttributesRequestRequestTypeDef",
+    "AutoScalingGroupProviderOutputTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
+    "ContainerOverrideOutputTypeDef",
+    "LogConfigurationOutputTypeDef",
+    "ProxyConfigurationTypeDef",
     "ContainerOverrideTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
+    "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
+    "EFSVolumeConfigurationOutputTypeDef",
     "EFSVolumeConfigurationTypeDef",
+    "ExecuteCommandConfigurationOutputTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
+    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
+    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
+    "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
-    "CreateTaskSetRequestRequestTypeDef",
     "TaskSetTypeDef",
+    "CreateTaskSetRequestRequestTypeDef",
+    "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
+    "ClusterConfigurationOutputTypeDef",
     "ClusterConfigurationTypeDef",
+    "VolumeOutputTypeDef",
     "VolumeTypeDef",
+    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
+    "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
-    "TaskTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
     "TaskDefinitionTypeDef",
-    "CreateServiceRequestRequestTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -293,23 +354,44 @@
     "AttachmentStateChangeTypeDef",
     {
         "attachmentArn": str,
         "status": str,
     },
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
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "value": str,
+        "targetType": Literal["container-instance"],
+        "targetId": str,
+    },
+    total=False,
+)
+
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "name": str,
     },
 )
 _OptionalAttributeTypeDef = TypedDict(
@@ -323,26 +405,60 @@
 )
 
 
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
 
+ManagedScalingOutputTypeDef = TypedDict(
+    "ManagedScalingOutputTypeDef",
+    {
+        "status": ManagedScalingStatusType,
+        "targetCapacity": int,
+        "minimumScalingStepSize": int,
+        "maximumScalingStepSize": int,
+        "instanceWarmupPeriod": int,
+    },
+    total=False,
+)
+
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
         "instanceWarmupPeriod": int,
     },
     total=False,
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": AssignPublicIpType,
+    },
+    total=False,
+)
+
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -357,14 +473,37 @@
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
 
+_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "capacityProvider": str,
+    },
+)
+_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "weight": int,
+        "base": int,
+    },
+    total=False,
+)
+
+
+class CapacityProviderStrategyItemOutputTypeDef(
+    _RequiredCapacityProviderStrategyItemOutputTypeDef,
+    _OptionalCapacityProviderStrategyItemOutputTypeDef,
+):
+    pass
+
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -379,16 +518,16 @@
 
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
@@ -403,23 +542,174 @@
     "ClusterServiceConnectDefaultsTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
+ClusterSettingOutputTypeDef = TypedDict(
+    "ClusterSettingOutputTypeDef",
+    {
+        "name": Literal["containerInsights"],
+        "value": str,
+    },
+    total=False,
+)
+
 ClusterSettingTypeDef = TypedDict(
     "ClusterSettingTypeDef",
     {
         "name": Literal["containerInsights"],
         "value": str,
     },
     total=False,
 )
 
+ContainerDependencyOutputTypeDef = TypedDict(
+    "ContainerDependencyOutputTypeDef",
+    {
+        "containerName": str,
+        "condition": ContainerConditionType,
+    },
+)
+
+EnvironmentFileOutputTypeDef = TypedDict(
+    "EnvironmentFileOutputTypeDef",
+    {
+        "value": str,
+        "type": Literal["s3"],
+    },
+)
+
+_RequiredFirelensConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationOutputTypeDef",
+    {
+        "type": FirelensConfigurationTypeType,
+    },
+)
+_OptionalFirelensConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationOutputTypeDef",
+    {
+        "options": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class FirelensConfigurationOutputTypeDef(
+    _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
+):
+    pass
+
+
+_RequiredHealthCheckOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckOutputTypeDef",
+    {
+        "command": List[str],
+    },
+)
+_OptionalHealthCheckOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckOutputTypeDef",
+    {
+        "interval": int,
+        "timeout": int,
+        "retries": int,
+        "startPeriod": int,
+    },
+    total=False,
+)
+
+
+class HealthCheckOutputTypeDef(
+    _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
+):
+    pass
+
+
+HostEntryOutputTypeDef = TypedDict(
+    "HostEntryOutputTypeDef",
+    {
+        "hostname": str,
+        "ipAddress": str,
+    },
+)
+
+MountPointOutputTypeDef = TypedDict(
+    "MountPointOutputTypeDef",
+    {
+        "sourceVolume": str,
+        "containerPath": str,
+        "readOnly": bool,
+    },
+    total=False,
+)
+
+PortMappingOutputTypeDef = TypedDict(
+    "PortMappingOutputTypeDef",
+    {
+        "containerPort": int,
+        "hostPort": int,
+        "protocol": TransportProtocolType,
+        "name": str,
+        "appProtocol": ApplicationProtocolType,
+        "containerPortRange": str,
+    },
+    total=False,
+)
+
+RepositoryCredentialsOutputTypeDef = TypedDict(
+    "RepositoryCredentialsOutputTypeDef",
+    {
+        "credentialsParameter": str,
+    },
+)
+
+ResourceRequirementOutputTypeDef = TypedDict(
+    "ResourceRequirementOutputTypeDef",
+    {
+        "value": str,
+        "type": ResourceTypeType,
+    },
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
+SystemControlOutputTypeDef = TypedDict(
+    "SystemControlOutputTypeDef",
+    {
+        "namespace": str,
+        "value": str,
+    },
+    total=False,
+)
+
+UlimitOutputTypeDef = TypedDict(
+    "UlimitOutputTypeDef",
+    {
+        "name": UlimitNameType,
+        "softLimit": int,
+        "hardLimit": int,
+    },
+)
+
+VolumeFromOutputTypeDef = TypedDict(
+    "VolumeFromOutputTypeDef",
+    {
+        "sourceContainer": str,
+        "readOnly": bool,
+    },
+    total=False,
+)
+
 ContainerDependencyTypeDef = TypedDict(
     "ContainerDependencyTypeDef",
     {
         "containerName": str,
         "condition": ContainerConditionType,
     },
 )
@@ -437,30 +727,30 @@
     {
         "type": FirelensConfigurationTypeType,
     },
 )
 _OptionalFirelensConfigurationTypeDef = TypedDict(
     "_OptionalFirelensConfigurationTypeDef",
     {
-        "options": Dict[str, str],
+        "options": Mapping[str, str],
     },
     total=False,
 )
 
 
 class FirelensConfigurationTypeDef(
     _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
-        "command": List[str],
+        "command": Sequence[str],
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "interval": int,
         "timeout": int,
@@ -479,14 +769,23 @@
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
 
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
+    {
+        "name": str,
+        "value": str,
+    },
+    total=False,
+)
+
 MountPointTypeDef = TypedDict(
     "MountPointTypeDef",
     {
         "sourceVolume": str,
         "containerPath": str,
         "readOnly": bool,
     },
@@ -563,29 +862,29 @@
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
     {
         "name": str,
         "type": str,
         "doubleValue": float,
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
     },
     total=False,
 )
 
-VersionInfoTypeDef = TypedDict(
-    "VersionInfoTypeDef",
+VersionInfoOutputTypeDef = TypedDict(
+    "VersionInfoOutputTypeDef",
     {
         "agentVersion": str,
         "agentHash": str,
         "dockerVersion": str,
     },
     total=False,
 )
@@ -610,24 +909,46 @@
         "name": Literal["ExecuteCommandAgent"],
         "reason": str,
         "lastStatus": str,
     },
     total=False,
 )
 
+NetworkBindingOutputTypeDef = TypedDict(
+    "NetworkBindingOutputTypeDef",
+    {
+        "bindIP": str,
+        "containerPort": int,
+        "hostPort": int,
+        "protocol": TransportProtocolType,
+        "containerPortRange": str,
+        "hostPortRange": str,
+    },
+    total=False,
+)
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
 )
 
@@ -784,31 +1105,55 @@
 
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
 
+DeploymentAlarmsOutputTypeDef = TypedDict(
+    "DeploymentAlarmsOutputTypeDef",
+    {
+        "alarmNames": List[str],
+        "enable": bool,
+        "rollback": bool,
+    },
+)
+
 DeploymentAlarmsTypeDef = TypedDict(
     "DeploymentAlarmsTypeDef",
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
     },
 )
 
+DeploymentCircuitBreakerOutputTypeDef = TypedDict(
+    "DeploymentCircuitBreakerOutputTypeDef",
+    {
+        "enable": bool,
+        "rollback": bool,
+    },
+)
+
 DeploymentCircuitBreakerTypeDef = TypedDict(
     "DeploymentCircuitBreakerTypeDef",
     {
         "enable": bool,
         "rollback": bool,
     },
 )
 
+DeploymentControllerOutputTypeDef = TypedDict(
+    "DeploymentControllerOutputTypeDef",
+    {
+        "type": DeploymentControllerTypeType,
+    },
+)
+
 ServiceConnectServiceResourceTypeDef = TypedDict(
     "ServiceConnectServiceResourceTypeDef",
     {
         "discoveryName": str,
         "discoveryArn": str,
     },
     total=False,
@@ -981,25 +1326,45 @@
 
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
 
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
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
+
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
@@ -1020,42 +1385,82 @@
         "endpoint": str,
         "telemetryEndpoint": str,
         "serviceConnectEndpoint": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DockerVolumeConfigurationTypeDef = TypedDict(
-    "DockerVolumeConfigurationTypeDef",
+DockerVolumeConfigurationOutputTypeDef = TypedDict(
+    "DockerVolumeConfigurationOutputTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
         "driverOpts": Dict[str, str],
         "labels": Dict[str, str],
     },
     total=False,
 )
 
+DockerVolumeConfigurationTypeDef = TypedDict(
+    "DockerVolumeConfigurationTypeDef",
+    {
+        "scope": ScopeType,
+        "autoprovision": bool,
+        "driver": str,
+        "driverOpts": Mapping[str, str],
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
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
 )
 
+EphemeralStorageOutputTypeDef = TypedDict(
+    "EphemeralStorageOutputTypeDef",
+    {
+        "sizeInGiB": int,
+    },
+)
+
 EphemeralStorageTypeDef = TypedDict(
     "EphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
+ExecuteCommandLogConfigurationOutputTypeDef = TypedDict(
+    "ExecuteCommandLogConfigurationOutputTypeDef",
+    {
+        "cloudWatchLogGroupName": str,
+        "cloudWatchEncryptionEnabled": bool,
+        "s3BucketName": str,
+        "s3EncryptionEnabled": bool,
+        "s3KeyPrefix": str,
+    },
+    total=False,
+)
+
 ExecuteCommandLogConfigurationTypeDef = TypedDict(
     "ExecuteCommandLogConfigurationTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "cloudWatchEncryptionEnabled": bool,
         "s3BucketName": str,
         "s3EncryptionEnabled": bool,
@@ -1094,14 +1499,22 @@
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
     total=False,
 )
 
+FSxWindowsFileServerAuthorizationConfigOutputTypeDef = TypedDict(
+    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
+    {
+        "credentialsParameter": str,
+        "domain": str,
+    },
+)
+
 FSxWindowsFileServerAuthorizationConfigTypeDef = TypedDict(
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     {
         "credentialsParameter": str,
         "domain": str,
     },
 )
@@ -1133,22 +1546,47 @@
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
     total=False,
 )
 
+HostVolumePropertiesOutputTypeDef = TypedDict(
+    "HostVolumePropertiesOutputTypeDef",
+    {
+        "sourcePath": str,
+    },
+    total=False,
+)
+
 HostVolumePropertiesTypeDef = TypedDict(
     "HostVolumePropertiesTypeDef",
     {
         "sourcePath": str,
     },
     total=False,
 )
 
+InferenceAcceleratorOutputTypeDef = TypedDict(
+    "InferenceAcceleratorOutputTypeDef",
+    {
+        "deviceName": str,
+        "deviceType": str,
+    },
+)
+
+InferenceAcceleratorOverrideOutputTypeDef = TypedDict(
+    "InferenceAcceleratorOverrideOutputTypeDef",
+    {
+        "deviceName": str,
+        "deviceType": str,
+    },
+    total=False,
+)
+
 InferenceAcceleratorOverrideTypeDef = TypedDict(
     "InferenceAcceleratorOverrideTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
     total=False,
@@ -1158,34 +1596,63 @@
     "InferenceAcceleratorTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
 )
 
-KernelCapabilitiesTypeDef = TypedDict(
-    "KernelCapabilitiesTypeDef",
+KernelCapabilitiesOutputTypeDef = TypedDict(
+    "KernelCapabilitiesOutputTypeDef",
     {
         "add": List[str],
         "drop": List[str],
     },
     total=False,
 )
 
+KernelCapabilitiesTypeDef = TypedDict(
+    "KernelCapabilitiesTypeDef",
+    {
+        "add": Sequence[str],
+        "drop": Sequence[str],
+    },
+    total=False,
+)
+
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
+
+class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
+    pass
+
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
@@ -1515,14 +1982,25 @@
     {
         "taskArns": List[str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoadBalancerOutputTypeDef = TypedDict(
+    "LoadBalancerOutputTypeDef",
+    {
+        "targetGroupArn": str,
+        "loadBalancerName": str,
+        "containerName": str,
+        "containerPort": int,
+    },
+    total=False,
+)
+
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -1548,14 +2026,32 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PlacementConstraintOutputTypeDef = TypedDict(
+    "PlacementConstraintOutputTypeDef",
+    {
+        "type": PlacementConstraintTypeType,
+        "expression": str,
+    },
+    total=False,
+)
+
+PlacementStrategyOutputTypeDef = TypedDict(
+    "PlacementStrategyOutputTypeDef",
+    {
+        "type": PlacementStrategyTypeType,
+        "field": str,
+    },
+    total=False,
+)
+
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1586,14 +2082,37 @@
 
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
 
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
+    {
+        "name": str,
+        "type": str,
+        "doubleValue": float,
+        "longValue": int,
+        "integerValue": int,
+        "stringSetValue": Sequence[str],
+    },
+    total=False,
+)
+
+VersionInfoTypeDef = TypedDict(
+    "VersionInfoTypeDef",
+    {
+        "agentVersion": str,
+        "agentHash": str,
+        "dockerVersion": str,
+    },
+    total=False,
+)
+
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -1615,14 +2134,53 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+RuntimePlatformOutputTypeDef = TypedDict(
+    "RuntimePlatformOutputTypeDef",
+    {
+        "cpuArchitecture": CPUArchitectureType,
+        "operatingSystemFamily": OSFamilyType,
+    },
+    total=False,
+)
+
+ScaleOutputTypeDef = TypedDict(
+    "ScaleOutputTypeDef",
+    {
+        "value": float,
+        "unit": Literal["PERCENT"],
+    },
+    total=False,
+)
+
+_RequiredServiceConnectClientAliasOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectClientAliasOutputTypeDef",
+    {
+        "port": int,
+    },
+)
+_OptionalServiceConnectClientAliasOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectClientAliasOutputTypeDef",
+    {
+        "dnsName": str,
+    },
+    total=False,
+)
+
+
+class ServiceConnectClientAliasOutputTypeDef(
+    _RequiredServiceConnectClientAliasOutputTypeDef, _OptionalServiceConnectClientAliasOutputTypeDef
+):
+    pass
+
+
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -1646,14 +2204,25 @@
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
     total=False,
 )
 
+ServiceRegistryOutputTypeDef = TypedDict(
+    "ServiceRegistryOutputTypeDef",
+    {
+        "registryArn": str,
+        "port": int,
+        "containerName": str,
+        "containerPort": int,
+    },
+    total=False,
+)
+
 _RequiredStopTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStopTaskRequestRequestTypeDef",
     {
         "task": str,
     },
 )
 _OptionalStopTaskRequestRequestTypeDef = TypedDict(
@@ -1692,14 +2261,23 @@
     "SubmitTaskStateChangeResponseTypeDef",
     {
         "acknowledgment": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TaskDefinitionPlacementConstraintOutputTypeDef = TypedDict(
+    "TaskDefinitionPlacementConstraintOutputTypeDef",
+    {
+        "type": Literal["memberOf"],
+        "expression": str,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1806,41 +2384,66 @@
 
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
-        "details": List[KeyValuePairTypeDef],
+        "details": List[KeyValuePairOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredProxyConfigurationTypeDef = TypedDict(
-    "_RequiredProxyConfigurationTypeDef",
+_RequiredProxyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredProxyConfigurationOutputTypeDef",
     {
         "containerName": str,
     },
 )
-_OptionalProxyConfigurationTypeDef = TypedDict(
-    "_OptionalProxyConfigurationTypeDef",
+_OptionalProxyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalProxyConfigurationOutputTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairTypeDef],
+        "properties": List[KeyValuePairOutputTypeDef],
     },
     total=False,
 )
 
 
-class ProxyConfigurationTypeDef(
-    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
+class ProxyConfigurationOutputTypeDef(
+    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
 ):
     pass
 
 
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
@@ -1854,31 +2457,14 @@
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
 
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
@@ -1892,21 +2478,35 @@
 
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
 
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
+_RequiredAutoScalingGroupProviderOutputTypeDef = TypedDict(
+    "_RequiredAutoScalingGroupProviderOutputTypeDef",
     {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "autoScalingGroupArn": str,
     },
 )
+_OptionalAutoScalingGroupProviderOutputTypeDef = TypedDict(
+    "_OptionalAutoScalingGroupProviderOutputTypeDef",
+    {
+        "managedScaling": ManagedScalingOutputTypeDef,
+        "managedTerminationProtection": ManagedTerminationProtectionType,
+    },
+    total=False,
+)
+
+
+class AutoScalingGroupProviderOutputTypeDef(
+    _RequiredAutoScalingGroupProviderOutputTypeDef, _OptionalAutoScalingGroupProviderOutputTypeDef
+):
+    pass
+
 
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
@@ -1931,14 +2531,22 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1951,46 +2559,97 @@
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
 UpdateClusterSettingsRequestRequestTypeDef = TypedDict(
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
         "settings": Sequence[ClusterSettingTypeDef],
     },
 )
 
+ContainerOverrideOutputTypeDef = TypedDict(
+    "ContainerOverrideOutputTypeDef",
+    {
+        "name": str,
+        "command": List[str],
+        "environment": List[KeyValuePairOutputTypeDef],
+        "environmentFiles": List[EnvironmentFileOutputTypeDef],
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+    },
+    total=False,
+)
+
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
+
+class LogConfigurationOutputTypeDef(
+    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
+):
+    pass
+
+
+_RequiredProxyConfigurationTypeDef = TypedDict(
+    "_RequiredProxyConfigurationTypeDef",
+    {
+        "containerName": str,
+    },
+)
+_OptionalProxyConfigurationTypeDef = TypedDict(
+    "_OptionalProxyConfigurationTypeDef",
+    {
+        "type": Literal["APPMESH"],
+        "properties": Sequence[KeyValuePairTypeDef],
+    },
+    total=False,
+)
+
+
+class ProxyConfigurationTypeDef(
+    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
+):
+    pass
+
+
 ContainerOverrideTypeDef = TypedDict(
     "ContainerOverrideTypeDef",
     {
         "name": str,
-        "command": List[str],
-        "environment": List[KeyValuePairTypeDef],
-        "environmentFiles": List[EnvironmentFileTypeDef],
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
-        "resourceRequirements": List[ResourceRequirementTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
@@ -2057,26 +2716,34 @@
         "name": str,
         "image": str,
         "imageDigest": str,
         "runtimeId": str,
         "lastStatus": str,
         "exitCode": int,
         "reason": str,
-        "networkBindings": List[NetworkBindingTypeDef],
+        "networkBindings": List[NetworkBindingOutputTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "healthStatus": HealthStatusType,
         "managedAgents": List[ManagedAgentTypeDef],
         "cpu": str,
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
         "scale": ScaleTypeDef,
@@ -2112,14 +2779,25 @@
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentConfigurationOutputTypeDef = TypedDict(
+    "DeploymentConfigurationOutputTypeDef",
+    {
+        "deploymentCircuitBreaker": DeploymentCircuitBreakerOutputTypeDef,
+        "maximumPercent": int,
+        "minimumHealthyPercent": int,
+        "alarms": DeploymentAlarmsOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsTypeDef,
@@ -2219,14 +2897,38 @@
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
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
+
+class EFSVolumeConfigurationOutputTypeDef(
+    _RequiredEFSVolumeConfigurationOutputTypeDef, _OptionalEFSVolumeConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -2243,14 +2945,24 @@
 
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
 
+ExecuteCommandConfigurationOutputTypeDef = TypedDict(
+    "ExecuteCommandConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+        "logging": ExecuteCommandLoggingType,
+        "logConfiguration": ExecuteCommandLogConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2266,14 +2978,23 @@
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FSxWindowsFileServerVolumeConfigurationOutputTypeDef = TypedDict(
+    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
+    {
+        "fileSystemId": str,
+        "rootDirectory": str,
+        "authorizationConfig": FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
+    },
+)
+
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
         "rootDirectory": str,
         "authorizationConfig": FSxWindowsFileServerAuthorizationConfigTypeDef,
     },
@@ -2293,22 +3014,36 @@
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LinuxParametersOutputTypeDef = TypedDict(
+    "LinuxParametersOutputTypeDef",
+    {
+        "capabilities": KernelCapabilitiesOutputTypeDef,
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
         "capabilities": KernelCapabilitiesTypeDef,
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
 
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
@@ -2323,14 +3058,37 @@
         "attributes": Sequence[AttributeTypeDef],
         "platformDevices": Sequence[PlatformDeviceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredServiceConnectServiceOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectServiceOutputTypeDef",
+    {
+        "portName": str,
+    },
+)
+_OptionalServiceConnectServiceOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectServiceOutputTypeDef",
+    {
+        "discoveryName": str,
+        "clientAliases": List[ServiceConnectClientAliasOutputTypeDef],
+        "ingressPortOverride": int,
+    },
+    total=False,
+)
+
+
+class ServiceConnectServiceOutputTypeDef(
+    _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
+):
+    pass
+
+
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2352,18 +3110,18 @@
 
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
-        "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
+        "autoScalingGroupProvider": AutoScalingGroupProviderOutputTypeDef,
         "updateStatus": CapacityProviderUpdateStatusType,
         "updateStatusReason": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateCapacityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCapacityProviderRequestRequestTypeDef",
     {
@@ -2391,14 +3149,45 @@
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
 
+TaskSetTypeDef = TypedDict(
+    "TaskSetTypeDef",
+    {
+        "id": str,
+        "taskSetArn": str,
+        "serviceArn": str,
+        "clusterArn": str,
+        "startedBy": str,
+        "externalId": str,
+        "status": str,
+        "taskDefinition": str,
+        "computedDesiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "loadBalancers": List[LoadBalancerOutputTypeDef],
+        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
+        "scale": ScaleOutputTypeDef,
+        "stabilityStatus": StabilityStatusType,
+        "stabilityStatusAt": datetime,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
         "service": str,
         "cluster": str,
         "taskDefinition": str,
     },
@@ -2423,51 +3212,34 @@
 
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
 
-TaskSetTypeDef = TypedDict(
-    "TaskSetTypeDef",
+TaskOverrideOutputTypeDef = TypedDict(
+    "TaskOverrideOutputTypeDef",
     {
-        "id": str,
-        "taskSetArn": str,
-        "serviceArn": str,
-        "clusterArn": str,
-        "startedBy": str,
-        "externalId": str,
-        "status": str,
-        "taskDefinition": str,
-        "computedDesiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "scale": ScaleTypeDef,
-        "stabilityStatus": StabilityStatusType,
-        "stabilityStatusAt": datetime,
-        "tags": List[TagTypeDef],
+        "containerOverrides": List[ContainerOverrideOutputTypeDef],
+        "cpu": str,
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideOutputTypeDef],
+        "executionRoleArn": str,
+        "memory": str,
+        "taskRoleArn": str,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
-        "containerOverrides": List[ContainerOverrideTypeDef],
+        "containerOverrides": Sequence[ContainerOverrideTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
+        "inferenceAcceleratorOverrides": Sequence[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
@@ -2475,27 +3247,27 @@
 ContainerInstanceTypeDef = TypedDict(
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
-        "versionInfo": VersionInfoTypeDef,
-        "remainingResources": List[ResourceTypeDef],
-        "registeredResources": List[ResourceTypeDef],
+        "versionInfo": VersionInfoOutputTypeDef,
+        "remainingResources": List[ResourceOutputTypeDef],
+        "registeredResources": List[ResourceOutputTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
-        "attributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
         "registeredAt": datetime,
         "attachments": List[AttachmentTypeDef],
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "healthStatus": ContainerInstanceHealthStatusTypeDef,
     },
     total=False,
 )
 
 SubmitTaskStateChangeRequestRequestTypeDef = TypedDict(
     "SubmitTaskStateChangeRequestRequestTypeDef",
@@ -2510,81 +3282,174 @@
         "pullStartedAt": Union[datetime, str],
         "pullStoppedAt": Union[datetime, str],
         "executionStoppedAt": Union[datetime, str],
     },
     total=False,
 )
 
+ClusterConfigurationOutputTypeDef = TypedDict(
+    "ClusterConfigurationOutputTypeDef",
+    {
+        "executeCommandConfiguration": ExecuteCommandConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
+VolumeOutputTypeDef = TypedDict(
+    "VolumeOutputTypeDef",
+    {
+        "name": str,
+        "host": HostVolumePropertiesOutputTypeDef,
+        "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
+        "efsVolumeConfiguration": EFSVolumeConfigurationOutputTypeDef,
+        "fsxWindowsFileServerVolumeConfiguration": (
+            FSxWindowsFileServerVolumeConfigurationOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "name": str,
         "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationTypeDef,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
         "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionTypeDef = TypedDict(
-    "ContainerDefinitionTypeDef",
+ContainerDefinitionOutputTypeDef = TypedDict(
+    "ContainerDefinitionOutputTypeDef",
     {
         "name": str,
         "image": str,
-        "repositoryCredentials": RepositoryCredentialsTypeDef,
+        "repositoryCredentials": RepositoryCredentialsOutputTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "links": List[str],
-        "portMappings": List[PortMappingTypeDef],
+        "portMappings": List[PortMappingOutputTypeDef],
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
-        "environment": List[KeyValuePairTypeDef],
-        "environmentFiles": List[EnvironmentFileTypeDef],
-        "mountPoints": List[MountPointTypeDef],
-        "volumesFrom": List[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
-        "secrets": List[SecretTypeDef],
-        "dependsOn": List[ContainerDependencyTypeDef],
+        "environment": List[KeyValuePairOutputTypeDef],
+        "environmentFiles": List[EnvironmentFileOutputTypeDef],
+        "mountPoints": List[MountPointOutputTypeDef],
+        "volumesFrom": List[VolumeFromOutputTypeDef],
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "secrets": List[SecretOutputTypeDef],
+        "dependsOn": List[ContainerDependencyOutputTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
         "disableNetworking": bool,
         "privileged": bool,
         "readonlyRootFilesystem": bool,
         "dnsServers": List[str],
         "dnsSearchDomains": List[str],
-        "extraHosts": List[HostEntryTypeDef],
+        "extraHosts": List[HostEntryOutputTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
-        "ulimits": List[UlimitTypeDef],
+        "ulimits": List[UlimitOutputTypeDef],
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "healthCheck": HealthCheckOutputTypeDef,
+        "systemControls": List[SystemControlOutputTypeDef],
+        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "firelensConfiguration": FirelensConfigurationOutputTypeDef,
+        "credentialSpecs": List[str],
+    },
+    total=False,
+)
+
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
+    {
+        "name": str,
+        "image": str,
+        "repositoryCredentials": RepositoryCredentialsTypeDef,
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "links": Sequence[str],
+        "portMappings": Sequence[PortMappingTypeDef],
+        "essential": bool,
+        "entryPoint": Sequence[str],
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
+        "mountPoints": Sequence[MountPointTypeDef],
+        "volumesFrom": Sequence[VolumeFromTypeDef],
+        "linuxParameters": LinuxParametersTypeDef,
+        "secrets": Sequence[SecretTypeDef],
+        "dependsOn": Sequence[ContainerDependencyTypeDef],
+        "startTimeout": int,
+        "stopTimeout": int,
+        "hostname": str,
+        "user": str,
+        "workingDirectory": str,
+        "disableNetworking": bool,
+        "privileged": bool,
+        "readonlyRootFilesystem": bool,
+        "dnsServers": Sequence[str],
+        "dnsSearchDomains": Sequence[str],
+        "extraHosts": Sequence[HostEntryTypeDef],
+        "dockerSecurityOptions": Sequence[str],
+        "interactive": bool,
+        "pseudoTerminal": bool,
+        "dockerLabels": Mapping[str, str],
+        "ulimits": Sequence[UlimitTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
         "healthCheck": HealthCheckTypeDef,
-        "systemControls": List[SystemControlTypeDef],
-        "resourceRequirements": List[ResourceRequirementTypeDef],
+        "systemControls": Sequence[SystemControlTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
-        "credentialSpecs": List[str],
+        "credentialSpecs": Sequence[str],
+    },
+    total=False,
+)
+
+_RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectConfigurationOutputTypeDef",
+    {
+        "namespace": str,
+        "services": List[ServiceConnectServiceOutputTypeDef],
+        "logConfiguration": LogConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
+class ServiceConnectConfigurationOutputTypeDef(
+    _RequiredServiceConnectConfigurationOutputTypeDef,
+    _OptionalServiceConnectConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -2675,14 +3540,57 @@
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TaskTypeDef = TypedDict(
+    "TaskTypeDef",
+    {
+        "attachments": List[AttachmentTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
+        "availabilityZone": str,
+        "capacityProviderName": str,
+        "clusterArn": str,
+        "connectivity": ConnectivityType,
+        "connectivityAt": datetime,
+        "containerInstanceArn": str,
+        "containers": List[ContainerTypeDef],
+        "cpu": str,
+        "createdAt": datetime,
+        "desiredStatus": str,
+        "enableExecuteCommand": bool,
+        "executionStoppedAt": datetime,
+        "group": str,
+        "healthStatus": HealthStatusType,
+        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "lastStatus": str,
+        "launchType": LaunchTypeType,
+        "memory": str,
+        "overrides": TaskOverrideOutputTypeDef,
+        "platformVersion": str,
+        "platformFamily": str,
+        "pullStartedAt": datetime,
+        "pullStoppedAt": datetime,
+        "startedAt": datetime,
+        "startedBy": str,
+        "stopCode": TaskStopCodeType,
+        "stoppedAt": datetime,
+        "stoppedReason": str,
+        "stoppingAt": datetime,
+        "tags": List[TagOutputTypeDef],
+        "taskArn": str,
+        "taskDefinitionArn": str,
+        "version": int,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 _OptionalRunTaskRequestRequestTypeDef = TypedDict(
@@ -2742,57 +3650,14 @@
 
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
 
-TaskTypeDef = TypedDict(
-    "TaskTypeDef",
-    {
-        "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeTypeDef],
-        "availabilityZone": str,
-        "capacityProviderName": str,
-        "clusterArn": str,
-        "connectivity": ConnectivityType,
-        "connectivityAt": datetime,
-        "containerInstanceArn": str,
-        "containers": List[ContainerTypeDef],
-        "cpu": str,
-        "createdAt": datetime,
-        "desiredStatus": str,
-        "enableExecuteCommand": bool,
-        "executionStoppedAt": datetime,
-        "group": str,
-        "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "lastStatus": str,
-        "launchType": LaunchTypeType,
-        "memory": str,
-        "overrides": TaskOverrideTypeDef,
-        "platformVersion": str,
-        "platformFamily": str,
-        "pullStartedAt": datetime,
-        "pullStoppedAt": datetime,
-        "startedAt": datetime,
-        "startedBy": str,
-        "stopCode": TaskStopCodeType,
-        "stoppedAt": datetime,
-        "stoppedReason": str,
-        "stoppingAt": datetime,
-        "tags": List[TagTypeDef],
-        "taskArn": str,
-        "taskDefinitionArn": str,
-        "version": int,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
-
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2832,25 +3697,25 @@
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
-        "configuration": ClusterConfigurationTypeDef,
+        "configuration": ClusterConfigurationOutputTypeDef,
         "status": str,
         "registeredContainerInstancesCount": int,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "activeServicesCount": int,
-        "statistics": List[KeyValuePairTypeDef],
-        "tags": List[TagTypeDef],
-        "settings": List[ClusterSettingTypeDef],
+        "statistics": List[KeyValuePairOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "settings": List[ClusterSettingOutputTypeDef],
         "capacityProviders": List[str],
-        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
         "attachments": List[AttachmentTypeDef],
         "attachmentsStatus": str,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsTypeDef,
     },
     total=False,
 )
 
@@ -2887,14 +3752,45 @@
 
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
 
+TaskDefinitionTypeDef = TypedDict(
+    "TaskDefinitionTypeDef",
+    {
+        "taskDefinitionArn": str,
+        "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
+        "family": str,
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "revision": int,
+        "volumes": List[VolumeOutputTypeDef],
+        "status": TaskDefinitionStatusType,
+        "requiresAttributes": List[AttributeOutputTypeDef],
+        "placementConstraints": List[TaskDefinitionPlacementConstraintOutputTypeDef],
+        "compatibilities": List[CompatibilityType],
+        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "requiresCompatibilities": List[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "registeredAt": datetime,
+        "deregisteredAt": datetime,
+        "registeredBy": str,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "family": str,
         "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
     },
 )
@@ -2924,41 +3820,35 @@
 class RegisterTaskDefinitionRequestRequestTypeDef(
     _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
     _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-TaskDefinitionTypeDef = TypedDict(
-    "TaskDefinitionTypeDef",
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
     {
-        "taskDefinitionArn": str,
-        "containerDefinitions": List[ContainerDefinitionTypeDef],
-        "family": str,
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "revision": int,
-        "volumes": List[VolumeTypeDef],
-        "status": TaskDefinitionStatusType,
-        "requiresAttributes": List[AttributeTypeDef],
-        "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
-        "compatibilities": List[CompatibilityType],
-        "runtimePlatform": RuntimePlatformTypeDef,
-        "requiresCompatibilities": List[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "registeredAt": datetime,
-        "deregisteredAt": datetime,
-        "registeredBy": str,
-        "ephemeralStorage": EphemeralStorageTypeDef,
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
@@ -2997,39 +3887,14 @@
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
 
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
-        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -3164,58 +4029,58 @@
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "loadBalancers": List[LoadBalancerOutputTypeDef],
+        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
         "status": str,
         "desiredCount": int,
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
-        "placementConstraints": List[PlacementConstraintTypeDef],
-        "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "placementConstraints": List[PlacementConstraintOutputTypeDef],
+        "placementStrategy": List[PlacementStrategyOutputTypeDef],
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerTypeDef,
-        "tags": List[TagTypeDef],
+        "deploymentController": DeploymentControllerOutputTypeDef,
+        "tags": List[TagOutputTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -69,85 +69,120 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentStateChangeTypeDef",
-    "KeyValuePairTypeDef",
+    "KeyValuePairOutputTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
+    "ManagedScalingOutputTypeDef",
     "ManagedScalingTypeDef",
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
+    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
+    "ClusterSettingOutputTypeDef",
     "ClusterSettingTypeDef",
+    "ContainerDependencyOutputTypeDef",
+    "EnvironmentFileOutputTypeDef",
+    "FirelensConfigurationOutputTypeDef",
+    "HealthCheckOutputTypeDef",
+    "HostEntryOutputTypeDef",
+    "MountPointOutputTypeDef",
+    "PortMappingOutputTypeDef",
+    "RepositoryCredentialsOutputTypeDef",
+    "ResourceRequirementOutputTypeDef",
+    "SecretOutputTypeDef",
+    "SystemControlOutputTypeDef",
+    "UlimitOutputTypeDef",
+    "VolumeFromOutputTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
     "FirelensConfigurationTypeDef",
     "HealthCheckTypeDef",
     "HostEntryTypeDef",
+    "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
     "InstanceHealthCheckResultTypeDef",
-    "ResourceTypeDef",
-    "VersionInfoTypeDef",
+    "ResourceOutputTypeDef",
+    "VersionInfoOutputTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
+    "NetworkBindingOutputTypeDef",
     "NetworkInterfaceTypeDef",
+    "TagTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
+    "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
+    "DeploymentCircuitBreakerOutputTypeDef",
     "DeploymentCircuitBreakerTypeDef",
+    "DeploymentControllerOutputTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
+    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
     "DiscoverPollEndpointResponseTypeDef",
+    "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
+    "EFSAuthorizationConfigOutputTypeDef",
     "EFSAuthorizationConfigTypeDef",
+    "EphemeralStorageOutputTypeDef",
     "EphemeralStorageTypeDef",
+    "ExecuteCommandLogConfigurationOutputTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
+    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
+    "HostVolumePropertiesOutputTypeDef",
     "HostVolumePropertiesTypeDef",
+    "InferenceAcceleratorOutputTypeDef",
+    "InferenceAcceleratorOverrideOutputTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
+    "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
+    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
     "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
     "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
@@ -167,109 +202,135 @@
     "ListTaskDefinitionFamiliesResponseTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
     "ListTaskDefinitionsResponseTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
     "ListTasksResponseTypeDef",
+    "LoadBalancerOutputTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PaginatorConfigTypeDef",
+    "PlacementConstraintOutputTypeDef",
+    "PlacementStrategyOutputTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
+    "ResourceTypeDef",
+    "VersionInfoTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
     "ResponseMetadataTypeDef",
+    "RuntimePlatformOutputTypeDef",
+    "ScaleOutputTypeDef",
+    "ServiceConnectClientAliasOutputTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
+    "ServiceRegistryOutputTypeDef",
     "StopTaskRequestRequestTypeDef",
     "SubmitAttachmentStateChangesResponseTypeDef",
     "SubmitContainerStateChangeResponseTypeDef",
     "SubmitTaskStateChangeResponseTypeDef",
+    "TaskDefinitionPlacementConstraintOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
-    "ProxyConfigurationTypeDef",
-    "DeleteAttributesRequestRequestTypeDef",
+    "ProxyConfigurationOutputTypeDef",
     "DeleteAttributesResponseTypeDef",
     "ListAttributesResponseTypeDef",
-    "PutAttributesRequestRequestTypeDef",
     "PutAttributesResponseTypeDef",
+    "DeleteAttributesRequestRequestTypeDef",
+    "PutAttributesRequestRequestTypeDef",
+    "AutoScalingGroupProviderOutputTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
+    "ContainerOverrideOutputTypeDef",
+    "LogConfigurationOutputTypeDef",
+    "ProxyConfigurationTypeDef",
     "ContainerOverrideTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
+    "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
+    "EFSVolumeConfigurationOutputTypeDef",
     "EFSVolumeConfigurationTypeDef",
+    "ExecuteCommandConfigurationOutputTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
+    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
+    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
+    "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
-    "CreateTaskSetRequestRequestTypeDef",
     "TaskSetTypeDef",
+    "CreateTaskSetRequestRequestTypeDef",
+    "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
+    "ClusterConfigurationOutputTypeDef",
     "ClusterConfigurationTypeDef",
+    "VolumeOutputTypeDef",
     "VolumeTypeDef",
+    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
+    "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
-    "TaskTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
     "TaskDefinitionTypeDef",
-    "CreateServiceRequestRequestTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -292,23 +353,42 @@
     "AttachmentStateChangeTypeDef",
     {
         "attachmentArn": str,
         "status": str,
     },
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
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "value": str,
+        "targetType": Literal["container-instance"],
+        "targetId": str,
+    },
+    total=False,
+)
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "name": str,
     },
 )
 _OptionalAttributeTypeDef = TypedDict(
@@ -320,26 +400,58 @@
     },
     total=False,
 )
 
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+ManagedScalingOutputTypeDef = TypedDict(
+    "ManagedScalingOutputTypeDef",
+    {
+        "status": ManagedScalingStatusType,
+        "targetCapacity": int,
+        "minimumScalingStepSize": int,
+        "maximumScalingStepSize": int,
+        "instanceWarmupPeriod": int,
+    },
+    total=False,
+)
+
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
         "instanceWarmupPeriod": int,
     },
     total=False,
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": AssignPublicIpType,
+    },
+    total=False,
+)
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -352,14 +464,35 @@
 )
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "capacityProvider": str,
+    },
+)
+_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "weight": int,
+        "base": int,
+    },
+    total=False,
+)
+
+class CapacityProviderStrategyItemOutputTypeDef(
+    _RequiredCapacityProviderStrategyItemOutputTypeDef,
+    _OptionalCapacityProviderStrategyItemOutputTypeDef,
+):
+    pass
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -372,16 +505,16 @@
 )
 
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
@@ -396,23 +529,170 @@
     "ClusterServiceConnectDefaultsTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
+ClusterSettingOutputTypeDef = TypedDict(
+    "ClusterSettingOutputTypeDef",
+    {
+        "name": Literal["containerInsights"],
+        "value": str,
+    },
+    total=False,
+)
+
 ClusterSettingTypeDef = TypedDict(
     "ClusterSettingTypeDef",
     {
         "name": Literal["containerInsights"],
         "value": str,
     },
     total=False,
 )
 
+ContainerDependencyOutputTypeDef = TypedDict(
+    "ContainerDependencyOutputTypeDef",
+    {
+        "containerName": str,
+        "condition": ContainerConditionType,
+    },
+)
+
+EnvironmentFileOutputTypeDef = TypedDict(
+    "EnvironmentFileOutputTypeDef",
+    {
+        "value": str,
+        "type": Literal["s3"],
+    },
+)
+
+_RequiredFirelensConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationOutputTypeDef",
+    {
+        "type": FirelensConfigurationTypeType,
+    },
+)
+_OptionalFirelensConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationOutputTypeDef",
+    {
+        "options": Dict[str, str],
+    },
+    total=False,
+)
+
+class FirelensConfigurationOutputTypeDef(
+    _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredHealthCheckOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckOutputTypeDef",
+    {
+        "command": List[str],
+    },
+)
+_OptionalHealthCheckOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckOutputTypeDef",
+    {
+        "interval": int,
+        "timeout": int,
+        "retries": int,
+        "startPeriod": int,
+    },
+    total=False,
+)
+
+class HealthCheckOutputTypeDef(
+    _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
+):
+    pass
+
+HostEntryOutputTypeDef = TypedDict(
+    "HostEntryOutputTypeDef",
+    {
+        "hostname": str,
+        "ipAddress": str,
+    },
+)
+
+MountPointOutputTypeDef = TypedDict(
+    "MountPointOutputTypeDef",
+    {
+        "sourceVolume": str,
+        "containerPath": str,
+        "readOnly": bool,
+    },
+    total=False,
+)
+
+PortMappingOutputTypeDef = TypedDict(
+    "PortMappingOutputTypeDef",
+    {
+        "containerPort": int,
+        "hostPort": int,
+        "protocol": TransportProtocolType,
+        "name": str,
+        "appProtocol": ApplicationProtocolType,
+        "containerPortRange": str,
+    },
+    total=False,
+)
+
+RepositoryCredentialsOutputTypeDef = TypedDict(
+    "RepositoryCredentialsOutputTypeDef",
+    {
+        "credentialsParameter": str,
+    },
+)
+
+ResourceRequirementOutputTypeDef = TypedDict(
+    "ResourceRequirementOutputTypeDef",
+    {
+        "value": str,
+        "type": ResourceTypeType,
+    },
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
+SystemControlOutputTypeDef = TypedDict(
+    "SystemControlOutputTypeDef",
+    {
+        "namespace": str,
+        "value": str,
+    },
+    total=False,
+)
+
+UlimitOutputTypeDef = TypedDict(
+    "UlimitOutputTypeDef",
+    {
+        "name": UlimitNameType,
+        "softLimit": int,
+        "hardLimit": int,
+    },
+)
+
+VolumeFromOutputTypeDef = TypedDict(
+    "VolumeFromOutputTypeDef",
+    {
+        "sourceContainer": str,
+        "readOnly": bool,
+    },
+    total=False,
+)
+
 ContainerDependencyTypeDef = TypedDict(
     "ContainerDependencyTypeDef",
     {
         "containerName": str,
         "condition": ContainerConditionType,
     },
 )
@@ -430,28 +710,28 @@
     {
         "type": FirelensConfigurationTypeType,
     },
 )
 _OptionalFirelensConfigurationTypeDef = TypedDict(
     "_OptionalFirelensConfigurationTypeDef",
     {
-        "options": Dict[str, str],
+        "options": Mapping[str, str],
     },
     total=False,
 )
 
 class FirelensConfigurationTypeDef(
     _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
-        "command": List[str],
+        "command": Sequence[str],
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "interval": int,
         "timeout": int,
@@ -468,14 +748,23 @@
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
 
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
+    {
+        "name": str,
+        "value": str,
+    },
+    total=False,
+)
+
 MountPointTypeDef = TypedDict(
     "MountPointTypeDef",
     {
         "sourceVolume": str,
         "containerPath": str,
         "readOnly": bool,
     },
@@ -552,29 +841,29 @@
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
     {
         "name": str,
         "type": str,
         "doubleValue": float,
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
     },
     total=False,
 )
 
-VersionInfoTypeDef = TypedDict(
-    "VersionInfoTypeDef",
+VersionInfoOutputTypeDef = TypedDict(
+    "VersionInfoOutputTypeDef",
     {
         "agentVersion": str,
         "agentHash": str,
         "dockerVersion": str,
     },
     total=False,
 )
@@ -599,24 +888,46 @@
         "name": Literal["ExecuteCommandAgent"],
         "reason": str,
         "lastStatus": str,
     },
     total=False,
 )
 
+NetworkBindingOutputTypeDef = TypedDict(
+    "NetworkBindingOutputTypeDef",
+    {
+        "bindIP": str,
+        "containerPort": int,
+        "hostPort": int,
+        "protocol": TransportProtocolType,
+        "containerPortRange": str,
+        "hostPortRange": str,
+    },
+    total=False,
+)
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
 )
 
@@ -767,31 +1078,55 @@
 )
 
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
+DeploymentAlarmsOutputTypeDef = TypedDict(
+    "DeploymentAlarmsOutputTypeDef",
+    {
+        "alarmNames": List[str],
+        "enable": bool,
+        "rollback": bool,
+    },
+)
+
 DeploymentAlarmsTypeDef = TypedDict(
     "DeploymentAlarmsTypeDef",
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
     },
 )
 
+DeploymentCircuitBreakerOutputTypeDef = TypedDict(
+    "DeploymentCircuitBreakerOutputTypeDef",
+    {
+        "enable": bool,
+        "rollback": bool,
+    },
+)
+
 DeploymentCircuitBreakerTypeDef = TypedDict(
     "DeploymentCircuitBreakerTypeDef",
     {
         "enable": bool,
         "rollback": bool,
     },
 )
 
+DeploymentControllerOutputTypeDef = TypedDict(
+    "DeploymentControllerOutputTypeDef",
+    {
+        "type": DeploymentControllerTypeType,
+    },
+)
+
 ServiceConnectServiceResourceTypeDef = TypedDict(
     "ServiceConnectServiceResourceTypeDef",
     {
         "discoveryName": str,
         "discoveryArn": str,
     },
     total=False,
@@ -952,25 +1287,43 @@
 )
 
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
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
 
@@ -989,42 +1342,82 @@
         "endpoint": str,
         "telemetryEndpoint": str,
         "serviceConnectEndpoint": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DockerVolumeConfigurationTypeDef = TypedDict(
-    "DockerVolumeConfigurationTypeDef",
+DockerVolumeConfigurationOutputTypeDef = TypedDict(
+    "DockerVolumeConfigurationOutputTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
         "driverOpts": Dict[str, str],
         "labels": Dict[str, str],
     },
     total=False,
 )
 
+DockerVolumeConfigurationTypeDef = TypedDict(
+    "DockerVolumeConfigurationTypeDef",
+    {
+        "scope": ScopeType,
+        "autoprovision": bool,
+        "driver": str,
+        "driverOpts": Mapping[str, str],
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
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
 )
 
+EphemeralStorageOutputTypeDef = TypedDict(
+    "EphemeralStorageOutputTypeDef",
+    {
+        "sizeInGiB": int,
+    },
+)
+
 EphemeralStorageTypeDef = TypedDict(
     "EphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
+ExecuteCommandLogConfigurationOutputTypeDef = TypedDict(
+    "ExecuteCommandLogConfigurationOutputTypeDef",
+    {
+        "cloudWatchLogGroupName": str,
+        "cloudWatchEncryptionEnabled": bool,
+        "s3BucketName": str,
+        "s3EncryptionEnabled": bool,
+        "s3KeyPrefix": str,
+    },
+    total=False,
+)
+
 ExecuteCommandLogConfigurationTypeDef = TypedDict(
     "ExecuteCommandLogConfigurationTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "cloudWatchEncryptionEnabled": bool,
         "s3BucketName": str,
         "s3EncryptionEnabled": bool,
@@ -1061,14 +1454,22 @@
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
     total=False,
 )
 
+FSxWindowsFileServerAuthorizationConfigOutputTypeDef = TypedDict(
+    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
+    {
+        "credentialsParameter": str,
+        "domain": str,
+    },
+)
+
 FSxWindowsFileServerAuthorizationConfigTypeDef = TypedDict(
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     {
         "credentialsParameter": str,
         "domain": str,
     },
 )
@@ -1098,22 +1499,47 @@
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
     total=False,
 )
 
+HostVolumePropertiesOutputTypeDef = TypedDict(
+    "HostVolumePropertiesOutputTypeDef",
+    {
+        "sourcePath": str,
+    },
+    total=False,
+)
+
 HostVolumePropertiesTypeDef = TypedDict(
     "HostVolumePropertiesTypeDef",
     {
         "sourcePath": str,
     },
     total=False,
 )
 
+InferenceAcceleratorOutputTypeDef = TypedDict(
+    "InferenceAcceleratorOutputTypeDef",
+    {
+        "deviceName": str,
+        "deviceType": str,
+    },
+)
+
+InferenceAcceleratorOverrideOutputTypeDef = TypedDict(
+    "InferenceAcceleratorOverrideOutputTypeDef",
+    {
+        "deviceName": str,
+        "deviceType": str,
+    },
+    total=False,
+)
+
 InferenceAcceleratorOverrideTypeDef = TypedDict(
     "InferenceAcceleratorOverrideTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
     total=False,
@@ -1123,34 +1549,61 @@
     "InferenceAcceleratorTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
 )
 
-KernelCapabilitiesTypeDef = TypedDict(
-    "KernelCapabilitiesTypeDef",
+KernelCapabilitiesOutputTypeDef = TypedDict(
+    "KernelCapabilitiesOutputTypeDef",
     {
         "add": List[str],
         "drop": List[str],
     },
     total=False,
 )
 
+KernelCapabilitiesTypeDef = TypedDict(
+    "KernelCapabilitiesTypeDef",
+    {
+        "add": Sequence[str],
+        "drop": Sequence[str],
+    },
+    total=False,
+)
+
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
 
@@ -1470,14 +1923,25 @@
     {
         "taskArns": List[str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoadBalancerOutputTypeDef = TypedDict(
+    "LoadBalancerOutputTypeDef",
+    {
+        "targetGroupArn": str,
+        "loadBalancerName": str,
+        "containerName": str,
+        "containerPort": int,
+    },
+    total=False,
+)
+
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -1501,14 +1965,32 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PlacementConstraintOutputTypeDef = TypedDict(
+    "PlacementConstraintOutputTypeDef",
+    {
+        "type": PlacementConstraintTypeType,
+        "expression": str,
+    },
+    total=False,
+)
+
+PlacementStrategyOutputTypeDef = TypedDict(
+    "PlacementStrategyOutputTypeDef",
+    {
+        "type": PlacementStrategyTypeType,
+        "field": str,
+    },
+    total=False,
+)
+
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1537,14 +2019,37 @@
 )
 
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
+    {
+        "name": str,
+        "type": str,
+        "doubleValue": float,
+        "longValue": int,
+        "integerValue": int,
+        "stringSetValue": Sequence[str],
+    },
+    total=False,
+)
+
+VersionInfoTypeDef = TypedDict(
+    "VersionInfoTypeDef",
+    {
+        "agentVersion": str,
+        "agentHash": str,
+        "dockerVersion": str,
+    },
+    total=False,
+)
+
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -1566,14 +2071,51 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+RuntimePlatformOutputTypeDef = TypedDict(
+    "RuntimePlatformOutputTypeDef",
+    {
+        "cpuArchitecture": CPUArchitectureType,
+        "operatingSystemFamily": OSFamilyType,
+    },
+    total=False,
+)
+
+ScaleOutputTypeDef = TypedDict(
+    "ScaleOutputTypeDef",
+    {
+        "value": float,
+        "unit": Literal["PERCENT"],
+    },
+    total=False,
+)
+
+_RequiredServiceConnectClientAliasOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectClientAliasOutputTypeDef",
+    {
+        "port": int,
+    },
+)
+_OptionalServiceConnectClientAliasOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectClientAliasOutputTypeDef",
+    {
+        "dnsName": str,
+    },
+    total=False,
+)
+
+class ServiceConnectClientAliasOutputTypeDef(
+    _RequiredServiceConnectClientAliasOutputTypeDef, _OptionalServiceConnectClientAliasOutputTypeDef
+):
+    pass
+
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -1595,14 +2137,25 @@
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
     total=False,
 )
 
+ServiceRegistryOutputTypeDef = TypedDict(
+    "ServiceRegistryOutputTypeDef",
+    {
+        "registryArn": str,
+        "port": int,
+        "containerName": str,
+        "containerPort": int,
+    },
+    total=False,
+)
+
 _RequiredStopTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStopTaskRequestRequestTypeDef",
     {
         "task": str,
     },
 )
 _OptionalStopTaskRequestRequestTypeDef = TypedDict(
@@ -1639,14 +2192,23 @@
     "SubmitTaskStateChangeResponseTypeDef",
     {
         "acknowledgment": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TaskDefinitionPlacementConstraintOutputTypeDef = TypedDict(
+    "TaskDefinitionPlacementConstraintOutputTypeDef",
+    {
+        "type": Literal["memberOf"],
+        "expression": str,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1745,39 +2307,64 @@
 
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
-        "details": List[KeyValuePairTypeDef],
+        "details": List[KeyValuePairOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredProxyConfigurationTypeDef = TypedDict(
-    "_RequiredProxyConfigurationTypeDef",
+_RequiredProxyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredProxyConfigurationOutputTypeDef",
     {
         "containerName": str,
     },
 )
-_OptionalProxyConfigurationTypeDef = TypedDict(
-    "_OptionalProxyConfigurationTypeDef",
+_OptionalProxyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalProxyConfigurationOutputTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairTypeDef],
+        "properties": List[KeyValuePairOutputTypeDef],
     },
     total=False,
 )
 
-class ProxyConfigurationTypeDef(
-    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
+class ProxyConfigurationOutputTypeDef(
+    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
 ):
     pass
 
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
@@ -1789,31 +2376,14 @@
 )
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
@@ -1825,22 +2395,34 @@
 )
 
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
+_RequiredAutoScalingGroupProviderOutputTypeDef = TypedDict(
+    "_RequiredAutoScalingGroupProviderOutputTypeDef",
     {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "autoScalingGroupArn": str,
+    },
+)
+_OptionalAutoScalingGroupProviderOutputTypeDef = TypedDict(
+    "_OptionalAutoScalingGroupProviderOutputTypeDef",
+    {
+        "managedScaling": ManagedScalingOutputTypeDef,
+        "managedTerminationProtection": ManagedTerminationProtectionType,
     },
+    total=False,
 )
 
+class AutoScalingGroupProviderOutputTypeDef(
+    _RequiredAutoScalingGroupProviderOutputTypeDef, _OptionalAutoScalingGroupProviderOutputTypeDef
+):
+    pass
+
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1862,14 +2444,22 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1882,46 +2472,93 @@
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
 UpdateClusterSettingsRequestRequestTypeDef = TypedDict(
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
         "settings": Sequence[ClusterSettingTypeDef],
     },
 )
 
+ContainerOverrideOutputTypeDef = TypedDict(
+    "ContainerOverrideOutputTypeDef",
+    {
+        "name": str,
+        "command": List[str],
+        "environment": List[KeyValuePairOutputTypeDef],
+        "environmentFiles": List[EnvironmentFileOutputTypeDef],
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+    },
+    total=False,
+)
+
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
+_RequiredProxyConfigurationTypeDef = TypedDict(
+    "_RequiredProxyConfigurationTypeDef",
+    {
+        "containerName": str,
+    },
+)
+_OptionalProxyConfigurationTypeDef = TypedDict(
+    "_OptionalProxyConfigurationTypeDef",
+    {
+        "type": Literal["APPMESH"],
+        "properties": Sequence[KeyValuePairTypeDef],
+    },
+    total=False,
+)
+
+class ProxyConfigurationTypeDef(
+    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
+):
+    pass
+
 ContainerOverrideTypeDef = TypedDict(
     "ContainerOverrideTypeDef",
     {
         "name": str,
-        "command": List[str],
-        "environment": List[KeyValuePairTypeDef],
-        "environmentFiles": List[EnvironmentFileTypeDef],
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
-        "resourceRequirements": List[ResourceRequirementTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
@@ -1986,26 +2623,34 @@
         "name": str,
         "image": str,
         "imageDigest": str,
         "runtimeId": str,
         "lastStatus": str,
         "exitCode": int,
         "reason": str,
-        "networkBindings": List[NetworkBindingTypeDef],
+        "networkBindings": List[NetworkBindingOutputTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "healthStatus": HealthStatusType,
         "managedAgents": List[ManagedAgentTypeDef],
         "cpu": str,
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
         "scale": ScaleTypeDef,
@@ -2041,14 +2686,25 @@
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentConfigurationOutputTypeDef = TypedDict(
+    "DeploymentConfigurationOutputTypeDef",
+    {
+        "deploymentCircuitBreaker": DeploymentCircuitBreakerOutputTypeDef,
+        "maximumPercent": int,
+        "minimumHealthyPercent": int,
+        "alarms": DeploymentAlarmsOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsTypeDef,
@@ -2140,14 +2796,36 @@
 
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
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
@@ -2162,14 +2840,24 @@
 )
 
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
+ExecuteCommandConfigurationOutputTypeDef = TypedDict(
+    "ExecuteCommandConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+        "logging": ExecuteCommandLoggingType,
+        "logConfiguration": ExecuteCommandLogConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2185,14 +2873,23 @@
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FSxWindowsFileServerVolumeConfigurationOutputTypeDef = TypedDict(
+    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
+    {
+        "fileSystemId": str,
+        "rootDirectory": str,
+        "authorizationConfig": FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
+    },
+)
+
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
         "rootDirectory": str,
         "authorizationConfig": FSxWindowsFileServerAuthorizationConfigTypeDef,
     },
@@ -2212,22 +2909,36 @@
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LinuxParametersOutputTypeDef = TypedDict(
+    "LinuxParametersOutputTypeDef",
+    {
+        "capabilities": KernelCapabilitiesOutputTypeDef,
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
         "capabilities": KernelCapabilitiesTypeDef,
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
 
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
@@ -2242,14 +2953,35 @@
         "attributes": Sequence[AttributeTypeDef],
         "platformDevices": Sequence[PlatformDeviceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredServiceConnectServiceOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectServiceOutputTypeDef",
+    {
+        "portName": str,
+    },
+)
+_OptionalServiceConnectServiceOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectServiceOutputTypeDef",
+    {
+        "discoveryName": str,
+        "clientAliases": List[ServiceConnectClientAliasOutputTypeDef],
+        "ingressPortOverride": int,
+    },
+    total=False,
+)
+
+class ServiceConnectServiceOutputTypeDef(
+    _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
+):
+    pass
+
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2269,18 +3001,18 @@
 
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
-        "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
+        "autoScalingGroupProvider": AutoScalingGroupProviderOutputTypeDef,
         "updateStatus": CapacityProviderUpdateStatusType,
         "updateStatusReason": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateCapacityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCapacityProviderRequestRequestTypeDef",
     {
@@ -2306,14 +3038,45 @@
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
 
+TaskSetTypeDef = TypedDict(
+    "TaskSetTypeDef",
+    {
+        "id": str,
+        "taskSetArn": str,
+        "serviceArn": str,
+        "clusterArn": str,
+        "startedBy": str,
+        "externalId": str,
+        "status": str,
+        "taskDefinition": str,
+        "computedDesiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "loadBalancers": List[LoadBalancerOutputTypeDef],
+        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
+        "scale": ScaleOutputTypeDef,
+        "stabilityStatus": StabilityStatusType,
+        "stabilityStatusAt": datetime,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
         "service": str,
         "cluster": str,
         "taskDefinition": str,
     },
@@ -2336,51 +3099,34 @@
 )
 
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
-TaskSetTypeDef = TypedDict(
-    "TaskSetTypeDef",
+TaskOverrideOutputTypeDef = TypedDict(
+    "TaskOverrideOutputTypeDef",
     {
-        "id": str,
-        "taskSetArn": str,
-        "serviceArn": str,
-        "clusterArn": str,
-        "startedBy": str,
-        "externalId": str,
-        "status": str,
-        "taskDefinition": str,
-        "computedDesiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "scale": ScaleTypeDef,
-        "stabilityStatus": StabilityStatusType,
-        "stabilityStatusAt": datetime,
-        "tags": List[TagTypeDef],
+        "containerOverrides": List[ContainerOverrideOutputTypeDef],
+        "cpu": str,
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideOutputTypeDef],
+        "executionRoleArn": str,
+        "memory": str,
+        "taskRoleArn": str,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
-        "containerOverrides": List[ContainerOverrideTypeDef],
+        "containerOverrides": Sequence[ContainerOverrideTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
+        "inferenceAcceleratorOverrides": Sequence[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
@@ -2388,27 +3134,27 @@
 ContainerInstanceTypeDef = TypedDict(
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
-        "versionInfo": VersionInfoTypeDef,
-        "remainingResources": List[ResourceTypeDef],
-        "registeredResources": List[ResourceTypeDef],
+        "versionInfo": VersionInfoOutputTypeDef,
+        "remainingResources": List[ResourceOutputTypeDef],
+        "registeredResources": List[ResourceOutputTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
-        "attributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
         "registeredAt": datetime,
         "attachments": List[AttachmentTypeDef],
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "healthStatus": ContainerInstanceHealthStatusTypeDef,
     },
     total=False,
 )
 
 SubmitTaskStateChangeRequestRequestTypeDef = TypedDict(
     "SubmitTaskStateChangeRequestRequestTypeDef",
@@ -2423,81 +3169,172 @@
         "pullStartedAt": Union[datetime, str],
         "pullStoppedAt": Union[datetime, str],
         "executionStoppedAt": Union[datetime, str],
     },
     total=False,
 )
 
+ClusterConfigurationOutputTypeDef = TypedDict(
+    "ClusterConfigurationOutputTypeDef",
+    {
+        "executeCommandConfiguration": ExecuteCommandConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
+VolumeOutputTypeDef = TypedDict(
+    "VolumeOutputTypeDef",
+    {
+        "name": str,
+        "host": HostVolumePropertiesOutputTypeDef,
+        "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
+        "efsVolumeConfiguration": EFSVolumeConfigurationOutputTypeDef,
+        "fsxWindowsFileServerVolumeConfiguration": (
+            FSxWindowsFileServerVolumeConfigurationOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "name": str,
         "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationTypeDef,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
         "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionTypeDef = TypedDict(
-    "ContainerDefinitionTypeDef",
+ContainerDefinitionOutputTypeDef = TypedDict(
+    "ContainerDefinitionOutputTypeDef",
     {
         "name": str,
         "image": str,
-        "repositoryCredentials": RepositoryCredentialsTypeDef,
+        "repositoryCredentials": RepositoryCredentialsOutputTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "links": List[str],
-        "portMappings": List[PortMappingTypeDef],
+        "portMappings": List[PortMappingOutputTypeDef],
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
-        "environment": List[KeyValuePairTypeDef],
-        "environmentFiles": List[EnvironmentFileTypeDef],
-        "mountPoints": List[MountPointTypeDef],
-        "volumesFrom": List[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
-        "secrets": List[SecretTypeDef],
-        "dependsOn": List[ContainerDependencyTypeDef],
+        "environment": List[KeyValuePairOutputTypeDef],
+        "environmentFiles": List[EnvironmentFileOutputTypeDef],
+        "mountPoints": List[MountPointOutputTypeDef],
+        "volumesFrom": List[VolumeFromOutputTypeDef],
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "secrets": List[SecretOutputTypeDef],
+        "dependsOn": List[ContainerDependencyOutputTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
         "disableNetworking": bool,
         "privileged": bool,
         "readonlyRootFilesystem": bool,
         "dnsServers": List[str],
         "dnsSearchDomains": List[str],
-        "extraHosts": List[HostEntryTypeDef],
+        "extraHosts": List[HostEntryOutputTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
-        "ulimits": List[UlimitTypeDef],
+        "ulimits": List[UlimitOutputTypeDef],
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "healthCheck": HealthCheckOutputTypeDef,
+        "systemControls": List[SystemControlOutputTypeDef],
+        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "firelensConfiguration": FirelensConfigurationOutputTypeDef,
+        "credentialSpecs": List[str],
+    },
+    total=False,
+)
+
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
+    {
+        "name": str,
+        "image": str,
+        "repositoryCredentials": RepositoryCredentialsTypeDef,
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "links": Sequence[str],
+        "portMappings": Sequence[PortMappingTypeDef],
+        "essential": bool,
+        "entryPoint": Sequence[str],
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
+        "mountPoints": Sequence[MountPointTypeDef],
+        "volumesFrom": Sequence[VolumeFromTypeDef],
+        "linuxParameters": LinuxParametersTypeDef,
+        "secrets": Sequence[SecretTypeDef],
+        "dependsOn": Sequence[ContainerDependencyTypeDef],
+        "startTimeout": int,
+        "stopTimeout": int,
+        "hostname": str,
+        "user": str,
+        "workingDirectory": str,
+        "disableNetworking": bool,
+        "privileged": bool,
+        "readonlyRootFilesystem": bool,
+        "dnsServers": Sequence[str],
+        "dnsSearchDomains": Sequence[str],
+        "extraHosts": Sequence[HostEntryTypeDef],
+        "dockerSecurityOptions": Sequence[str],
+        "interactive": bool,
+        "pseudoTerminal": bool,
+        "dockerLabels": Mapping[str, str],
+        "ulimits": Sequence[UlimitTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
         "healthCheck": HealthCheckTypeDef,
-        "systemControls": List[SystemControlTypeDef],
-        "resourceRequirements": List[ResourceRequirementTypeDef],
+        "systemControls": Sequence[SystemControlTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
-        "credentialSpecs": List[str],
+        "credentialSpecs": Sequence[str],
     },
     total=False,
 )
 
+_RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectConfigurationOutputTypeDef",
+    {
+        "namespace": str,
+        "services": List[ServiceConnectServiceOutputTypeDef],
+        "logConfiguration": LogConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class ServiceConnectConfigurationOutputTypeDef(
+    _RequiredServiceConnectConfigurationOutputTypeDef,
+    _OptionalServiceConnectConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -2586,14 +3423,57 @@
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TaskTypeDef = TypedDict(
+    "TaskTypeDef",
+    {
+        "attachments": List[AttachmentTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
+        "availabilityZone": str,
+        "capacityProviderName": str,
+        "clusterArn": str,
+        "connectivity": ConnectivityType,
+        "connectivityAt": datetime,
+        "containerInstanceArn": str,
+        "containers": List[ContainerTypeDef],
+        "cpu": str,
+        "createdAt": datetime,
+        "desiredStatus": str,
+        "enableExecuteCommand": bool,
+        "executionStoppedAt": datetime,
+        "group": str,
+        "healthStatus": HealthStatusType,
+        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "lastStatus": str,
+        "launchType": LaunchTypeType,
+        "memory": str,
+        "overrides": TaskOverrideOutputTypeDef,
+        "platformVersion": str,
+        "platformFamily": str,
+        "pullStartedAt": datetime,
+        "pullStoppedAt": datetime,
+        "startedAt": datetime,
+        "startedBy": str,
+        "stopCode": TaskStopCodeType,
+        "stoppedAt": datetime,
+        "stoppedReason": str,
+        "stoppingAt": datetime,
+        "tags": List[TagOutputTypeDef],
+        "taskArn": str,
+        "taskDefinitionArn": str,
+        "version": int,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 _OptionalRunTaskRequestRequestTypeDef = TypedDict(
@@ -2649,57 +3529,14 @@
 )
 
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
-TaskTypeDef = TypedDict(
-    "TaskTypeDef",
-    {
-        "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeTypeDef],
-        "availabilityZone": str,
-        "capacityProviderName": str,
-        "clusterArn": str,
-        "connectivity": ConnectivityType,
-        "connectivityAt": datetime,
-        "containerInstanceArn": str,
-        "containers": List[ContainerTypeDef],
-        "cpu": str,
-        "createdAt": datetime,
-        "desiredStatus": str,
-        "enableExecuteCommand": bool,
-        "executionStoppedAt": datetime,
-        "group": str,
-        "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "lastStatus": str,
-        "launchType": LaunchTypeType,
-        "memory": str,
-        "overrides": TaskOverrideTypeDef,
-        "platformVersion": str,
-        "platformFamily": str,
-        "pullStartedAt": datetime,
-        "pullStoppedAt": datetime,
-        "startedAt": datetime,
-        "startedBy": str,
-        "stopCode": TaskStopCodeType,
-        "stoppedAt": datetime,
-        "stoppedReason": str,
-        "stoppingAt": datetime,
-        "tags": List[TagTypeDef],
-        "taskArn": str,
-        "taskDefinitionArn": str,
-        "version": int,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
-
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2739,25 +3576,25 @@
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
-        "configuration": ClusterConfigurationTypeDef,
+        "configuration": ClusterConfigurationOutputTypeDef,
         "status": str,
         "registeredContainerInstancesCount": int,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "activeServicesCount": int,
-        "statistics": List[KeyValuePairTypeDef],
-        "tags": List[TagTypeDef],
-        "settings": List[ClusterSettingTypeDef],
+        "statistics": List[KeyValuePairOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "settings": List[ClusterSettingOutputTypeDef],
         "capacityProviders": List[str],
-        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
         "attachments": List[AttachmentTypeDef],
         "attachmentsStatus": str,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsTypeDef,
     },
     total=False,
 )
 
@@ -2792,14 +3629,45 @@
 )
 
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
+TaskDefinitionTypeDef = TypedDict(
+    "TaskDefinitionTypeDef",
+    {
+        "taskDefinitionArn": str,
+        "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
+        "family": str,
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "revision": int,
+        "volumes": List[VolumeOutputTypeDef],
+        "status": TaskDefinitionStatusType,
+        "requiresAttributes": List[AttributeOutputTypeDef],
+        "placementConstraints": List[TaskDefinitionPlacementConstraintOutputTypeDef],
+        "compatibilities": List[CompatibilityType],
+        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "requiresCompatibilities": List[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "registeredAt": datetime,
+        "deregisteredAt": datetime,
+        "registeredBy": str,
+        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "family": str,
         "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
     },
 )
@@ -2827,41 +3695,35 @@
 
 class RegisterTaskDefinitionRequestRequestTypeDef(
     _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
     _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-TaskDefinitionTypeDef = TypedDict(
-    "TaskDefinitionTypeDef",
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
     {
-        "taskDefinitionArn": str,
-        "containerDefinitions": List[ContainerDefinitionTypeDef],
-        "family": str,
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "revision": int,
-        "volumes": List[VolumeTypeDef],
-        "status": TaskDefinitionStatusType,
-        "requiresAttributes": List[AttributeTypeDef],
-        "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
-        "compatibilities": List[CompatibilityType],
-        "runtimePlatform": RuntimePlatformTypeDef,
-        "requiresCompatibilities": List[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "registeredAt": datetime,
-        "deregisteredAt": datetime,
-        "registeredBy": str,
-        "ephemeralStorage": EphemeralStorageTypeDef,
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
@@ -2898,39 +3760,14 @@
 )
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
-        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -3063,58 +3900,58 @@
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "loadBalancers": List[LoadBalancerOutputTypeDef],
+        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
         "status": str,
         "desiredCount": int,
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
-        "placementConstraints": List[PlacementConstraintTypeDef],
-        "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "placementConstraints": List[PlacementConstraintOutputTypeDef],
+        "placementStrategy": List[PlacementStrategyOutputTypeDef],
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerTypeDef,
-        "tags": List[TagTypeDef],
+        "deploymentController": DeploymentControllerOutputTypeDef,
+        "tags": List[TagOutputTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/PKG-INFO` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.0
-Summary: Type annotations for boto3.ECS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ECS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ecs"></a>
 
 # mypy-boto3-ecs
 
 [![PyPI - mypy-boto3-ecs](https://img.shields.io/pypi/v/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -445,85 +445,120 @@
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
-    KeyValuePairTypeDef,
+    KeyValuePairOutputTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
+    ManagedScalingOutputTypeDef,
     ManagedScalingTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
+    ClusterSettingOutputTypeDef,
     ClusterSettingTypeDef,
+    ContainerDependencyOutputTypeDef,
+    EnvironmentFileOutputTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
+    HostEntryOutputTypeDef,
+    MountPointOutputTypeDef,
+    PortMappingOutputTypeDef,
+    RepositoryCredentialsOutputTypeDef,
+    ResourceRequirementOutputTypeDef,
+    SecretOutputTypeDef,
+    SystemControlOutputTypeDef,
+    UlimitOutputTypeDef,
+    VolumeFromOutputTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
     FirelensConfigurationTypeDef,
     HealthCheckTypeDef,
     HostEntryTypeDef,
+    KeyValuePairTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
     InstanceHealthCheckResultTypeDef,
-    ResourceTypeDef,
-    VersionInfoTypeDef,
+    ResourceOutputTypeDef,
+    VersionInfoOutputTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
+    NetworkBindingOutputTypeDef,
     NetworkInterfaceTypeDef,
+    TagTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
+    DeploymentCircuitBreakerOutputTypeDef,
     DeploymentCircuitBreakerTypeDef,
+    DeploymentControllerOutputTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
     DiscoverPollEndpointResponseTypeDef,
+    DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
+    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
+    EphemeralStorageOutputTypeDef,
     EphemeralStorageTypeDef,
+    ExecuteCommandLogConfigurationOutputTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
+    FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
+    HostVolumePropertiesOutputTypeDef,
     HostVolumePropertiesTypeDef,
+    InferenceAcceleratorOutputTypeDef,
+    InferenceAcceleratorOverrideOutputTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
+    KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
     ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
     ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
@@ -543,109 +578,135 @@
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
     ListTasksResponseTypeDef,
+    LoadBalancerOutputTypeDef,
     ManagedAgentStateChangeTypeDef,
     PaginatorConfigTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
+    ResourceTypeDef,
+    VersionInfoTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
     ResponseMetadataTypeDef,
+    RuntimePlatformOutputTypeDef,
+    ScaleOutputTypeDef,
+    ServiceConnectClientAliasOutputTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
+    ServiceRegistryOutputTypeDef,
     StopTaskRequestRequestTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
+    TaskDefinitionPlacementConstraintOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
-    ProxyConfigurationTypeDef,
-    DeleteAttributesRequestRequestTypeDef,
+    ProxyConfigurationOutputTypeDef,
     DeleteAttributesResponseTypeDef,
     ListAttributesResponseTypeDef,
-    PutAttributesRequestRequestTypeDef,
     PutAttributesResponseTypeDef,
+    DeleteAttributesRequestRequestTypeDef,
+    PutAttributesRequestRequestTypeDef,
+    AutoScalingGroupProviderOutputTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
+    ContainerOverrideOutputTypeDef,
+    LogConfigurationOutputTypeDef,
+    ProxyConfigurationTypeDef,
     ContainerOverrideTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
+    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
+    ExecuteCommandConfigurationOutputTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
+    FSxWindowsFileServerVolumeConfigurationOutputTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
-    CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
+    CreateTaskSetRequestRequestTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    ClusterConfigurationOutputTypeDef,
     ClusterConfigurationTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
+    TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
-    TaskTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceRequestRequestTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
+    CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
```

### Comparing `mypy-boto3-ecs-1.28.0/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.0/setup.py` & `mypy-boto3-ecs-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ECS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

