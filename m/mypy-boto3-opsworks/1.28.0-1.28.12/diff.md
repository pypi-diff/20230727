# Comparing `tmp/mypy-boto3-opsworks-1.28.0.tar.gz` & `tmp/mypy-boto3-opsworks-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworks-1.28.0.tar", last modified: Thu Jul  6 21:00:14 2023, max compression
+gzip compressed data, was "mypy-boto3-opsworks-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-opsworks-1.28.0.tar` & `mypy-boto3-opsworks-1.28.12.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.858385 mypy-boto3-opsworks-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-07-06 21:00:14.858385 mypy-boto3-opsworks-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.854385 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51761 2023-07-06 20:48:44.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51673 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-07-06 20:48:47.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-07-06 20:48:46.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-06 20:48:46.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:48:46.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-07-06 20:48:46.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-07-06 20:48:44.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    64297 2023-07-06 20:48:49.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64230 2023-07-06 20:48:48.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-06 20:48:46.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-06 20:48:46.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.858385 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-07-06 21:00:14.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 21:00:14.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:14.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:14.000000 mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:14.858385 mypy-boto3-opsworks-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:48:43.000000 mypy-boto3-opsworks-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.829133 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51761 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51673 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19590 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    70410 2023-07-27 11:41:02.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70335 2023-07-27 11:41:01.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/setup.py
```

### Comparing `mypy-boto3-opsworks-1.28.0/LICENSE` & `mypy-boto3-opsworks-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/PKG-INFO` & `mypy-boto3-opsworks-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.0
-Summary: Type annotations for boto3.OpsWorks 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpsWorks 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworks?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,55 +438,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
-    StackConfigurationManagerTypeDef,
-    DataSourceTypeDef,
-    EnvironmentVariableTypeDef,
-    SourceTypeDef,
-    SslConfigurationTypeDef,
+    StackConfigurationManagerOutputTypeDef,
+    DataSourceOutputTypeDef,
+    EnvironmentVariableOutputTypeDef,
+    SourceOutputTypeDef,
+    SslConfigurationOutputTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
+    AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
+    EbsBlockDeviceOutputTypeDef,
     EbsBlockDeviceTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
-    CloneStackResultTypeDef,
+    SourceTypeDef,
+    StackConfigurationManagerTypeDef,
+    CloudWatchLogsLogStreamOutputTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
-    CreateAppResultTypeDef,
+    DataSourceTypeDef,
+    EnvironmentVariableTypeDef,
+    SslConfigurationTypeDef,
     DeploymentCommandTypeDef,
-    CreateDeploymentResultTypeDef,
-    CreateInstanceResultTypeDef,
     RecipesTypeDef,
     VolumeConfigurationTypeDef,
-    CreateLayerResultTypeDef,
-    CreateStackResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
+    DeploymentCommandOutputTypeDef,
     DeregisterEcsClusterRequestRequestTypeDef,
     DeregisterElasticIpRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DeregisterRdsDbInstanceRequestRequestTypeDef,
     DeregisterVolumeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAppsRequestRequestTypeDef,
     DescribeCommandsRequestRequestTypeDef,
     DescribeDeploymentsRequestRequestTypeDef,
-    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEcsClustersRequestRequestTypeDef,
     EcsClusterTypeDef,
     DescribeElasticIpsRequestRequestTypeDef,
     ElasticIpTypeDef,
     DescribeElasticLoadBalancersRequestRequestTypeDef,
     ElasticLoadBalancerTypeDef,
     DescribeInstancesRequestRequestTypeDef,
@@ -498,129 +501,143 @@
     DescribeRaidArraysRequestRequestTypeDef,
     RaidArrayTypeDef,
     DescribeRdsDbInstancesRequestRequestTypeDef,
     RdsDbInstanceTypeDef,
     DescribeServiceErrorsRequestRequestTypeDef,
     ServiceErrorTypeDef,
     DescribeStackProvisioningParametersRequestRequestTypeDef,
-    DescribeStackProvisioningParametersResultTypeDef,
     DescribeStackSummaryRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeTimeBasedAutoScalingRequestRequestTypeDef,
     DescribeUserProfilesRequestRequestTypeDef,
     UserProfileTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     VolumeTypeDef,
     DetachElasticLoadBalancerRequestRequestTypeDef,
     DisassociateElasticIpRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionRequestRequestTypeDef,
-    GetHostnameSuggestionResultTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
-    InstancesCountResponseMetadataTypeDef,
     InstancesCountTypeDef,
+    RecipesOutputTypeDef,
+    VolumeConfigurationOutputTypeDef,
+    ShutdownEventConfigurationOutputTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResultTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
-    PaginatorConfigTypeDef,
     RebootInstanceRequestRequestTypeDef,
-    RecipesResponseMetadataTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
-    RegisterEcsClusterResultTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
-    RegisterElasticIpResultTypeDef,
-    RegisterInstanceResultTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
     RegisterVolumeRequestRequestTypeDef,
-    RegisterVolumeResultTypeDef,
-    ResponseMetadataTypeDef,
     SetPermissionRequestRequestTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartStackRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopStackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    WeeklyAutoScalingScheduleOutputTypeDef,
     UnassignInstanceRequestRequestTypeDef,
     UnassignVolumeRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateElasticIpRequestRequestTypeDef,
     UpdateInstanceRequestRequestTypeDef,
     UpdateMyUserProfileRequestRequestTypeDef,
     UpdateRdsDbInstanceRequestRequestTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
-    DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
+    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
+    StackTypeDef,
+    ChefConfigurationResponseMetadataTypeDef,
+    CloneStackResultTypeDef,
+    CreateAppResultTypeDef,
+    CreateDeploymentResultTypeDef,
+    CreateInstanceResultTypeDef,
+    CreateLayerResultTypeDef,
+    CreateStackResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DescribeStackProvisioningParametersResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetHostnameSuggestionResultTypeDef,
+    InstancesCountResponseMetadataTypeDef,
+    ListTagsResultTypeDef,
+    RecipesResponseMetadataTypeDef,
+    RegisterEcsClusterResultTypeDef,
+    RegisterElasticIpResultTypeDef,
+    RegisterInstanceResultTypeDef,
+    RegisterVolumeResultTypeDef,
+    SourceResponseMetadataTypeDef,
+    StackConfigurationManagerResponseMetadataTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
-    StackTypeDef,
+    DescribeAgentVersionsRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
+    CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
+    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
     DescribeMyUserProfileResultTypeDef,
     DescribePermissionsResultTypeDef,
     DescribeRaidArraysResultTypeDef,
     DescribeRdsDbInstancesResultTypeDef,
     DescribeServiceErrorsResultTypeDef,
     DescribeUserProfilesResultTypeDef,
     DescribeVolumesResultTypeDef,
     GrantAccessResultTypeDef,
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
+    LifecycleEventConfigurationOutputTypeDef,
     LifecycleEventConfigurationResponseMetadataTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
-    CreateInstanceRequestRequestTypeDef,
     InstanceTypeDef,
+    CreateInstanceRequestRequestTypeDef,
     DescribeStacksResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
+    LayerTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
-    LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerTypeDef:
+def get_structure() -> StackConfigurationManagerOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.0/README.md` & `mypy-boto3-opsworks-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworks?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,55 +406,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
-    StackConfigurationManagerTypeDef,
-    DataSourceTypeDef,
-    EnvironmentVariableTypeDef,
-    SourceTypeDef,
-    SslConfigurationTypeDef,
+    StackConfigurationManagerOutputTypeDef,
+    DataSourceOutputTypeDef,
+    EnvironmentVariableOutputTypeDef,
+    SourceOutputTypeDef,
+    SslConfigurationOutputTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
+    AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
+    EbsBlockDeviceOutputTypeDef,
     EbsBlockDeviceTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
-    CloneStackResultTypeDef,
+    SourceTypeDef,
+    StackConfigurationManagerTypeDef,
+    CloudWatchLogsLogStreamOutputTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
-    CreateAppResultTypeDef,
+    DataSourceTypeDef,
+    EnvironmentVariableTypeDef,
+    SslConfigurationTypeDef,
     DeploymentCommandTypeDef,
-    CreateDeploymentResultTypeDef,
-    CreateInstanceResultTypeDef,
     RecipesTypeDef,
     VolumeConfigurationTypeDef,
-    CreateLayerResultTypeDef,
-    CreateStackResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
+    DeploymentCommandOutputTypeDef,
     DeregisterEcsClusterRequestRequestTypeDef,
     DeregisterElasticIpRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DeregisterRdsDbInstanceRequestRequestTypeDef,
     DeregisterVolumeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAppsRequestRequestTypeDef,
     DescribeCommandsRequestRequestTypeDef,
     DescribeDeploymentsRequestRequestTypeDef,
-    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEcsClustersRequestRequestTypeDef,
     EcsClusterTypeDef,
     DescribeElasticIpsRequestRequestTypeDef,
     ElasticIpTypeDef,
     DescribeElasticLoadBalancersRequestRequestTypeDef,
     ElasticLoadBalancerTypeDef,
     DescribeInstancesRequestRequestTypeDef,
@@ -466,129 +469,143 @@
     DescribeRaidArraysRequestRequestTypeDef,
     RaidArrayTypeDef,
     DescribeRdsDbInstancesRequestRequestTypeDef,
     RdsDbInstanceTypeDef,
     DescribeServiceErrorsRequestRequestTypeDef,
     ServiceErrorTypeDef,
     DescribeStackProvisioningParametersRequestRequestTypeDef,
-    DescribeStackProvisioningParametersResultTypeDef,
     DescribeStackSummaryRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeTimeBasedAutoScalingRequestRequestTypeDef,
     DescribeUserProfilesRequestRequestTypeDef,
     UserProfileTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     VolumeTypeDef,
     DetachElasticLoadBalancerRequestRequestTypeDef,
     DisassociateElasticIpRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionRequestRequestTypeDef,
-    GetHostnameSuggestionResultTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
-    InstancesCountResponseMetadataTypeDef,
     InstancesCountTypeDef,
+    RecipesOutputTypeDef,
+    VolumeConfigurationOutputTypeDef,
+    ShutdownEventConfigurationOutputTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResultTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
-    PaginatorConfigTypeDef,
     RebootInstanceRequestRequestTypeDef,
-    RecipesResponseMetadataTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
-    RegisterEcsClusterResultTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
-    RegisterElasticIpResultTypeDef,
-    RegisterInstanceResultTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
     RegisterVolumeRequestRequestTypeDef,
-    RegisterVolumeResultTypeDef,
-    ResponseMetadataTypeDef,
     SetPermissionRequestRequestTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartStackRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopStackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    WeeklyAutoScalingScheduleOutputTypeDef,
     UnassignInstanceRequestRequestTypeDef,
     UnassignVolumeRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateElasticIpRequestRequestTypeDef,
     UpdateInstanceRequestRequestTypeDef,
     UpdateMyUserProfileRequestRequestTypeDef,
     UpdateRdsDbInstanceRequestRequestTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
-    DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
+    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
+    StackTypeDef,
+    ChefConfigurationResponseMetadataTypeDef,
+    CloneStackResultTypeDef,
+    CreateAppResultTypeDef,
+    CreateDeploymentResultTypeDef,
+    CreateInstanceResultTypeDef,
+    CreateLayerResultTypeDef,
+    CreateStackResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DescribeStackProvisioningParametersResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetHostnameSuggestionResultTypeDef,
+    InstancesCountResponseMetadataTypeDef,
+    ListTagsResultTypeDef,
+    RecipesResponseMetadataTypeDef,
+    RegisterEcsClusterResultTypeDef,
+    RegisterElasticIpResultTypeDef,
+    RegisterInstanceResultTypeDef,
+    RegisterVolumeResultTypeDef,
+    SourceResponseMetadataTypeDef,
+    StackConfigurationManagerResponseMetadataTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
-    StackTypeDef,
+    DescribeAgentVersionsRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
+    CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
+    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
     DescribeMyUserProfileResultTypeDef,
     DescribePermissionsResultTypeDef,
     DescribeRaidArraysResultTypeDef,
     DescribeRdsDbInstancesResultTypeDef,
     DescribeServiceErrorsResultTypeDef,
     DescribeUserProfilesResultTypeDef,
     DescribeVolumesResultTypeDef,
     GrantAccessResultTypeDef,
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
+    LifecycleEventConfigurationOutputTypeDef,
     LifecycleEventConfigurationResponseMetadataTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
