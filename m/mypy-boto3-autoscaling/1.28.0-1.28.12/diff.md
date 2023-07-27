# Comparing `tmp/mypy-boto3-autoscaling-1.28.0.tar.gz` & `tmp/mypy-boto3-autoscaling-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.28.0.tar", last modified: Thu Jul  6 20:59:02 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.28.0.tar` & `mypy-boto3-autoscaling-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.122228 mypy-boto3-autoscaling-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:57.000000 mypy-boto3-autoscaling-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22717 2023-07-06 20:59:02.122228 mypy-boto3-autoscaling-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-06 20:33:57.000000 mypy-boto3-autoscaling-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.118228 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-06 20:33:57.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-06 20:33:57.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:33:57.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52425 2023-07-06 20:33:58.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52343 2023-07-06 20:33:58.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-06 20:33:58.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-06 20:33:58.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-06 20:33:58.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-06 20:33:58.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:57.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75407 2023-07-06 20:34:00.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75290 2023-07-06 20:33:59.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:57.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.122228 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22717 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:02.122228 mypy-boto3-autoscaling-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:33:56.000000 mypy-boto3-autoscaling-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.588572 mypy-boto3-autoscaling-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24474 2023-07-27 05:34:20.584572 mypy-boto3-autoscaling-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.580572 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52425 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52343 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-07-27 05:17:48.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-07-27 05:17:48.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94435 2023-07-27 05:17:49.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94282 2023-07-27 05:17:49.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24474 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.588572 mypy-boto3-autoscaling-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:17:46.000000 mypy-boto3-autoscaling-1.28.12/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.28.0/LICENSE` & `mypy-boto3-autoscaling-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/PKG-INFO` & `mypy-boto3-autoscaling-1.28.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.0
-Summary: Type annotations for boto3.AutoScaling 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AutoScaling 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-autoscaling"></a>
 
 # mypy-boto3-autoscaling
 
 [![PyPI - mypy-boto3-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,41 +389,48 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
+    AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
+    AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     EnabledMetricTypeDef,
-    LaunchTemplateSpecificationTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
+    TrafficSourceIdentifierOutputTypeDef,
+    BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
+    EbsOutputTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
+    LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
@@ -462,42 +469,58 @@
     DisableMetricsCollectionQueryRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
+    InstanceMetadataOptionsOutputTypeDef,
+    InstanceMonitoringOutputTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesOutputTypeDef,
+    MemoryGiBPerVCpuRequestOutputTypeDef,
+    MemoryMiBRequestOutputTypeDef,
+    NetworkBandwidthGbpsRequestOutputTypeDef,
+    NetworkInterfaceCountRequestOutputTypeDef,
+    TotalLocalStorageGBRequestOutputTypeDef,
+    VCpuCountRequestOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
+    InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
+    InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
     PaginatorConfigTypeDef,
+    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
+    PredictiveScalingPredefinedLoadMetricOutputTypeDef,
+    PredictiveScalingPredefinedMetricPairOutputTypeDef,
+    PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
+    RefreshPreferencesTypeDef,
     ResponseMetadataTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
+    StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
@@ -516,67 +539,85 @@
     DescribeTagsTypeRequestTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
+    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
+    InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
-    PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
+    PutWarmPoolTypeRequestTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
-    CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
+    CreateLaunchConfigurationTypeRequestTypeDef,
+    MetricStatOutputTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
     RollbackDetailsTypeDef,
+    LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
+    MetricDataQueryOutputTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    LaunchTemplateOutputTypeDef,
     LaunchTemplateTypeDef,
+    PredictiveScalingCustomizedCapacityMetricOutputTypeDef,
+    PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+    PredictiveScalingCustomizedScalingMetricOutputTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
+    PredictiveScalingMetricSpecificationOutputTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
-    PutScalingPolicyTypeRequestTypeDef,
     ScalingPolicyTypeDef,
+    PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_structure() -> AcceleratorCountRequestOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.0/README.md` & `mypy-boto3-autoscaling-1.28.12/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-autoscaling"></a>
 
 # mypy-boto3-autoscaling
 
 [![PyPI - mypy-boto3-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,41 +357,48 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
+    AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
+    AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     EnabledMetricTypeDef,
-    LaunchTemplateSpecificationTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
+    TrafficSourceIdentifierOutputTypeDef,
+    BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
+    EbsOutputTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
+    LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
@@ -430,42 +437,58 @@
     DisableMetricsCollectionQueryRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
+    InstanceMetadataOptionsOutputTypeDef,
+    InstanceMonitoringOutputTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesOutputTypeDef,
+    MemoryGiBPerVCpuRequestOutputTypeDef,
+    MemoryMiBRequestOutputTypeDef,
+    NetworkBandwidthGbpsRequestOutputTypeDef,
+    NetworkInterfaceCountRequestOutputTypeDef,
+    TotalLocalStorageGBRequestOutputTypeDef,
+    VCpuCountRequestOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
+    InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
+    InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
     PaginatorConfigTypeDef,
+    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
+    PredictiveScalingPredefinedLoadMetricOutputTypeDef,
+    PredictiveScalingPredefinedMetricPairOutputTypeDef,
+    PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
+    RefreshPreferencesTypeDef,
     ResponseMetadataTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
+    StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
@@ -484,67 +507,85 @@
     DescribeTagsTypeRequestTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
+    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
+    InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
-    PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
+    PutWarmPoolTypeRequestTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
-    CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
+    CreateLaunchConfigurationTypeRequestTypeDef,
+    MetricStatOutputTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
     RollbackDetailsTypeDef,
+    LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
+    MetricDataQueryOutputTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    LaunchTemplateOutputTypeDef,
     LaunchTemplateTypeDef,
+    PredictiveScalingCustomizedCapacityMetricOutputTypeDef,
+    PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+    PredictiveScalingCustomizedScalingMetricOutputTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
+    PredictiveScalingMetricSpecificationOutputTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
-    PutScalingPolicyTypeRequestTypeDef,
     ScalingPolicyTypeDef,
+    PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_structure() -> AcceleratorCountRequestOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AutoScaling 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
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

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,15 @@
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
@@ -367,26 +368,28 @@
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

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,15 @@
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
@@ -365,26 +366,28 @@
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

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestTypeDef
+    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestOutputTypeDef
 
-    data: AcceleratorCountRequestTypeDef = {...}
+    data: AcceleratorCountRequestOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -49,41 +49,48 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AcceleratorCountRequestOutputTypeDef",
     "AcceleratorCountRequestTypeDef",
+    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "EnabledMetricTypeDef",
-    "LaunchTemplateSpecificationTypeDef",
+    "LaunchTemplateSpecificationOutputTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
+    "TrafficSourceIdentifierOutputTypeDef",
+    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
+    "EbsOutputTypeDef",
     "EbsTypeDef",
     "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
+    "LaunchTemplateSpecificationTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
@@ -122,42 +129,58 @@
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
+    "InstanceMetadataOptionsOutputTypeDef",
+    "InstanceMonitoringOutputTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesTypeDef",
+    "RefreshPreferencesOutputTypeDef",
+    "MemoryGiBPerVCpuRequestOutputTypeDef",
+    "MemoryMiBRequestOutputTypeDef",
+    "NetworkBandwidthGbpsRequestOutputTypeDef",
+    "NetworkInterfaceCountRequestOutputTypeDef",
+    "TotalLocalStorageGBRequestOutputTypeDef",
+    "VCpuCountRequestOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
+    "InstanceReusePolicyOutputTypeDef",
     "InstanceReusePolicyTypeDef",
+    "InstancesDistributionOutputTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
+    "PredictiveScalingPredefinedLoadMetricOutputTypeDef",
+    "PredictiveScalingPredefinedMetricPairOutputTypeDef",
+    "PredictiveScalingPredefinedScalingMetricOutputTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
+    "RefreshPreferencesTypeDef",
     "ResponseMetadataTypeDef",
     "RollbackInstanceRefreshAnswerTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
+    "StepAdjustmentOutputTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
@@ -176,74 +199,110 @@
     "DescribeTagsTypeRequestTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
+    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
-    "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
+    "PutWarmPoolTypeRequestTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
-    "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
+    "CreateLaunchConfigurationTypeRequestTypeDef",
+    "MetricStatOutputTypeDef",
+    "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "RollbackDetailsTypeDef",
+    "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
+    "MetricDataQueryOutputTypeDef",
+    "TargetTrackingMetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
+    "LaunchTemplateOutputTypeDef",
     "LaunchTemplateTypeDef",
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    "CustomizedMetricSpecificationOutputTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     "CustomizedMetricSpecificationTypeDef",
+    "MixedInstancesPolicyOutputTypeDef",
     "MixedInstancesPolicyTypeDef",
+    "PredictiveScalingMetricSpecificationOutputTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
+    "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
-    "PutScalingPolicyTypeRequestTypeDef",
     "ScalingPolicyTypeDef",
+    "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
+AcceleratorCountRequestOutputTypeDef = TypedDict(
+    "AcceleratorCountRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
+AcceleratorTotalMemoryMiBRequestOutputTypeDef = TypedDict(
+    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
 AcceleratorTotalMemoryMiBRequestTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -367,16 +426,16 @@
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
 )
 
-LaunchTemplateSpecificationTypeDef = TypedDict(
-    "LaunchTemplateSpecificationTypeDef",
+LaunchTemplateSpecificationOutputTypeDef = TypedDict(
+    "LaunchTemplateSpecificationOutputTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
     total=False,
 )
@@ -398,14 +457,44 @@
         "Key": str,
         "Value": str,
         "PropagateAtLaunch": bool,
     },
     total=False,
 )
 
+_RequiredTrafficSourceIdentifierOutputTypeDef = TypedDict(
+    "_RequiredTrafficSourceIdentifierOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+_OptionalTrafficSourceIdentifierOutputTypeDef = TypedDict(
+    "_OptionalTrafficSourceIdentifierOutputTypeDef",
+    {
+        "Type": str,
+    },
+    total=False,
+)
+
+
+class TrafficSourceIdentifierOutputTypeDef(
+    _RequiredTrafficSourceIdentifierOutputTypeDef, _OptionalTrafficSourceIdentifierOutputTypeDef
+):
+    pass
+
+
+BaselineEbsBandwidthMbpsRequestOutputTypeDef = TypedDict(
+    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
 BaselineEbsBandwidthMbpsRequestTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -466,14 +555,28 @@
 class ScheduledUpdateGroupActionRequestTypeDef(
     _RequiredScheduledUpdateGroupActionRequestTypeDef,
     _OptionalScheduledUpdateGroupActionRequestTypeDef,
 ):
     pass
 
 
+EbsOutputTypeDef = TypedDict(
+    "EbsOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeSize": int,
+        "VolumeType": str,
+        "DeleteOnTermination": bool,
+        "Iops": int,
+        "Encrypted": bool,
+        "Throughput": int,
+    },
+    total=False,
+)
+
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
@@ -528,14 +631,24 @@
 class CompleteLifecycleActionTypeRequestTypeDef(
     _RequiredCompleteLifecycleActionTypeRequestTypeDef,
     _OptionalCompleteLifecycleActionTypeRequestTypeDef,
 ):
     pass
 
 
+LaunchTemplateSpecificationTypeDef = TypedDict(
+    "LaunchTemplateSpecificationTypeDef",
+    {
+        "LaunchTemplateId": str,
+        "LaunchTemplateName": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 _RequiredLifecycleHookSpecificationTypeDef = TypedDict(
     "_RequiredLifecycleHookSpecificationTypeDef",
     {
         "LifecycleHookName": str,
         "LifecycleTransition": str,
     },
 )
@@ -594,14 +707,22 @@
     "InstanceMonitoringTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1254,14 +1375,32 @@
         "AutoScalingGroupName": str,
         "PolicyName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
+InstanceMetadataOptionsOutputTypeDef = TypedDict(
+    "InstanceMetadataOptionsOutputTypeDef",
+    {
+        "HttpTokens": InstanceMetadataHttpTokensStateType,
+        "HttpPutResponseHopLimit": int,
+        "HttpEndpoint": InstanceMetadataEndpointStateType,
+    },
+    total=False,
+)
+
+InstanceMonitoringOutputTypeDef = TypedDict(
+    "InstanceMonitoringOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
@@ -1272,29 +1411,107 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
+RefreshPreferencesOutputTypeDef = TypedDict(
+    "RefreshPreferencesOutputTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
         "AutoRollback": bool,
         "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
         "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
+MemoryGiBPerVCpuRequestOutputTypeDef = TypedDict(
+    "MemoryGiBPerVCpuRequestOutputTypeDef",
+    {
+        "Min": float,
+        "Max": float,
+    },
+    total=False,
+)
+
+_RequiredMemoryMiBRequestOutputTypeDef = TypedDict(
+    "_RequiredMemoryMiBRequestOutputTypeDef",
+    {
+        "Min": int,
+    },
+)
+_OptionalMemoryMiBRequestOutputTypeDef = TypedDict(
+    "_OptionalMemoryMiBRequestOutputTypeDef",
+    {
+        "Max": int,
+    },
+    total=False,
+)
+
+
+class MemoryMiBRequestOutputTypeDef(
+    _RequiredMemoryMiBRequestOutputTypeDef, _OptionalMemoryMiBRequestOutputTypeDef
+):
+    pass
+
+
+NetworkBandwidthGbpsRequestOutputTypeDef = TypedDict(
+    "NetworkBandwidthGbpsRequestOutputTypeDef",
+    {
+        "Min": float,
+        "Max": float,
+    },
+    total=False,
+)
+
+NetworkInterfaceCountRequestOutputTypeDef = TypedDict(
+    "NetworkInterfaceCountRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
+TotalLocalStorageGBRequestOutputTypeDef = TypedDict(
+    "TotalLocalStorageGBRequestOutputTypeDef",
+    {
+        "Min": float,
+        "Max": float,
+    },
+    total=False,
+)
+
+_RequiredVCpuCountRequestOutputTypeDef = TypedDict(
+    "_RequiredVCpuCountRequestOutputTypeDef",
+    {
+        "Min": int,
+    },
+)
+_OptionalVCpuCountRequestOutputTypeDef = TypedDict(
+    "_OptionalVCpuCountRequestOutputTypeDef",
+    {
+        "Max": int,
+    },
+    total=False,
+)
+
+
+class VCpuCountRequestOutputTypeDef(
+    _RequiredVCpuCountRequestOutputTypeDef, _OptionalVCpuCountRequestOutputTypeDef
+):
+    pass
+
+
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1361,22 +1578,43 @@
 )
 
 
 class VCpuCountRequestTypeDef(_RequiredVCpuCountRequestTypeDef, _OptionalVCpuCountRequestTypeDef):
     pass
 
 
+InstanceReusePolicyOutputTypeDef = TypedDict(
+    "InstanceReusePolicyOutputTypeDef",
+    {
+        "ReuseOnScaleIn": bool,
+    },
+    total=False,
+)
+
 InstanceReusePolicyTypeDef = TypedDict(
     "InstanceReusePolicyTypeDef",
     {
         "ReuseOnScaleIn": bool,
     },
     total=False,
 )
 
+InstancesDistributionOutputTypeDef = TypedDict(
+    "InstancesDistributionOutputTypeDef",
+    {
+        "OnDemandAllocationStrategy": str,
+        "OnDemandBaseCapacity": int,
+        "OnDemandPercentageAboveBaseCapacity": int,
+        "SpotAllocationStrategy": str,
+        "SpotInstancePools": int,
+        "SpotMaxPrice": str,
+    },
+    total=False,
+)
+
 InstancesDistributionTypeDef = TypedDict(
     "InstancesDistributionTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
@@ -1418,14 +1656,36 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPredefinedMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredefinedMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedMetricType": MetricTypeType,
+    },
+)
+_OptionalPredefinedMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredefinedMetricSpecificationOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+
+class PredefinedMetricSpecificationOutputTypeDef(
+    _RequiredPredefinedMetricSpecificationOutputTypeDef,
+    _OptionalPredefinedMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1439,14 +1699,80 @@
 
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
 
+_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef",
+    {
+        "PredefinedMetricType": PredefinedLoadMetricTypeType,
+    },
+)
+_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+
+class PredictiveScalingPredefinedLoadMetricOutputTypeDef(
+    _RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef,
+    _OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef,
+):
+    pass
+
+
+_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef",
+    {
+        "PredefinedMetricType": PredefinedMetricPairTypeType,
+    },
+)
+_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+
+class PredictiveScalingPredefinedMetricPairOutputTypeDef(
+    _RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef,
+    _OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef,
+):
+    pass
+
+
+_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef",
+    {
+        "PredefinedMetricType": PredefinedScalingMetricTypeType,
+    },
+)
+_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+
+class PredictiveScalingPredefinedScalingMetricOutputTypeDef(
+    _RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef,
+    _OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedLoadMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
@@ -1622,14 +1948,29 @@
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
 
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": Sequence[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
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
@@ -1649,14 +1990,36 @@
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
     total=False,
 )
 
+_RequiredStepAdjustmentOutputTypeDef = TypedDict(
+    "_RequiredStepAdjustmentOutputTypeDef",
+    {
+        "ScalingAdjustment": int,
+    },
+)
+_OptionalStepAdjustmentOutputTypeDef = TypedDict(
+    "_OptionalStepAdjustmentOutputTypeDef",
+    {
+        "MetricIntervalLowerBound": float,
+        "MetricIntervalUpperBound": float,
+    },
+    total=False,
+)
+
+
+class StepAdjustmentOutputTypeDef(
+    _RequiredStepAdjustmentOutputTypeDef, _OptionalStepAdjustmentOutputTypeDef
+):
+    pass
+
+
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalScalingProcessQueryRequestTypeDef = TypedDict(
@@ -1887,15 +2250,15 @@
     },
 )
 _OptionalAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_OptionalAutoScalingInstanceDetailsTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 
 class AutoScalingInstanceDetailsTypeDef(
@@ -1915,15 +2278,15 @@
     },
 )
 _OptionalInstanceTypeDef = TypedDict(
     "_OptionalInstanceTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
@@ -1959,14 +2322,37 @@
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
     },
 )
 
+_RequiredBlockDeviceMappingOutputTypeDef = TypedDict(
+    "_RequiredBlockDeviceMappingOutputTypeDef",
+    {
+        "DeviceName": str,
+    },
+)
+_OptionalBlockDeviceMappingOutputTypeDef = TypedDict(
+    "_OptionalBlockDeviceMappingOutputTypeDef",
+    {
+        "VirtualName": str,
+        "Ebs": EbsOutputTypeDef,
+        "NoDevice": bool,
+    },
+    total=False,
+)
+
+
+class BlockDeviceMappingOutputTypeDef(
+    _RequiredBlockDeviceMappingOutputTypeDef, _OptionalBlockDeviceMappingOutputTypeDef
+):
+    pass
+
+
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
     },
 )
 _OptionalBlockDeviceMappingTypeDef = TypedDict(
@@ -1996,25 +2382,45 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
+
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricTypeDef = TypedDict(
     "_OptionalMetricTypeDef",
     {
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
@@ -2078,14 +2484,56 @@
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
         "WarmPoolProgress": InstanceRefreshWarmPoolProgressTypeDef,
     },
     total=False,
 )
 
+_RequiredInstanceRequirementsOutputTypeDef = TypedDict(
+    "_RequiredInstanceRequirementsOutputTypeDef",
+    {
+        "VCpuCount": VCpuCountRequestOutputTypeDef,
+        "MemoryMiB": MemoryMiBRequestOutputTypeDef,
+    },
+)
+_OptionalInstanceRequirementsOutputTypeDef = TypedDict(
+    "_OptionalInstanceRequirementsOutputTypeDef",
+    {
+        "CpuManufacturers": List[CpuManufacturerType],
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestOutputTypeDef,
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[InstanceGenerationType],
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "BareMetal": BareMetalType,
+        "BurstablePerformance": BurstablePerformanceType,
+        "RequireHibernateSupport": bool,
+        "NetworkInterfaceCount": NetworkInterfaceCountRequestOutputTypeDef,
+        "LocalStorage": LocalStorageType,
+        "LocalStorageTypes": List[LocalStorageTypeType],
+        "TotalLocalStorageGB": TotalLocalStorageGBRequestOutputTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestOutputTypeDef,
+        "AcceleratorTypes": List[AcceleratorTypeType],
+        "AcceleratorCount": AcceleratorCountRequestOutputTypeDef,
+        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
+        "AcceleratorNames": List[AcceleratorNameType],
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestOutputTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestOutputTypeDef,
+        "AllowedInstanceTypes": List[str],
+    },
+    total=False,
+)
+
+
+class InstanceRequirementsOutputTypeDef(
+    _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
+):
+    pass
+
+
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2120,14 +2568,26 @@
 
 class InstanceRequirementsTypeDef(
     _RequiredInstanceRequirementsTypeDef, _OptionalInstanceRequirementsTypeDef
 ):
     pass
 
 
+WarmPoolConfigurationTypeDef = TypedDict(
+    "WarmPoolConfigurationTypeDef",
+    {
+        "MaxGroupPreparedCapacity": int,
+        "MinSize": int,
+        "PoolState": WarmPoolStateType,
+        "Status": Literal["PendingDelete"],
+        "InstanceReusePolicy": InstanceReusePolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredPutWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredPutWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalPutWarmPoolTypeRequestTypeDef = TypedDict(
@@ -2144,26 +2604,14 @@
 
 class PutWarmPoolTypeRequestTypeDef(
     _RequiredPutWarmPoolTypeRequestTypeDef, _OptionalPutWarmPoolTypeRequestTypeDef
 ):
     pass
 
 
-WarmPoolConfigurationTypeDef = TypedDict(
-    "WarmPoolConfigurationTypeDef",
-    {
-        "MaxGroupPreparedCapacity": int,
-        "MinSize": int,
-        "PoolState": WarmPoolStateType,
-        "Status": Literal["PendingDelete"],
-        "InstanceReusePolicy": InstanceReusePolicyTypeDef,
-    },
-    total=False,
-)
-
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2182,14 +2630,53 @@
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredLaunchConfigurationTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTypeDef",
+    {
+        "LaunchConfigurationName": str,
+        "ImageId": str,
+        "InstanceType": str,
+        "CreatedTime": datetime,
+    },
+)
+_OptionalLaunchConfigurationTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTypeDef",
+    {
+        "LaunchConfigurationARN": str,
+        "KeyName": str,
+        "SecurityGroups": List[str],
+        "ClassicLinkVPCId": str,
+        "ClassicLinkVPCSecurityGroups": List[str],
+        "UserData": str,
+        "KernelId": str,
+        "RamdiskId": str,
+        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
+        "InstanceMonitoring": InstanceMonitoringOutputTypeDef,
+        "SpotPrice": str,
+        "IamInstanceProfile": str,
+        "EbsOptimized": bool,
+        "AssociatePublicIpAddress": bool,
+        "PlacementTenancy": str,
+        "MetadataOptions": InstanceMetadataOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class LaunchConfigurationTypeDef(
+    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
+):
+    pass
+
+
 _RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 _OptionalCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
@@ -2221,49 +2708,52 @@
 class CreateLaunchConfigurationTypeRequestTypeDef(
     _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
     _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
 ):
     pass
 
 
-_RequiredLaunchConfigurationTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTypeDef",
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
     {
-        "LaunchConfigurationName": str,
-        "ImageId": str,
-        "InstanceType": str,
-        "CreatedTime": datetime,
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
     },
 )
-_OptionalLaunchConfigurationTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTypeDef",
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
     {
-        "LaunchConfigurationARN": str,
-        "KeyName": str,
-        "SecurityGroups": List[str],
-        "ClassicLinkVPCId": str,
-        "ClassicLinkVPCSecurityGroups": List[str],
-        "UserData": str,
-        "KernelId": str,
-        "RamdiskId": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
-        "InstanceMonitoring": InstanceMonitoringTypeDef,
-        "SpotPrice": str,
-        "IamInstanceProfile": str,
-        "EbsOptimized": bool,
-        "AssociatePublicIpAddress": bool,
-        "PlacementTenancy": str,
-        "MetadataOptions": InstanceMetadataOptionsTypeDef,
+        "Unit": str,
     },
     total=False,
 )
 
 
-class LaunchConfigurationTypeDef(
-    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
+
+
+_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
+    },
+)
+_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Unit": str,
+    },
+    total=False,
+)
+
+
+class TargetTrackingMetricStatOutputTypeDef(
+    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
 ):
     pass
 
 
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
@@ -2314,14 +2804,25 @@
         "PercentageCompleteOnRollback": int,
         "InstancesToUpdateOnRollback": int,
         "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
     },
     total=False,
 )
 
+LaunchTemplateOverridesOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesOutputTypeDef",
+    {
+        "InstanceType": str,
+        "WeightedCapacity": str,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
+    },
+    total=False,
+)
+
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2344,14 +2845,63 @@
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": MetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+):
+    pass
+
+
+_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+
+class TargetTrackingMetricDataQueryOutputTypeDef(
+    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
+    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
+):
+    pass
+
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2390,66 +2940,175 @@
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
 
+LaunchTemplateOutputTypeDef = TypedDict(
+    "LaunchTemplateOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
+    },
+    total=False,
+)
+
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
+PredictiveScalingCustomizedCapacityMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedLoadMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedScalingMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+CustomizedMetricSpecificationOutputTypeDef = TypedDict(
+    "CustomizedMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Statistic": MetricStatisticType,
+        "Unit": str,
+        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
 PredictiveScalingCustomizedCapacityMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedLoadMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
+        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
+    },
+    total=False,
+)
+
+MixedInstancesPolicyOutputTypeDef = TypedDict(
+    "MixedInstancesPolicyOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateOutputTypeDef,
+        "InstancesDistribution": InstancesDistributionOutputTypeDef,
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
+_RequiredPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairOutputTypeDef,
+        "PredefinedScalingMetricSpecification": (
+            PredictiveScalingPredefinedScalingMetricOutputTypeDef
+        ),
+        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricOutputTypeDef,
+        "CustomizedScalingMetricSpecification": (
+            PredictiveScalingCustomizedScalingMetricOutputTypeDef
+        ),
+        "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+        "CustomizedCapacityMetricSpecification": (
+            PredictiveScalingCustomizedCapacityMetricOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
+
+class PredictiveScalingMetricSpecificationOutputTypeDef(
+    _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
+    _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationOutputTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+    },
+    total=False,
+)
+
+
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2510,16 +3169,16 @@
     },
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
         "PlacementGroup": str,
