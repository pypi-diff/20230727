# Comparing `tmp/mypy-boto3-emr-1.28.0.tar.gz` & `tmp/mypy-boto3-emr-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.28.0.tar", last modified: Thu Jul  6 20:59:33 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
```

## Comparing `mypy-boto3-emr-1.28.0.tar` & `mypy-boto3-emr-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.474299 mypy-boto3-emr-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-06 20:59:33.474299 mypy-boto3-emr-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.470299 mypy-boto3-emr-1.28.0/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-06 20:40:35.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79659 2023-07-06 20:40:38.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79553 2023-07-06 20:40:36.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.470299 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:33.474299 mypy-boto3-emr-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:40:33.000000 mypy-boto3-emr-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.264515 mypy-boto3-emr-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-27 05:34:40.256515 mypy-boto3-emr-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.256515 mypy-boto3-emr-1.28.12/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93670 2023-07-27 05:22:00.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93532 2023-07-27 05:21:59.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.256515 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.264515 mypy-boto3-emr-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/setup.py
```

### Comparing `mypy-boto3-emr-1.28.0/LICENSE` & `mypy-boto3-emr-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/PKG-INFO` & `mypy-boto3-emr-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.28.0
-Summary: Type annotations for boto3.EMR 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EMR 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -429,32 +429,41 @@
 
 ```python
 from mypy_boto3_emr.type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
     TagTypeDef,
+    ApplicationOutputTypeDef,
     ApplicationTypeDef,
-    ScalingConstraintsTypeDef,
+    ScalingConstraintsOutputTypeDef,
     AutoScalingPolicyStateChangeReasonTypeDef,
+    ScalingConstraintsTypeDef,
+    AutoTerminationPolicyOutputTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
+    PortRangeOutputTypeDef,
     PortRangeTypeDef,
+    ScriptBootstrapActionConfigOutputTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
     ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
-    KerberosAttributesTypeDef,
-    PlacementGroupConfigTypeDef,
+    KerberosAttributesOutputTypeDef,
+    PlacementGroupConfigOutputTypeDef,
+    TagOutputTypeDef,
     CommandTypeDef,
+    ComputeLimitsOutputTypeDef,
     ComputeLimitsTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
@@ -468,38 +477,47 @@
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
     DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
+    VolumeSpecificationOutputTypeDef,
     EbsVolumeTypeDef,
     EmptyResponseMetadataTypeDef,
+    ExecutionEngineConfigOutputTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
+    KeyValueOutputTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
+    SpotProvisioningSpecificationOutputTypeDef,
     SpotProvisioningSpecificationTypeDef,
+    OnDemandResizingSpecificationOutputTypeDef,
+    SpotResizingSpecificationOutputTypeDef,
     OnDemandResizingSpecificationTypeDef,
     SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
+    InstanceResizePolicyOutputTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
+    PlacementTypeOutputTypeDef,
+    KerberosAttributesTypeDef,
     ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
     ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
     ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
@@ -524,101 +542,117 @@
     ListSupportedInstanceTypesInputRequestTypeDef,
     SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
     ModifyClusterOutputTypeDef,
     NotebookS3LocationForOutputTypeDef,
     OutputNotebookS3LocationForOutputTypeDef,
     NotebookS3LocationFromInputTypeDef,
+    OnDemandCapacityReservationOptionsOutputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PaginatorConfigTypeDef,
+    PlacementGroupConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
     ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
     RunJobFlowOutputTypeDef,
+    SimpleScalingPolicyConfigurationOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
     StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
-    StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
+    BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
+    BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
+    CloudWatchAlarmDefinitionOutputTypeDef,
     CloudWatchAlarmDefinitionTypeDef,
     ClusterStatusTypeDef,
+    StudioTypeDef,
     ListBootstrapActionsOutputTypeDef,
+    ManagedScalingPolicyOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
+    HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
+    InstanceFleetResizingSpecificationsOutputTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
+    ShrinkPolicyOutputTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     ListSupportedInstanceTypesOutputTypeDef,
     NotebookExecutionSummaryTypeDef,
     NotebookExecutionTypeDef,
+    OnDemandProvisioningSpecificationOutputTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
+    ScalingActionOutputTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
-    DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
+    ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
+    DescribeStudioOutputTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
+    StepConfigOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
+    InstanceFleetProvisioningSpecificationsOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
+    ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
-    AddJobFlowStepsInputRequestTypeDef,
     StepDetailTypeDef,
+    AddJobFlowStepsInputRequestTypeDef,
     ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
```