-    CreateInstanceRequestRequestTypeDef,
     InstanceTypeDef,
+    CreateInstanceRequestRequestTypeDef,
     DescribeStacksResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
+    LayerTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
-    LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerTypeDef:
+def get_structure() -> StackConfigurationManagerOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/__init__.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/__init__.pyi` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/__main__.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorks 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.OpsWorks 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
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

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/client.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/client.pyi` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/literals.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,15 @@
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
@@ -422,26 +423,28 @@
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

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/literals.pyi` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -334,14 +334,15 @@
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
@@ -420,26 +421,28 @@
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

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/paginator.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/paginator.pyi` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,13 +42,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/service_resource.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     LifecycleEventConfigurationTypeDef,
     RecipesResponseMetadataTypeDef,
     RecipesTypeDef,
     SourceResponseMetadataTypeDef,
     SourceTypeDef,
     StackConfigurationManagerResponseMetadataTypeDef,
     StackConfigurationManagerTypeDef,
+    VolumeConfigurationOutputTypeDef,
     VolumeConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -166,15 +167,15 @@
     attributes: Dict[LayerAttributesKeysType, str]
     cloud_watch_logs_configuration: CloudWatchLogsConfigurationResponseMetadataTypeDef
     custom_instance_profile_arn: str
     custom_json: str
     custom_security_group_ids: List[str]
     default_security_group_names: List[str]
     packages: List[str]