@@ -2533,24 +3192,33 @@
         "MaxInstanceLifetime": int,
         "CapacityRebalance": bool,
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "WarmPoolSize": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
-        "TrafficSources": List[TrafficSourceIdentifierTypeDef],
+        "TrafficSources": List[TrafficSourceIdentifierOutputTypeDef],
     },
     total=False,
 )
 
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
 
+DesiredConfigurationOutputTypeDef = TypedDict(
+    "DesiredConfigurationOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
     },
@@ -2645,22 +3313,47 @@
 
 
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
-        "MetricSpecification": PredictiveScalingMetricSpecificationTypeDef,
+        "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
+    },
+)
+
+_RequiredPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "MetricSpecifications": List[PredictiveScalingMetricSpecificationOutputTypeDef],
+    },
+)
+_OptionalPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "Mode": PredictiveScalingModeType,
+        "SchedulingBufferTime": int,
+        "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
+        "MaxCapacityBuffer": int,
     },
+    total=False,
 )
 
+
+class PredictiveScalingConfigurationOutputTypeDef(
+    _RequiredPredictiveScalingConfigurationOutputTypeDef,
+    _OptionalPredictiveScalingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
-        "MetricSpecifications": List[PredictiveScalingMetricSpecificationTypeDef],
+        "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
     "_OptionalPredictiveScalingConfigurationTypeDef",
     {
         "Mode": PredictiveScalingModeType,
         "SchedulingBufferTime": int,
@@ -2694,16 +3387,16 @@
         "Status": InstanceRefreshStatusType,
         "StatusReason": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
-        "Preferences": RefreshPreferencesTypeDef,
-        "DesiredConfiguration": DesiredConfigurationTypeDef,
+        "Preferences": RefreshPreferencesOutputTypeDef,
+        "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
@@ -2734,70 +3427,70 @@
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyTypeRequestTypeDef",
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-    },
-)
-_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyTypeRequestTypeDef",
-    {
+        "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
+        "StepAdjustments": List[StepAdjustmentOutputTypeDef],
         "MetricAggregationType": str,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "Alarms": List[AlarmTypeDef],
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
-        "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
+        "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
-class PutScalingPolicyTypeRequestTypeDef(
-    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
-):
-    pass
-
-
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
+_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-        "PolicyARN": str,
+    },
+)
+_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyTypeRequestTypeDef",
+    {
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
+
+class PutScalingPolicyTypeRequestTypeDef(
+    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
+):
+    pass
+
+
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestTypeDef
+    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestOutputTypeDef
 
-    data: AcceleratorCountRequestTypeDef = {...}
+    data: AcceleratorCountRequestOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -48,41 +48,48 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AcceleratorCountRequestOutputTypeDef",
     "AcceleratorCountRequestTypeDef",
+    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "EnabledMetricTypeDef",
-    "LaunchTemplateSpecificationTypeDef",
+    "LaunchTemplateSpecificationOutputTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
+    "TrafficSourceIdentifierOutputTypeDef",
+    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
+    "EbsOutputTypeDef",
     "EbsTypeDef",
     "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
+    "LaunchTemplateSpecificationTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
@@ -121,42 +128,58 @@
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
+    "InstanceMetadataOptionsOutputTypeDef",
+    "InstanceMonitoringOutputTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesTypeDef",
+    "RefreshPreferencesOutputTypeDef",
+    "MemoryGiBPerVCpuRequestOutputTypeDef",
+    "MemoryMiBRequestOutputTypeDef",
+    "NetworkBandwidthGbpsRequestOutputTypeDef",
+    "NetworkInterfaceCountRequestOutputTypeDef",
+    "TotalLocalStorageGBRequestOutputTypeDef",
+    "VCpuCountRequestOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
+    "InstanceReusePolicyOutputTypeDef",
     "InstanceReusePolicyTypeDef",
+    "InstancesDistributionOutputTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
+    "PredictiveScalingPredefinedLoadMetricOutputTypeDef",
+    "PredictiveScalingPredefinedMetricPairOutputTypeDef",
+    "PredictiveScalingPredefinedScalingMetricOutputTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
+    "RefreshPreferencesTypeDef",
     "ResponseMetadataTypeDef",
     "RollbackInstanceRefreshAnswerTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
+    "StepAdjustmentOutputTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
@@ -175,74 +198,110 @@
     "DescribeTagsTypeRequestTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
+    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
-    "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
+    "PutWarmPoolTypeRequestTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
-    "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
+    "CreateLaunchConfigurationTypeRequestTypeDef",
+    "MetricStatOutputTypeDef",
+    "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "RollbackDetailsTypeDef",
+    "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
+    "MetricDataQueryOutputTypeDef",
+    "TargetTrackingMetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
+    "LaunchTemplateOutputTypeDef",
     "LaunchTemplateTypeDef",
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    "CustomizedMetricSpecificationOutputTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     "CustomizedMetricSpecificationTypeDef",
+    "MixedInstancesPolicyOutputTypeDef",
     "MixedInstancesPolicyTypeDef",
+    "PredictiveScalingMetricSpecificationOutputTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
+    "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
-    "PutScalingPolicyTypeRequestTypeDef",
     "ScalingPolicyTypeDef",
+    "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
+AcceleratorCountRequestOutputTypeDef = TypedDict(
+    "AcceleratorCountRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
+AcceleratorTotalMemoryMiBRequestOutputTypeDef = TypedDict(
+    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
 AcceleratorTotalMemoryMiBRequestTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -360,16 +419,16 @@
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
 )
 
-LaunchTemplateSpecificationTypeDef = TypedDict(
-    "LaunchTemplateSpecificationTypeDef",
+LaunchTemplateSpecificationOutputTypeDef = TypedDict(
+    "LaunchTemplateSpecificationOutputTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
     total=False,
 )
@@ -391,14 +450,42 @@
         "Key": str,
         "Value": str,
         "PropagateAtLaunch": bool,
     },
     total=False,
 )
 
+_RequiredTrafficSourceIdentifierOutputTypeDef = TypedDict(
+    "_RequiredTrafficSourceIdentifierOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+_OptionalTrafficSourceIdentifierOutputTypeDef = TypedDict(
+    "_OptionalTrafficSourceIdentifierOutputTypeDef",
+    {
+        "Type": str,
+    },
+    total=False,
+)
+
+class TrafficSourceIdentifierOutputTypeDef(
+    _RequiredTrafficSourceIdentifierOutputTypeDef, _OptionalTrafficSourceIdentifierOutputTypeDef
+):
+    pass
+
+BaselineEbsBandwidthMbpsRequestOutputTypeDef = TypedDict(
+    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
 BaselineEbsBandwidthMbpsRequestTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -455,14 +542,28 @@
 
 class ScheduledUpdateGroupActionRequestTypeDef(
     _RequiredScheduledUpdateGroupActionRequestTypeDef,
     _OptionalScheduledUpdateGroupActionRequestTypeDef,
 ):
     pass
 
+EbsOutputTypeDef = TypedDict(
+    "EbsOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeSize": int,
+        "VolumeType": str,
+        "DeleteOnTermination": bool,
+        "Iops": int,
+        "Encrypted": bool,
+        "Throughput": int,
+    },
+    total=False,
+)
+
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
@@ -515,14 +616,24 @@
 
 class CompleteLifecycleActionTypeRequestTypeDef(
     _RequiredCompleteLifecycleActionTypeRequestTypeDef,
     _OptionalCompleteLifecycleActionTypeRequestTypeDef,
 ):
     pass
 
+LaunchTemplateSpecificationTypeDef = TypedDict(
+    "LaunchTemplateSpecificationTypeDef",
+    {
+        "LaunchTemplateId": str,
+        "LaunchTemplateName": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 _RequiredLifecycleHookSpecificationTypeDef = TypedDict(
     "_RequiredLifecycleHookSpecificationTypeDef",
     {
         "LifecycleHookName": str,
         "LifecycleTransition": str,
     },
 )
@@ -577,14 +688,22 @@
     "InstanceMonitoringTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1203,14 +1322,32 @@
         "AutoScalingGroupName": str,
         "PolicyName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
+InstanceMetadataOptionsOutputTypeDef = TypedDict(
+    "InstanceMetadataOptionsOutputTypeDef",
+    {
+        "HttpTokens": InstanceMetadataHttpTokensStateType,
+        "HttpPutResponseHopLimit": int,
+        "HttpEndpoint": InstanceMetadataEndpointStateType,
+    },
+    total=False,
+)
+
+InstanceMonitoringOutputTypeDef = TypedDict(
+    "InstanceMonitoringOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
@@ -1221,29 +1358,103 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
+RefreshPreferencesOutputTypeDef = TypedDict(
+    "RefreshPreferencesOutputTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
         "AutoRollback": bool,
         "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
         "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
+MemoryGiBPerVCpuRequestOutputTypeDef = TypedDict(
+    "MemoryGiBPerVCpuRequestOutputTypeDef",
+    {
+        "Min": float,
+        "Max": float,
+    },
+    total=False,
+)
+
+_RequiredMemoryMiBRequestOutputTypeDef = TypedDict(
+    "_RequiredMemoryMiBRequestOutputTypeDef",
+    {
+        "Min": int,
+    },
+)
+_OptionalMemoryMiBRequestOutputTypeDef = TypedDict(
+    "_OptionalMemoryMiBRequestOutputTypeDef",
+    {
+        "Max": int,
+    },
+    total=False,
+)
+
+class MemoryMiBRequestOutputTypeDef(
+    _RequiredMemoryMiBRequestOutputTypeDef, _OptionalMemoryMiBRequestOutputTypeDef
+):
+    pass
+
+NetworkBandwidthGbpsRequestOutputTypeDef = TypedDict(
+    "NetworkBandwidthGbpsRequestOutputTypeDef",
+    {
+        "Min": float,
+        "Max": float,
+    },
+    total=False,
+)
+
+NetworkInterfaceCountRequestOutputTypeDef = TypedDict(
+    "NetworkInterfaceCountRequestOutputTypeDef",
+    {
+        "Min": int,
+        "Max": int,
+    },
+    total=False,
+)
+
+TotalLocalStorageGBRequestOutputTypeDef = TypedDict(
+    "TotalLocalStorageGBRequestOutputTypeDef",
+    {
+        "Min": float,
+        "Max": float,
+    },
+    total=False,
+)
+
+_RequiredVCpuCountRequestOutputTypeDef = TypedDict(
+    "_RequiredVCpuCountRequestOutputTypeDef",
+    {
+        "Min": int,
+    },
+)
+_OptionalVCpuCountRequestOutputTypeDef = TypedDict(
+    "_OptionalVCpuCountRequestOutputTypeDef",
+    {
+        "Max": int,
+    },
+    total=False,
+)
+
+class VCpuCountRequestOutputTypeDef(
+    _RequiredVCpuCountRequestOutputTypeDef, _OptionalVCpuCountRequestOutputTypeDef
+):
+    pass
+
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1306,22 +1517,43 @@
     },
     total=False,
 )
 
 class VCpuCountRequestTypeDef(_RequiredVCpuCountRequestTypeDef, _OptionalVCpuCountRequestTypeDef):
     pass
 
+InstanceReusePolicyOutputTypeDef = TypedDict(
+    "InstanceReusePolicyOutputTypeDef",
+    {
+        "ReuseOnScaleIn": bool,
+    },
+    total=False,
+)
+
 InstanceReusePolicyTypeDef = TypedDict(
     "InstanceReusePolicyTypeDef",
     {
         "ReuseOnScaleIn": bool,
     },
     total=False,
 )
 
+InstancesDistributionOutputTypeDef = TypedDict(
+    "InstancesDistributionOutputTypeDef",
+    {
+        "OnDemandAllocationStrategy": str,
+        "OnDemandBaseCapacity": int,
+        "OnDemandPercentageAboveBaseCapacity": int,
+        "SpotAllocationStrategy": str,
+        "SpotInstancePools": int,
+        "SpotMaxPrice": str,
+    },
+    total=False,
+)
+
 InstancesDistributionTypeDef = TypedDict(
     "InstancesDistributionTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
@@ -1363,14 +1595,34 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPredefinedMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredefinedMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedMetricType": MetricTypeType,
+    },
+)
+_OptionalPredefinedMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredefinedMetricSpecificationOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+class PredefinedMetricSpecificationOutputTypeDef(
+    _RequiredPredefinedMetricSpecificationOutputTypeDef,
+    _OptionalPredefinedMetricSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1382,14 +1634,74 @@
 )
 
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
+_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef",
+    {
+        "PredefinedMetricType": PredefinedLoadMetricTypeType,
+    },
+)
+_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+class PredictiveScalingPredefinedLoadMetricOutputTypeDef(
+    _RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef,
+    _OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef,
+):
+    pass
+
+_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef",
+    {
+        "PredefinedMetricType": PredefinedMetricPairTypeType,
+    },
+)
+_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+class PredictiveScalingPredefinedMetricPairOutputTypeDef(
+    _RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef,
+    _OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef,
+):
+    pass
+
+_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef",
+    {
+        "PredefinedMetricType": PredefinedScalingMetricTypeType,
+    },
+)
+_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+class PredictiveScalingPredefinedScalingMetricOutputTypeDef(
+    _RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef,
+    _OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef,
+):
+    pass
+
 _RequiredPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedLoadMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