### Comparing `mypy-boto3-emr-1.28.0/README.md` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-emr
+Version: 1.28.12
+Summary: Type annotations for boto3.EMR 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 emr type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,32 +429,41 @@
 
 ```python
 from mypy_boto3_emr.type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
     TagTypeDef,
+    ApplicationOutputTypeDef,
     ApplicationTypeDef,
-    ScalingConstraintsTypeDef,
+    ScalingConstraintsOutputTypeDef,
     AutoScalingPolicyStateChangeReasonTypeDef,
+    ScalingConstraintsTypeDef,
+    AutoTerminationPolicyOutputTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
+    PortRangeOutputTypeDef,
     PortRangeTypeDef,
+    ScriptBootstrapActionConfigOutputTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
     ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
-    KerberosAttributesTypeDef,
-    PlacementGroupConfigTypeDef,
+    KerberosAttributesOutputTypeDef,
+    PlacementGroupConfigOutputTypeDef,
+    TagOutputTypeDef,
     CommandTypeDef,
+    ComputeLimitsOutputTypeDef,
     ComputeLimitsTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
@@ -436,38 +477,47 @@
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
     DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
+    VolumeSpecificationOutputTypeDef,
     EbsVolumeTypeDef,
     EmptyResponseMetadataTypeDef,
+    ExecutionEngineConfigOutputTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
+    KeyValueOutputTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
+    SpotProvisioningSpecificationOutputTypeDef,
     SpotProvisioningSpecificationTypeDef,
+    OnDemandResizingSpecificationOutputTypeDef,
+    SpotResizingSpecificationOutputTypeDef,
     OnDemandResizingSpecificationTypeDef,
     SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
+    InstanceResizePolicyOutputTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
+    PlacementTypeOutputTypeDef,
+    KerberosAttributesTypeDef,
     ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
     ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
     ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
@@ -492,101 +542,117 @@
     ListSupportedInstanceTypesInputRequestTypeDef,
     SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
     ModifyClusterOutputTypeDef,
     NotebookS3LocationForOutputTypeDef,
     OutputNotebookS3LocationForOutputTypeDef,
     NotebookS3LocationFromInputTypeDef,
+    OnDemandCapacityReservationOptionsOutputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PaginatorConfigTypeDef,
+    PlacementGroupConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
     ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
     RunJobFlowOutputTypeDef,
+    SimpleScalingPolicyConfigurationOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
     StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
-    StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
+    BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
+    BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
+    CloudWatchAlarmDefinitionOutputTypeDef,
     CloudWatchAlarmDefinitionTypeDef,
     ClusterStatusTypeDef,
+    StudioTypeDef,
     ListBootstrapActionsOutputTypeDef,
+    ManagedScalingPolicyOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
+    HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
+    InstanceFleetResizingSpecificationsOutputTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
+    ShrinkPolicyOutputTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     ListSupportedInstanceTypesOutputTypeDef,
     NotebookExecutionSummaryTypeDef,
     NotebookExecutionTypeDef,
+    OnDemandProvisioningSpecificationOutputTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
+    ScalingActionOutputTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
-    DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
+    ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
+    DescribeStudioOutputTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
+    StepConfigOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
+    InstanceFleetProvisioningSpecificationsOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
+    ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
-    AddJobFlowStepsInputRequestTypeDef,
     StepDetailTypeDef,
+    AddJobFlowStepsInputRequestTypeDef,
     ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
```

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/__main__.py` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMR 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EMR 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
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

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,14 +358,15 @@
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
@@ -444,26 +445,28 @@
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

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,15 @@
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
@@ -442,26 +443,28 @@
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

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -59,38 +59,46 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddInstanceFleetOutputTypeDef",
     "AddInstanceGroupsOutputTypeDef",
     "AddJobFlowStepsOutputTypeDef",
     "TagTypeDef",
+    "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
-    "ScalingConstraintsTypeDef",
+    "ScalingConstraintsOutputTypeDef",
     "AutoScalingPolicyStateChangeReasonTypeDef",
+    "ScalingConstraintsTypeDef",
+    "AutoTerminationPolicyOutputTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
+    "PortRangeOutputTypeDef",
     "PortRangeTypeDef",
+    "ScriptBootstrapActionConfigOutputTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
     "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
-    "KerberosAttributesTypeDef",
-    "PlacementGroupConfigTypeDef",
+    "KerberosAttributesOutputTypeDef",
+    "PlacementGroupConfigOutputTypeDef",
+    "TagOutputTypeDef",
     "CommandTypeDef",
+    "ComputeLimitsOutputTypeDef",
     "ComputeLimitsTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
     "CreateSecurityConfigurationOutputTypeDef",
     "CreateStudioOutputTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
@@ -104,38 +112,47 @@
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
     "DescribeSecurityConfigurationOutputTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
     "VolumeSpecificationTypeDef",
+    "VolumeSpecificationOutputTypeDef",
     "EbsVolumeTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ExecutionEngineConfigOutputTypeDef",
     "ExecutionEngineConfigTypeDef",
     "FailureDetailsTypeDef",
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
+    "KeyValueOutputTypeDef",
     "KeyValueTypeDef",
     "HadoopStepConfigTypeDef",
+    "SpotProvisioningSpecificationOutputTypeDef",
     "SpotProvisioningSpecificationTypeDef",
+    "OnDemandResizingSpecificationOutputTypeDef",
+    "SpotResizingSpecificationOutputTypeDef",
     "OnDemandResizingSpecificationTypeDef",
     "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
+    "InstanceResizePolicyOutputTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
+    "PlacementTypeOutputTypeDef",
+    "KerberosAttributesTypeDef",
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
     "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
     "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
@@ -160,101 +177,117 @@
     "ListSupportedInstanceTypesInputRequestTypeDef",
     "SupportedInstanceTypeTypeDef",
     "ModifyClusterInputRequestTypeDef",
     "ModifyClusterOutputTypeDef",
     "NotebookS3LocationForOutputTypeDef",
     "OutputNotebookS3LocationForOutputTypeDef",
     "NotebookS3LocationFromInputTypeDef",
+    "OnDemandCapacityReservationOptionsOutputTypeDef",
     "OnDemandCapacityReservationOptionsTypeDef",
     "OutputNotebookS3LocationFromInputTypeDef",
     "PaginatorConfigTypeDef",
+    "PlacementGroupConfigTypeDef",
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SupportedProductConfigTypeDef",
     "RunJobFlowOutputTypeDef",
+    "SimpleScalingPolicyConfigurationOutputTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
     "StartNotebookExecutionOutputTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
     "UpdateStudioSessionMappingInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
-    "StudioTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
+    "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
+    "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
     "CancelStepsOutputTypeDef",
+    "CloudWatchAlarmDefinitionOutputTypeDef",
     "CloudWatchAlarmDefinitionTypeDef",
     "ClusterStatusTypeDef",
+    "StudioTypeDef",
     "ListBootstrapActionsOutputTypeDef",
+    "ManagedScalingPolicyOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
+    "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
+    "InstanceFleetResizingSpecificationsOutputTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
+    "ShrinkPolicyOutputTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
     "ListReleaseLabelsInputRequestTypeDef",
     "ListSecurityConfigurationsOutputTypeDef",
     "ListStudioSessionMappingsOutputTypeDef",
     "ListStudiosOutputTypeDef",
     "ListSupportedInstanceTypesOutputTypeDef",
     "NotebookExecutionSummaryTypeDef",
     "NotebookExecutionTypeDef",
+    "OnDemandProvisioningSpecificationOutputTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
+    "ScalingActionOutputTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
-    "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
+    "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
+    "DescribeStudioOutputTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
+    "StepConfigOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "ListNotebookExecutionsOutputTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
+    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
+    "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
-    "AddJobFlowStepsInputRequestTypeDef",
     "StepDetailTypeDef",
+    "AddJobFlowStepsInputRequestTypeDef",
     "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
@@ -307,27 +340,38 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+ApplicationOutputTypeDef = TypedDict(
+    "ApplicationOutputTypeDef",
     {
         "Name": str,
         "Version": str,
         "Args": List[str],
         "AdditionalInfo": Dict[str, str],
     },
     total=False,
 )
 
-ScalingConstraintsTypeDef = TypedDict(
-    "ScalingConstraintsTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+        "Args": Sequence[str],
+        "AdditionalInfo": Mapping[str, str],
+    },
+    total=False,
+)
+
+ScalingConstraintsOutputTypeDef = TypedDict(
+    "ScalingConstraintsOutputTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
 )
 
 AutoScalingPolicyStateChangeReasonTypeDef = TypedDict(
@@ -335,14 +379,30 @@
     {
         "Code": AutoScalingPolicyStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
 )
 
+ScalingConstraintsTypeDef = TypedDict(
+    "ScalingConstraintsTypeDef",
+    {
+        "MinCapacity": int,
+        "MaxCapacity": int,
+    },
+)
+
+AutoTerminationPolicyOutputTypeDef = TypedDict(
+    "AutoTerminationPolicyOutputTypeDef",
+    {
+        "IdleTimeout": int,
+    },
+    total=False,
+)
+
 AutoTerminationPolicyTypeDef = TypedDict(
     "AutoTerminationPolicyTypeDef",
     {
         "IdleTimeout": int,
     },
     total=False,
 )
@@ -351,54 +411,87 @@
     "BlockPublicAccessConfigurationMetadataTypeDef",
     {
         "CreationDateTime": datetime,
         "CreatedByArn": str,
     },
 )
 
+_RequiredPortRangeOutputTypeDef = TypedDict(
+    "_RequiredPortRangeOutputTypeDef",
+    {
+        "MinRange": int,
+    },
+)
+_OptionalPortRangeOutputTypeDef = TypedDict(
+    "_OptionalPortRangeOutputTypeDef",
+    {
+        "MaxRange": int,
+    },
+    total=False,
+)
+
+class PortRangeOutputTypeDef(_RequiredPortRangeOutputTypeDef, _OptionalPortRangeOutputTypeDef):
+    pass
+
 _RequiredPortRangeTypeDef = TypedDict(
     "_RequiredPortRangeTypeDef",
     {
         "MinRange": int,
     },
 )
 _OptionalPortRangeTypeDef = TypedDict(
     "_OptionalPortRangeTypeDef",
     {
         "MaxRange": int,
     },
     total=False,
 )
 
-
 class PortRangeTypeDef(_RequiredPortRangeTypeDef, _OptionalPortRangeTypeDef):
     pass
 
+_RequiredScriptBootstrapActionConfigOutputTypeDef = TypedDict(
+    "_RequiredScriptBootstrapActionConfigOutputTypeDef",
+    {
+        "Path": str,
+    },
+)
+_OptionalScriptBootstrapActionConfigOutputTypeDef = TypedDict(
+    "_OptionalScriptBootstrapActionConfigOutputTypeDef",
+    {
+        "Args": List[str],
+    },
+    total=False,
+)
+
+class ScriptBootstrapActionConfigOutputTypeDef(
+    _RequiredScriptBootstrapActionConfigOutputTypeDef,
+    _OptionalScriptBootstrapActionConfigOutputTypeDef,
+):
+    pass
 
 _RequiredScriptBootstrapActionConfigTypeDef = TypedDict(
     "_RequiredScriptBootstrapActionConfigTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalScriptBootstrapActionConfigTypeDef = TypedDict(
     "_OptionalScriptBootstrapActionConfigTypeDef",
     {
-        "Args": List[str],
+        "Args": Sequence[str],
     },
     total=False,
 )
 
-
 class ScriptBootstrapActionConfigTypeDef(
     _RequiredScriptBootstrapActionConfigTypeDef, _OptionalScriptBootstrapActionConfigTypeDef
 ):
     pass
 
-
 CancelStepsInfoTypeDef = TypedDict(
     "CancelStepsInfoTypeDef",
     {
         "StepId": str,
         "Status": CancelStepsRequestStatusType,
         "Reason": str,
     },
@@ -416,20 +509,27 @@
     "_OptionalCancelStepsInputRequestTypeDef",
     {
         "StepCancellationOption": StepCancellationOptionType,
     },
     total=False,
 )
 
-
 class CancelStepsInputRequestTypeDef(
     _RequiredCancelStepsInputRequestTypeDef, _OptionalCancelStepsInputRequestTypeDef
 ):
     pass
 
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
 
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Key": str,
         "Value": str,
     },
@@ -479,69 +579,96 @@
         "ServiceAccessSecurityGroup": str,
         "AdditionalMasterSecurityGroups": List[str],
         "AdditionalSlaveSecurityGroups": List[str],
     },
     total=False,
 )
 
-_RequiredKerberosAttributesTypeDef = TypedDict(
-    "_RequiredKerberosAttributesTypeDef",
+_RequiredKerberosAttributesOutputTypeDef = TypedDict(
+    "_RequiredKerberosAttributesOutputTypeDef",
     {
         "Realm": str,
         "KdcAdminPassword": str,
     },
 )
-_OptionalKerberosAttributesTypeDef = TypedDict(
-    "_OptionalKerberosAttributesTypeDef",
+_OptionalKerberosAttributesOutputTypeDef = TypedDict(
+    "_OptionalKerberosAttributesOutputTypeDef",
     {
         "CrossRealmTrustPrincipalPassword": str,
         "ADDomainJoinUser": str,
         "ADDomainJoinPassword": str,
     },
     total=False,
 )
 
-
-class KerberosAttributesTypeDef(
-    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
+class KerberosAttributesOutputTypeDef(
+    _RequiredKerberosAttributesOutputTypeDef, _OptionalKerberosAttributesOutputTypeDef
 ):
     pass
 
-
-_RequiredPlacementGroupConfigTypeDef = TypedDict(
-    "_RequiredPlacementGroupConfigTypeDef",
+_RequiredPlacementGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredPlacementGroupConfigOutputTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
     },
 )
-_OptionalPlacementGroupConfigTypeDef = TypedDict(
-    "_OptionalPlacementGroupConfigTypeDef",
+_OptionalPlacementGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalPlacementGroupConfigOutputTypeDef",
     {
         "PlacementStrategy": PlacementGroupStrategyType,
     },
     total=False,
 )
 
-
-class PlacementGroupConfigTypeDef(
-    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
+class PlacementGroupConfigOutputTypeDef(
+    _RequiredPlacementGroupConfigOutputTypeDef, _OptionalPlacementGroupConfigOutputTypeDef
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
 
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
     {
         "Name": str,
         "ScriptPath": str,
         "Args": List[str],
     },
     total=False,
 )
 
+_RequiredComputeLimitsOutputTypeDef = TypedDict(
+    "_RequiredComputeLimitsOutputTypeDef",
+    {
+        "UnitType": ComputeLimitsUnitTypeType,
+        "MinimumCapacityUnits": int,
+        "MaximumCapacityUnits": int,
+    },
+)
+_OptionalComputeLimitsOutputTypeDef = TypedDict(
+    "_OptionalComputeLimitsOutputTypeDef",
+    {
+        "MaximumOnDemandCapacityUnits": int,
+        "MaximumCoreCapacityUnits": int,
+    },
+    total=False,
+)
+
+class ComputeLimitsOutputTypeDef(
+    _RequiredComputeLimitsOutputTypeDef, _OptionalComputeLimitsOutputTypeDef
+):
+    pass
+
 _RequiredComputeLimitsTypeDef = TypedDict(
     "_RequiredComputeLimitsTypeDef",
     {
         "UnitType": ComputeLimitsUnitTypeType,
         "MinimumCapacityUnits": int,
         "MaximumCapacityUnits": int,
     },
@@ -551,18 +678,26 @@
     {
         "MaximumOnDemandCapacityUnits": int,
         "MaximumCoreCapacityUnits": int,
     },
     total=False,
 )
 
-
 class ComputeLimitsTypeDef(_RequiredComputeLimitsTypeDef, _OptionalComputeLimitsTypeDef):
     pass
 
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
+    {
+        "Classification": str,
+        "Configurations": List[Dict[str, Any]],
+        "Properties": Dict[str, str],
+    },
+    total=False,
+)
 
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Classification": str,
         "Configurations": Sequence[Dict[str, Any]],
         "Properties": Mapping[str, str],
@@ -609,22 +744,20 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
-
 class CreateStudioSessionMappingInputRequestTypeDef(
     _RequiredCreateStudioSessionMappingInputRequestTypeDef,
     _OptionalCreateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
-
 UsernamePasswordTypeDef = TypedDict(
     "UsernamePasswordTypeDef",
     {
         "Username": str,
         "Password": str,
     },
     total=False,
@@ -656,22 +789,20 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
-
 class DeleteStudioSessionMappingInputRequestTypeDef(
     _RequiredDeleteStudioSessionMappingInputRequestTypeDef,
     _OptionalDeleteStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -773,20 +904,39 @@
     {
         "Iops": int,
         "Throughput": int,
     },
     total=False,
 )
 
-
 class VolumeSpecificationTypeDef(
     _RequiredVolumeSpecificationTypeDef, _OptionalVolumeSpecificationTypeDef
 ):
     pass
 
+_RequiredVolumeSpecificationOutputTypeDef = TypedDict(
+    "_RequiredVolumeSpecificationOutputTypeDef",
+    {
+        "VolumeType": str,
+        "SizeInGB": int,
+    },
+)
+_OptionalVolumeSpecificationOutputTypeDef = TypedDict(
+    "_OptionalVolumeSpecificationOutputTypeDef",
+    {
+        "Iops": int,
+        "Throughput": int,
+    },
+    total=False,
+)
+
+class VolumeSpecificationOutputTypeDef(
+    _RequiredVolumeSpecificationOutputTypeDef, _OptionalVolumeSpecificationOutputTypeDef
+):
+    pass
 
 EbsVolumeTypeDef = TypedDict(
     "EbsVolumeTypeDef",
     {
         "Device": str,
         "VolumeId": str,
     },
@@ -796,14 +946,35 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredExecutionEngineConfigOutputTypeDef = TypedDict(
+    "_RequiredExecutionEngineConfigOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalExecutionEngineConfigOutputTypeDef = TypedDict(
+    "_OptionalExecutionEngineConfigOutputTypeDef",
+    {
+        "Type": Literal["EMR"],
+        "MasterInstanceSecurityGroupId": str,
+        "ExecutionRoleArn": str,
+    },
+    total=False,
+)
+
+class ExecutionEngineConfigOutputTypeDef(
+    _RequiredExecutionEngineConfigOutputTypeDef, _OptionalExecutionEngineConfigOutputTypeDef
+):
+    pass
+
 _RequiredExecutionEngineConfigTypeDef = TypedDict(
     "_RequiredExecutionEngineConfigTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalExecutionEngineConfigTypeDef = TypedDict(
@@ -812,21 +983,19 @@
         "Type": Literal["EMR"],
         "MasterInstanceSecurityGroupId": str,
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
-
 class ExecutionEngineConfigTypeDef(
     _RequiredExecutionEngineConfigTypeDef, _OptionalExecutionEngineConfigTypeDef
 ):
     pass
 
-
 FailureDetailsTypeDef = TypedDict(
     "FailureDetailsTypeDef",
     {
         "Reason": str,
         "Message": str,
         "LogFile": str,
     },
@@ -867,36 +1036,43 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
-
 class GetStudioSessionMappingInputRequestTypeDef(
     _RequiredGetStudioSessionMappingInputRequestTypeDef,
     _OptionalGetStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
-
 SessionMappingDetailTypeDef = TypedDict(
     "SessionMappingDetailTypeDef",
     {
         "StudioId": str,
         "IdentityId": str,
         "IdentityName": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+KeyValueOutputTypeDef = TypedDict(
+    "KeyValueOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 KeyValueTypeDef = TypedDict(
     "KeyValueTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -909,14 +1085,36 @@
         "Properties": Dict[str, str],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
+_RequiredSpotProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_RequiredSpotProvisioningSpecificationOutputTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+        "TimeoutAction": SpotProvisioningTimeoutActionType,
+    },
+)
+_OptionalSpotProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_OptionalSpotProvisioningSpecificationOutputTypeDef",
+    {
+        "BlockDurationMinutes": int,
+        "AllocationStrategy": SpotProvisioningAllocationStrategyType,
+    },
+    total=False,
+)
+
+class SpotProvisioningSpecificationOutputTypeDef(
+    _RequiredSpotProvisioningSpecificationOutputTypeDef,
+    _OptionalSpotProvisioningSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredSpotProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredSpotProvisioningSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
@@ -925,20 +1123,32 @@
     {
         "BlockDurationMinutes": int,
         "AllocationStrategy": SpotProvisioningAllocationStrategyType,
     },
     total=False,
 )
 
-
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
 ):
     pass
 
+OnDemandResizingSpecificationOutputTypeDef = TypedDict(
+    "OnDemandResizingSpecificationOutputTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
+
+SpotResizingSpecificationOutputTypeDef = TypedDict(
+    "SpotResizingSpecificationOutputTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
 
 OnDemandResizingSpecificationTypeDef = TypedDict(
     "OnDemandResizingSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
     },
 )
@@ -992,21 +1202,19 @@
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
         "CustomAmiId": str,
     },
     total=False,
 )
 
-
 class InstanceGroupDetailTypeDef(
     _RequiredInstanceGroupDetailTypeDef, _OptionalInstanceGroupDetailTypeDef
 ):
     pass
 
-
 InstanceGroupStateChangeReasonTypeDef = TypedDict(
     "InstanceGroupStateChangeReasonTypeDef",
     {
         "Code": InstanceGroupStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
@@ -1018,24 +1226,34 @@
         "CreationDateTime": datetime,
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-InstanceResizePolicyTypeDef = TypedDict(
-    "InstanceResizePolicyTypeDef",
+InstanceResizePolicyOutputTypeDef = TypedDict(
+    "InstanceResizePolicyOutputTypeDef",
     {
         "InstancesToTerminate": List[str],
         "InstancesToProtect": List[str],
         "InstanceTerminationTimeout": int,
     },
     total=False,
 )
 
+InstanceResizePolicyTypeDef = TypedDict(
+    "InstanceResizePolicyTypeDef",
+    {
+        "InstancesToTerminate": Sequence[str],
+        "InstancesToProtect": Sequence[str],
+        "InstanceTerminationTimeout": int,
+    },
+    total=False,
+)
+
 InstanceStateChangeReasonTypeDef = TypedDict(
     "InstanceStateChangeReasonTypeDef",
     {
         "Code": InstanceStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
@@ -1065,74 +1283,99 @@
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
         "LastStateChangeReason": str,
     },
     total=False,
 )
 
-
 class JobFlowExecutionStatusDetailTypeDef(
     _RequiredJobFlowExecutionStatusDetailTypeDef, _OptionalJobFlowExecutionStatusDetailTypeDef
 ):
     pass
 
-
 PlacementTypeTypeDef = TypedDict(
     "PlacementTypeTypeDef",
     {
         "AvailabilityZone": str,
+        "AvailabilityZones": Sequence[str],
+    },
+    total=False,
+)
+
+PlacementTypeOutputTypeDef = TypedDict(
+    "PlacementTypeOutputTypeDef",
+    {
+        "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
+_RequiredKerberosAttributesTypeDef = TypedDict(
+    "_RequiredKerberosAttributesTypeDef",
+    {
+        "Realm": str,
+        "KdcAdminPassword": str,
+    },
+)
+_OptionalKerberosAttributesTypeDef = TypedDict(
+    "_OptionalKerberosAttributesTypeDef",
+    {
+        "CrossRealmTrustPrincipalPassword": str,
+        "ADDomainJoinUser": str,
+        "ADDomainJoinPassword": str,
+    },
+    total=False,
+)
+
+class KerberosAttributesTypeDef(
+    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
+):
+    pass
+
 _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
     "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
     _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_OptionalListBootstrapActionsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
-
 ListClustersInputListClustersPaginateTypeDef = TypedDict(
     "ListClustersInputListClustersPaginateTypeDef",
     {
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ClusterStates": Sequence[ClusterStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1161,86 +1404,78 @@
     "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
     _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_OptionalListInstanceFleetsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListInstanceFleetsInputRequestTypeDef(
     _RequiredListInstanceFleetsInputRequestTypeDef, _OptionalListInstanceFleetsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
     "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
     _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_OptionalListInstanceGroupsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListInstanceGroupsInputRequestTypeDef(
     _RequiredListInstanceGroupsInputRequestTypeDef, _OptionalListInstanceGroupsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
     "_RequiredListInstancesInputListInstancesPaginateTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
@@ -1252,22 +1487,20 @@
         "InstanceFleetType": InstanceFleetTypeType,
         "InstanceStates": Sequence[InstanceStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInstancesInputListInstancesPaginateTypeDef(
     _RequiredListInstancesInputListInstancesPaginateTypeDef,
     _OptionalListInstancesInputListInstancesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListInstancesInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputRequestTypeDef = TypedDict(
@@ -1279,21 +1512,19 @@
         "InstanceFleetType": InstanceFleetTypeType,
         "InstanceStates": Sequence[InstanceStateType],
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
-
 ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
     "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
         "From": Union[datetime, str],
         "To": Union[datetime, str],
@@ -1371,21 +1602,19 @@
         "StepStates": Sequence[StepStateType],
         "StepIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListStepsInputListStepsPaginateTypeDef(
     _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
 ):
     pass
 
-
 _RequiredListStepsInputRequestTypeDef = TypedDict(
     "_RequiredListStepsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListStepsInputRequestTypeDef = TypedDict(
@@ -1394,21 +1623,19 @@
         "StepStates": Sequence[StepStateType],
         "StepIds": Sequence[str],
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListStepsInputRequestTypeDef(
     _RequiredListStepsInputRequestTypeDef, _OptionalListStepsInputRequestTypeDef
 ):
     pass
 
-
 ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
     "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -1478,22 +1705,20 @@
     "_OptionalListSupportedInstanceTypesInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListSupportedInstanceTypesInputRequestTypeDef(
     _RequiredListSupportedInstanceTypesInputRequestTypeDef,
     _OptionalListSupportedInstanceTypesInputRequestTypeDef,
 ):
     pass
 
-
 SupportedInstanceTypeTypeDef = TypedDict(
     "SupportedInstanceTypeTypeDef",
     {
         "Type": str,
         "MemoryGB": float,
         "StorageGB": int,
         "VCPU": int,
@@ -1518,21 +1743,19 @@
     "_OptionalModifyClusterInputRequestTypeDef",
     {
         "StepConcurrencyLevel": int,
     },
     total=False,
 )
 
-
 class ModifyClusterInputRequestTypeDef(
     _RequiredModifyClusterInputRequestTypeDef, _OptionalModifyClusterInputRequestTypeDef
 ):
     pass
 
-
 ModifyClusterOutputTypeDef = TypedDict(
     "ModifyClusterOutputTypeDef",
     {
         "StepConcurrencyLevel": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1560,14 +1783,24 @@
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
+OnDemandCapacityReservationOptionsOutputTypeDef = TypedDict(
+    "OnDemandCapacityReservationOptionsOutputTypeDef",
+    {
+        "UsageStrategy": Literal["use-capacity-reservations-first"],
+        "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
+        "CapacityReservationResourceGroupArn": str,
+    },
+    total=False,
+)
+
 OnDemandCapacityReservationOptionsTypeDef = TypedDict(
     "OnDemandCapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
         "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
         "CapacityReservationResourceGroupArn": str,
     },
@@ -1589,14 +1822,33 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPlacementGroupConfigTypeDef = TypedDict(
+    "_RequiredPlacementGroupConfigTypeDef",
+    {
+        "InstanceRole": InstanceRoleTypeType,
+    },
+)
+_OptionalPlacementGroupConfigTypeDef = TypedDict(
+    "_OptionalPlacementGroupConfigTypeDef",
+    {
+        "PlacementStrategy": PlacementGroupStrategyType,
+    },
+    total=False,
+)
+
+class PlacementGroupConfigTypeDef(
+    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
+):
+    pass
+
 RemoveAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
     },
 )
@@ -1648,14 +1900,35 @@
     {
         "JobFlowId": str,
         "ClusterArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSimpleScalingPolicyConfigurationOutputTypeDef",
+    {
+        "ScalingAdjustment": int,
+    },
+)
+_OptionalSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSimpleScalingPolicyConfigurationOutputTypeDef",
+    {
+        "AdjustmentType": AdjustmentTypeType,
+        "CoolDown": int,
+    },
+    total=False,
+)
+
+class SimpleScalingPolicyConfigurationOutputTypeDef(
+    _RequiredSimpleScalingPolicyConfigurationOutputTypeDef,
+    _OptionalSimpleScalingPolicyConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredSimpleScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredSimpleScalingPolicyConfigurationTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalSimpleScalingPolicyConfigurationTypeDef = TypedDict(
@@ -1663,22 +1936,20 @@
     {
         "AdjustmentType": AdjustmentTypeType,
         "CoolDown": int,
     },
     total=False,
 )
 
-
 class SimpleScalingPolicyConfigurationTypeDef(
     _RequiredSimpleScalingPolicyConfigurationTypeDef,
     _OptionalSimpleScalingPolicyConfigurationTypeDef,
 ):
     pass
 
-
 SetTerminationProtectionInputRequestTypeDef = TypedDict(
     "SetTerminationProtectionInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "TerminationProtected": bool,
     },
 )
@@ -1712,21 +1983,19 @@
         "StartDateTime": datetime,
         "EndDateTime": datetime,
         "LastStateChangeReason": str,
     },
     total=False,
 )
 
-
 class StepExecutionStatusDetailTypeDef(
     _RequiredStepExecutionStatusDetailTypeDef, _OptionalStepExecutionStatusDetailTypeDef
 ):
     pass
 
-
 StepStateChangeReasonTypeDef = TypedDict(
     "StepStateChangeReasonTypeDef",
     {
         "Code": Literal["NONE"],
         "Message": str,
     },
     total=False,
@@ -1769,21 +2038,19 @@
         "Description": str,
         "SubnetIds": Sequence[str],
         "DefaultS3Location": str,
     },
     total=False,
 )
 
-
 class UpdateStudioInputRequestTypeDef(
     _RequiredUpdateStudioInputRequestTypeDef, _OptionalUpdateStudioInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStudioSessionMappingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioSessionMappingInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
     },
@@ -1793,22 +2060,20 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
-
 class UpdateStudioSessionMappingInputRequestTypeDef(
     _RequiredUpdateStudioSessionMappingInputRequestTypeDef,
     _OptionalUpdateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1834,58 +2099,32 @@
         "IdpAuthUrl": str,
         "IdpRelayStateParameterName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateStudioInputRequestTypeDef(
     _RequiredCreateStudioInputRequestTypeDef, _OptionalCreateStudioInputRequestTypeDef
 ):
     pass
 
-
-StudioTypeDef = TypedDict(
-    "StudioTypeDef",
-    {
-        "StudioId": str,
-        "StudioArn": str,
-        "Name": str,
-        "Description": str,
-        "AuthMode": AuthModeType,
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "ServiceRole": str,
-        "UserRole": str,
-        "WorkspaceSecurityGroupId": str,
-        "EngineSecurityGroupId": str,
-        "Url": str,
-        "CreationTime": datetime,
-        "DefaultS3Location": str,
-        "IdpAuthUrl": str,
-        "IdpRelayStateParameterName": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
 )
 
 GetAutoTerminationPolicyOutputTypeDef = TypedDict(
     "GetAutoTerminationPolicyOutputTypeDef",
     {
-        "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
+        "AutoTerminationPolicy": AutoTerminationPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAutoTerminationPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutAutoTerminationPolicyInputRequestTypeDef",
     {
@@ -1896,42 +2135,66 @@
     "_OptionalPutAutoTerminationPolicyInputRequestTypeDef",
     {
         "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
     },
     total=False,
 )
 
-
 class PutAutoTerminationPolicyInputRequestTypeDef(
     _RequiredPutAutoTerminationPolicyInputRequestTypeDef,
     _OptionalPutAutoTerminationPolicyInputRequestTypeDef,
 ):
     pass
 
+_RequiredBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
+    "_RequiredBlockPublicAccessConfigurationOutputTypeDef",
+    {
+        "BlockPublicSecurityGroupRules": bool,
+    },
+)
+_OptionalBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
+    "_OptionalBlockPublicAccessConfigurationOutputTypeDef",
+    {
+        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeOutputTypeDef],
+    },
+    total=False,
+)
+
+class BlockPublicAccessConfigurationOutputTypeDef(
+    _RequiredBlockPublicAccessConfigurationOutputTypeDef,
+    _OptionalBlockPublicAccessConfigurationOutputTypeDef,
+):
+    pass
 
 _RequiredBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_RequiredBlockPublicAccessConfigurationTypeDef",
     {
         "BlockPublicSecurityGroupRules": bool,
     },
 )
 _OptionalBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_OptionalBlockPublicAccessConfigurationTypeDef",
     {
-        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
+        "PermittedPublicSecurityGroupRuleRanges": Sequence[PortRangeTypeDef],
     },
     total=False,
 )
 
-
 class BlockPublicAccessConfigurationTypeDef(
     _RequiredBlockPublicAccessConfigurationTypeDef, _OptionalBlockPublicAccessConfigurationTypeDef
 ):
     pass
 
+BootstrapActionConfigOutputTypeDef = TypedDict(
+    "BootstrapActionConfigOutputTypeDef",
+    {
+        "Name": str,
+        "ScriptBootstrapAction": ScriptBootstrapActionConfigOutputTypeDef,
+    },
+)
 
 BootstrapActionConfigTypeDef = TypedDict(
     "BootstrapActionConfigTypeDef",
     {
         "Name": str,
         "ScriptBootstrapAction": ScriptBootstrapActionConfigTypeDef,
     },
@@ -1941,14 +2204,40 @@
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchAlarmDefinitionOutputTypeDef",
+    {
+        "ComparisonOperator": ComparisonOperatorType,
+        "MetricName": str,
+        "Period": int,
+        "Threshold": float,
+    },
+)
+_OptionalCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchAlarmDefinitionOutputTypeDef",
+    {
+        "EvaluationPeriods": int,
+        "Namespace": str,
+        "Statistic": StatisticType,
+        "Unit": UnitType,
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+class CloudWatchAlarmDefinitionOutputTypeDef(
+    _RequiredCloudWatchAlarmDefinitionOutputTypeDef, _OptionalCloudWatchAlarmDefinitionOutputTypeDef
+):
+    pass
+
 _RequiredCloudWatchAlarmDefinitionTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
         "MetricName": str,
         "Period": int,
         "Threshold": float,
@@ -1962,41 +2251,71 @@
         "Statistic": StatisticType,
         "Unit": UnitType,
         "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
-
 class CloudWatchAlarmDefinitionTypeDef(
     _RequiredCloudWatchAlarmDefinitionTypeDef, _OptionalCloudWatchAlarmDefinitionTypeDef
 ):
     pass
 
-
 ClusterStatusTypeDef = TypedDict(
     "ClusterStatusTypeDef",
     {
         "State": ClusterStateType,
         "StateChangeReason": ClusterStateChangeReasonTypeDef,
         "Timeline": ClusterTimelineTypeDef,
         "ErrorDetails": List[ErrorDetailTypeDef],
     },
     total=False,
 )
 
+StudioTypeDef = TypedDict(
+    "StudioTypeDef",
+    {
+        "StudioId": str,
+        "StudioArn": str,
+        "Name": str,
+        "Description": str,
+        "AuthMode": AuthModeType,
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "ServiceRole": str,
+        "UserRole": str,
+        "WorkspaceSecurityGroupId": str,
+        "EngineSecurityGroupId": str,
+        "Url": str,
+        "CreationTime": datetime,
+        "DefaultS3Location": str,
+        "IdpAuthUrl": str,
+        "IdpRelayStateParameterName": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 ListBootstrapActionsOutputTypeDef = TypedDict(
     "ListBootstrapActionsOutputTypeDef",
     {
         "BootstrapActions": List[CommandTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ManagedScalingPolicyOutputTypeDef = TypedDict(
+    "ManagedScalingPolicyOutputTypeDef",
+    {
+        "ComputeLimits": ComputeLimitsOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagedScalingPolicyTypeDef = TypedDict(
     "ManagedScalingPolicyTypeDef",
     {
         "ComputeLimits": ComputeLimitsTypeDef,
     },
     total=False,
 )
@@ -2019,44 +2338,40 @@
     "_OptionalDescribeClusterInputClusterRunningWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeClusterInputClusterRunningWaitTypeDef(
     _RequiredDescribeClusterInputClusterRunningWaitTypeDef,
     _OptionalDescribeClusterInputClusterRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeClusterInputClusterTerminatedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterInputClusterTerminatedWaitTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalDescribeClusterInputClusterTerminatedWaitTypeDef = TypedDict(
     "_OptionalDescribeClusterInputClusterTerminatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeClusterInputClusterTerminatedWaitTypeDef(
     _RequiredDescribeClusterInputClusterTerminatedWaitTypeDef,
     _OptionalDescribeClusterInputClusterTerminatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeStepInputStepCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeStepInputStepCompleteWaitTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
     },
 )
@@ -2064,22 +2379,20 @@
     "_OptionalDescribeStepInputStepCompleteWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeStepInputStepCompleteWaitTypeDef(
     _RequiredDescribeStepInputStepCompleteWaitTypeDef,
     _OptionalDescribeStepInputStepCompleteWaitTypeDef,
 ):
     pass
 
-
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
@@ -2097,38 +2410,57 @@
     "_OptionalEbsBlockDeviceConfigTypeDef",
     {
         "VolumesPerInstance": int,
     },
     total=False,
 )
 
-
 class EbsBlockDeviceConfigTypeDef(
     _RequiredEbsBlockDeviceConfigTypeDef, _OptionalEbsBlockDeviceConfigTypeDef
 ):
     pass
 
-
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
-        "VolumeSpecification": VolumeSpecificationTypeDef,
+        "VolumeSpecification": VolumeSpecificationOutputTypeDef,
         "Device": str,
     },
     total=False,
 )
 
 GetStudioSessionMappingOutputTypeDef = TypedDict(
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredHadoopJarStepConfigOutputTypeDef = TypedDict(
+    "_RequiredHadoopJarStepConfigOutputTypeDef",
+    {
+        "Jar": str,
+    },
+)
+_OptionalHadoopJarStepConfigOutputTypeDef = TypedDict(
+    "_OptionalHadoopJarStepConfigOutputTypeDef",
+    {
+        "Properties": List[KeyValueOutputTypeDef],
+        "MainClass": str,
+        "Args": List[str],
+    },
+    total=False,
+)
+
+class HadoopJarStepConfigOutputTypeDef(
+    _RequiredHadoopJarStepConfigOutputTypeDef, _OptionalHadoopJarStepConfigOutputTypeDef
+):
+    pass
+
 _RequiredHadoopJarStepConfigTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigTypeDef",
     {
         "Jar": str,
     },
 )
 _OptionalHadoopJarStepConfigTypeDef = TypedDict(
@@ -2137,20 +2469,27 @@
         "Properties": Sequence[KeyValueTypeDef],
         "MainClass": str,
         "Args": Sequence[str],
     },
     total=False,
 )
 
-
 class HadoopJarStepConfigTypeDef(
     _RequiredHadoopJarStepConfigTypeDef, _OptionalHadoopJarStepConfigTypeDef
 ):
     pass
 
+InstanceFleetResizingSpecificationsOutputTypeDef = TypedDict(
+    "InstanceFleetResizingSpecificationsOutputTypeDef",
+    {
+        "SpotResizeSpecification": SpotResizingSpecificationOutputTypeDef,
+        "OnDemandResizeSpecification": OnDemandResizingSpecificationOutputTypeDef,
+    },
+    total=False,
+)
 
 InstanceFleetResizingSpecificationsTypeDef = TypedDict(
     "InstanceFleetResizingSpecificationsTypeDef",
     {
         "SpotResizeSpecification": SpotResizingSpecificationTypeDef,
         "OnDemandResizeSpecification": OnDemandResizingSpecificationTypeDef,
     },
@@ -2173,14 +2512,23 @@
         "State": InstanceGroupStateType,
         "StateChangeReason": InstanceGroupStateChangeReasonTypeDef,
         "Timeline": InstanceGroupTimelineTypeDef,
     },
     total=False,
 )
 
+ShrinkPolicyOutputTypeDef = TypedDict(
+    "ShrinkPolicyOutputTypeDef",
+    {
+        "DecommissionTimeout": int,
+        "InstanceResizePolicy": InstanceResizePolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 ShrinkPolicyTypeDef = TypedDict(
     "ShrinkPolicyTypeDef",
     {
         "DecommissionTimeout": int,
         "InstanceResizePolicy": InstanceResizePolicyTypeDef,
     },
     total=False,
@@ -2209,29 +2557,27 @@
     {
         "MasterPublicDnsName": str,
         "MasterInstanceId": str,
         "InstanceGroups": List[InstanceGroupDetailTypeDef],
         "NormalizedInstanceHours": int,
         "Ec2KeyName": str,
         "Ec2SubnetId": str,
-        "Placement": PlacementTypeTypeDef,
+        "Placement": PlacementTypeOutputTypeDef,
         "KeepJobFlowAliveWhenNoSteps": bool,
         "TerminationProtected": bool,
         "HadoopVersion": str,
     },
     total=False,
 )
 
-
 class JobFlowInstancesDetailTypeDef(
     _RequiredJobFlowInstancesDetailTypeDef, _OptionalJobFlowInstancesDetailTypeDef
 ):
     pass
 
-
 ListReleaseLabelsInputRequestTypeDef = TypedDict(
     "ListReleaseLabelsInputRequestTypeDef",
     {
         "Filters": ReleaseLabelFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2290,55 +2636,73 @@
 )
 
 NotebookExecutionTypeDef = TypedDict(
     "NotebookExecutionTypeDef",
     {
         "NotebookExecutionId": str,
         "EditorId": str,
-        "ExecutionEngine": ExecutionEngineConfigTypeDef,
+        "ExecutionEngine": ExecutionEngineConfigOutputTypeDef,
         "NotebookExecutionName": str,
         "NotebookParams": str,
         "Status": NotebookExecutionStatusType,
         "StartTime": datetime,
         "EndTime": datetime,
         "Arn": str,
         "OutputNotebookURI": str,
         "LastStateChangeReason": str,
         "NotebookInstanceSecurityGroupId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
         "OutputNotebookS3Location": OutputNotebookS3LocationForOutputTypeDef,
         "OutputNotebookFormat": Literal["HTML"],
         "EnvironmentVariables": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_RequiredOnDemandProvisioningSpecificationOutputTypeDef",
+    {
+        "AllocationStrategy": Literal["lowest-price"],
+    },
+)
+_OptionalOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_OptionalOnDemandProvisioningSpecificationOutputTypeDef",
+    {
+        "CapacityReservationOptions": OnDemandCapacityReservationOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class OnDemandProvisioningSpecificationOutputTypeDef(
+    _RequiredOnDemandProvisioningSpecificationOutputTypeDef,
+    _OptionalOnDemandProvisioningSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredOnDemandProvisioningSpecificationTypeDef",
     {
         "AllocationStrategy": Literal["lowest-price"],
     },
 )
 _OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
     "_OptionalOnDemandProvisioningSpecificationTypeDef",
     {
         "CapacityReservationOptions": OnDemandCapacityReservationOptionsTypeDef,
     },
     total=False,
 )
 
-
 class OnDemandProvisioningSpecificationTypeDef(
     _RequiredOnDemandProvisioningSpecificationTypeDef,
     _OptionalOnDemandProvisioningSpecificationTypeDef,
 ):
     pass
 
-
 _RequiredStartNotebookExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartNotebookExecutionInputRequestTypeDef",
     {
         "ExecutionEngine": ExecutionEngineConfigTypeDef,
         "ServiceRole": str,
     },
 )
@@ -2355,21 +2719,38 @@
         "OutputNotebookS3Location": OutputNotebookS3LocationFromInputTypeDef,
         "OutputNotebookFormat": Literal["HTML"],
         "EnvironmentVariables": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartNotebookExecutionInputRequestTypeDef(
     _RequiredStartNotebookExecutionInputRequestTypeDef,
     _OptionalStartNotebookExecutionInputRequestTypeDef,
 ):
     pass
 
+_RequiredScalingActionOutputTypeDef = TypedDict(
+    "_RequiredScalingActionOutputTypeDef",
+    {
+        "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationOutputTypeDef,
+    },
+)
+_OptionalScalingActionOutputTypeDef = TypedDict(
+    "_OptionalScalingActionOutputTypeDef",
+    {
+        "Market": MarketTypeType,
+    },
+    total=False,
+)
+
+class ScalingActionOutputTypeDef(
+    _RequiredScalingActionOutputTypeDef, _OptionalScalingActionOutputTypeDef
+):
+    pass
 
 _RequiredScalingActionTypeDef = TypedDict(
     "_RequiredScalingActionTypeDef",
     {
         "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationTypeDef,
     },
 )
@@ -2377,42 +2758,32 @@
     "_OptionalScalingActionTypeDef",
     {
         "Market": MarketTypeType,
     },
     total=False,
 )
 
-
 class ScalingActionTypeDef(_RequiredScalingActionTypeDef, _OptionalScalingActionTypeDef):
     pass
 
-
 StepStatusTypeDef = TypedDict(
     "StepStatusTypeDef",
     {
         "State": StepStateType,
         "StateChangeReason": StepStateChangeReasonTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "Timeline": StepTimelineTypeDef,
     },
     total=False,
 )
 
-DescribeStudioOutputTypeDef = TypedDict(
-    "DescribeStudioOutputTypeDef",
-    {
-        "Studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
-        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
+        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
@@ -2420,19 +2791,26 @@
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
     },
 )
 
 BootstrapActionDetailTypeDef = TypedDict(
     "BootstrapActionDetailTypeDef",
     {
-        "BootstrapActionConfig": BootstrapActionConfigTypeDef,
+        "BootstrapActionConfig": BootstrapActionConfigOutputTypeDef,
     },
     total=False,
 )
 
+ScalingTriggerOutputTypeDef = TypedDict(
+    "ScalingTriggerOutputTypeDef",
+    {
+        "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionOutputTypeDef,
+    },
+)
+
 ScalingTriggerTypeDef = TypedDict(
     "ScalingTriggerTypeDef",
     {
         "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionTypeDef,
     },
 )
 
@@ -2461,40 +2839,48 @@
         "LogEncryptionKmsKeyId": str,
         "RequestedAmiVersion": str,
         "RunningAmiVersion": str,
         "ReleaseLabel": str,
         "AutoTerminate": bool,
         "TerminationProtected": bool,
         "VisibleToAllUsers": bool,
-        "Applications": List[ApplicationTypeDef],
-        "Tags": List[TagTypeDef],
+        "Applications": List[ApplicationOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ServiceRole": str,
         "NormalizedInstanceHours": int,
         "MasterPublicDnsName": str,
-        "Configurations": List["ConfigurationTypeDef"],
+        "Configurations": List["ConfigurationOutputTypeDef"],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
         "CustomAmiId": str,
         "EbsRootVolumeSize": int,
         "RepoUpgradeOnBoot": RepoUpgradeOnBootType,
-        "KerberosAttributes": KerberosAttributesTypeDef,
+        "KerberosAttributes": KerberosAttributesOutputTypeDef,
         "ClusterArn": str,
         "OutpostArn": str,
         "StepConcurrencyLevel": int,
-        "PlacementGroups": List[PlacementGroupConfigTypeDef],
+        "PlacementGroups": List[PlacementGroupConfigOutputTypeDef],
         "OSReleaseLabel": str,
     },
     total=False,
 )
 
+DescribeStudioOutputTypeDef = TypedDict(
+    "DescribeStudioOutputTypeDef",
+    {
+        "Studio": StudioTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetManagedScalingPolicyOutputTypeDef = TypedDict(
     "GetManagedScalingPolicyOutputTypeDef",
     {
-        "ManagedScalingPolicy": ManagedScalingPolicyTypeDef,
+        "ManagedScalingPolicy": ManagedScalingPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedScalingPolicyInputRequestTypeDef = TypedDict(
     "PutManagedScalingPolicyInputRequestTypeDef",
     {
@@ -2524,22 +2910,40 @@
 InstanceTypeSpecificationTypeDef = TypedDict(
     "InstanceTypeSpecificationTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": int,
         "BidPrice": str,
         "BidPriceAsPercentageOfOnDemandPrice": float,
-        "Configurations": List["ConfigurationTypeDef"],
+        "Configurations": List["ConfigurationOutputTypeDef"],
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
         "CustomAmiId": str,
     },
     total=False,
 )
 
+_RequiredStepConfigOutputTypeDef = TypedDict(
+    "_RequiredStepConfigOutputTypeDef",
+    {
+        "Name": str,
+        "HadoopJarStep": HadoopJarStepConfigOutputTypeDef,
+    },
+)
+_OptionalStepConfigOutputTypeDef = TypedDict(
+    "_OptionalStepConfigOutputTypeDef",
+    {
+        "ActionOnFailure": ActionOnFailureType,
+    },
+    total=False,
+)
+
+class StepConfigOutputTypeDef(_RequiredStepConfigOutputTypeDef, _OptionalStepConfigOutputTypeDef):
+    pass
+
 _RequiredStepConfigTypeDef = TypedDict(
     "_RequiredStepConfigTypeDef",
     {
         "Name": str,
         "HadoopJarStep": HadoopJarStepConfigTypeDef,
     },
 )
@@ -2547,19 +2951,17 @@
     "_OptionalStepConfigTypeDef",
     {
         "ActionOnFailure": ActionOnFailureType,
     },
     total=False,
 )
 
-
 class StepConfigTypeDef(_RequiredStepConfigTypeDef, _OptionalStepConfigTypeDef):
     pass
 
-
 _RequiredInstanceFleetModifyConfigTypeDef = TypedDict(
     "_RequiredInstanceFleetModifyConfigTypeDef",
     {
         "InstanceFleetId": str,
     },
 )
 _OptionalInstanceFleetModifyConfigTypeDef = TypedDict(
@@ -2568,21 +2970,19 @@
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
-
 class InstanceFleetModifyConfigTypeDef(
     _RequiredInstanceFleetModifyConfigTypeDef, _OptionalInstanceFleetModifyConfigTypeDef
 ):
     pass
 
-
 _RequiredInstanceGroupModifyConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupModifyConfigTypeDef",
     {
         "InstanceGroupId": str,
     },
 )
 _OptionalInstanceGroupModifyConfigTypeDef = TypedDict(
@@ -2593,21 +2993,19 @@
         "ShrinkPolicy": ShrinkPolicyTypeDef,
         "ReconfigurationType": ReconfigurationTypeType,
         "Configurations": Sequence["ConfigurationTypeDef"],
     },
     total=False,
 )
 
-
 class InstanceGroupModifyConfigTypeDef(
     _RequiredInstanceGroupModifyConfigTypeDef, _OptionalInstanceGroupModifyConfigTypeDef
 ):
     pass
 
-
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "Id": str,
         "Ec2InstanceId": str,
         "PublicDnsName": str,
         "PublicIpAddress": str,
@@ -2636,14 +3034,23 @@
     "DescribeNotebookExecutionOutputTypeDef",
     {
         "NotebookExecution": NotebookExecutionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InstanceFleetProvisioningSpecificationsOutputTypeDef = TypedDict(
+    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
+    {
+        "SpotSpecification": SpotProvisioningSpecificationOutputTypeDef,
+        "OnDemandSpecification": OnDemandProvisioningSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
 InstanceFleetProvisioningSpecificationsTypeDef = TypedDict(
     "InstanceFleetProvisioningSpecificationsTypeDef",
     {
         "SpotSpecification": SpotProvisioningSpecificationTypeDef,
         "OnDemandSpecification": OnDemandProvisioningSpecificationTypeDef,
     },
     total=False,
@@ -2670,14 +3077,35 @@
         "ActionOnFailure": ActionOnFailureType,
         "Status": StepStatusTypeDef,
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
+_RequiredScalingRuleOutputTypeDef = TypedDict(
+    "_RequiredScalingRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Action": ScalingActionOutputTypeDef,
+        "Trigger": ScalingTriggerOutputTypeDef,
+    },
+)
+_OptionalScalingRuleOutputTypeDef = TypedDict(
+    "_OptionalScalingRuleOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class ScalingRuleOutputTypeDef(
+    _RequiredScalingRuleOutputTypeDef, _OptionalScalingRuleOutputTypeDef
+):
+    pass
+
 _RequiredScalingRuleTypeDef = TypedDict(
     "_RequiredScalingRuleTypeDef",
     {
         "Name": str,
         "Action": ScalingActionTypeDef,
         "Trigger": ScalingTriggerTypeDef,
     },
@@ -2686,19 +3114,17 @@
     "_OptionalScalingRuleTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ScalingRuleTypeDef(_RequiredScalingRuleTypeDef, _OptionalScalingRuleTypeDef):
     pass
 
-
 ListClustersOutputTypeDef = TypedDict(
     "ListClustersOutputTypeDef",
     {
         "Clusters": List[ClusterSummaryTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2727,20 +3153,26 @@
         "EbsConfiguration": EbsConfigurationTypeDef,
         "Configurations": Sequence["ConfigurationTypeDef"],
         "CustomAmiId": str,
     },
     total=False,
 )
 
-
 class InstanceTypeConfigTypeDef(
     _RequiredInstanceTypeConfigTypeDef, _OptionalInstanceTypeConfigTypeDef
 ):
     pass
 
+StepDetailTypeDef = TypedDict(
+    "StepDetailTypeDef",
+    {
+        "StepConfig": StepConfigOutputTypeDef,
+        "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
+    },
+)
 
 _RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
     "_RequiredAddJobFlowStepsInputRequestTypeDef",
     {
         "JobFlowId": str,
         "Steps": Sequence[StepConfigTypeDef],
     },
@@ -2749,29 +3181,19 @@
     "_OptionalAddJobFlowStepsInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
-
 class AddJobFlowStepsInputRequestTypeDef(
     _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
 ):
     pass
 
-
-StepDetailTypeDef = TypedDict(
-    "StepDetailTypeDef",
-    {
-        "StepConfig": StepConfigTypeDef,
-        "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
-    },
-)
-
 ModifyInstanceFleetInputRequestTypeDef = TypedDict(
     "ModifyInstanceFleetInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceFleet": InstanceFleetModifyConfigTypeDef,
     },
 )
@@ -2802,16 +3224,16 @@
         "Status": InstanceFleetStatusTypeDef,
         "InstanceFleetType": InstanceFleetTypeType,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ProvisionedOnDemandCapacity": int,
         "ProvisionedSpotCapacity": int,
         "InstanceTypeSpecifications": List[InstanceTypeSpecificationTypeDef],
-        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
-        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
+        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsOutputTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsOutputTypeDef,
     },
     total=False,
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
@@ -2829,16 +3251,16 @@
     },
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
-        "Constraints": ScalingConstraintsTypeDef,
-        "Rules": List[ScalingRuleTypeDef],
+        "Constraints": ScalingConstraintsOutputTypeDef,
+        "Rules": List[ScalingRuleOutputTypeDef],
     },
     total=False,
 )
 
 AutoScalingPolicyTypeDef = TypedDict(
     "AutoScalingPolicyTypeDef",
     {
@@ -2862,21 +3284,19 @@
         "InstanceTypeConfigs": Sequence[InstanceTypeConfigTypeDef],
         "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
         "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
-
 class InstanceFleetConfigTypeDef(
     _RequiredInstanceFleetConfigTypeDef, _OptionalInstanceFleetConfigTypeDef
 ):
     pass
 
-
 _RequiredJobFlowDetailTypeDef = TypedDict(
     "_RequiredJobFlowDetailTypeDef",
     {
         "JobFlowId": str,
         "Name": str,
         "ExecutionStatusDetail": JobFlowExecutionStatusDetailTypeDef,
         "Instances": JobFlowInstancesDetailTypeDef,
@@ -2896,19 +3316,17 @@
         "ServiceRole": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
     },
     total=False,
 )
 
-
 class JobFlowDetailTypeDef(_RequiredJobFlowDetailTypeDef, _OptionalJobFlowDetailTypeDef):
     pass
 
-
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2922,21 +3340,21 @@
         "Market": MarketTypeType,
         "InstanceGroupType": InstanceGroupTypeType,
         "BidPrice": str,
         "InstanceType": str,
         "RequestedInstanceCount": int,
         "RunningInstanceCount": int,
         "Status": InstanceGroupStatusTypeDef,
-        "Configurations": List["ConfigurationTypeDef"],
+        "Configurations": List["ConfigurationOutputTypeDef"],
         "ConfigurationsVersion": int,
-        "LastSuccessfullyAppliedConfigurations": List["ConfigurationTypeDef"],
+        "LastSuccessfullyAppliedConfigurations": List["ConfigurationOutputTypeDef"],
         "LastSuccessfullyAppliedConfigurationsVersion": int,
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
-        "ShrinkPolicy": ShrinkPolicyTypeDef,
+        "ShrinkPolicy": ShrinkPolicyOutputTypeDef,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "CustomAmiId": str,
     },
     total=False,
 )
 
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
@@ -2968,21 +3386,19 @@
         "EbsConfiguration": EbsConfigurationTypeDef,
         "AutoScalingPolicy": AutoScalingPolicyTypeDef,
         "CustomAmiId": str,
     },
     total=False,
 )
 
-
 class InstanceGroupConfigTypeDef(
     _RequiredInstanceGroupConfigTypeDef, _OptionalInstanceGroupConfigTypeDef
 ):
     pass
 
-
 PutAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "PutAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
         "AutoScalingPolicy": AutoScalingPolicyTypeDef,
     },
@@ -3082,12 +3498,11 @@
         "PlacementGroupConfigs": Sequence[PlacementGroupConfigTypeDef],
         "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
         "OSReleaseLabel": str,
     },
     total=False,
 )
 
-
 class RunJobFlowInputRequestTypeDef(
     _RequiredRunJobFlowInputRequestTypeDef, _OptionalRunJobFlowInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,37 +59,47 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddInstanceFleetOutputTypeDef",
     "AddInstanceGroupsOutputTypeDef",
     "AddJobFlowStepsOutputTypeDef",
     "TagTypeDef",
+    "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
-    "ScalingConstraintsTypeDef",
+    "ScalingConstraintsOutputTypeDef",
     "AutoScalingPolicyStateChangeReasonTypeDef",
+    "ScalingConstraintsTypeDef",
+    "AutoTerminationPolicyOutputTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
+    "PortRangeOutputTypeDef",
     "PortRangeTypeDef",
+    "ScriptBootstrapActionConfigOutputTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
     "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
-    "KerberosAttributesTypeDef",
-    "PlacementGroupConfigTypeDef",
+    "KerberosAttributesOutputTypeDef",
+    "PlacementGroupConfigOutputTypeDef",
+    "TagOutputTypeDef",
     "CommandTypeDef",
+    "ComputeLimitsOutputTypeDef",
     "ComputeLimitsTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
     "CreateSecurityConfigurationOutputTypeDef",
     "CreateStudioOutputTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
@@ -103,38 +113,47 @@
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
     "DescribeSecurityConfigurationOutputTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
     "VolumeSpecificationTypeDef",
+    "VolumeSpecificationOutputTypeDef",
     "EbsVolumeTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ExecutionEngineConfigOutputTypeDef",
     "ExecutionEngineConfigTypeDef",
     "FailureDetailsTypeDef",
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
+    "KeyValueOutputTypeDef",
     "KeyValueTypeDef",
     "HadoopStepConfigTypeDef",
+    "SpotProvisioningSpecificationOutputTypeDef",
     "SpotProvisioningSpecificationTypeDef",
+    "OnDemandResizingSpecificationOutputTypeDef",
+    "SpotResizingSpecificationOutputTypeDef",
     "OnDemandResizingSpecificationTypeDef",
     "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
+    "InstanceResizePolicyOutputTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
+    "PlacementTypeOutputTypeDef",
+    "KerberosAttributesTypeDef",
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
     "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
     "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
@@ -159,101 +178,117 @@
     "ListSupportedInstanceTypesInputRequestTypeDef",
     "SupportedInstanceTypeTypeDef",
     "ModifyClusterInputRequestTypeDef",
     "ModifyClusterOutputTypeDef",
     "NotebookS3LocationForOutputTypeDef",
     "OutputNotebookS3LocationForOutputTypeDef",
     "NotebookS3LocationFromInputTypeDef",
+    "OnDemandCapacityReservationOptionsOutputTypeDef",
     "OnDemandCapacityReservationOptionsTypeDef",
     "OutputNotebookS3LocationFromInputTypeDef",
     "PaginatorConfigTypeDef",
+    "PlacementGroupConfigTypeDef",
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SupportedProductConfigTypeDef",
     "RunJobFlowOutputTypeDef",
+    "SimpleScalingPolicyConfigurationOutputTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
     "StartNotebookExecutionOutputTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
     "UpdateStudioSessionMappingInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
-    "StudioTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
+    "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
+    "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
     "CancelStepsOutputTypeDef",
+    "CloudWatchAlarmDefinitionOutputTypeDef",
     "CloudWatchAlarmDefinitionTypeDef",
     "ClusterStatusTypeDef",
+    "StudioTypeDef",
     "ListBootstrapActionsOutputTypeDef",
+    "ManagedScalingPolicyOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
+    "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
+    "InstanceFleetResizingSpecificationsOutputTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
+    "ShrinkPolicyOutputTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
     "ListReleaseLabelsInputRequestTypeDef",
     "ListSecurityConfigurationsOutputTypeDef",
     "ListStudioSessionMappingsOutputTypeDef",
     "ListStudiosOutputTypeDef",
     "ListSupportedInstanceTypesOutputTypeDef",
     "NotebookExecutionSummaryTypeDef",
     "NotebookExecutionTypeDef",
+    "OnDemandProvisioningSpecificationOutputTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
+    "ScalingActionOutputTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
-    "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
+    "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
+    "DescribeStudioOutputTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
+    "StepConfigOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "ListNotebookExecutionsOutputTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
+    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
+    "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
-    "AddJobFlowStepsInputRequestTypeDef",
     "StepDetailTypeDef",
+    "AddJobFlowStepsInputRequestTypeDef",
     "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
@@ -306,27 +341,38 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+ApplicationOutputTypeDef = TypedDict(
+    "ApplicationOutputTypeDef",
     {
         "Name": str,
         "Version": str,
         "Args": List[str],
         "AdditionalInfo": Dict[str, str],
     },
     total=False,
 )
 
-ScalingConstraintsTypeDef = TypedDict(
-    "ScalingConstraintsTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+        "Args": Sequence[str],
+        "AdditionalInfo": Mapping[str, str],
+    },
+    total=False,
+)
+
+ScalingConstraintsOutputTypeDef = TypedDict(
+    "ScalingConstraintsOutputTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
 )
 
 AutoScalingPolicyStateChangeReasonTypeDef = TypedDict(
@@ -334,14 +380,30 @@
     {
         "Code": AutoScalingPolicyStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
 )
 
+ScalingConstraintsTypeDef = TypedDict(
+    "ScalingConstraintsTypeDef",
+    {
+        "MinCapacity": int,
+        "MaxCapacity": int,
+    },
+)
+
+AutoTerminationPolicyOutputTypeDef = TypedDict(
+    "AutoTerminationPolicyOutputTypeDef",
+    {
+        "IdleTimeout": int,
+    },
+    total=False,
+)
+
 AutoTerminationPolicyTypeDef = TypedDict(
     "AutoTerminationPolicyTypeDef",
     {
         "IdleTimeout": int,
     },
     total=False,
 )
@@ -350,50 +412,95 @@
     "BlockPublicAccessConfigurationMetadataTypeDef",
     {
         "CreationDateTime": datetime,
         "CreatedByArn": str,
     },
 )
 
+_RequiredPortRangeOutputTypeDef = TypedDict(
+    "_RequiredPortRangeOutputTypeDef",
+    {
+        "MinRange": int,
+    },
+)
+_OptionalPortRangeOutputTypeDef = TypedDict(
+    "_OptionalPortRangeOutputTypeDef",
+    {
+        "MaxRange": int,
+    },
+    total=False,
+)
+
+
+class PortRangeOutputTypeDef(_RequiredPortRangeOutputTypeDef, _OptionalPortRangeOutputTypeDef):
+    pass
+
+
 _RequiredPortRangeTypeDef = TypedDict(
     "_RequiredPortRangeTypeDef",
     {
         "MinRange": int,
     },
 )
 _OptionalPortRangeTypeDef = TypedDict(
     "_OptionalPortRangeTypeDef",
     {
         "MaxRange": int,
     },
     total=False,
 )
 
+
 class PortRangeTypeDef(_RequiredPortRangeTypeDef, _OptionalPortRangeTypeDef):
     pass
 
+
+_RequiredScriptBootstrapActionConfigOutputTypeDef = TypedDict(
+    "_RequiredScriptBootstrapActionConfigOutputTypeDef",
+    {
+        "Path": str,
+    },
+)
+_OptionalScriptBootstrapActionConfigOutputTypeDef = TypedDict(
+    "_OptionalScriptBootstrapActionConfigOutputTypeDef",
+    {
+        "Args": List[str],
+    },
+    total=False,
+)
+
+
+class ScriptBootstrapActionConfigOutputTypeDef(
+    _RequiredScriptBootstrapActionConfigOutputTypeDef,
+    _OptionalScriptBootstrapActionConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredScriptBootstrapActionConfigTypeDef = TypedDict(
     "_RequiredScriptBootstrapActionConfigTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalScriptBootstrapActionConfigTypeDef = TypedDict(
     "_OptionalScriptBootstrapActionConfigTypeDef",
     {
-        "Args": List[str],
+        "Args": Sequence[str],
     },
     total=False,
 )
 
+
 class ScriptBootstrapActionConfigTypeDef(
     _RequiredScriptBootstrapActionConfigTypeDef, _OptionalScriptBootstrapActionConfigTypeDef
 ):
     pass
 
+
 CancelStepsInfoTypeDef = TypedDict(
     "CancelStepsInfoTypeDef",
     {
         "StepId": str,
         "Status": CancelStepsRequestStatusType,
         "Reason": str,
     },
@@ -411,19 +518,30 @@
     "_OptionalCancelStepsInputRequestTypeDef",
     {
         "StepCancellationOption": StepCancellationOptionType,
     },
     total=False,
 )
 
+
 class CancelStepsInputRequestTypeDef(
     _RequiredCancelStepsInputRequestTypeDef, _OptionalCancelStepsInputRequestTypeDef
 ):
     pass
 
+
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -472,65 +590,102 @@
         "ServiceAccessSecurityGroup": str,
         "AdditionalMasterSecurityGroups": List[str],
         "AdditionalSlaveSecurityGroups": List[str],
     },
     total=False,
 )
 
-_RequiredKerberosAttributesTypeDef = TypedDict(
-    "_RequiredKerberosAttributesTypeDef",
+_RequiredKerberosAttributesOutputTypeDef = TypedDict(
+    "_RequiredKerberosAttributesOutputTypeDef",
     {
         "Realm": str,
         "KdcAdminPassword": str,
     },
 )
-_OptionalKerberosAttributesTypeDef = TypedDict(
-    "_OptionalKerberosAttributesTypeDef",
+_OptionalKerberosAttributesOutputTypeDef = TypedDict(
+    "_OptionalKerberosAttributesOutputTypeDef",
     {
         "CrossRealmTrustPrincipalPassword": str,
         "ADDomainJoinUser": str,
         "ADDomainJoinPassword": str,
     },
     total=False,
 )
 
-class KerberosAttributesTypeDef(
-    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
+
+class KerberosAttributesOutputTypeDef(
+    _RequiredKerberosAttributesOutputTypeDef, _OptionalKerberosAttributesOutputTypeDef
 ):
     pass
 
-_RequiredPlacementGroupConfigTypeDef = TypedDict(
-    "_RequiredPlacementGroupConfigTypeDef",
+
+_RequiredPlacementGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredPlacementGroupConfigOutputTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
     },
 )
-_OptionalPlacementGroupConfigTypeDef = TypedDict(
-    "_OptionalPlacementGroupConfigTypeDef",
+_OptionalPlacementGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalPlacementGroupConfigOutputTypeDef",
     {
         "PlacementStrategy": PlacementGroupStrategyType,
     },
     total=False,
 )
 
-class PlacementGroupConfigTypeDef(
-    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
+
+class PlacementGroupConfigOutputTypeDef(
+    _RequiredPlacementGroupConfigOutputTypeDef, _OptionalPlacementGroupConfigOutputTypeDef
 ):
     pass
 
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
     {
         "Name": str,
         "ScriptPath": str,
         "Args": List[str],
     },
     total=False,
 )
 
+_RequiredComputeLimitsOutputTypeDef = TypedDict(
+    "_RequiredComputeLimitsOutputTypeDef",
+    {
+        "UnitType": ComputeLimitsUnitTypeType,
+        "MinimumCapacityUnits": int,
+        "MaximumCapacityUnits": int,
+    },
+)
+_OptionalComputeLimitsOutputTypeDef = TypedDict(
+    "_OptionalComputeLimitsOutputTypeDef",
+    {
+        "MaximumOnDemandCapacityUnits": int,
+        "MaximumCoreCapacityUnits": int,
+    },
+    total=False,
+)
+
+
+class ComputeLimitsOutputTypeDef(
+    _RequiredComputeLimitsOutputTypeDef, _OptionalComputeLimitsOutputTypeDef
+):
+    pass
+
+
 _RequiredComputeLimitsTypeDef = TypedDict(
     "_RequiredComputeLimitsTypeDef",
     {
         "UnitType": ComputeLimitsUnitTypeType,
         "MinimumCapacityUnits": int,
         "MaximumCapacityUnits": int,
     },
@@ -540,17 +695,29 @@
     {
         "MaximumOnDemandCapacityUnits": int,
         "MaximumCoreCapacityUnits": int,
     },
     total=False,
 )
 
+
 class ComputeLimitsTypeDef(_RequiredComputeLimitsTypeDef, _OptionalComputeLimitsTypeDef):
     pass
 
+
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
+    {
+        "Classification": str,
+        "Configurations": List[Dict[str, Any]],
+        "Properties": Dict[str, str],
+    },
+    total=False,
+)
+
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Classification": str,
         "Configurations": Sequence[Dict[str, Any]],
         "Properties": Mapping[str, str],
     },
@@ -596,20 +763,22 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
+
 class CreateStudioSessionMappingInputRequestTypeDef(
     _RequiredCreateStudioSessionMappingInputRequestTypeDef,
     _OptionalCreateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
+
 UsernamePasswordTypeDef = TypedDict(
     "UsernamePasswordTypeDef",
     {
         "Username": str,
         "Password": str,
     },
     total=False,
@@ -641,20 +810,22 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
+
 class DeleteStudioSessionMappingInputRequestTypeDef(
     _RequiredDeleteStudioSessionMappingInputRequestTypeDef,
     _OptionalDeleteStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -756,19 +927,44 @@
     {
         "Iops": int,
         "Throughput": int,
     },
     total=False,
 )
 
+
 class VolumeSpecificationTypeDef(
     _RequiredVolumeSpecificationTypeDef, _OptionalVolumeSpecificationTypeDef
 ):
     pass
 
+
+_RequiredVolumeSpecificationOutputTypeDef = TypedDict(
+    "_RequiredVolumeSpecificationOutputTypeDef",
+    {
+        "VolumeType": str,
+        "SizeInGB": int,
+    },
+)
+_OptionalVolumeSpecificationOutputTypeDef = TypedDict(
+    "_OptionalVolumeSpecificationOutputTypeDef",
+    {
+        "Iops": int,
+        "Throughput": int,
+    },
+    total=False,
+)
+
+
+class VolumeSpecificationOutputTypeDef(
+    _RequiredVolumeSpecificationOutputTypeDef, _OptionalVolumeSpecificationOutputTypeDef
+):
+    pass
+
+
 EbsVolumeTypeDef = TypedDict(
     "EbsVolumeTypeDef",
     {
         "Device": str,
         "VolumeId": str,
     },
     total=False,
@@ -777,14 +973,37 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredExecutionEngineConfigOutputTypeDef = TypedDict(
+    "_RequiredExecutionEngineConfigOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalExecutionEngineConfigOutputTypeDef = TypedDict(
+    "_OptionalExecutionEngineConfigOutputTypeDef",
+    {
+        "Type": Literal["EMR"],
+        "MasterInstanceSecurityGroupId": str,
+        "ExecutionRoleArn": str,
+    },
+    total=False,
+)
+
+
+class ExecutionEngineConfigOutputTypeDef(
+    _RequiredExecutionEngineConfigOutputTypeDef, _OptionalExecutionEngineConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredExecutionEngineConfigTypeDef = TypedDict(
     "_RequiredExecutionEngineConfigTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalExecutionEngineConfigTypeDef = TypedDict(
@@ -793,19 +1012,21 @@
         "Type": Literal["EMR"],
         "MasterInstanceSecurityGroupId": str,
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
+
 class ExecutionEngineConfigTypeDef(
     _RequiredExecutionEngineConfigTypeDef, _OptionalExecutionEngineConfigTypeDef
 ):
     pass
 
+
 FailureDetailsTypeDef = TypedDict(
     "FailureDetailsTypeDef",
     {
         "Reason": str,
         "Message": str,
         "LogFile": str,
     },
@@ -846,34 +1067,45 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
+
 class GetStudioSessionMappingInputRequestTypeDef(
     _RequiredGetStudioSessionMappingInputRequestTypeDef,
     _OptionalGetStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
+
 SessionMappingDetailTypeDef = TypedDict(
     "SessionMappingDetailTypeDef",
     {
         "StudioId": str,
         "IdentityId": str,
         "IdentityName": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+KeyValueOutputTypeDef = TypedDict(
+    "KeyValueOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 KeyValueTypeDef = TypedDict(
     "KeyValueTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -886,14 +1118,38 @@
         "Properties": Dict[str, str],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
+_RequiredSpotProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_RequiredSpotProvisioningSpecificationOutputTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+        "TimeoutAction": SpotProvisioningTimeoutActionType,
+    },
+)
+_OptionalSpotProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_OptionalSpotProvisioningSpecificationOutputTypeDef",
+    {
+        "BlockDurationMinutes": int,
+        "AllocationStrategy": SpotProvisioningAllocationStrategyType,
+    },
+    total=False,
+)
+
+
+class SpotProvisioningSpecificationOutputTypeDef(
+    _RequiredSpotProvisioningSpecificationOutputTypeDef,
+    _OptionalSpotProvisioningSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredSpotProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredSpotProvisioningSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
@@ -902,19 +1158,35 @@
     {
         "BlockDurationMinutes": int,
         "AllocationStrategy": SpotProvisioningAllocationStrategyType,
     },
     total=False,
 )
 
+
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
 ):
     pass
 
+
+OnDemandResizingSpecificationOutputTypeDef = TypedDict(
+    "OnDemandResizingSpecificationOutputTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
+
+SpotResizingSpecificationOutputTypeDef = TypedDict(
+    "SpotResizingSpecificationOutputTypeDef",
+    {
+        "TimeoutDurationMinutes": int,
+    },
+)
+
 OnDemandResizingSpecificationTypeDef = TypedDict(
     "OnDemandResizingSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
     },
 )
 
@@ -967,19 +1239,21 @@
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
         "CustomAmiId": str,
     },
     total=False,
 )
 
+
 class InstanceGroupDetailTypeDef(
     _RequiredInstanceGroupDetailTypeDef, _OptionalInstanceGroupDetailTypeDef
 ):
     pass
 
+
 InstanceGroupStateChangeReasonTypeDef = TypedDict(
     "InstanceGroupStateChangeReasonTypeDef",
     {
         "Code": InstanceGroupStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
@@ -991,24 +1265,34 @@
         "CreationDateTime": datetime,
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-InstanceResizePolicyTypeDef = TypedDict(
-    "InstanceResizePolicyTypeDef",
+InstanceResizePolicyOutputTypeDef = TypedDict(
+    "InstanceResizePolicyOutputTypeDef",
     {
         "InstancesToTerminate": List[str],
         "InstancesToProtect": List[str],
         "InstanceTerminationTimeout": int,
     },
     total=False,
 )
 
+InstanceResizePolicyTypeDef = TypedDict(
+    "InstanceResizePolicyTypeDef",
+    {
+        "InstancesToTerminate": Sequence[str],
+        "InstancesToProtect": Sequence[str],
+        "InstanceTerminationTimeout": int,
+    },
+    total=False,
+)
+
 InstanceStateChangeReasonTypeDef = TypedDict(
     "InstanceStateChangeReasonTypeDef",
     {
         "Code": InstanceStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
@@ -1038,68 +1322,107 @@
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
         "LastStateChangeReason": str,
     },
     total=False,
 )
 
+
 class JobFlowExecutionStatusDetailTypeDef(
     _RequiredJobFlowExecutionStatusDetailTypeDef, _OptionalJobFlowExecutionStatusDetailTypeDef
 ):
     pass
 
+
 PlacementTypeTypeDef = TypedDict(
     "PlacementTypeTypeDef",
     {
         "AvailabilityZone": str,
+        "AvailabilityZones": Sequence[str],
+    },
+    total=False,
+)
+
+PlacementTypeOutputTypeDef = TypedDict(
+    "PlacementTypeOutputTypeDef",
+    {
+        "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
+_RequiredKerberosAttributesTypeDef = TypedDict(
+    "_RequiredKerberosAttributesTypeDef",
+    {
+        "Realm": str,
+        "KdcAdminPassword": str,
+    },
+)
+_OptionalKerberosAttributesTypeDef = TypedDict(
+    "_OptionalKerberosAttributesTypeDef",
+    {
+        "CrossRealmTrustPrincipalPassword": str,
+        "ADDomainJoinUser": str,
+        "ADDomainJoinPassword": str,
+    },
+    total=False,
+)
+
+
+class KerberosAttributesTypeDef(
+    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
+):
+    pass
+
+
 _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
     "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
     _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_OptionalListBootstrapActionsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
+
 ListClustersInputListClustersPaginateTypeDef = TypedDict(
     "ListClustersInputListClustersPaginateTypeDef",
     {
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ClusterStates": Sequence[ClusterStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1128,78 +1451,86 @@
     "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
     _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_OptionalListInstanceFleetsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListInstanceFleetsInputRequestTypeDef(
     _RequiredListInstanceFleetsInputRequestTypeDef, _OptionalListInstanceFleetsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
     "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
     _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_OptionalListInstanceGroupsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListInstanceGroupsInputRequestTypeDef(
     _RequiredListInstanceGroupsInputRequestTypeDef, _OptionalListInstanceGroupsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
     "_RequiredListInstancesInputListInstancesPaginateTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
@@ -1211,20 +1542,22 @@
         "InstanceFleetType": InstanceFleetTypeType,
         "InstanceStates": Sequence[InstanceStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInstancesInputListInstancesPaginateTypeDef(
     _RequiredListInstancesInputListInstancesPaginateTypeDef,
     _OptionalListInstancesInputListInstancesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListInstancesInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputRequestTypeDef = TypedDict(
@@ -1236,19 +1569,21 @@
         "InstanceFleetType": InstanceFleetTypeType,
         "InstanceStates": Sequence[InstanceStateType],
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
+
 ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
     "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
         "From": Union[datetime, str],
         "To": Union[datetime, str],
@@ -1326,19 +1661,21 @@
         "StepStates": Sequence[StepStateType],
         "StepIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListStepsInputListStepsPaginateTypeDef(
     _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
 ):
     pass
 
+
 _RequiredListStepsInputRequestTypeDef = TypedDict(
     "_RequiredListStepsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListStepsInputRequestTypeDef = TypedDict(
@@ -1347,19 +1684,21 @@
         "StepStates": Sequence[StepStateType],
         "StepIds": Sequence[str],
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListStepsInputRequestTypeDef(
     _RequiredListStepsInputRequestTypeDef, _OptionalListStepsInputRequestTypeDef
 ):
     pass
 
+
 ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
     "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -1429,20 +1768,22 @@
     "_OptionalListSupportedInstanceTypesInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListSupportedInstanceTypesInputRequestTypeDef(
     _RequiredListSupportedInstanceTypesInputRequestTypeDef,
     _OptionalListSupportedInstanceTypesInputRequestTypeDef,
 ):
     pass
 
+
 SupportedInstanceTypeTypeDef = TypedDict(
     "SupportedInstanceTypeTypeDef",
     {
         "Type": str,
         "MemoryGB": float,
         "StorageGB": int,
         "VCPU": int,
@@ -1467,19 +1808,21 @@
     "_OptionalModifyClusterInputRequestTypeDef",
     {
         "StepConcurrencyLevel": int,
     },
     total=False,
 )
 
+
 class ModifyClusterInputRequestTypeDef(
     _RequiredModifyClusterInputRequestTypeDef, _OptionalModifyClusterInputRequestTypeDef
 ):
     pass
 
+
 ModifyClusterOutputTypeDef = TypedDict(
     "ModifyClusterOutputTypeDef",
     {
         "StepConcurrencyLevel": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1507,14 +1850,24 @@
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
+OnDemandCapacityReservationOptionsOutputTypeDef = TypedDict(
+    "OnDemandCapacityReservationOptionsOutputTypeDef",
+    {
+        "UsageStrategy": Literal["use-capacity-reservations-first"],
+        "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
+        "CapacityReservationResourceGroupArn": str,
+    },
+    total=False,
+)
+
 OnDemandCapacityReservationOptionsTypeDef = TypedDict(
     "OnDemandCapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
         "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
         "CapacityReservationResourceGroupArn": str,
     },
@@ -1536,14 +1889,35 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPlacementGroupConfigTypeDef = TypedDict(
+    "_RequiredPlacementGroupConfigTypeDef",
+    {
+        "InstanceRole": InstanceRoleTypeType,
+    },
+)
+_OptionalPlacementGroupConfigTypeDef = TypedDict(
+    "_OptionalPlacementGroupConfigTypeDef",
+    {
+        "PlacementStrategy": PlacementGroupStrategyType,
+    },
+    total=False,
+)
+
+
+class PlacementGroupConfigTypeDef(
+    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
+):
+    pass
+
+
 RemoveAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
     },
 )
@@ -1595,14 +1969,37 @@
     {
         "JobFlowId": str,
         "ClusterArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSimpleScalingPolicyConfigurationOutputTypeDef",
+    {
+        "ScalingAdjustment": int,
+    },
+)
+_OptionalSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSimpleScalingPolicyConfigurationOutputTypeDef",
+    {
+        "AdjustmentType": AdjustmentTypeType,
+        "CoolDown": int,
+    },
+    total=False,
+)
+
+
+class SimpleScalingPolicyConfigurationOutputTypeDef(
+    _RequiredSimpleScalingPolicyConfigurationOutputTypeDef,
+    _OptionalSimpleScalingPolicyConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredSimpleScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredSimpleScalingPolicyConfigurationTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalSimpleScalingPolicyConfigurationTypeDef = TypedDict(
@@ -1610,20 +2007,22 @@
     {
         "AdjustmentType": AdjustmentTypeType,
         "CoolDown": int,
     },
     total=False,
 )
 
+
 class SimpleScalingPolicyConfigurationTypeDef(
     _RequiredSimpleScalingPolicyConfigurationTypeDef,
     _OptionalSimpleScalingPolicyConfigurationTypeDef,
 ):
     pass
 
+
 SetTerminationProtectionInputRequestTypeDef = TypedDict(
     "SetTerminationProtectionInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "TerminationProtected": bool,
     },
 )
@@ -1657,19 +2056,21 @@
         "StartDateTime": datetime,
         "EndDateTime": datetime,
         "LastStateChangeReason": str,
     },
     total=False,
 )
 
+
 class StepExecutionStatusDetailTypeDef(
     _RequiredStepExecutionStatusDetailTypeDef, _OptionalStepExecutionStatusDetailTypeDef
 ):
     pass
 
+
 StepStateChangeReasonTypeDef = TypedDict(
     "StepStateChangeReasonTypeDef",
     {
         "Code": Literal["NONE"],
         "Message": str,
     },
     total=False,
@@ -1712,19 +2113,21 @@
         "Description": str,
         "SubnetIds": Sequence[str],
         "DefaultS3Location": str,
     },
     total=False,
 )
 
+
 class UpdateStudioInputRequestTypeDef(
     _RequiredUpdateStudioInputRequestTypeDef, _OptionalUpdateStudioInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStudioSessionMappingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioSessionMappingInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
     },
@@ -1734,20 +2137,22 @@
     {
         "IdentityId": str,
         "IdentityName": str,
     },
     total=False,
 )
 
+
 class UpdateStudioSessionMappingInputRequestTypeDef(
     _RequiredUpdateStudioSessionMappingInputRequestTypeDef,
     _OptionalUpdateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1773,56 +2178,34 @@
         "IdpAuthUrl": str,
         "IdpRelayStateParameterName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateStudioInputRequestTypeDef(
     _RequiredCreateStudioInputRequestTypeDef, _OptionalCreateStudioInputRequestTypeDef
 ):
     pass
 
-StudioTypeDef = TypedDict(
-    "StudioTypeDef",
-    {
-        "StudioId": str,
-        "StudioArn": str,
-        "Name": str,
-        "Description": str,
-        "AuthMode": AuthModeType,
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "ServiceRole": str,
-        "UserRole": str,
-        "WorkspaceSecurityGroupId": str,
-        "EngineSecurityGroupId": str,
-        "Url": str,
-        "CreationTime": datetime,
-        "DefaultS3Location": str,
-        "IdpAuthUrl": str,
-        "IdpRelayStateParameterName": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
 
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
 )
 
 GetAutoTerminationPolicyOutputTypeDef = TypedDict(
     "GetAutoTerminationPolicyOutputTypeDef",
     {
-        "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
+        "AutoTerminationPolicy": AutoTerminationPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAutoTerminationPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutAutoTerminationPolicyInputRequestTypeDef",
     {
@@ -1833,39 +2216,73 @@
     "_OptionalPutAutoTerminationPolicyInputRequestTypeDef",
     {
         "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
     },
     total=False,
 )
 
+
 class PutAutoTerminationPolicyInputRequestTypeDef(
     _RequiredPutAutoTerminationPolicyInputRequestTypeDef,
     _OptionalPutAutoTerminationPolicyInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
+    "_RequiredBlockPublicAccessConfigurationOutputTypeDef",
+    {
+        "BlockPublicSecurityGroupRules": bool,
+    },
+)
+_OptionalBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
+    "_OptionalBlockPublicAccessConfigurationOutputTypeDef",
+    {
+        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class BlockPublicAccessConfigurationOutputTypeDef(
+    _RequiredBlockPublicAccessConfigurationOutputTypeDef,
+    _OptionalBlockPublicAccessConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_RequiredBlockPublicAccessConfigurationTypeDef",
     {
         "BlockPublicSecurityGroupRules": bool,
     },
 )
 _OptionalBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_OptionalBlockPublicAccessConfigurationTypeDef",
     {
-        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
+        "PermittedPublicSecurityGroupRuleRanges": Sequence[PortRangeTypeDef],
     },
     total=False,
 )
 
+
 class BlockPublicAccessConfigurationTypeDef(
     _RequiredBlockPublicAccessConfigurationTypeDef, _OptionalBlockPublicAccessConfigurationTypeDef
 ):
     pass
 
+
+BootstrapActionConfigOutputTypeDef = TypedDict(
+    "BootstrapActionConfigOutputTypeDef",
+    {
+        "Name": str,
+        "ScriptBootstrapAction": ScriptBootstrapActionConfigOutputTypeDef,
+    },
+)
+
 BootstrapActionConfigTypeDef = TypedDict(
     "BootstrapActionConfigTypeDef",
     {
         "Name": str,
         "ScriptBootstrapAction": ScriptBootstrapActionConfigTypeDef,
     },
 )
@@ -1874,14 +2291,42 @@
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchAlarmDefinitionOutputTypeDef",
+    {
+        "ComparisonOperator": ComparisonOperatorType,
+        "MetricName": str,
+        "Period": int,
+        "Threshold": float,
+    },
+)
+_OptionalCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchAlarmDefinitionOutputTypeDef",
+    {
+        "EvaluationPeriods": int,
+        "Namespace": str,
+        "Statistic": StatisticType,
+        "Unit": UnitType,
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class CloudWatchAlarmDefinitionOutputTypeDef(
+    _RequiredCloudWatchAlarmDefinitionOutputTypeDef, _OptionalCloudWatchAlarmDefinitionOutputTypeDef
+):
+    pass
+
+
 _RequiredCloudWatchAlarmDefinitionTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
         "MetricName": str,
         "Period": int,
         "Threshold": float,
@@ -1895,39 +2340,73 @@
         "Statistic": StatisticType,
         "Unit": UnitType,
         "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
+
 class CloudWatchAlarmDefinitionTypeDef(
     _RequiredCloudWatchAlarmDefinitionTypeDef, _OptionalCloudWatchAlarmDefinitionTypeDef
 ):
     pass
 
+
 ClusterStatusTypeDef = TypedDict(
     "ClusterStatusTypeDef",
     {
         "State": ClusterStateType,
         "StateChangeReason": ClusterStateChangeReasonTypeDef,
         "Timeline": ClusterTimelineTypeDef,
         "ErrorDetails": List[ErrorDetailTypeDef],
     },
     total=False,
 )
 
+StudioTypeDef = TypedDict(
+    "StudioTypeDef",
+    {
+        "StudioId": str,
+        "StudioArn": str,
+        "Name": str,
+        "Description": str,
+        "AuthMode": AuthModeType,
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "ServiceRole": str,
+        "UserRole": str,
+        "WorkspaceSecurityGroupId": str,
+        "EngineSecurityGroupId": str,
+        "Url": str,
+        "CreationTime": datetime,
+        "DefaultS3Location": str,
+        "IdpAuthUrl": str,
+        "IdpRelayStateParameterName": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 ListBootstrapActionsOutputTypeDef = TypedDict(
     "ListBootstrapActionsOutputTypeDef",
     {
         "BootstrapActions": List[CommandTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ManagedScalingPolicyOutputTypeDef = TypedDict(
+    "ManagedScalingPolicyOutputTypeDef",
+    {
+        "ComputeLimits": ComputeLimitsOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagedScalingPolicyTypeDef = TypedDict(
     "ManagedScalingPolicyTypeDef",
     {
         "ComputeLimits": ComputeLimitsTypeDef,
     },
     total=False,
 )
@@ -1950,40 +2429,44 @@
     "_OptionalDescribeClusterInputClusterRunningWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeClusterInputClusterRunningWaitTypeDef(
     _RequiredDescribeClusterInputClusterRunningWaitTypeDef,
     _OptionalDescribeClusterInputClusterRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeClusterInputClusterTerminatedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterInputClusterTerminatedWaitTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalDescribeClusterInputClusterTerminatedWaitTypeDef = TypedDict(
     "_OptionalDescribeClusterInputClusterTerminatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeClusterInputClusterTerminatedWaitTypeDef(
     _RequiredDescribeClusterInputClusterTerminatedWaitTypeDef,
     _OptionalDescribeClusterInputClusterTerminatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeStepInputStepCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeStepInputStepCompleteWaitTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
     },
 )
@@ -1991,20 +2474,22 @@
     "_OptionalDescribeStepInputStepCompleteWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeStepInputStepCompleteWaitTypeDef(
     _RequiredDescribeStepInputStepCompleteWaitTypeDef,
     _OptionalDescribeStepInputStepCompleteWaitTypeDef,
 ):
     pass
 
+
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
@@ -2022,36 +2507,61 @@
     "_OptionalEbsBlockDeviceConfigTypeDef",
     {
         "VolumesPerInstance": int,
     },
     total=False,
 )
 
+
 class EbsBlockDeviceConfigTypeDef(
     _RequiredEbsBlockDeviceConfigTypeDef, _OptionalEbsBlockDeviceConfigTypeDef
 ):
     pass
 
+
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
-        "VolumeSpecification": VolumeSpecificationTypeDef,
+        "VolumeSpecification": VolumeSpecificationOutputTypeDef,
         "Device": str,
     },
     total=False,
 )
 
 GetStudioSessionMappingOutputTypeDef = TypedDict(
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredHadoopJarStepConfigOutputTypeDef = TypedDict(
+    "_RequiredHadoopJarStepConfigOutputTypeDef",
+    {
+        "Jar": str,
+    },
+)
+_OptionalHadoopJarStepConfigOutputTypeDef = TypedDict(
+    "_OptionalHadoopJarStepConfigOutputTypeDef",
+    {
+        "Properties": List[KeyValueOutputTypeDef],
+        "MainClass": str,
+        "Args": List[str],
+    },
+    total=False,
+)
+
+
+class HadoopJarStepConfigOutputTypeDef(
+    _RequiredHadoopJarStepConfigOutputTypeDef, _OptionalHadoopJarStepConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredHadoopJarStepConfigTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigTypeDef",
     {
         "Jar": str,
     },
 )
 _OptionalHadoopJarStepConfigTypeDef = TypedDict(
@@ -2060,19 +2570,30 @@
         "Properties": Sequence[KeyValueTypeDef],
         "MainClass": str,
         "Args": Sequence[str],
     },
     total=False,
 )
 
+
 class HadoopJarStepConfigTypeDef(
     _RequiredHadoopJarStepConfigTypeDef, _OptionalHadoopJarStepConfigTypeDef
 ):
     pass
 
+
+InstanceFleetResizingSpecificationsOutputTypeDef = TypedDict(
+    "InstanceFleetResizingSpecificationsOutputTypeDef",
+    {
+        "SpotResizeSpecification": SpotResizingSpecificationOutputTypeDef,
+        "OnDemandResizeSpecification": OnDemandResizingSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
 InstanceFleetResizingSpecificationsTypeDef = TypedDict(
     "InstanceFleetResizingSpecificationsTypeDef",
     {
         "SpotResizeSpecification": SpotResizingSpecificationTypeDef,
         "OnDemandResizeSpecification": OnDemandResizingSpecificationTypeDef,
     },
     total=False,
@@ -2094,14 +2615,23 @@
         "State": InstanceGroupStateType,
         "StateChangeReason": InstanceGroupStateChangeReasonTypeDef,
         "Timeline": InstanceGroupTimelineTypeDef,
     },
     total=False,
 )
 
+ShrinkPolicyOutputTypeDef = TypedDict(
+    "ShrinkPolicyOutputTypeDef",
+    {
+        "DecommissionTimeout": int,
+        "InstanceResizePolicy": InstanceResizePolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 ShrinkPolicyTypeDef = TypedDict(
     "ShrinkPolicyTypeDef",
     {
         "DecommissionTimeout": int,
         "InstanceResizePolicy": InstanceResizePolicyTypeDef,
     },
     total=False,
@@ -2130,27 +2660,29 @@
     {
         "MasterPublicDnsName": str,
         "MasterInstanceId": str,
         "InstanceGroups": List[InstanceGroupDetailTypeDef],
         "NormalizedInstanceHours": int,
         "Ec2KeyName": str,
         "Ec2SubnetId": str,
-        "Placement": PlacementTypeTypeDef,
+        "Placement": PlacementTypeOutputTypeDef,
         "KeepJobFlowAliveWhenNoSteps": bool,
         "TerminationProtected": bool,
         "HadoopVersion": str,
     },
     total=False,
 )
 
+
 class JobFlowInstancesDetailTypeDef(
     _RequiredJobFlowInstancesDetailTypeDef, _OptionalJobFlowInstancesDetailTypeDef
 ):
     pass
 
+
 ListReleaseLabelsInputRequestTypeDef = TypedDict(
     "ListReleaseLabelsInputRequestTypeDef",
     {
         "Filters": ReleaseLabelFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2209,53 +2741,77 @@
 )
 
 NotebookExecutionTypeDef = TypedDict(
     "NotebookExecutionTypeDef",
     {
         "NotebookExecutionId": str,
         "EditorId": str,
-        "ExecutionEngine": ExecutionEngineConfigTypeDef,
+        "ExecutionEngine": ExecutionEngineConfigOutputTypeDef,
         "NotebookExecutionName": str,
         "NotebookParams": str,
         "Status": NotebookExecutionStatusType,
         "StartTime": datetime,
         "EndTime": datetime,
         "Arn": str,
         "OutputNotebookURI": str,
         "LastStateChangeReason": str,
         "NotebookInstanceSecurityGroupId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
         "OutputNotebookS3Location": OutputNotebookS3LocationForOutputTypeDef,
         "OutputNotebookFormat": Literal["HTML"],
         "EnvironmentVariables": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_RequiredOnDemandProvisioningSpecificationOutputTypeDef",
+    {
+        "AllocationStrategy": Literal["lowest-price"],
+    },
+)
+_OptionalOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
+    "_OptionalOnDemandProvisioningSpecificationOutputTypeDef",
+    {
+        "CapacityReservationOptions": OnDemandCapacityReservationOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OnDemandProvisioningSpecificationOutputTypeDef(
+    _RequiredOnDemandProvisioningSpecificationOutputTypeDef,
+    _OptionalOnDemandProvisioningSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredOnDemandProvisioningSpecificationTypeDef",
     {
         "AllocationStrategy": Literal["lowest-price"],
     },
 )
 _OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
     "_OptionalOnDemandProvisioningSpecificationTypeDef",
     {
         "CapacityReservationOptions": OnDemandCapacityReservationOptionsTypeDef,
     },
     total=False,
 )
 
+
 class OnDemandProvisioningSpecificationTypeDef(
     _RequiredOnDemandProvisioningSpecificationTypeDef,
     _OptionalOnDemandProvisioningSpecificationTypeDef,
 ):
     pass
 
+
 _RequiredStartNotebookExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartNotebookExecutionInputRequestTypeDef",
     {
         "ExecutionEngine": ExecutionEngineConfigTypeDef,
         "ServiceRole": str,
     },
 )
@@ -2272,60 +2828,77 @@
         "OutputNotebookS3Location": OutputNotebookS3LocationFromInputTypeDef,
         "OutputNotebookFormat": Literal["HTML"],
         "EnvironmentVariables": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartNotebookExecutionInputRequestTypeDef(
     _RequiredStartNotebookExecutionInputRequestTypeDef,
     _OptionalStartNotebookExecutionInputRequestTypeDef,
 ):
     pass
 
+
+_RequiredScalingActionOutputTypeDef = TypedDict(
+    "_RequiredScalingActionOutputTypeDef",
+    {
+        "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationOutputTypeDef,
+    },
+)
+_OptionalScalingActionOutputTypeDef = TypedDict(
+    "_OptionalScalingActionOutputTypeDef",
+    {
+        "Market": MarketTypeType,
+    },
+    total=False,
+)
+
+
+class ScalingActionOutputTypeDef(
+    _RequiredScalingActionOutputTypeDef, _OptionalScalingActionOutputTypeDef
+):
+    pass
+
+
 _RequiredScalingActionTypeDef = TypedDict(
     "_RequiredScalingActionTypeDef",
     {
         "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationTypeDef,
     },
 )
 _OptionalScalingActionTypeDef = TypedDict(
     "_OptionalScalingActionTypeDef",
     {
         "Market": MarketTypeType,
     },
     total=False,
 )
 
+
 class ScalingActionTypeDef(_RequiredScalingActionTypeDef, _OptionalScalingActionTypeDef):
     pass
 
+
 StepStatusTypeDef = TypedDict(
     "StepStatusTypeDef",
     {
         "State": StepStateType,
         "StateChangeReason": StepStateChangeReasonTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "Timeline": StepTimelineTypeDef,
     },
     total=False,
 )
 
-DescribeStudioOutputTypeDef = TypedDict(
-    "DescribeStudioOutputTypeDef",
-    {
-        "Studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
-        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
+        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
@@ -2333,19 +2906,26 @@
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
     },
 )
 
 BootstrapActionDetailTypeDef = TypedDict(
     "BootstrapActionDetailTypeDef",
     {
-        "BootstrapActionConfig": BootstrapActionConfigTypeDef,
+        "BootstrapActionConfig": BootstrapActionConfigOutputTypeDef,
     },
     total=False,
 )
 
+ScalingTriggerOutputTypeDef = TypedDict(
+    "ScalingTriggerOutputTypeDef",
+    {
+        "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionOutputTypeDef,
+    },
+)
+
 ScalingTriggerTypeDef = TypedDict(
     "ScalingTriggerTypeDef",
     {
         "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionTypeDef,
     },
 )
 
@@ -2374,40 +2954,48 @@
         "LogEncryptionKmsKeyId": str,
         "RequestedAmiVersion": str,
         "RunningAmiVersion": str,
         "ReleaseLabel": str,
         "AutoTerminate": bool,
         "TerminationProtected": bool,
         "VisibleToAllUsers": bool,
-        "Applications": List[ApplicationTypeDef],
-        "Tags": List[TagTypeDef],
+        "Applications": List[ApplicationOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ServiceRole": str,
         "NormalizedInstanceHours": int,
         "MasterPublicDnsName": str,
-        "Configurations": List["ConfigurationTypeDef"],
+        "Configurations": List["ConfigurationOutputTypeDef"],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
         "CustomAmiId": str,
         "EbsRootVolumeSize": int,
         "RepoUpgradeOnBoot": RepoUpgradeOnBootType,
-        "KerberosAttributes": KerberosAttributesTypeDef,
+        "KerberosAttributes": KerberosAttributesOutputTypeDef,
         "ClusterArn": str,
         "OutpostArn": str,
         "StepConcurrencyLevel": int,
-        "PlacementGroups": List[PlacementGroupConfigTypeDef],
+        "PlacementGroups": List[PlacementGroupConfigOutputTypeDef],
         "OSReleaseLabel": str,
     },
     total=False,
 )
 
+DescribeStudioOutputTypeDef = TypedDict(
+    "DescribeStudioOutputTypeDef",
+    {
+        "Studio": StudioTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetManagedScalingPolicyOutputTypeDef = TypedDict(
     "GetManagedScalingPolicyOutputTypeDef",
     {
-        "ManagedScalingPolicy": ManagedScalingPolicyTypeDef,
+        "ManagedScalingPolicy": ManagedScalingPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedScalingPolicyInputRequestTypeDef = TypedDict(
     "PutManagedScalingPolicyInputRequestTypeDef",
     {
@@ -2437,22 +3025,42 @@
 InstanceTypeSpecificationTypeDef = TypedDict(
     "InstanceTypeSpecificationTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": int,
         "BidPrice": str,
         "BidPriceAsPercentageOfOnDemandPrice": float,
-        "Configurations": List["ConfigurationTypeDef"],
+        "Configurations": List["ConfigurationOutputTypeDef"],
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
         "CustomAmiId": str,
     },
     total=False,
 )
 
+_RequiredStepConfigOutputTypeDef = TypedDict(
+    "_RequiredStepConfigOutputTypeDef",
+    {
+        "Name": str,
+        "HadoopJarStep": HadoopJarStepConfigOutputTypeDef,
+    },
+)
+_OptionalStepConfigOutputTypeDef = TypedDict(
+    "_OptionalStepConfigOutputTypeDef",
+    {
+        "ActionOnFailure": ActionOnFailureType,
+    },
+    total=False,
+)
+
+
+class StepConfigOutputTypeDef(_RequiredStepConfigOutputTypeDef, _OptionalStepConfigOutputTypeDef):
+    pass
+
+
 _RequiredStepConfigTypeDef = TypedDict(
     "_RequiredStepConfigTypeDef",
     {
         "Name": str,
         "HadoopJarStep": HadoopJarStepConfigTypeDef,
     },
 )
@@ -2460,17 +3068,19 @@
     "_OptionalStepConfigTypeDef",
     {
         "ActionOnFailure": ActionOnFailureType,
     },
     total=False,
 )
 
+
 class StepConfigTypeDef(_RequiredStepConfigTypeDef, _OptionalStepConfigTypeDef):
     pass
 
+
 _RequiredInstanceFleetModifyConfigTypeDef = TypedDict(
     "_RequiredInstanceFleetModifyConfigTypeDef",
     {
         "InstanceFleetId": str,
     },
 )
 _OptionalInstanceFleetModifyConfigTypeDef = TypedDict(
@@ -2479,19 +3089,21 @@
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
+
 class InstanceFleetModifyConfigTypeDef(
     _RequiredInstanceFleetModifyConfigTypeDef, _OptionalInstanceFleetModifyConfigTypeDef
 ):
     pass
 
+
 _RequiredInstanceGroupModifyConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupModifyConfigTypeDef",
     {
         "InstanceGroupId": str,
     },
 )
 _OptionalInstanceGroupModifyConfigTypeDef = TypedDict(
@@ -2502,19 +3114,21 @@
         "ShrinkPolicy": ShrinkPolicyTypeDef,
         "ReconfigurationType": ReconfigurationTypeType,
         "Configurations": Sequence["ConfigurationTypeDef"],
     },
     total=False,
 )
 
+
 class InstanceGroupModifyConfigTypeDef(
     _RequiredInstanceGroupModifyConfigTypeDef, _OptionalInstanceGroupModifyConfigTypeDef
 ):
     pass
 
+
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "Id": str,
         "Ec2InstanceId": str,
         "PublicDnsName": str,
         "PublicIpAddress": str,
@@ -2543,14 +3157,23 @@
     "DescribeNotebookExecutionOutputTypeDef",
     {
         "NotebookExecution": NotebookExecutionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InstanceFleetProvisioningSpecificationsOutputTypeDef = TypedDict(
+    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
+    {
+        "SpotSpecification": SpotProvisioningSpecificationOutputTypeDef,
+        "OnDemandSpecification": OnDemandProvisioningSpecificationOutputTypeDef,
+    },
+    total=False,
+)
+
 InstanceFleetProvisioningSpecificationsTypeDef = TypedDict(
     "InstanceFleetProvisioningSpecificationsTypeDef",
     {
         "SpotSpecification": SpotProvisioningSpecificationTypeDef,
         "OnDemandSpecification": OnDemandProvisioningSpecificationTypeDef,
     },
     total=False,
@@ -2577,14 +3200,37 @@
         "ActionOnFailure": ActionOnFailureType,
         "Status": StepStatusTypeDef,
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
+_RequiredScalingRuleOutputTypeDef = TypedDict(
+    "_RequiredScalingRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Action": ScalingActionOutputTypeDef,
+        "Trigger": ScalingTriggerOutputTypeDef,
+    },
+)
+_OptionalScalingRuleOutputTypeDef = TypedDict(
+    "_OptionalScalingRuleOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class ScalingRuleOutputTypeDef(
+    _RequiredScalingRuleOutputTypeDef, _OptionalScalingRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredScalingRuleTypeDef = TypedDict(
     "_RequiredScalingRuleTypeDef",
     {
         "Name": str,
         "Action": ScalingActionTypeDef,
         "Trigger": ScalingTriggerTypeDef,
     },
@@ -2593,17 +3239,19 @@
     "_OptionalScalingRuleTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ScalingRuleTypeDef(_RequiredScalingRuleTypeDef, _OptionalScalingRuleTypeDef):
     pass
 
+
 ListClustersOutputTypeDef = TypedDict(
     "ListClustersOutputTypeDef",
     {
         "Clusters": List[ClusterSummaryTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2632,19 +3280,29 @@
         "EbsConfiguration": EbsConfigurationTypeDef,
         "Configurations": Sequence["ConfigurationTypeDef"],
         "CustomAmiId": str,
     },
     total=False,
 )
 
+
 class InstanceTypeConfigTypeDef(
     _RequiredInstanceTypeConfigTypeDef, _OptionalInstanceTypeConfigTypeDef
 ):
     pass
 
+
+StepDetailTypeDef = TypedDict(
+    "StepDetailTypeDef",
+    {
+        "StepConfig": StepConfigOutputTypeDef,
+        "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
+    },
+)
+
 _RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
     "_RequiredAddJobFlowStepsInputRequestTypeDef",
     {
         "JobFlowId": str,
         "Steps": Sequence[StepConfigTypeDef],
     },
 )
@@ -2652,26 +3310,20 @@
     "_OptionalAddJobFlowStepsInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
+
 class AddJobFlowStepsInputRequestTypeDef(
     _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
 ):
     pass
 
-StepDetailTypeDef = TypedDict(
-    "StepDetailTypeDef",
-    {
-        "StepConfig": StepConfigTypeDef,
-        "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
-    },
-)
 
 ModifyInstanceFleetInputRequestTypeDef = TypedDict(
     "ModifyInstanceFleetInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceFleet": InstanceFleetModifyConfigTypeDef,
     },
@@ -2703,16 +3355,16 @@
         "Status": InstanceFleetStatusTypeDef,
         "InstanceFleetType": InstanceFleetTypeType,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ProvisionedOnDemandCapacity": int,
         "ProvisionedSpotCapacity": int,
         "InstanceTypeSpecifications": List[InstanceTypeSpecificationTypeDef],
-        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
-        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
+        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsOutputTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsOutputTypeDef,
     },
     total=False,
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
@@ -2730,16 +3382,16 @@
     },
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
-        "Constraints": ScalingConstraintsTypeDef,
-        "Rules": List[ScalingRuleTypeDef],
+        "Constraints": ScalingConstraintsOutputTypeDef,
+        "Rules": List[ScalingRuleOutputTypeDef],
     },
     total=False,
 )
 
 AutoScalingPolicyTypeDef = TypedDict(
     "AutoScalingPolicyTypeDef",
     {
@@ -2763,19 +3415,21 @@
         "InstanceTypeConfigs": Sequence[InstanceTypeConfigTypeDef],
         "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
         "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
+
 class InstanceFleetConfigTypeDef(
     _RequiredInstanceFleetConfigTypeDef, _OptionalInstanceFleetConfigTypeDef
 ):
     pass
 
+
 _RequiredJobFlowDetailTypeDef = TypedDict(
     "_RequiredJobFlowDetailTypeDef",
     {
         "JobFlowId": str,
         "Name": str,
         "ExecutionStatusDetail": JobFlowExecutionStatusDetailTypeDef,
         "Instances": JobFlowInstancesDetailTypeDef,
@@ -2795,17 +3449,19 @@
         "ServiceRole": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
     },
     total=False,
 )
 
+
 class JobFlowDetailTypeDef(_RequiredJobFlowDetailTypeDef, _OptionalJobFlowDetailTypeDef):
     pass
 
+
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2819,21 +3475,21 @@
         "Market": MarketTypeType,
         "InstanceGroupType": InstanceGroupTypeType,
         "BidPrice": str,
         "InstanceType": str,
         "RequestedInstanceCount": int,
         "RunningInstanceCount": int,
         "Status": InstanceGroupStatusTypeDef,
-        "Configurations": List["ConfigurationTypeDef"],
+        "Configurations": List["ConfigurationOutputTypeDef"],
         "ConfigurationsVersion": int,
-        "LastSuccessfullyAppliedConfigurations": List["ConfigurationTypeDef"],
+        "LastSuccessfullyAppliedConfigurations": List["ConfigurationOutputTypeDef"],
         "LastSuccessfullyAppliedConfigurationsVersion": int,
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
-        "ShrinkPolicy": ShrinkPolicyTypeDef,
+        "ShrinkPolicy": ShrinkPolicyOutputTypeDef,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "CustomAmiId": str,
     },
     total=False,
 )
 
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
@@ -2865,19 +3521,21 @@
         "EbsConfiguration": EbsConfigurationTypeDef,
         "AutoScalingPolicy": AutoScalingPolicyTypeDef,
         "CustomAmiId": str,
     },
     total=False,
 )
 
+
 class InstanceGroupConfigTypeDef(
     _RequiredInstanceGroupConfigTypeDef, _OptionalInstanceGroupConfigTypeDef
 ):
     pass
 
+
 PutAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "PutAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
         "AutoScalingPolicy": AutoScalingPolicyTypeDef,
     },
@@ -2977,11 +3635,12 @@
         "PlacementGroupConfigs": Sequence[PlacementGroupConfigTypeDef],
         "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
         "OSReleaseLabel": str,
     },
     total=False,
 )
 
+
 class RunJobFlowInputRequestTypeDef(
     _RequiredRunJobFlowInputRequestTypeDef, _OptionalRunJobFlowInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.28.12/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-emr
-Version: 1.28.0
-Summary: Type annotations for boto3.EMR 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -429,32 +397,41 @@
 
 ```python
 from mypy_boto3_emr.type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
     TagTypeDef,