-    volume_configurations: List[VolumeConfigurationTypeDef]
+    volume_configurations: List[VolumeConfigurationOutputTypeDef]
     enable_auto_healing: bool
     auto_assign_elastic_ips: bool
     auto_assign_public_ips: bool
     default_recipes: RecipesResponseMetadataTypeDef
     custom_recipes: RecipesResponseMetadataTypeDef
     created_at: str
     install_updates_on_boot: bool
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/service_resource.pyi` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     LifecycleEventConfigurationTypeDef,
     RecipesResponseMetadataTypeDef,
     RecipesTypeDef,
     SourceResponseMetadataTypeDef,
     SourceTypeDef,
     StackConfigurationManagerResponseMetadataTypeDef,
     StackConfigurationManagerTypeDef,
+    VolumeConfigurationOutputTypeDef,
     VolumeConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -152,15 +153,15 @@
     attributes: Dict[LayerAttributesKeysType, str]
     cloud_watch_logs_configuration: CloudWatchLogsConfigurationResponseMetadataTypeDef
     custom_instance_profile_arn: str
     custom_json: str
     custom_security_group_ids: List[str]
     default_security_group_names: List[str]
     packages: List[str]
-    volume_configurations: List[VolumeConfigurationTypeDef]
+    volume_configurations: List[VolumeConfigurationOutputTypeDef]
     enable_auto_healing: bool
     auto_assign_elastic_ips: bool
     auto_assign_public_ips: bool
     default_recipes: RecipesResponseMetadataTypeDef
     custom_recipes: RecipesResponseMetadataTypeDef
     created_at: str
     install_updates_on_boot: bool
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/type_defs.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opsworks service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
+    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerOutputTypeDef
 
-    data: StackConfigurationManagerTypeDef = {...}
+    data: StackConfigurationManagerOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AppAttributesKeysType,
@@ -38,55 +38,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "StackConfigurationManagerTypeDef",
-    "DataSourceTypeDef",
-    "EnvironmentVariableTypeDef",
-    "SourceTypeDef",
-    "SslConfigurationTypeDef",
+    "StackConfigurationManagerOutputTypeDef",
+    "DataSourceOutputTypeDef",
+    "EnvironmentVariableOutputTypeDef",
+    "SourceOutputTypeDef",
+    "SslConfigurationOutputTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
+    "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
+    "EbsBlockDeviceOutputTypeDef",
     "EbsBlockDeviceTypeDef",
-    "ChefConfigurationResponseMetadataTypeDef",
+    "ChefConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
-    "CloneStackResultTypeDef",
+    "SourceTypeDef",
+    "StackConfigurationManagerTypeDef",
+    "CloudWatchLogsLogStreamOutputTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
-    "CreateAppResultTypeDef",
+    "DataSourceTypeDef",
+    "EnvironmentVariableTypeDef",
+    "SslConfigurationTypeDef",
     "DeploymentCommandTypeDef",
-    "CreateDeploymentResultTypeDef",
-    "CreateInstanceResultTypeDef",
     "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
-    "CreateLayerResultTypeDef",
-    "CreateStackResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
-    "CreateUserProfileResultTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
+    "DeploymentCommandOutputTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
     "DescribeCommandsRequestRequestTypeDef",
     "DescribeDeploymentsRequestRequestTypeDef",
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEcsClustersRequestRequestTypeDef",
     "EcsClusterTypeDef",
     "DescribeElasticIpsRequestRequestTypeDef",
     "ElasticIpTypeDef",
     "DescribeElasticLoadBalancersRequestRequestTypeDef",
     "ElasticLoadBalancerTypeDef",
     "DescribeInstancesRequestRequestTypeDef",
@@ -98,198 +101,214 @@
     "DescribeRaidArraysRequestRequestTypeDef",
     "RaidArrayTypeDef",
     "DescribeRdsDbInstancesRequestRequestTypeDef",
     "RdsDbInstanceTypeDef",
     "DescribeServiceErrorsRequestRequestTypeDef",
     "ServiceErrorTypeDef",
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
-    "DescribeStackProvisioningParametersResultTypeDef",
     "DescribeStackSummaryRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeTimeBasedAutoScalingRequestRequestTypeDef",
     "DescribeUserProfilesRequestRequestTypeDef",
     "UserProfileTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "VolumeTypeDef",
     "DetachElasticLoadBalancerRequestRequestTypeDef",
     "DisassociateElasticIpRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
-    "GetHostnameSuggestionResultTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
-    "InstancesCountResponseMetadataTypeDef",
     "InstancesCountTypeDef",
+    "RecipesOutputTypeDef",
+    "VolumeConfigurationOutputTypeDef",
+    "ShutdownEventConfigurationOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTagsResultTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
-    "PaginatorConfigTypeDef",
     "RebootInstanceRequestRequestTypeDef",
-    "RecipesResponseMetadataTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
-    "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
-    "RegisterElasticIpResultTypeDef",
-    "RegisterInstanceResultTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     "RegisterVolumeRequestRequestTypeDef",
-    "RegisterVolumeResultTypeDef",
-    "ResponseMetadataTypeDef",
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
-    "SourceResponseMetadataTypeDef",
-    "StackConfigurationManagerResponseMetadataTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "WeeklyAutoScalingScheduleOutputTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
-    "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
+    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
+    "StackTypeDef",
+    "ChefConfigurationResponseMetadataTypeDef",
+    "CloneStackResultTypeDef",
+    "CreateAppResultTypeDef",
+    "CreateDeploymentResultTypeDef",
+    "CreateInstanceResultTypeDef",
+    "CreateLayerResultTypeDef",
+    "CreateStackResultTypeDef",
+    "CreateUserProfileResultTypeDef",
+    "DescribeStackProvisioningParametersResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetHostnameSuggestionResultTypeDef",
+    "InstancesCountResponseMetadataTypeDef",
+    "ListTagsResultTypeDef",
+    "RecipesResponseMetadataTypeDef",
+    "RegisterEcsClusterResultTypeDef",
+    "RegisterElasticIpResultTypeDef",
+    "RegisterInstanceResultTypeDef",
+    "RegisterVolumeResultTypeDef",
+    "SourceResponseMetadataTypeDef",
+    "StackConfigurationManagerResponseMetadataTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
-    "StackTypeDef",
+    "DescribeAgentVersionsRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
+    "CloudWatchLogsConfigurationOutputTypeDef",
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     "DescribeEcsClustersResultTypeDef",
     "DescribeElasticIpsResultTypeDef",
     "DescribeElasticLoadBalancersResultTypeDef",
     "DescribeMyUserProfileResultTypeDef",
     "DescribePermissionsResultTypeDef",
     "DescribeRaidArraysResultTypeDef",
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
+    "LifecycleEventConfigurationOutputTypeDef",
     "LifecycleEventConfigurationResponseMetadataTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
-    "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
+    "CreateInstanceRequestRequestTypeDef",
     "DescribeStacksResultTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
+    "LayerTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
-    "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
     "DescribeTimeBasedAutoScalingResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "DescribeLayersResultTypeDef",
 )
 
-StackConfigurationManagerTypeDef = TypedDict(
-    "StackConfigurationManagerTypeDef",
+StackConfigurationManagerOutputTypeDef = TypedDict(
+    "StackConfigurationManagerOutputTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
     {
         "Type": str,
         "Arn": str,
         "DatabaseName": str,
     },
     total=False,
 )
 
-_RequiredEnvironmentVariableTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableTypeDef",
+_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
-_OptionalEnvironmentVariableTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableTypeDef",
+_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableOutputTypeDef",
     {
         "Secure": bool,
     },
     total=False,
 )
 
 
-class EnvironmentVariableTypeDef(
-    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
+class EnvironmentVariableOutputTypeDef(
+    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
 ):
     pass
 
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
         "SshKey": str,
         "Revision": str,
     },
     total=False,
 )
 
-_RequiredSslConfigurationTypeDef = TypedDict(
-    "_RequiredSslConfigurationTypeDef",
+_RequiredSslConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSslConfigurationOutputTypeDef",
     {
         "Certificate": str,
         "PrivateKey": str,
     },
 )
-_OptionalSslConfigurationTypeDef = TypedDict(
-    "_OptionalSslConfigurationTypeDef",
+_OptionalSslConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSslConfigurationOutputTypeDef",
     {
         "Chain": str,
     },
     total=False,
 )
 
 
-class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
+class SslConfigurationOutputTypeDef(
+    _RequiredSslConfigurationOutputTypeDef, _OptionalSslConfigurationOutputTypeDef
+):
     pass
 
 
 AssignInstanceRequestRequestTypeDef = TypedDict(
     "AssignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -344,24 +363,50 @@
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
 
+AutoScalingThresholdsOutputTypeDef = TypedDict(
+    "AutoScalingThresholdsOutputTypeDef",
+    {
+        "InstanceCount": int,
+        "ThresholdsWaitTime": int,
+        "IgnoreMetricsTime": int,
+        "CpuThreshold": float,
+        "MemoryThreshold": float,
+        "LoadThreshold": float,
+        "Alarms": List[str],
+    },
+    total=False,
+)
+
 AutoScalingThresholdsTypeDef = TypedDict(
     "AutoScalingThresholdsTypeDef",
     {
         "InstanceCount": int,
         "ThresholdsWaitTime": int,
         "IgnoreMetricsTime": int,
         "CpuThreshold": float,
         "MemoryThreshold": float,
         "LoadThreshold": float,
-        "Alarms": List[str],
+        "Alarms": Sequence[str],
+    },
+    total=False,
+)
+
+EbsBlockDeviceOutputTypeDef = TypedDict(
+    "EbsBlockDeviceOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "Iops": int,
+        "VolumeSize": int,
+        "VolumeType": VolumeTypeType,
+        "DeleteOnTermination": bool,
     },
     total=False,
 )
 
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
@@ -370,38 +415,81 @@
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "DeleteOnTermination": bool,
     },
     total=False,
 )
 
-ChefConfigurationResponseMetadataTypeDef = TypedDict(
-    "ChefConfigurationResponseMetadataTypeDef",
+ChefConfigurationOutputTypeDef = TypedDict(
+    "ChefConfigurationOutputTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
     },
 )
 
 ChefConfigurationTypeDef = TypedDict(
     "ChefConfigurationTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
     },
     total=False,
 )
 
-CloneStackResultTypeDef = TypedDict(
-    "CloneStackResultTypeDef",
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
     {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": SourceTypeType,
+        "Url": str,
+        "Username": str,
+        "Password": str,
+        "SshKey": str,
+        "Revision": str,
     },
+    total=False,
+)
+
+StackConfigurationManagerTypeDef = TypedDict(
+    "StackConfigurationManagerTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+CloudWatchLogsLogStreamOutputTypeDef = TypedDict(
+    "CloudWatchLogsLogStreamOutputTypeDef",
+    {
+        "LogGroupName": str,
+        "DatetimeFormat": str,
+        "TimeZone": CloudWatchLogsTimeZoneType,
+        "File": str,
+        "FileFingerprintLines": str,
+        "MultiLineStartPattern": str,
+        "InitialPosition": CloudWatchLogsInitialPositionType,
+        "Encoding": CloudWatchLogsEncodingType,
+        "BufferDuration": int,
+        "BatchCount": int,
+        "BatchSize": int,
+    },
+    total=False,
 )
 
 CloudWatchLogsLogStreamTypeDef = TypedDict(
     "CloudWatchLogsLogStreamTypeDef",
     {
         "LogGroupName": str,
         "DatetimeFormat": str,
@@ -431,59 +519,87 @@
         "ExitCode": int,
         "LogUrl": str,
         "Type": str,
     },
     total=False,
 )
 
-CreateAppResultTypeDef = TypedDict(
-    "CreateAppResultTypeDef",
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
     {
-        "AppId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": str,
+        "Arn": str,
+        "DatabaseName": str,
     },
+    total=False,
 )
 
-_RequiredDeploymentCommandTypeDef = TypedDict(
-    "_RequiredDeploymentCommandTypeDef",
+_RequiredEnvironmentVariableTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableTypeDef",
     {
-        "Name": DeploymentCommandNameType,
+        "Key": str,
+        "Value": str,
     },
 )
-_OptionalDeploymentCommandTypeDef = TypedDict(
-    "_OptionalDeploymentCommandTypeDef",
+_OptionalEnvironmentVariableTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableTypeDef",
     {
-        "Args": Mapping[str, Sequence[str]],
+        "Secure": bool,
     },
     total=False,
 )
 
 
-class DeploymentCommandTypeDef(
-    _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
+class EnvironmentVariableTypeDef(
+    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
 
-CreateDeploymentResultTypeDef = TypedDict(
-    "CreateDeploymentResultTypeDef",
+_RequiredSslConfigurationTypeDef = TypedDict(
+    "_RequiredSslConfigurationTypeDef",
     {
-        "DeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Certificate": str,
+        "PrivateKey": str,
+    },
+)
+_OptionalSslConfigurationTypeDef = TypedDict(
+    "_OptionalSslConfigurationTypeDef",
+    {
+        "Chain": str,
     },
+    total=False,
 )
 
-CreateInstanceResultTypeDef = TypedDict(
-    "CreateInstanceResultTypeDef",
+
+class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
+    pass
+
+
+_RequiredDeploymentCommandTypeDef = TypedDict(
+    "_RequiredDeploymentCommandTypeDef",
     {
-        "InstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": DeploymentCommandNameType,
+    },
+)
+_OptionalDeploymentCommandTypeDef = TypedDict(
+    "_OptionalDeploymentCommandTypeDef",
+    {
+        "Args": Mapping[str, Sequence[str]],
     },
+    total=False,
 )
 
+
+class DeploymentCommandTypeDef(
+    _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
+):
+    pass
+
+
 RecipesTypeDef = TypedDict(
     "RecipesTypeDef",
     {
         "Setup": Sequence[str],
         "Configure": Sequence[str],
         "Deploy": Sequence[str],
         "Undeploy": Sequence[str],
@@ -514,30 +630,14 @@
 
 class VolumeConfigurationTypeDef(
     _RequiredVolumeConfigurationTypeDef, _OptionalVolumeConfigurationTypeDef
 ):
     pass
 
 
-CreateLayerResultTypeDef = TypedDict(
-    "CreateLayerResultTypeDef",
-    {
-        "LayerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackResultTypeDef = TypedDict(
-    "CreateStackResultTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 _OptionalCreateUserProfileRequestRequestTypeDef = TypedDict(
@@ -553,22 +653,14 @@
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "IamUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAppRequestRequestTypeDef = TypedDict(
     "DeleteAppRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 
@@ -611,14 +703,35 @@
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 
+_RequiredDeploymentCommandOutputTypeDef = TypedDict(
+    "_RequiredDeploymentCommandOutputTypeDef",
+    {
+        "Name": DeploymentCommandNameType,
+    },
+)
+_OptionalDeploymentCommandOutputTypeDef = TypedDict(
+    "_OptionalDeploymentCommandOutputTypeDef",
+    {
+        "Args": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+
+class DeploymentCommandOutputTypeDef(
+    _RequiredDeploymentCommandOutputTypeDef, _OptionalDeploymentCommandOutputTypeDef
+):
+    pass
+
+
 DeregisterEcsClusterRequestRequestTypeDef = TypedDict(
     "DeregisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
     },
 )
 
@@ -684,20 +797,20 @@
         "StackId": str,
         "AppId": str,
         "DeploymentIds": Sequence[str],
     },
     total=False,
 )
 
-DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EcsClusterArns": Sequence[str],
-        "StackId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEcsClustersRequestRequestTypeDef = TypedDict(
     "DescribeEcsClustersRequestRequestTypeDef",
     {
@@ -919,23 +1032,14 @@
 DescribeStackProvisioningParametersRequestRequestTypeDef = TypedDict(
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
-DescribeStackProvisioningParametersResultTypeDef = TypedDict(
-    "DescribeStackProvisioningParametersResultTypeDef",
-    {
-        "AgentInstallerUrl": str,
-        "Parameters": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStackSummaryRequestRequestTypeDef = TypedDict(
     "DescribeStackSummaryRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
@@ -1017,37 +1121,21 @@
 DisassociateElasticIpRequestRequestTypeDef = TypedDict(
     "DisassociateElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHostnameSuggestionRequestRequestTypeDef = TypedDict(
     "GetHostnameSuggestionRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 
-GetHostnameSuggestionResultTypeDef = TypedDict(
-    "GetHostnameSuggestionResultTypeDef",
-    {
-        "LayerId": str,
-        "Hostname": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGrantAccessRequestRequestTypeDef = TypedDict(
     "_RequiredGrantAccessRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalGrantAccessRequestRequestTypeDef = TypedDict(
@@ -1091,16 +1179,16 @@
         "Family": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-InstancesCountResponseMetadataTypeDef = TypedDict(
-    "InstancesCountResponseMetadataTypeDef",
+InstancesCountTypeDef = TypedDict(
+    "InstancesCountTypeDef",
     {
         "Assigning": int,
         "Booting": int,
         "ConnectionLost": int,
         "Deregistering": int,
         "Online": int,
         "Pending": int,
@@ -1114,41 +1202,61 @@
         "StartFailed": int,
         "StopFailed": int,
         "Stopped": int,
         "Stopping": int,
         "Terminated": int,
         "Terminating": int,
         "Unassigning": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-InstancesCountTypeDef = TypedDict(
-    "InstancesCountTypeDef",
+RecipesOutputTypeDef = TypedDict(
+    "RecipesOutputTypeDef",
     {
-        "Assigning": int,
-        "Booting": int,
-        "ConnectionLost": int,
-        "Deregistering": int,
-        "Online": int,
-        "Pending": int,
-        "Rebooting": int,
-        "Registered": int,
-        "Registering": int,
-        "Requested": int,
-        "RunningSetup": int,
-        "SetupFailed": int,
-        "ShuttingDown": int,
-        "StartFailed": int,
-        "StopFailed": int,
-        "Stopped": int,
-        "Stopping": int,
-        "Terminated": int,
-        "Terminating": int,
-        "Unassigning": int,
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+    },
+    total=False,
+)
+
+_RequiredVolumeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVolumeConfigurationOutputTypeDef",
+    {
+        "MountPoint": str,
+        "NumberOfDisks": int,
+        "Size": int,
+    },
+)
+_OptionalVolumeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVolumeConfigurationOutputTypeDef",
+    {
+        "RaidLevel": int,
+        "VolumeType": str,
+        "Iops": int,
+        "Encrypted": bool,
+    },
+    total=False,
+)
+
+
+class VolumeConfigurationOutputTypeDef(
+    _RequiredVolumeConfigurationOutputTypeDef, _OptionalVolumeConfigurationOutputTypeDef
+):
+    pass
+
+
+ShutdownEventConfigurationOutputTypeDef = TypedDict(
+    "ShutdownEventConfigurationOutputTypeDef",
+    {
+        "ExecutionTimeout": int,
+        "DelayUntilElbConnectionsDrained": bool,
     },
     total=False,
 )
 
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
@@ -1176,101 +1284,46 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsResultTypeDef = TypedDict(
-    "ListTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OperatingSystemConfigurationManagerTypeDef = TypedDict(
     "OperatingSystemConfigurationManagerTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 RebootInstanceRequestRequestTypeDef = TypedDict(
     "RebootInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-RecipesResponseMetadataTypeDef = TypedDict(
-    "RecipesResponseMetadataTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterEcsClusterRequestRequestTypeDef = TypedDict(
     "RegisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
         "StackId": str,
     },
 )
 
-RegisterEcsClusterResultTypeDef = TypedDict(
-    "RegisterEcsClusterResultTypeDef",
-    {
-        "EcsClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterElasticIpRequestRequestTypeDef = TypedDict(
     "RegisterElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
         "StackId": str,
     },
 )
 
-RegisterElasticIpResultTypeDef = TypedDict(
-    "RegisterElasticIpResultTypeDef",
-    {
-        "ElasticIp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterInstanceResultTypeDef = TypedDict(
-    "RegisterInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterRdsDbInstanceRequestRequestTypeDef = TypedDict(
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     {
         "StackId": str,
         "RdsDbInstanceArn": str,
         "DbUser": str,
         "DbPassword": str,
@@ -1294,33 +1347,14 @@
 
 class RegisterVolumeRequestRequestTypeDef(
     _RequiredRegisterVolumeRequestRequestTypeDef, _OptionalRegisterVolumeRequestRequestTypeDef
 ):
     pass
 
 
-RegisterVolumeResultTypeDef = TypedDict(
-    "RegisterVolumeResultTypeDef",
-    {
-        "VolumeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredSetPermissionRequestRequestTypeDef",
     {
         "StackId": str,
         "IamUserArn": str,
     },
 )
@@ -1340,47 +1374,25 @@
 ):
     pass
 
 
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
-        "Monday": Dict[str, str],
-        "Tuesday": Dict[str, str],
-        "Wednesday": Dict[str, str],
-        "Thursday": Dict[str, str],
-        "Friday": Dict[str, str],
-        "Saturday": Dict[str, str],
-        "Sunday": Dict[str, str],
+        "Monday": Mapping[str, str],
+        "Tuesday": Mapping[str, str],
+        "Wednesday": Mapping[str, str],
+        "Thursday": Mapping[str, str],
+        "Friday": Mapping[str, str],
+        "Saturday": Mapping[str, str],
+        "Sunday": Mapping[str, str],
     },
     total=False,
 )
 
-SourceResponseMetadataTypeDef = TypedDict(
-    "SourceResponseMetadataTypeDef",
-    {
-        "Type": SourceTypeType,
-        "Url": str,
-        "Username": str,
-        "Password": str,
-        "SshKey": str,
-        "Revision": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
-    "StackConfigurationManagerResponseMetadataTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1423,14 +1435,28 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+WeeklyAutoScalingScheduleOutputTypeDef = TypedDict(
+    "WeeklyAutoScalingScheduleOutputTypeDef",
+    {
+        "Monday": Dict[str, str],
+        "Tuesday": Dict[str, str],
+        "Wednesday": Dict[str, str],
+        "Thursday": Dict[str, str],
+        "Friday": Dict[str, str],
+        "Saturday": Dict[str, str],
+        "Sunday": Dict[str, str],
+    },
+    total=False,
+)
+
 UnassignInstanceRequestRequestTypeDef = TypedDict(
     "UnassignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1577,154 +1603,316 @@
     pass
 
 
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "Version": str,
-        "ConfigurationManager": StackConfigurationManagerTypeDef,
-    },
-    total=False,
-)
-
-DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentVersionsRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "ConfigurationManager": StackConfigurationManagerTypeDef,
+        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppId": str,
         "StackId": str,
         "Shortname": str,
         "Name": str,
         "Description": str,
-        "DataSources": List[DataSourceTypeDef],
+        "DataSources": List[DataSourceOutputTypeDef],
         "Type": AppTypeType,
-        "AppSource": SourceTypeDef,
+        "AppSource": SourceOutputTypeDef,
         "Domains": List[str],
         "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
+        "SslConfiguration": SslConfigurationOutputTypeDef,
         "Attributes": Dict[AppAttributesKeysType, str],
         "CreatedAt": str,
-        "Environment": List[EnvironmentVariableTypeDef],
+        "Environment": List[EnvironmentVariableOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
+LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
+    "LoadBasedAutoScalingConfigurationTypeDef",
     {
-        "StackId": str,
-        "Name": str,
-        "Type": AppTypeType,
+        "LayerId": str,
+        "Enable": bool,
+        "UpScaling": AutoScalingThresholdsOutputTypeDef,
+        "DownScaling": AutoScalingThresholdsOutputTypeDef,
     },
+    total=False,
 )
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
+
+_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
+    "_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef",
     {
-        "Shortname": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
+        "LayerId": str,
+    },
+)
+_OptionalSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
+    "_OptionalSetLoadBasedAutoScalingRequestRequestTypeDef",
+    {
+        "Enable": bool,
+        "UpScaling": AutoScalingThresholdsTypeDef,
+        "DownScaling": AutoScalingThresholdsTypeDef,
     },
     total=False,
 )
 
 
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+class SetLoadBasedAutoScalingRequestRequestTypeDef(
+    _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef,
+    _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
+BlockDeviceMappingOutputTypeDef = TypedDict(
+    "BlockDeviceMappingOutputTypeDef",
     {
-        "AppId": str,
+        "DeviceName": str,
+        "NoDevice": str,
+        "VirtualName": str,
+        "Ebs": EbsBlockDeviceOutputTypeDef,
     },
+    total=False,
 )
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
+
+BlockDeviceMappingTypeDef = TypedDict(
+    "BlockDeviceMappingTypeDef",
     {
+        "DeviceName": str,
+        "NoDevice": str,
+        "VirtualName": str,
+        "Ebs": EbsBlockDeviceTypeDef,
+    },
+    total=False,
+)
+
+StackTypeDef = TypedDict(
+    "StackTypeDef",
+    {
+        "StackId": str,
         "Name": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "Type": AppTypeType,
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
+        "Arn": str,
+        "Region": str,
+        "VpcId": str,
+        "Attributes": Dict[Literal["Color"], str],
+        "ServiceRoleArn": str,
+        "DefaultInstanceProfileArn": str,
+        "DefaultOs": str,
+        "HostnameTheme": str,
+        "DefaultAvailabilityZone": str,
+        "DefaultSubnetId": str,
+        "CustomJson": str,
+        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
+        "ChefConfiguration": ChefConfigurationOutputTypeDef,
+        "UseCustomCookbooks": bool,
+        "UseOpsworksSecurityGroups": bool,
+        "CustomCookbooksSource": SourceOutputTypeDef,
+        "DefaultSshKeyName": str,
+        "CreatedAt": str,
+        "DefaultRootDeviceType": RootDeviceTypeType,
+        "AgentVersion": str,
     },
     total=False,
 )
 
+ChefConfigurationResponseMetadataTypeDef = TypedDict(
+    "ChefConfigurationResponseMetadataTypeDef",
+    {
+        "ManageBerkshelf": bool,
+        "BerkshelfVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
+CloneStackResultTypeDef = TypedDict(
+    "CloneStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+CreateAppResultTypeDef = TypedDict(
+    "CreateAppResultTypeDef",
+    {
+        "AppId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
-    "LoadBasedAutoScalingConfigurationTypeDef",
+CreateDeploymentResultTypeDef = TypedDict(
+    "CreateDeploymentResultTypeDef",
+    {
+        "DeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInstanceResultTypeDef = TypedDict(
+    "CreateInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayerResultTypeDef = TypedDict(
+    "CreateLayerResultTypeDef",
     {
         "LayerId": str,
-        "Enable": bool,
-        "UpScaling": AutoScalingThresholdsTypeDef,
-        "DownScaling": AutoScalingThresholdsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
-    "_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef",
+CreateStackResultTypeDef = TypedDict(
+    "CreateStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "IamUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackProvisioningParametersResultTypeDef = TypedDict(
+    "DescribeStackProvisioningParametersResultTypeDef",
+    {
+        "AgentInstallerUrl": str,
+        "Parameters": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHostnameSuggestionResultTypeDef = TypedDict(
+    "GetHostnameSuggestionResultTypeDef",
     {
         "LayerId": str,
+        "Hostname": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
-    "_OptionalSetLoadBasedAutoScalingRequestRequestTypeDef",
+
+InstancesCountResponseMetadataTypeDef = TypedDict(
+    "InstancesCountResponseMetadataTypeDef",
     {
-        "Enable": bool,
-        "UpScaling": AutoScalingThresholdsTypeDef,
-        "DownScaling": AutoScalingThresholdsTypeDef,
+        "Assigning": int,
+        "Booting": int,
+        "ConnectionLost": int,
+        "Deregistering": int,
+        "Online": int,
+        "Pending": int,
+        "Rebooting": int,
+        "Registered": int,
+        "Registering": int,
+        "Requested": int,
+        "RunningSetup": int,
+        "SetupFailed": int,
+        "ShuttingDown": int,
+        "StartFailed": int,
+        "StopFailed": int,
+        "Stopped": int,
+        "Stopping": int,
+        "Terminated": int,
+        "Terminating": int,
+        "Unassigning": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTagsResultTypeDef = TypedDict(
+    "ListTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class SetLoadBasedAutoScalingRequestRequestTypeDef(
-    _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef,
-    _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef,
-):
-    pass
+RecipesResponseMetadataTypeDef = TypedDict(
+    "RecipesResponseMetadataTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+RegisterEcsClusterResultTypeDef = TypedDict(
+    "RegisterEcsClusterResultTypeDef",
+    {
+        "EcsClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-BlockDeviceMappingTypeDef = TypedDict(
-    "BlockDeviceMappingTypeDef",
+RegisterElasticIpResultTypeDef = TypedDict(
+    "RegisterElasticIpResultTypeDef",
     {
-        "DeviceName": str,
-        "NoDevice": str,
-        "VirtualName": str,
-        "Ebs": EbsBlockDeviceTypeDef,
+        "ElasticIp": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterInstanceResultTypeDef = TypedDict(
+    "RegisterInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterVolumeResultTypeDef = TypedDict(
+    "RegisterVolumeResultTypeDef",
+    {
+        "VolumeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SourceResponseMetadataTypeDef = TypedDict(
+    "SourceResponseMetadataTypeDef",
+    {
+        "Type": SourceTypeType,
+        "Url": str,
+        "Username": str,
+        "Password": str,
+        "SshKey": str,
+        "Revision": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
+    "StackConfigurationManagerResponseMetadataTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCloneStackRequestRequestTypeDef = TypedDict(
     "_RequiredCloneStackRequestRequestTypeDef",
     {
         "SourceStackId": str,
         "ServiceRoleArn": str,
@@ -1837,39 +2025,19 @@
 class CreateStackRequestServiceResourceCreateStackTypeDef(
     _RequiredCreateStackRequestServiceResourceCreateStackTypeDef,
     _OptionalCreateStackRequestServiceResourceCreateStackTypeDef,
 ):
     pass
 
 
-StackTypeDef = TypedDict(
-    "StackTypeDef",
+DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentVersionsRequestRequestTypeDef",
     {
         "StackId": str,
-        "Name": str,
-        "Arn": str,
-        "Region": str,
-        "VpcId": str,
-        "Attributes": Dict[Literal["Color"], str],
-        "ServiceRoleArn": str,
-        "DefaultInstanceProfileArn": str,
-        "DefaultOs": str,
-        "HostnameTheme": str,
-        "DefaultAvailabilityZone": str,
-        "DefaultSubnetId": str,
-        "CustomJson": str,
         "ConfigurationManager": StackConfigurationManagerTypeDef,
-        "ChefConfiguration": ChefConfigurationTypeDef,
-        "UseCustomCookbooks": bool,
-        "UseOpsworksSecurityGroups": bool,
-        "CustomCookbooksSource": SourceTypeDef,
-        "DefaultSshKeyName": str,
-        "CreatedAt": str,
-        "DefaultRootDeviceType": RootDeviceTypeType,
-        "AgentVersion": str,
     },
     total=False,
 )
 
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
@@ -1903,20 +2071,29 @@
 
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
 
+CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLogsConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
+    },
+    total=False,
+)
+
 CloudWatchLogsConfigurationResponseMetadataTypeDef = TypedDict(
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
@@ -1925,17 +2102,78 @@
     total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "Name": str,
+        "Type": AppTypeType,
     },
 )
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "Shortname": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "AppId": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "Type": AppTypeType,
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "StackId": str,
         "Command": DeploymentCommandTypeDef,
     },
@@ -1966,15 +2204,15 @@
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
         "CompletedAt": str,
         "Duration": int,
         "IamUserArn": str,
         "Comment": str,
-        "Command": DeploymentCommandTypeDef,
+        "Command": DeploymentCommandOutputTypeDef,
         "Status": str,
         "CustomJson": str,
         "InstanceIds": List[str],
     },
     total=False,
 )
 
@@ -2039,100 +2277,110 @@
         "LayerId": str,
         "InstanceIds": Sequence[str],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
+    {
+        "EcsClusterArns": Sequence[str],
+        "StackId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEcsClustersResultTypeDef = TypedDict(
     "DescribeEcsClustersResultTypeDef",
     {
         "EcsClusters": List[EcsClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticIpsResultTypeDef = TypedDict(
     "DescribeElasticIpsResultTypeDef",
     {
         "ElasticIps": List[ElasticIpTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticLoadBalancersResultTypeDef = TypedDict(
     "DescribeElasticLoadBalancersResultTypeDef",
     {
         "ElasticLoadBalancers": List[ElasticLoadBalancerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMyUserProfileResultTypeDef = TypedDict(
     "DescribeMyUserProfileResultTypeDef",
     {
         "UserProfile": SelfUserProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePermissionsResultTypeDef = TypedDict(
     "DescribePermissionsResultTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRaidArraysResultTypeDef = TypedDict(
     "DescribeRaidArraysResultTypeDef",
     {
         "RaidArrays": List[RaidArrayTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRdsDbInstancesResultTypeDef = TypedDict(
     "DescribeRdsDbInstancesResultTypeDef",
     {
         "RdsDbInstances": List[RdsDbInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceErrorsResultTypeDef = TypedDict(
     "DescribeServiceErrorsResultTypeDef",
     {
         "ServiceErrors": List[ServiceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserProfilesResultTypeDef = TypedDict(
     "DescribeUserProfilesResultTypeDef",
     {
         "UserProfiles": List[UserProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVolumesResultTypeDef = TypedDict(
     "DescribeVolumesResultTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GrantAccessResultTypeDef = TypedDict(
     "GrantAccessResultTypeDef",
     {
         "TemporaryCredential": TemporaryCredentialTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2167,19 +2415,27 @@
         "LayersCount": int,
         "AppsCount": int,
         "InstancesCount": InstancesCountTypeDef,
     },
     total=False,
 )
 
+LifecycleEventConfigurationOutputTypeDef = TypedDict(
+    "LifecycleEventConfigurationOutputTypeDef",
+    {
+        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LifecycleEventConfigurationResponseMetadataTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseMetadataTypeDef",
     {
-        "Shutdown": ShutdownEventConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleEventConfigurationTypeDef = TypedDict(
     "LifecycleEventConfigurationTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
@@ -2223,90 +2479,53 @@
     pass
 
 
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": str,
-        "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
+        "AutoScalingSchedule": WeeklyAutoScalingScheduleOutputTypeDef,
     },
     total=False,
 )
 
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppsResultTypeDef = TypedDict(
     "DescribeAppsResultTypeDef",
     {
         "Apps": List[AppTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeLoadBasedAutoScalingResultTypeDef",
     {
         "LoadBasedAutoScalingConfigurations": List[LoadBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "LayerIds": Sequence[str],
-        "InstanceType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceRequestRequestTypeDef",
-    {
-        "AutoScalingType": AutoScalingTypeType,
-        "Hostname": str,
-        "Os": str,
-        "AmiId": str,
-        "SshKeyName": str,
-        "AvailabilityZone": str,
-        "VirtualizationType": str,
-        "SubnetId": str,
-        "Architecture": ArchitectureType,
-        "RootDeviceType": RootDeviceTypeType,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "InstallUpdatesOnBoot": bool,
-        "EbsOptimized": bool,
-        "AgentVersion": str,
-        "Tenancy": str,
-    },
-    total=False,
-)
-
-
-class CreateInstanceRequestRequestTypeDef(
-    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
-):
-    pass
-
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AgentVersion": str,
         "AmiId": str,
         "Architecture": ArchitectureType,
         "Arn": str,
         "AutoScalingType": AutoScalingTypeType,
         "AvailabilityZone": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
+        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
         "CreatedAt": str,
         "EbsOptimized": bool,
         "Ec2InstanceId": str,
         "EcsClusterArn": str,
         "EcsContainerInstanceArn": str,
         "ElasticIp": str,
         "Hostname": str,
@@ -2337,36 +2556,103 @@
         "SubnetId": str,
         "Tenancy": str,
         "VirtualizationType": VirtualizationTypeType,
     },
     total=False,
 )
 
+_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "LayerIds": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceRequestRequestTypeDef",
+    {
+        "AutoScalingType": AutoScalingTypeType,
+        "Hostname": str,
+        "Os": str,
+        "AmiId": str,
+        "SshKeyName": str,
+        "AvailabilityZone": str,
+        "VirtualizationType": str,
+        "SubnetId": str,
+        "Architecture": ArchitectureType,
+        "RootDeviceType": RootDeviceTypeType,
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "InstallUpdatesOnBoot": bool,
+        "EbsOptimized": bool,
+        "AgentVersion": str,
+        "Tenancy": str,
+    },
+    total=False,
+)
+
+
+class CreateInstanceRequestRequestTypeDef(
+    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
+):
+    pass
+
+
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSummaryResultTypeDef = TypedDict(
     "DescribeStackSummaryResultTypeDef",
     {
         "StackSummary": StackSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LayerTypeDef = TypedDict(
+    "LayerTypeDef",
+    {
+        "Arn": str,
+        "StackId": str,
+        "LayerId": str,
+        "Type": LayerTypeType,
+        "Name": str,
+        "Shortname": str,
+        "Attributes": Dict[LayerAttributesKeysType, str],
+        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
+        "CustomInstanceProfileArn": str,
+        "CustomJson": str,
+        "CustomSecurityGroupIds": List[str],
+        "DefaultSecurityGroupNames": List[str],
+        "Packages": List[str],
+        "VolumeConfigurations": List[VolumeConfigurationOutputTypeDef],
+        "EnableAutoHealing": bool,
+        "AutoAssignElasticIps": bool,
+        "AutoAssignPublicIps": bool,
+        "DefaultRecipes": RecipesOutputTypeDef,
+        "CustomRecipes": RecipesOutputTypeDef,
+        "CreatedAt": str,
+        "InstallUpdatesOnBoot": bool,
+        "UseEbsOptimizedInstances": bool,
+        "LifecycleEventConfiguration": LifecycleEventConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLayerRequestRequestTypeDef",
     {
         "StackId": str,
         "Type": LayerTypeType,
@@ -2435,44 +2721,14 @@
 class CreateLayerRequestStackCreateLayerTypeDef(
     _RequiredCreateLayerRequestStackCreateLayerTypeDef,
     _OptionalCreateLayerRequestStackCreateLayerTypeDef,
 ):
     pass
 
 
-LayerTypeDef = TypedDict(
-    "LayerTypeDef",
-    {
-        "Arn": str,
-        "StackId": str,
-        "LayerId": str,
-        "Type": LayerTypeType,
-        "Name": str,
-        "Shortname": str,
-        "Attributes": Dict[LayerAttributesKeysType, str],
-        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationTypeDef,
-        "CustomInstanceProfileArn": str,
-        "CustomJson": str,
-        "CustomSecurityGroupIds": List[str],
-        "DefaultSecurityGroupNames": List[str],
-        "Packages": List[str],
-        "VolumeConfigurations": List[VolumeConfigurationTypeDef],
-        "EnableAutoHealing": bool,
-        "AutoAssignElasticIps": bool,
-        "AutoAssignPublicIps": bool,
-        "DefaultRecipes": RecipesTypeDef,
-        "CustomRecipes": RecipesTypeDef,
-        "CreatedAt": str,
-        "InstallUpdatesOnBoot": bool,
-        "UseEbsOptimizedInstances": bool,
-        "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayerRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalUpdateLayerRequestRequestTypeDef = TypedDict(
@@ -2505,34 +2761,34 @@
     pass
 
 
 DescribeOperatingSystemsResponseTypeDef = TypedDict(
     "DescribeOperatingSystemsResponseTypeDef",
     {
         "OperatingSystems": List[OperatingSystemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTimeBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeTimeBasedAutoScalingResultTypeDef",
     {
         "TimeBasedAutoScalingConfigurations": List[TimeBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancesResultTypeDef = TypedDict(
     "DescribeInstancesResultTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLayersResultTypeDef = TypedDict(
     "DescribeLayersResultTypeDef",
     {
         "Layers": List[LayerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/type_defs.pyi` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opsworks service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