@@ -1551,14 +1863,29 @@
 
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": Sequence[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
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
@@ -1578,14 +1905,34 @@
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
     total=False,
 )
 
+_RequiredStepAdjustmentOutputTypeDef = TypedDict(
+    "_RequiredStepAdjustmentOutputTypeDef",
+    {
+        "ScalingAdjustment": int,
+    },
+)
+_OptionalStepAdjustmentOutputTypeDef = TypedDict(
+    "_OptionalStepAdjustmentOutputTypeDef",
+    {
+        "MetricIntervalLowerBound": float,
+        "MetricIntervalUpperBound": float,
+    },
+    total=False,
+)
+
+class StepAdjustmentOutputTypeDef(
+    _RequiredStepAdjustmentOutputTypeDef, _OptionalStepAdjustmentOutputTypeDef
+):
+    pass
+
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalScalingProcessQueryRequestTypeDef = TypedDict(
@@ -1810,15 +2157,15 @@
     },
 )
 _OptionalAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_OptionalAutoScalingInstanceDetailsTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 class AutoScalingInstanceDetailsTypeDef(
     _RequiredAutoScalingInstanceDetailsTypeDef, _OptionalAutoScalingInstanceDetailsTypeDef
@@ -1836,15 +2183,15 @@
     },
 )
 _OptionalInstanceTypeDef = TypedDict(
     "_OptionalInstanceTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
@@ -1878,14 +2225,35 @@
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
     },
 )
 