+    ApplicationOutputTypeDef,
     ApplicationTypeDef,
-    ScalingConstraintsTypeDef,
+    ScalingConstraintsOutputTypeDef,
     AutoScalingPolicyStateChangeReasonTypeDef,
+    ScalingConstraintsTypeDef,
+    AutoTerminationPolicyOutputTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
+    PortRangeOutputTypeDef,
     PortRangeTypeDef,
+    ScriptBootstrapActionConfigOutputTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
     ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
-    KerberosAttributesTypeDef,
-    PlacementGroupConfigTypeDef,
+    KerberosAttributesOutputTypeDef,
+    PlacementGroupConfigOutputTypeDef,
+    TagOutputTypeDef,
     CommandTypeDef,
+    ComputeLimitsOutputTypeDef,
     ComputeLimitsTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
@@ -468,38 +445,47 @@
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
     DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
+    VolumeSpecificationOutputTypeDef,
     EbsVolumeTypeDef,
     EmptyResponseMetadataTypeDef,
+    ExecutionEngineConfigOutputTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
+    KeyValueOutputTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
+    SpotProvisioningSpecificationOutputTypeDef,
     SpotProvisioningSpecificationTypeDef,
+    OnDemandResizingSpecificationOutputTypeDef,
+    SpotResizingSpecificationOutputTypeDef,
     OnDemandResizingSpecificationTypeDef,
     SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
+    InstanceResizePolicyOutputTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
+    PlacementTypeOutputTypeDef,
+    KerberosAttributesTypeDef,
     ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
     ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
     ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
@@ -524,101 +510,117 @@
     ListSupportedInstanceTypesInputRequestTypeDef,
     SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
     ModifyClusterOutputTypeDef,
     NotebookS3LocationForOutputTypeDef,
     OutputNotebookS3LocationForOutputTypeDef,
     NotebookS3LocationFromInputTypeDef,
+    OnDemandCapacityReservationOptionsOutputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PaginatorConfigTypeDef,
+    PlacementGroupConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
     ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
     RunJobFlowOutputTypeDef,
+    SimpleScalingPolicyConfigurationOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
     StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
-    StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
+    BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
+    BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
+    CloudWatchAlarmDefinitionOutputTypeDef,
     CloudWatchAlarmDefinitionTypeDef,
     ClusterStatusTypeDef,
+    StudioTypeDef,
     ListBootstrapActionsOutputTypeDef,
+    ManagedScalingPolicyOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
+    HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
+    InstanceFleetResizingSpecificationsOutputTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
+    ShrinkPolicyOutputTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     ListSupportedInstanceTypesOutputTypeDef,
     NotebookExecutionSummaryTypeDef,
     NotebookExecutionTypeDef,
+    OnDemandProvisioningSpecificationOutputTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
+    ScalingActionOutputTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
-    DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
+    ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
+    DescribeStudioOutputTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
+    StepConfigOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
+    InstanceFleetProvisioningSpecificationsOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
+    ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
-    AddJobFlowStepsInputRequestTypeDef,
     StepDetailTypeDef,
+    AddJobFlowStepsInputRequestTypeDef,
     ModifyInstanceFleetInputRequestTypeDef,
     ModifyInstanceGroupsInputRequestTypeDef,
     ListInstancesOutputTypeDef,
     InstanceFleetTypeDef,
     ListStepsOutputTypeDef,
     DescribeStepOutputTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
```

### Comparing `mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.0/setup.py` & `mypy-boto3-emr-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMR 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EMR 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