+    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerOutputTypeDef
 
-    data: StackConfigurationManagerTypeDef = {...}
+    data: StackConfigurationManagerOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AppAttributesKeysType,
@@ -37,55 +37,58 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "StackConfigurationManagerTypeDef",
-    "DataSourceTypeDef",
-    "EnvironmentVariableTypeDef",
-    "SourceTypeDef",
-    "SslConfigurationTypeDef",
+    "StackConfigurationManagerOutputTypeDef",
+    "DataSourceOutputTypeDef",
+    "EnvironmentVariableOutputTypeDef",
+    "SourceOutputTypeDef",
+    "SslConfigurationOutputTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
+    "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
+    "EbsBlockDeviceOutputTypeDef",
     "EbsBlockDeviceTypeDef",
-    "ChefConfigurationResponseMetadataTypeDef",
+    "ChefConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
-    "CloneStackResultTypeDef",
+    "SourceTypeDef",
+    "StackConfigurationManagerTypeDef",
+    "CloudWatchLogsLogStreamOutputTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
-    "CreateAppResultTypeDef",
+    "DataSourceTypeDef",
+    "EnvironmentVariableTypeDef",
+    "SslConfigurationTypeDef",
     "DeploymentCommandTypeDef",
-    "CreateDeploymentResultTypeDef",
-    "CreateInstanceResultTypeDef",
     "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