+_RequiredBlockDeviceMappingOutputTypeDef = TypedDict(
+    "_RequiredBlockDeviceMappingOutputTypeDef",
+    {
+        "DeviceName": str,
+    },
+)
+_OptionalBlockDeviceMappingOutputTypeDef = TypedDict(
+    "_OptionalBlockDeviceMappingOutputTypeDef",
+    {
+        "VirtualName": str,
+        "Ebs": EbsOutputTypeDef,
+        "NoDevice": bool,
+    },
+    total=False,
+)
+
+class BlockDeviceMappingOutputTypeDef(
+    _RequiredBlockDeviceMappingOutputTypeDef, _OptionalBlockDeviceMappingOutputTypeDef
+):
+    pass
+
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
     },
 )
 _OptionalBlockDeviceMappingTypeDef = TypedDict(
@@ -1913,25 +2281,43 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricTypeDef = TypedDict(
     "_OptionalMetricTypeDef",
     {
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
@@ -1993,14 +2379,54 @@
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
         "WarmPoolProgress": InstanceRefreshWarmPoolProgressTypeDef,
     },
     total=False,
 )
 
+_RequiredInstanceRequirementsOutputTypeDef = TypedDict(
+    "_RequiredInstanceRequirementsOutputTypeDef",
+    {
+        "VCpuCount": VCpuCountRequestOutputTypeDef,
+        "MemoryMiB": MemoryMiBRequestOutputTypeDef,
+    },
+)
+_OptionalInstanceRequirementsOutputTypeDef = TypedDict(
+    "_OptionalInstanceRequirementsOutputTypeDef",
+    {
+        "CpuManufacturers": List[CpuManufacturerType],
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestOutputTypeDef,
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[InstanceGenerationType],
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "BareMetal": BareMetalType,
+        "BurstablePerformance": BurstablePerformanceType,
+        "RequireHibernateSupport": bool,
+        "NetworkInterfaceCount": NetworkInterfaceCountRequestOutputTypeDef,
+        "LocalStorage": LocalStorageType,
+        "LocalStorageTypes": List[LocalStorageTypeType],
+        "TotalLocalStorageGB": TotalLocalStorageGBRequestOutputTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestOutputTypeDef,
+        "AcceleratorTypes": List[AcceleratorTypeType],
+        "AcceleratorCount": AcceleratorCountRequestOutputTypeDef,
+        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
+        "AcceleratorNames": List[AcceleratorNameType],
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestOutputTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestOutputTypeDef,
+        "AllowedInstanceTypes": List[str],
+    },
+    total=False,
+)
+
+class InstanceRequirementsOutputTypeDef(
+    _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
+):
+    pass
+
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2033,14 +2459,26 @@
 )
 
 class InstanceRequirementsTypeDef(
     _RequiredInstanceRequirementsTypeDef, _OptionalInstanceRequirementsTypeDef
 ):
     pass
 
+WarmPoolConfigurationTypeDef = TypedDict(
+    "WarmPoolConfigurationTypeDef",
+    {
+        "MaxGroupPreparedCapacity": int,
+        "MinSize": int,
+        "PoolState": WarmPoolStateType,
+        "Status": Literal["PendingDelete"],
+        "InstanceReusePolicy": InstanceReusePolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredPutWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredPutWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalPutWarmPoolTypeRequestTypeDef = TypedDict(
@@ -2055,26 +2493,14 @@
 )
 
 class PutWarmPoolTypeRequestTypeDef(
     _RequiredPutWarmPoolTypeRequestTypeDef, _OptionalPutWarmPoolTypeRequestTypeDef
 ):
     pass
 
-WarmPoolConfigurationTypeDef = TypedDict(
-    "WarmPoolConfigurationTypeDef",
-    {
-        "MaxGroupPreparedCapacity": int,
-        "MinSize": int,
-        "PoolState": WarmPoolStateType,
-        "Status": Literal["PendingDelete"],
-        "InstanceReusePolicy": InstanceReusePolicyTypeDef,
-    },
-    total=False,
-)
-
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2093,14 +2519,51 @@
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredLaunchConfigurationTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTypeDef",
+    {
+        "LaunchConfigurationName": str,
+        "ImageId": str,
+        "InstanceType": str,
+        "CreatedTime": datetime,
+    },
+)
+_OptionalLaunchConfigurationTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTypeDef",
+    {
+        "LaunchConfigurationARN": str,
+        "KeyName": str,
+        "SecurityGroups": List[str],
+        "ClassicLinkVPCId": str,
+        "ClassicLinkVPCSecurityGroups": List[str],
+        "UserData": str,
+        "KernelId": str,
+        "RamdiskId": str,
+        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
+        "InstanceMonitoring": InstanceMonitoringOutputTypeDef,
+        "SpotPrice": str,
+        "IamInstanceProfile": str,
+        "EbsOptimized": bool,
+        "AssociatePublicIpAddress": bool,
+        "PlacementTenancy": str,
+        "MetadataOptions": InstanceMetadataOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class LaunchConfigurationTypeDef(
+    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
+):
+    pass
+
 _RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 _OptionalCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
@@ -2130,48 +2593,49 @@
 
 class CreateLaunchConfigurationTypeRequestTypeDef(
     _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
     _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
 ):
     pass
 
-_RequiredLaunchConfigurationTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTypeDef",
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
     {
-        "LaunchConfigurationName": str,
-        "ImageId": str,
-        "InstanceType": str,
-        "CreatedTime": datetime,
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
     },
 )
-_OptionalLaunchConfigurationTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTypeDef",
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
     {
-        "LaunchConfigurationARN": str,
-        "KeyName": str,
-        "SecurityGroups": List[str],
-        "ClassicLinkVPCId": str,
-        "ClassicLinkVPCSecurityGroups": List[str],
-        "UserData": str,
-        "KernelId": str,
-        "RamdiskId": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
-        "InstanceMonitoring": InstanceMonitoringTypeDef,
-        "SpotPrice": str,
-        "IamInstanceProfile": str,
-        "EbsOptimized": bool,
-        "AssociatePublicIpAddress": bool,
-        "PlacementTenancy": str,
-        "MetadataOptions": InstanceMetadataOptionsTypeDef,
+        "Unit": str,
     },
     total=False,
 )
 