-    "CreateLayerResultTypeDef",
-    "CreateStackResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
-    "CreateUserProfileResultTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
+    "DeploymentCommandOutputTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
     "DescribeCommandsRequestRequestTypeDef",
     "DescribeDeploymentsRequestRequestTypeDef",
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEcsClustersRequestRequestTypeDef",
     "EcsClusterTypeDef",
     "DescribeElasticIpsRequestRequestTypeDef",
     "ElasticIpTypeDef",
     "DescribeElasticLoadBalancersRequestRequestTypeDef",
     "ElasticLoadBalancerTypeDef",
     "DescribeInstancesRequestRequestTypeDef",
@@ -97,195 +100,211 @@
     "DescribeRaidArraysRequestRequestTypeDef",
     "RaidArrayTypeDef",
     "DescribeRdsDbInstancesRequestRequestTypeDef",
     "RdsDbInstanceTypeDef",
     "DescribeServiceErrorsRequestRequestTypeDef",
     "ServiceErrorTypeDef",
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
-    "DescribeStackProvisioningParametersResultTypeDef",
     "DescribeStackSummaryRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeTimeBasedAutoScalingRequestRequestTypeDef",
     "DescribeUserProfilesRequestRequestTypeDef",
     "UserProfileTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "VolumeTypeDef",
     "DetachElasticLoadBalancerRequestRequestTypeDef",
     "DisassociateElasticIpRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
-    "GetHostnameSuggestionResultTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
-    "InstancesCountResponseMetadataTypeDef",
     "InstancesCountTypeDef",
+    "RecipesOutputTypeDef",
+    "VolumeConfigurationOutputTypeDef",
+    "ShutdownEventConfigurationOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTagsResultTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
-    "PaginatorConfigTypeDef",
     "RebootInstanceRequestRequestTypeDef",
-    "RecipesResponseMetadataTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
-    "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
-    "RegisterElasticIpResultTypeDef",
-    "RegisterInstanceResultTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     "RegisterVolumeRequestRequestTypeDef",
-    "RegisterVolumeResultTypeDef",
-    "ResponseMetadataTypeDef",
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
-    "SourceResponseMetadataTypeDef",
-    "StackConfigurationManagerResponseMetadataTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "WeeklyAutoScalingScheduleOutputTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
-    "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
+    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
+    "StackTypeDef",
+    "ChefConfigurationResponseMetadataTypeDef",
+    "CloneStackResultTypeDef",
+    "CreateAppResultTypeDef",
+    "CreateDeploymentResultTypeDef",
+    "CreateInstanceResultTypeDef",
+    "CreateLayerResultTypeDef",
+    "CreateStackResultTypeDef",
+    "CreateUserProfileResultTypeDef",
+    "DescribeStackProvisioningParametersResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetHostnameSuggestionResultTypeDef",
+    "InstancesCountResponseMetadataTypeDef",
+    "ListTagsResultTypeDef",
+    "RecipesResponseMetadataTypeDef",
+    "RegisterEcsClusterResultTypeDef",
+    "RegisterElasticIpResultTypeDef",
+    "RegisterInstanceResultTypeDef",
+    "RegisterVolumeResultTypeDef",
+    "SourceResponseMetadataTypeDef",
+    "StackConfigurationManagerResponseMetadataTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
-    "StackTypeDef",
+    "DescribeAgentVersionsRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
+    "CloudWatchLogsConfigurationOutputTypeDef",
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     "DescribeEcsClustersResultTypeDef",
     "DescribeElasticIpsResultTypeDef",
     "DescribeElasticLoadBalancersResultTypeDef",
     "DescribeMyUserProfileResultTypeDef",
     "DescribePermissionsResultTypeDef",
     "DescribeRaidArraysResultTypeDef",
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
+    "LifecycleEventConfigurationOutputTypeDef",
     "LifecycleEventConfigurationResponseMetadataTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
-    "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
+    "CreateInstanceRequestRequestTypeDef",
     "DescribeStacksResultTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
+    "LayerTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
-    "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
     "DescribeTimeBasedAutoScalingResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "DescribeLayersResultTypeDef",
 )
 
-StackConfigurationManagerTypeDef = TypedDict(
-    "StackConfigurationManagerTypeDef",
+StackConfigurationManagerOutputTypeDef = TypedDict(
+    "StackConfigurationManagerOutputTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
     {
         "Type": str,
         "Arn": str,
         "DatabaseName": str,
     },
     total=False,
 )
 
-_RequiredEnvironmentVariableTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableTypeDef",
+_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
-_OptionalEnvironmentVariableTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableTypeDef",
+_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableOutputTypeDef",
     {
         "Secure": bool,
     },
     total=False,
 )
 
-class EnvironmentVariableTypeDef(
-    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
+class EnvironmentVariableOutputTypeDef(
+    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
 ):
     pass
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
         "SshKey": str,
         "Revision": str,
     },
     total=False,
 )
 
-_RequiredSslConfigurationTypeDef = TypedDict(
-    "_RequiredSslConfigurationTypeDef",
+_RequiredSslConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSslConfigurationOutputTypeDef",
     {
         "Certificate": str,
         "PrivateKey": str,
     },
 )
-_OptionalSslConfigurationTypeDef = TypedDict(
-    "_OptionalSslConfigurationTypeDef",
+_OptionalSslConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSslConfigurationOutputTypeDef",
     {
         "Chain": str,
     },
     total=False,
 )
 
-class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
+class SslConfigurationOutputTypeDef(
+    _RequiredSslConfigurationOutputTypeDef, _OptionalSslConfigurationOutputTypeDef
+):
     pass
 
 AssignInstanceRequestRequestTypeDef = TypedDict(
     "AssignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LayerIds": Sequence[str],
@@ -335,24 +354,50 @@
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
 
+AutoScalingThresholdsOutputTypeDef = TypedDict(
+    "AutoScalingThresholdsOutputTypeDef",
+    {
+        "InstanceCount": int,
+        "ThresholdsWaitTime": int,
+        "IgnoreMetricsTime": int,
+        "CpuThreshold": float,
+        "MemoryThreshold": float,
+        "LoadThreshold": float,
+        "Alarms": List[str],
+    },
+    total=False,
+)
+
 AutoScalingThresholdsTypeDef = TypedDict(
     "AutoScalingThresholdsTypeDef",
     {
         "InstanceCount": int,
         "ThresholdsWaitTime": int,
         "IgnoreMetricsTime": int,
         "CpuThreshold": float,
         "MemoryThreshold": float,
         "LoadThreshold": float,
-        "Alarms": List[str],
+        "Alarms": Sequence[str],
+    },
+    total=False,
+)
+
+EbsBlockDeviceOutputTypeDef = TypedDict(
+    "EbsBlockDeviceOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "Iops": int,
+        "VolumeSize": int,
+        "VolumeType": VolumeTypeType,
+        "DeleteOnTermination": bool,
     },
     total=False,
 )
 
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
@@ -361,38 +406,81 @@
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "DeleteOnTermination": bool,
     },
     total=False,
 )
 
-ChefConfigurationResponseMetadataTypeDef = TypedDict(
-    "ChefConfigurationResponseMetadataTypeDef",
+ChefConfigurationOutputTypeDef = TypedDict(
+    "ChefConfigurationOutputTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
     },
 )
 
 ChefConfigurationTypeDef = TypedDict(
     "ChefConfigurationTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
     },
     total=False,
 )
 
-CloneStackResultTypeDef = TypedDict(
-    "CloneStackResultTypeDef",
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
     {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": SourceTypeType,
+        "Url": str,
+        "Username": str,
+        "Password": str,
+        "SshKey": str,
+        "Revision": str,
+    },
+    total=False,
+)
+
+StackConfigurationManagerTypeDef = TypedDict(
+    "StackConfigurationManagerTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+CloudWatchLogsLogStreamOutputTypeDef = TypedDict(
+    "CloudWatchLogsLogStreamOutputTypeDef",
+    {
+        "LogGroupName": str,
+        "DatetimeFormat": str,
+        "TimeZone": CloudWatchLogsTimeZoneType,
+        "File": str,
+        "FileFingerprintLines": str,
+        "MultiLineStartPattern": str,
+        "InitialPosition": CloudWatchLogsInitialPositionType,
+        "Encoding": CloudWatchLogsEncodingType,
+        "BufferDuration": int,
+        "BatchCount": int,
+        "BatchSize": int,
     },
+    total=False,
 )
 
 CloudWatchLogsLogStreamTypeDef = TypedDict(
     "CloudWatchLogsLogStreamTypeDef",
     {
         "LogGroupName": str,
         "DatetimeFormat": str,
@@ -422,56 +510,80 @@
         "ExitCode": int,
         "LogUrl": str,
         "Type": str,
     },
     total=False,
 )
 
-CreateAppResultTypeDef = TypedDict(
-    "CreateAppResultTypeDef",
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
     {
-        "AppId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": str,
+        "Arn": str,
+        "DatabaseName": str,
     },
+    total=False,
 )
 
-_RequiredDeploymentCommandTypeDef = TypedDict(
-    "_RequiredDeploymentCommandTypeDef",
+_RequiredEnvironmentVariableTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableTypeDef",
     {
-        "Name": DeploymentCommandNameType,
+        "Key": str,
+        "Value": str,
     },
 )
-_OptionalDeploymentCommandTypeDef = TypedDict(
-    "_OptionalDeploymentCommandTypeDef",
+_OptionalEnvironmentVariableTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableTypeDef",
     {
-        "Args": Mapping[str, Sequence[str]],
+        "Secure": bool,
     },
     total=False,
 )
 