-class LaunchConfigurationTypeDef(
-    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
+
+_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
+    },
+)
+_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Unit": str,
+    },
+    total=False,
+)
+
+class TargetTrackingMetricStatOutputTypeDef(
+    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
 ):
     pass
 
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
@@ -2217,14 +2681,25 @@
         "PercentageCompleteOnRollback": int,
         "InstancesToUpdateOnRollback": int,
         "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
     },
     total=False,
 )
 
+LaunchTemplateOverridesOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesOutputTypeDef",
+    {
+        "InstanceType": str,
+        "WeightedCapacity": str,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
+    },
+    total=False,
+)
+
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2247,14 +2722,59 @@
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": MetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+):
+    pass
+
+_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+class TargetTrackingMetricDataQueryOutputTypeDef(
+    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
+    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
+):
+    pass
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2289,66 +2809,171 @@
 )
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
+LaunchTemplateOutputTypeDef = TypedDict(
+    "LaunchTemplateOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
+    },
+    total=False,
+)
+
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
+PredictiveScalingCustomizedCapacityMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedLoadMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedScalingMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+CustomizedMetricSpecificationOutputTypeDef = TypedDict(
+    "CustomizedMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Statistic": MetricStatisticType,
+        "Unit": str,
+        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
 PredictiveScalingCustomizedCapacityMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedLoadMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
+        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
+    },
+    total=False,
+)
+
+MixedInstancesPolicyOutputTypeDef = TypedDict(
+    "MixedInstancesPolicyOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateOutputTypeDef,
+        "InstancesDistribution": InstancesDistributionOutputTypeDef,
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
+_RequiredPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairOutputTypeDef,
+        "PredefinedScalingMetricSpecification": (
+            PredictiveScalingPredefinedScalingMetricOutputTypeDef
+        ),
+        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricOutputTypeDef,
+        "CustomizedScalingMetricSpecification": (
+            PredictiveScalingCustomizedScalingMetricOutputTypeDef
+        ),
+        "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+        "CustomizedCapacityMetricSpecification": (
+            PredictiveScalingCustomizedCapacityMetricOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
+class PredictiveScalingMetricSpecificationOutputTypeDef(
+    _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
+    _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationOutputTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+    },
+    total=False,
+)
+
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2405,16 +3030,16 @@
     },
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
         "PlacementGroup": str,
@@ -2428,22 +3053,31 @@
         "MaxInstanceLifetime": int,
         "CapacityRebalance": bool,
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "WarmPoolSize": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
-        "TrafficSources": List[TrafficSourceIdentifierTypeDef],
+        "TrafficSources": List[TrafficSourceIdentifierOutputTypeDef],
     },
     total=False,
 )
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
+DesiredConfigurationOutputTypeDef = TypedDict(
+    "DesiredConfigurationOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
     },
@@ -2534,22 +3168,45 @@
     pass
 
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
-        "MetricSpecification": PredictiveScalingMetricSpecificationTypeDef,
+        "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
     },
 )
 
+_RequiredPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "MetricSpecifications": List[PredictiveScalingMetricSpecificationOutputTypeDef],
+    },
+)
+_OptionalPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "Mode": PredictiveScalingModeType,
+        "SchedulingBufferTime": int,
+        "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
+        "MaxCapacityBuffer": int,
+    },
+    total=False,
+)
+
+class PredictiveScalingConfigurationOutputTypeDef(
+    _RequiredPredictiveScalingConfigurationOutputTypeDef,
+    _OptionalPredictiveScalingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
-        "MetricSpecifications": List[PredictiveScalingMetricSpecificationTypeDef],
+        "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
     "_OptionalPredictiveScalingConfigurationTypeDef",
     {
         "Mode": PredictiveScalingModeType,
         "SchedulingBufferTime": int,
@@ -2581,16 +3238,16 @@
         "Status": InstanceRefreshStatusType,
         "StatusReason": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
-        "Preferences": RefreshPreferencesTypeDef,
-        "DesiredConfiguration": DesiredConfigurationTypeDef,
+        "Preferences": RefreshPreferencesOutputTypeDef,
+        "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
@@ -2619,68 +3276,68 @@
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyTypeRequestTypeDef",
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-    },
-)
-_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyTypeRequestTypeDef",
-    {
+        "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
+        "StepAdjustments": List[StepAdjustmentOutputTypeDef],
         "MetricAggregationType": str,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "Alarms": List[AlarmTypeDef],
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
-        "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
+        "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class PutScalingPolicyTypeRequestTypeDef(
-    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
-):
-    pass
-
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
+_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-        "PolicyARN": str,
+    },
+)
+_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyTypeRequestTypeDef",
+    {
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
+class PutScalingPolicyTypeRequestTypeDef(
+    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
+):
+    pass
+
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.0
-Summary: Type annotations for boto3.AutoScaling 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AutoScaling 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-autoscaling"></a>
 
 # mypy-boto3-autoscaling
 
 [![PyPI - mypy-boto3-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,41 +389,48 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
+    AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
+    AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     EnabledMetricTypeDef,
-    LaunchTemplateSpecificationTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
+    TrafficSourceIdentifierOutputTypeDef,
+    BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
+    EbsOutputTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
+    LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
@@ -462,42 +469,58 @@
     DisableMetricsCollectionQueryRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
+    InstanceMetadataOptionsOutputTypeDef,
+    InstanceMonitoringOutputTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesOutputTypeDef,
+    MemoryGiBPerVCpuRequestOutputTypeDef,
+    MemoryMiBRequestOutputTypeDef,
+    NetworkBandwidthGbpsRequestOutputTypeDef,
+    NetworkInterfaceCountRequestOutputTypeDef,
+    TotalLocalStorageGBRequestOutputTypeDef,
+    VCpuCountRequestOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
+    InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
+    InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
     PaginatorConfigTypeDef,
+    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
+    PredictiveScalingPredefinedLoadMetricOutputTypeDef,
+    PredictiveScalingPredefinedMetricPairOutputTypeDef,
+    PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
+    RefreshPreferencesTypeDef,
     ResponseMetadataTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
+    StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
@@ -516,67 +539,85 @@
     DescribeTagsTypeRequestTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
+    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
+    InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
-    PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
+    PutWarmPoolTypeRequestTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
-    CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
+    CreateLaunchConfigurationTypeRequestTypeDef,
+    MetricStatOutputTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
     RollbackDetailsTypeDef,
+    LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
+    MetricDataQueryOutputTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    LaunchTemplateOutputTypeDef,
     LaunchTemplateTypeDef,
+    PredictiveScalingCustomizedCapacityMetricOutputTypeDef,
+    PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+    PredictiveScalingCustomizedScalingMetricOutputTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
+    PredictiveScalingMetricSpecificationOutputTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
-    PutScalingPolicyTypeRequestTypeDef,
     ScalingPolicyTypeDef,
+    PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_structure() -> AcceleratorCountRequestOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.0/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.0/setup.py` & `mypy-boto3-autoscaling-1.28.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScaling 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AutoScaling 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