-class DeploymentCommandTypeDef(
-    _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
+class EnvironmentVariableTypeDef(
+    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
-CreateDeploymentResultTypeDef = TypedDict(
-    "CreateDeploymentResultTypeDef",
+_RequiredSslConfigurationTypeDef = TypedDict(
+    "_RequiredSslConfigurationTypeDef",
     {
-        "DeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Certificate": str,
+        "PrivateKey": str,
+    },
+)
+_OptionalSslConfigurationTypeDef = TypedDict(
+    "_OptionalSslConfigurationTypeDef",
+    {
+        "Chain": str,
     },
+    total=False,
 )
 
-CreateInstanceResultTypeDef = TypedDict(
-    "CreateInstanceResultTypeDef",
+class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
+    pass
+
+_RequiredDeploymentCommandTypeDef = TypedDict(
+    "_RequiredDeploymentCommandTypeDef",
     {
-        "InstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": DeploymentCommandNameType,
     },
 )
+_OptionalDeploymentCommandTypeDef = TypedDict(
+    "_OptionalDeploymentCommandTypeDef",
+    {
+        "Args": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+class DeploymentCommandTypeDef(
+    _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
+):
+    pass
 
 RecipesTypeDef = TypedDict(
     "RecipesTypeDef",
     {
         "Setup": Sequence[str],
         "Configure": Sequence[str],
         "Deploy": Sequence[str],
@@ -501,30 +613,14 @@
 )
 
 class VolumeConfigurationTypeDef(
     _RequiredVolumeConfigurationTypeDef, _OptionalVolumeConfigurationTypeDef
 ):
     pass
 
-CreateLayerResultTypeDef = TypedDict(
-    "CreateLayerResultTypeDef",
-    {
-        "LayerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackResultTypeDef = TypedDict(
-    "CreateStackResultTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 _OptionalCreateUserProfileRequestRequestTypeDef = TypedDict(
@@ -538,22 +634,14 @@
 )
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "IamUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAppRequestRequestTypeDef = TypedDict(
     "DeleteAppRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 
@@ -594,14 +682,33 @@
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 
+_RequiredDeploymentCommandOutputTypeDef = TypedDict(
+    "_RequiredDeploymentCommandOutputTypeDef",
+    {
+        "Name": DeploymentCommandNameType,
+    },
+)
+_OptionalDeploymentCommandOutputTypeDef = TypedDict(
+    "_OptionalDeploymentCommandOutputTypeDef",
+    {
+        "Args": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+class DeploymentCommandOutputTypeDef(
+    _RequiredDeploymentCommandOutputTypeDef, _OptionalDeploymentCommandOutputTypeDef
+):
+    pass
+
 DeregisterEcsClusterRequestRequestTypeDef = TypedDict(
     "DeregisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
     },
 )
 
@@ -667,20 +774,20 @@
         "StackId": str,
         "AppId": str,
         "DeploymentIds": Sequence[str],
     },
     total=False,
 )
 
-DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EcsClusterArns": Sequence[str],
-        "StackId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEcsClustersRequestRequestTypeDef = TypedDict(
     "DescribeEcsClustersRequestRequestTypeDef",
     {
@@ -900,23 +1007,14 @@
 DescribeStackProvisioningParametersRequestRequestTypeDef = TypedDict(
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
-DescribeStackProvisioningParametersResultTypeDef = TypedDict(
-    "DescribeStackProvisioningParametersResultTypeDef",
-    {
-        "AgentInstallerUrl": str,
-        "Parameters": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStackSummaryRequestRequestTypeDef = TypedDict(
     "DescribeStackSummaryRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
@@ -998,37 +1096,21 @@
 DisassociateElasticIpRequestRequestTypeDef = TypedDict(
     "DisassociateElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHostnameSuggestionRequestRequestTypeDef = TypedDict(
     "GetHostnameSuggestionRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 
-GetHostnameSuggestionResultTypeDef = TypedDict(
-    "GetHostnameSuggestionResultTypeDef",
-    {
-        "LayerId": str,
-        "Hostname": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGrantAccessRequestRequestTypeDef = TypedDict(
     "_RequiredGrantAccessRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalGrantAccessRequestRequestTypeDef = TypedDict(
@@ -1070,16 +1152,16 @@
         "Family": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-InstancesCountResponseMetadataTypeDef = TypedDict(
-    "InstancesCountResponseMetadataTypeDef",
+InstancesCountTypeDef = TypedDict(
+    "InstancesCountTypeDef",
     {
         "Assigning": int,
         "Booting": int,
         "ConnectionLost": int,
         "Deregistering": int,
         "Online": int,
         "Pending": int,
@@ -1093,41 +1175,59 @@
         "StartFailed": int,
         "StopFailed": int,
         "Stopped": int,
         "Stopping": int,
         "Terminated": int,
         "Terminating": int,
         "Unassigning": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-InstancesCountTypeDef = TypedDict(
-    "InstancesCountTypeDef",
+RecipesOutputTypeDef = TypedDict(
+    "RecipesOutputTypeDef",
     {
-        "Assigning": int,
-        "Booting": int,
-        "ConnectionLost": int,
-        "Deregistering": int,
-        "Online": int,
-        "Pending": int,
-        "Rebooting": int,
-        "Registered": int,
-        "Registering": int,
-        "Requested": int,
-        "RunningSetup": int,
-        "SetupFailed": int,
-        "ShuttingDown": int,
-        "StartFailed": int,
-        "StopFailed": int,
-        "Stopped": int,
-        "Stopping": int,
-        "Terminated": int,
-        "Terminating": int,
-        "Unassigning": int,
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+    },
+    total=False,
+)
+
+_RequiredVolumeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVolumeConfigurationOutputTypeDef",
+    {
+        "MountPoint": str,
+        "NumberOfDisks": int,
+        "Size": int,
+    },
+)
+_OptionalVolumeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVolumeConfigurationOutputTypeDef",
+    {
+        "RaidLevel": int,
+        "VolumeType": str,
+        "Iops": int,
+        "Encrypted": bool,
+    },
+    total=False,
+)
+
+class VolumeConfigurationOutputTypeDef(
+    _RequiredVolumeConfigurationOutputTypeDef, _OptionalVolumeConfigurationOutputTypeDef
+):
+    pass
+
+ShutdownEventConfigurationOutputTypeDef = TypedDict(
+    "ShutdownEventConfigurationOutputTypeDef",
+    {
+        "ExecutionTimeout": int,
+        "DelayUntilElbConnectionsDrained": bool,
     },
     total=False,
 )
 
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
@@ -1153,101 +1253,46 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-ListTagsResultTypeDef = TypedDict(
-    "ListTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OperatingSystemConfigurationManagerTypeDef = TypedDict(
     "OperatingSystemConfigurationManagerTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 RebootInstanceRequestRequestTypeDef = TypedDict(
     "RebootInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-RecipesResponseMetadataTypeDef = TypedDict(
-    "RecipesResponseMetadataTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterEcsClusterRequestRequestTypeDef = TypedDict(
     "RegisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
         "StackId": str,
     },
 )
 
-RegisterEcsClusterResultTypeDef = TypedDict(
-    "RegisterEcsClusterResultTypeDef",
-    {
-        "EcsClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterElasticIpRequestRequestTypeDef = TypedDict(
     "RegisterElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
         "StackId": str,
     },
 )
 
-RegisterElasticIpResultTypeDef = TypedDict(
-    "RegisterElasticIpResultTypeDef",
-    {
-        "ElasticIp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterInstanceResultTypeDef = TypedDict(
-    "RegisterInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterRdsDbInstanceRequestRequestTypeDef = TypedDict(
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     {
         "StackId": str,
         "RdsDbInstanceArn": str,
         "DbUser": str,
         "DbPassword": str,
@@ -1269,33 +1314,14 @@
 )
 
 class RegisterVolumeRequestRequestTypeDef(
     _RequiredRegisterVolumeRequestRequestTypeDef, _OptionalRegisterVolumeRequestRequestTypeDef
 ):
     pass
 
-RegisterVolumeResultTypeDef = TypedDict(
-    "RegisterVolumeResultTypeDef",
-    {
-        "VolumeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredSetPermissionRequestRequestTypeDef",
     {
         "StackId": str,
         "IamUserArn": str,
     },
 )
@@ -1313,47 +1339,25 @@
     _RequiredSetPermissionRequestRequestTypeDef, _OptionalSetPermissionRequestRequestTypeDef
 ):
     pass
 
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
-        "Monday": Dict[str, str],
-        "Tuesday": Dict[str, str],
-        "Wednesday": Dict[str, str],
-        "Thursday": Dict[str, str],
-        "Friday": Dict[str, str],
-        "Saturday": Dict[str, str],
-        "Sunday": Dict[str, str],
+        "Monday": Mapping[str, str],
+        "Tuesday": Mapping[str, str],
+        "Wednesday": Mapping[str, str],
+        "Thursday": Mapping[str, str],
+        "Friday": Mapping[str, str],
+        "Saturday": Mapping[str, str],
+        "Sunday": Mapping[str, str],
     },
     total=False,
 )
 
-SourceResponseMetadataTypeDef = TypedDict(
-    "SourceResponseMetadataTypeDef",
-    {
-        "Type": SourceTypeType,
-        "Url": str,
-        "Username": str,
-        "Password": str,
-        "SshKey": str,
-        "Revision": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
-    "StackConfigurationManagerResponseMetadataTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1394,14 +1398,28 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+WeeklyAutoScalingScheduleOutputTypeDef = TypedDict(
+    "WeeklyAutoScalingScheduleOutputTypeDef",
+    {
+        "Monday": Dict[str, str],
+        "Tuesday": Dict[str, str],
+        "Wednesday": Dict[str, str],
+        "Thursday": Dict[str, str],
+        "Friday": Dict[str, str],
+        "Saturday": Dict[str, str],
+        "Sunday": Dict[str, str],
+    },
+    total=False,
+)
+
 UnassignInstanceRequestRequestTypeDef = TypedDict(
     "UnassignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1538,113 +1556,47 @@
 ):
     pass
 
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "Version": str,
-        "ConfigurationManager": StackConfigurationManagerTypeDef,
-    },
-    total=False,
-)
-
-DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentVersionsRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "ConfigurationManager": StackConfigurationManagerTypeDef,
+        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppId": str,
         "StackId": str,
         "Shortname": str,
         "Name": str,
         "Description": str,
-        "DataSources": List[DataSourceTypeDef],
+        "DataSources": List[DataSourceOutputTypeDef],
         "Type": AppTypeType,
-        "AppSource": SourceTypeDef,
+        "AppSource": SourceOutputTypeDef,
         "Domains": List[str],
         "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
+        "SslConfiguration": SslConfigurationOutputTypeDef,
         "Attributes": Dict[AppAttributesKeysType, str],
         "CreatedAt": str,
-        "Environment": List[EnvironmentVariableTypeDef],
+        "Environment": List[EnvironmentVariableOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "Name": str,
-        "Type": AppTypeType,
-    },
-)
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
-    {
-        "Shortname": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
-    },
-    total=False,
-)
-
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "AppId": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "Type": AppTypeType,
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
-    },
-    total=False,
-)
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": str,
         "Enable": bool,
-        "UpScaling": AutoScalingThresholdsTypeDef,
-        "DownScaling": AutoScalingThresholdsTypeDef,
+        "UpScaling": AutoScalingThresholdsOutputTypeDef,
+        "DownScaling": AutoScalingThresholdsOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
     "_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef",
     {
@@ -1663,25 +1615,257 @@
 
 class SetLoadBasedAutoScalingRequestRequestTypeDef(
     _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef,
     _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
+BlockDeviceMappingOutputTypeDef = TypedDict(
+    "BlockDeviceMappingOutputTypeDef",
+    {
+        "DeviceName": str,
+        "NoDevice": str,
+        "VirtualName": str,
+        "Ebs": EbsBlockDeviceOutputTypeDef,
+    },
+    total=False,
+)
+
 BlockDeviceMappingTypeDef = TypedDict(
     "BlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "NoDevice": str,
         "VirtualName": str,
         "Ebs": EbsBlockDeviceTypeDef,
     },
     total=False,
 )
 
+StackTypeDef = TypedDict(
+    "StackTypeDef",
+    {
+        "StackId": str,
+        "Name": str,
+        "Arn": str,
+        "Region": str,
+        "VpcId": str,
+        "Attributes": Dict[Literal["Color"], str],
+        "ServiceRoleArn": str,
+        "DefaultInstanceProfileArn": str,
+        "DefaultOs": str,
+        "HostnameTheme": str,
+        "DefaultAvailabilityZone": str,
+        "DefaultSubnetId": str,
+        "CustomJson": str,
+        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
+        "ChefConfiguration": ChefConfigurationOutputTypeDef,
+        "UseCustomCookbooks": bool,
+        "UseOpsworksSecurityGroups": bool,
+        "CustomCookbooksSource": SourceOutputTypeDef,
+        "DefaultSshKeyName": str,
+        "CreatedAt": str,
+        "DefaultRootDeviceType": RootDeviceTypeType,
+        "AgentVersion": str,
+    },
+    total=False,
+)
+
+ChefConfigurationResponseMetadataTypeDef = TypedDict(
+    "ChefConfigurationResponseMetadataTypeDef",
+    {
+        "ManageBerkshelf": bool,
+        "BerkshelfVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CloneStackResultTypeDef = TypedDict(
+    "CloneStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppResultTypeDef = TypedDict(
+    "CreateAppResultTypeDef",
+    {
+        "AppId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResultTypeDef = TypedDict(
+    "CreateDeploymentResultTypeDef",
+    {
+        "DeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInstanceResultTypeDef = TypedDict(
+    "CreateInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayerResultTypeDef = TypedDict(
+    "CreateLayerResultTypeDef",
+    {
+        "LayerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackResultTypeDef = TypedDict(
+    "CreateStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "IamUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackProvisioningParametersResultTypeDef = TypedDict(
+    "DescribeStackProvisioningParametersResultTypeDef",
+    {
+        "AgentInstallerUrl": str,
+        "Parameters": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHostnameSuggestionResultTypeDef = TypedDict(
+    "GetHostnameSuggestionResultTypeDef",
+    {
+        "LayerId": str,
+        "Hostname": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InstancesCountResponseMetadataTypeDef = TypedDict(
+    "InstancesCountResponseMetadataTypeDef",
+    {
+        "Assigning": int,
+        "Booting": int,
+        "ConnectionLost": int,
+        "Deregistering": int,
+        "Online": int,
+        "Pending": int,
+        "Rebooting": int,
+        "Registered": int,
+        "Registering": int,
+        "Requested": int,
+        "RunningSetup": int,
+        "SetupFailed": int,
+        "ShuttingDown": int,
+        "StartFailed": int,
+        "StopFailed": int,
+        "Stopped": int,
+        "Stopping": int,
+        "Terminated": int,
+        "Terminating": int,
+        "Unassigning": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResultTypeDef = TypedDict(
+    "ListTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecipesResponseMetadataTypeDef = TypedDict(
+    "RecipesResponseMetadataTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterEcsClusterResultTypeDef = TypedDict(
+    "RegisterEcsClusterResultTypeDef",
+    {
+        "EcsClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterElasticIpResultTypeDef = TypedDict(
+    "RegisterElasticIpResultTypeDef",
+    {
+        "ElasticIp": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterInstanceResultTypeDef = TypedDict(
+    "RegisterInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterVolumeResultTypeDef = TypedDict(
+    "RegisterVolumeResultTypeDef",
+    {
+        "VolumeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SourceResponseMetadataTypeDef = TypedDict(
+    "SourceResponseMetadataTypeDef",
+    {
+        "Type": SourceTypeType,
+        "Url": str,
+        "Username": str,
+        "Password": str,
+        "SshKey": str,
+        "Revision": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
+    "StackConfigurationManagerResponseMetadataTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCloneStackRequestRequestTypeDef = TypedDict(
     "_RequiredCloneStackRequestRequestTypeDef",
     {
         "SourceStackId": str,
         "ServiceRoleArn": str,
     },
 )
@@ -1786,39 +1970,19 @@
 
 class CreateStackRequestServiceResourceCreateStackTypeDef(
     _RequiredCreateStackRequestServiceResourceCreateStackTypeDef,
     _OptionalCreateStackRequestServiceResourceCreateStackTypeDef,
 ):
     pass
 
-StackTypeDef = TypedDict(
-    "StackTypeDef",
+DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentVersionsRequestRequestTypeDef",
     {
         "StackId": str,
-        "Name": str,
-        "Arn": str,
-        "Region": str,
-        "VpcId": str,
-        "Attributes": Dict[Literal["Color"], str],
-        "ServiceRoleArn": str,
-        "DefaultInstanceProfileArn": str,
-        "DefaultOs": str,
-        "HostnameTheme": str,
-        "DefaultAvailabilityZone": str,
-        "DefaultSubnetId": str,
-        "CustomJson": str,
         "ConfigurationManager": StackConfigurationManagerTypeDef,
-        "ChefConfiguration": ChefConfigurationTypeDef,
-        "UseCustomCookbooks": bool,
-        "UseOpsworksSecurityGroups": bool,
-        "CustomCookbooksSource": SourceTypeDef,
-        "DefaultSshKeyName": str,
-        "CreatedAt": str,
-        "DefaultRootDeviceType": RootDeviceTypeType,
-        "AgentVersion": str,
     },
     total=False,
 )
 
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
@@ -1850,20 +2014,29 @@
 )
 
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
+CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLogsConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
+    },
+    total=False,
+)
+
 CloudWatchLogsConfigurationResponseMetadataTypeDef = TypedDict(
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
@@ -1872,18 +2045,75 @@
     total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "Name": str,
+        "Type": AppTypeType,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "Shortname": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "AppId": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "Type": AppTypeType,
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "StackId": str,
         "Command": DeploymentCommandTypeDef,
     },
 )
@@ -1911,15 +2141,15 @@
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
         "CompletedAt": str,
         "Duration": int,
         "IamUserArn": str,
         "Comment": str,
-        "Command": DeploymentCommandTypeDef,
+        "Command": DeploymentCommandOutputTypeDef,
         "Status": str,
         "CustomJson": str,
         "InstanceIds": List[str],
     },
     total=False,
 )
 
@@ -1984,100 +2214,110 @@
         "LayerId": str,
         "InstanceIds": Sequence[str],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
+    {
+        "EcsClusterArns": Sequence[str],
+        "StackId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEcsClustersResultTypeDef = TypedDict(
     "DescribeEcsClustersResultTypeDef",
     {
         "EcsClusters": List[EcsClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticIpsResultTypeDef = TypedDict(
     "DescribeElasticIpsResultTypeDef",
     {
         "ElasticIps": List[ElasticIpTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticLoadBalancersResultTypeDef = TypedDict(
     "DescribeElasticLoadBalancersResultTypeDef",
     {
         "ElasticLoadBalancers": List[ElasticLoadBalancerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMyUserProfileResultTypeDef = TypedDict(
     "DescribeMyUserProfileResultTypeDef",
     {
         "UserProfile": SelfUserProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePermissionsResultTypeDef = TypedDict(
     "DescribePermissionsResultTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRaidArraysResultTypeDef = TypedDict(
     "DescribeRaidArraysResultTypeDef",
     {
         "RaidArrays": List[RaidArrayTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRdsDbInstancesResultTypeDef = TypedDict(
     "DescribeRdsDbInstancesResultTypeDef",
     {
         "RdsDbInstances": List[RdsDbInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceErrorsResultTypeDef = TypedDict(
     "DescribeServiceErrorsResultTypeDef",
     {
         "ServiceErrors": List[ServiceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserProfilesResultTypeDef = TypedDict(
     "DescribeUserProfilesResultTypeDef",
     {
         "UserProfiles": List[UserProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVolumesResultTypeDef = TypedDict(
     "DescribeVolumesResultTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GrantAccessResultTypeDef = TypedDict(
     "GrantAccessResultTypeDef",
     {
         "TemporaryCredential": TemporaryCredentialTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2110,19 +2350,27 @@
         "LayersCount": int,
         "AppsCount": int,
         "InstancesCount": InstancesCountTypeDef,
     },
     total=False,
 )
 
+LifecycleEventConfigurationOutputTypeDef = TypedDict(
+    "LifecycleEventConfigurationOutputTypeDef",
+    {
+        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LifecycleEventConfigurationResponseMetadataTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseMetadataTypeDef",
     {
-        "Shutdown": ShutdownEventConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleEventConfigurationTypeDef = TypedDict(
     "LifecycleEventConfigurationTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
@@ -2164,88 +2412,53 @@
 ):
     pass
 
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": str,
-        "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
+        "AutoScalingSchedule": WeeklyAutoScalingScheduleOutputTypeDef,
     },
     total=False,
 )
 
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppsResultTypeDef = TypedDict(
     "DescribeAppsResultTypeDef",
     {
         "Apps": List[AppTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeLoadBasedAutoScalingResultTypeDef",
     {
         "LoadBasedAutoScalingConfigurations": List[LoadBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "LayerIds": Sequence[str],
-        "InstanceType": str,
-    },
-)
-_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceRequestRequestTypeDef",
-    {
-        "AutoScalingType": AutoScalingTypeType,
-        "Hostname": str,
-        "Os": str,
-        "AmiId": str,
-        "SshKeyName": str,
-        "AvailabilityZone": str,
-        "VirtualizationType": str,
-        "SubnetId": str,
-        "Architecture": ArchitectureType,
-        "RootDeviceType": RootDeviceTypeType,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "InstallUpdatesOnBoot": bool,
-        "EbsOptimized": bool,
-        "AgentVersion": str,
-        "Tenancy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateInstanceRequestRequestTypeDef(
-    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
-):
-    pass
-
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AgentVersion": str,
         "AmiId": str,
         "Architecture": ArchitectureType,
         "Arn": str,
         "AutoScalingType": AutoScalingTypeType,
         "AvailabilityZone": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
+        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
         "CreatedAt": str,
         "EbsOptimized": bool,
         "Ec2InstanceId": str,
         "EcsClusterArn": str,
         "EcsContainerInstanceArn": str,
         "ElasticIp": str,
         "Hostname": str,
@@ -2276,38 +2489,103 @@
         "SubnetId": str,
         "Tenancy": str,
         "VirtualizationType": VirtualizationTypeType,
     },
     total=False,
 )
 
+_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "LayerIds": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceRequestRequestTypeDef",
+    {
+        "AutoScalingType": AutoScalingTypeType,
+        "Hostname": str,
+        "Os": str,
+        "AmiId": str,
+        "SshKeyName": str,
+        "AvailabilityZone": str,
+        "VirtualizationType": str,
+        "SubnetId": str,
+        "Architecture": ArchitectureType,
+        "RootDeviceType": RootDeviceTypeType,
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "InstallUpdatesOnBoot": bool,
+        "EbsOptimized": bool,
+        "AgentVersion": str,
+        "Tenancy": str,
+    },
+    total=False,
+)
+
+class CreateInstanceRequestRequestTypeDef(
+    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
+):
+    pass
+
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSummaryResultTypeDef = TypedDict(
     "DescribeStackSummaryResultTypeDef",
     {
         "StackSummary": StackSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LayerTypeDef = TypedDict(
+    "LayerTypeDef",
+    {
+        "Arn": str,
+        "StackId": str,
+        "LayerId": str,
+        "Type": LayerTypeType,
+        "Name": str,
+        "Shortname": str,
+        "Attributes": Dict[LayerAttributesKeysType, str],
+        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
+        "CustomInstanceProfileArn": str,
+        "CustomJson": str,
+        "CustomSecurityGroupIds": List[str],
+        "DefaultSecurityGroupNames": List[str],
+        "Packages": List[str],
+        "VolumeConfigurations": List[VolumeConfigurationOutputTypeDef],
+        "EnableAutoHealing": bool,
+        "AutoAssignElasticIps": bool,
+        "AutoAssignPublicIps": bool,
+        "DefaultRecipes": RecipesOutputTypeDef,
+        "CustomRecipes": RecipesOutputTypeDef,
+        "CreatedAt": str,
+        "InstallUpdatesOnBoot": bool,
+        "UseEbsOptimizedInstances": bool,
+        "LifecycleEventConfiguration": LifecycleEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLayerRequestRequestTypeDef",
     {
         "StackId": str,
         "Type": LayerTypeType,
         "Name": str,
         "Shortname": str,
@@ -2370,44 +2648,14 @@
 
 class CreateLayerRequestStackCreateLayerTypeDef(
     _RequiredCreateLayerRequestStackCreateLayerTypeDef,
     _OptionalCreateLayerRequestStackCreateLayerTypeDef,
 ):
     pass
 
-LayerTypeDef = TypedDict(
-    "LayerTypeDef",
-    {
-        "Arn": str,
-        "StackId": str,
-        "LayerId": str,
-        "Type": LayerTypeType,
-        "Name": str,
-        "Shortname": str,
-        "Attributes": Dict[LayerAttributesKeysType, str],
-        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationTypeDef,
-        "CustomInstanceProfileArn": str,
-        "CustomJson": str,
-        "CustomSecurityGroupIds": List[str],
-        "DefaultSecurityGroupNames": List[str],
-        "Packages": List[str],
-        "VolumeConfigurations": List[VolumeConfigurationTypeDef],
-        "EnableAutoHealing": bool,
-        "AutoAssignElasticIps": bool,
-        "AutoAssignPublicIps": bool,
-        "DefaultRecipes": RecipesTypeDef,
-        "CustomRecipes": RecipesTypeDef,
-        "CreatedAt": str,
-        "InstallUpdatesOnBoot": bool,
-        "UseEbsOptimizedInstances": bool,
-        "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayerRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalUpdateLayerRequestRequestTypeDef = TypedDict(
@@ -2438,34 +2686,34 @@
 ):
     pass
 
 DescribeOperatingSystemsResponseTypeDef = TypedDict(
     "DescribeOperatingSystemsResponseTypeDef",
     {
         "OperatingSystems": List[OperatingSystemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTimeBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeTimeBasedAutoScalingResultTypeDef",
     {
         "TimeBasedAutoScalingConfigurations": List[TimeBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancesResultTypeDef = TypedDict(
     "DescribeInstancesResultTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLayersResultTypeDef = TypedDict(
     "DescribeLayersResultTypeDef",
     {
         "Layers": List[LayerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/waiter.py` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks/waiter.pyi` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/PKG-INFO` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.0
-Summary: Type annotations for boto3.OpsWorks 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpsWorks 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworks?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,55 +438,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
-    StackConfigurationManagerTypeDef,
-    DataSourceTypeDef,
-    EnvironmentVariableTypeDef,
-    SourceTypeDef,
-    SslConfigurationTypeDef,
+    StackConfigurationManagerOutputTypeDef,
+    DataSourceOutputTypeDef,
+    EnvironmentVariableOutputTypeDef,
+    SourceOutputTypeDef,
+    SslConfigurationOutputTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
+    AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
+    EbsBlockDeviceOutputTypeDef,
     EbsBlockDeviceTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
-    CloneStackResultTypeDef,
+    SourceTypeDef,
+    StackConfigurationManagerTypeDef,
+    CloudWatchLogsLogStreamOutputTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
-    CreateAppResultTypeDef,
+    DataSourceTypeDef,
+    EnvironmentVariableTypeDef,
+    SslConfigurationTypeDef,
     DeploymentCommandTypeDef,
-    CreateDeploymentResultTypeDef,
-    CreateInstanceResultTypeDef,
     RecipesTypeDef,
     VolumeConfigurationTypeDef,
-    CreateLayerResultTypeDef,
-    CreateStackResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
+    DeploymentCommandOutputTypeDef,
     DeregisterEcsClusterRequestRequestTypeDef,
     DeregisterElasticIpRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DeregisterRdsDbInstanceRequestRequestTypeDef,
     DeregisterVolumeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAppsRequestRequestTypeDef,
     DescribeCommandsRequestRequestTypeDef,
     DescribeDeploymentsRequestRequestTypeDef,
-    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEcsClustersRequestRequestTypeDef,
     EcsClusterTypeDef,
     DescribeElasticIpsRequestRequestTypeDef,
     ElasticIpTypeDef,
     DescribeElasticLoadBalancersRequestRequestTypeDef,
     ElasticLoadBalancerTypeDef,
     DescribeInstancesRequestRequestTypeDef,
@@ -498,129 +501,143 @@
     DescribeRaidArraysRequestRequestTypeDef,
     RaidArrayTypeDef,
     DescribeRdsDbInstancesRequestRequestTypeDef,
     RdsDbInstanceTypeDef,
     DescribeServiceErrorsRequestRequestTypeDef,
     ServiceErrorTypeDef,
     DescribeStackProvisioningParametersRequestRequestTypeDef,
-    DescribeStackProvisioningParametersResultTypeDef,
     DescribeStackSummaryRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeTimeBasedAutoScalingRequestRequestTypeDef,
     DescribeUserProfilesRequestRequestTypeDef,
     UserProfileTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     VolumeTypeDef,
     DetachElasticLoadBalancerRequestRequestTypeDef,
     DisassociateElasticIpRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionRequestRequestTypeDef,
-    GetHostnameSuggestionResultTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
-    InstancesCountResponseMetadataTypeDef,
     InstancesCountTypeDef,
+    RecipesOutputTypeDef,
+    VolumeConfigurationOutputTypeDef,
+    ShutdownEventConfigurationOutputTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResultTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
-    PaginatorConfigTypeDef,
     RebootInstanceRequestRequestTypeDef,
-    RecipesResponseMetadataTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
-    RegisterEcsClusterResultTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
-    RegisterElasticIpResultTypeDef,
-    RegisterInstanceResultTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
     RegisterVolumeRequestRequestTypeDef,
-    RegisterVolumeResultTypeDef,
-    ResponseMetadataTypeDef,
     SetPermissionRequestRequestTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartStackRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopStackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    WeeklyAutoScalingScheduleOutputTypeDef,
     UnassignInstanceRequestRequestTypeDef,
     UnassignVolumeRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateElasticIpRequestRequestTypeDef,
     UpdateInstanceRequestRequestTypeDef,
     UpdateMyUserProfileRequestRequestTypeDef,
     UpdateRdsDbInstanceRequestRequestTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
-    DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
+    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
+    StackTypeDef,
+    ChefConfigurationResponseMetadataTypeDef,
+    CloneStackResultTypeDef,
+    CreateAppResultTypeDef,
+    CreateDeploymentResultTypeDef,
+    CreateInstanceResultTypeDef,
+    CreateLayerResultTypeDef,
+    CreateStackResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DescribeStackProvisioningParametersResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetHostnameSuggestionResultTypeDef,
+    InstancesCountResponseMetadataTypeDef,
+    ListTagsResultTypeDef,
+    RecipesResponseMetadataTypeDef,
+    RegisterEcsClusterResultTypeDef,
+    RegisterElasticIpResultTypeDef,
+    RegisterInstanceResultTypeDef,
+    RegisterVolumeResultTypeDef,
+    SourceResponseMetadataTypeDef,
+    StackConfigurationManagerResponseMetadataTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
-    StackTypeDef,
+    DescribeAgentVersionsRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
+    CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
+    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
     DescribeMyUserProfileResultTypeDef,
     DescribePermissionsResultTypeDef,
     DescribeRaidArraysResultTypeDef,
     DescribeRdsDbInstancesResultTypeDef,
     DescribeServiceErrorsResultTypeDef,
     DescribeUserProfilesResultTypeDef,
     DescribeVolumesResultTypeDef,
     GrantAccessResultTypeDef,
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
+    LifecycleEventConfigurationOutputTypeDef,
     LifecycleEventConfigurationResponseMetadataTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
-    CreateInstanceRequestRequestTypeDef,
     InstanceTypeDef,
+    CreateInstanceRequestRequestTypeDef,
     DescribeStacksResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
+    LayerTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
-    LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerTypeDef:
+def get_structure() -> StackConfigurationManagerOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.0/mypy_boto3_opsworks.egg-info/SOURCES.txt` & `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.0/setup.py` & `mypy-boto3-opsworks-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworks",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorks 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.OpsWorks 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

