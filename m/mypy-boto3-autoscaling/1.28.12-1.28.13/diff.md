# Comparing `tmp/mypy-boto3-autoscaling-1.28.12.tar.gz` & `tmp/mypy-boto3-autoscaling-1.28.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.28.13.tar", last modified: Thu Jul 27 19:34:20 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.28.12.tar` & `mypy-boto3-autoscaling-1.28.13.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.588572 mypy-boto3-autoscaling-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24474 2023-07-27 05:34:20.584572 mypy-boto3-autoscaling-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.580572 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52425 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52343 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-07-27 05:17:48.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-07-27 05:17:48.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94435 2023-07-27 05:17:49.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94282 2023-07-27 05:17:49.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:47.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24474 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.588572 mypy-boto3-autoscaling-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:17:46.000000 mypy-boto3-autoscaling-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.119558 mypy-boto3-autoscaling-1.28.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-27 19:34:20.115558 mypy-boto3-autoscaling-1.28.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.111558 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52899 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-27 19:32:15.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    95018 2023-07-27 19:32:17.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94863 2023-07-27 19:32:16.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.115558 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:34:20.119558 mypy-boto3-autoscaling-1.28.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.28.12/LICENSE` & `mypy-boto3-autoscaling-1.28.13/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.12/PKG-INFO` & `mypy-boto3-autoscaling-1.28.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.12
-Summary: Type annotations for boto3.AutoScaling 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.13
+Summary: Type annotations for boto3.AutoScaling 1.28.13 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -289,14 +289,15 @@
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 client: AutoScalingClient = Session().client("autoscaling")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator(
@@ -321,14 +322,15 @@
 describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator(
     "describe_scaling_activities"
 )
 describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator(
     "describe_scheduled_actions"
 )
 describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_autoscaling.literals` module contains literals extracted from
@@ -348,14 +350,15 @@
     DescribeLoadBalancerTargetGroupsPaginatorName,
     DescribeLoadBalancersPaginatorName,
     DescribeNotificationConfigurationsPaginatorName,
     DescribePoliciesPaginatorName,
     DescribeScalingActivitiesPaginatorName,
     DescribeScheduledActionsPaginatorName,
     DescribeTagsPaginatorName,
+    DescribeWarmPoolPaginatorName,
     InstanceGenerationType,
     InstanceMetadataEndpointStateType,
     InstanceMetadataHttpTokensStateType,
     InstanceRefreshStatusType,
     LifecycleStateType,
     LocalStorageType,
     LocalStorageTypeType,
@@ -394,34 +397,35 @@
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
+    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationOutputTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     TrafficSourceIdentifierOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     EbsOutputTypeDef,
     EbsTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
@@ -430,48 +434,36 @@
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsTypeRequestTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceMetadataOptionsOutputTypeDef,
     InstanceMonitoringOutputTypeDef,
@@ -491,17 +483,15 @@
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricOutputTypeDef,
     PredictiveScalingPredefinedMetricPairOutputTypeDef,
     PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
@@ -509,38 +499,52 @@
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RefreshPreferencesTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackInstanceRefreshAnswerTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
-    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeTagsTypeRequestTypeDef,
+    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeTagsTypeDescribeTagsPaginateTypeDef,
+    DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingOutputTypeDef,
```

### Comparing `mypy-boto3-autoscaling-1.28.12/README.md` & `mypy-boto3-autoscaling-1.28.13/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -257,14 +257,15 @@
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 client: AutoScalingClient = Session().client("autoscaling")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator(
@@ -289,14 +290,15 @@
 describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator(
     "describe_scaling_activities"
 )
 describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator(
     "describe_scheduled_actions"
 )
 describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_autoscaling.literals` module contains literals extracted from
@@ -316,14 +318,15 @@
     DescribeLoadBalancerTargetGroupsPaginatorName,
     DescribeLoadBalancersPaginatorName,
     DescribeNotificationConfigurationsPaginatorName,
     DescribePoliciesPaginatorName,
     DescribeScalingActivitiesPaginatorName,
     DescribeScheduledActionsPaginatorName,
     DescribeTagsPaginatorName,
+    DescribeWarmPoolPaginatorName,
     InstanceGenerationType,
     InstanceMetadataEndpointStateType,
     InstanceMetadataHttpTokensStateType,
     InstanceRefreshStatusType,
     LifecycleStateType,
     LocalStorageType,
     LocalStorageTypeType,
@@ -362,34 +365,35 @@
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
+    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationOutputTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     TrafficSourceIdentifierOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     EbsOutputTypeDef,
     EbsTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
@@ -398,48 +402,36 @@
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsTypeRequestTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceMetadataOptionsOutputTypeDef,
     InstanceMonitoringOutputTypeDef,
@@ -459,17 +451,15 @@
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricOutputTypeDef,
     PredictiveScalingPredefinedMetricPairOutputTypeDef,
     PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
@@ -477,38 +467,52 @@
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RefreshPreferencesTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackInstanceRefreshAnswerTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
-    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeTagsTypeRequestTypeDef,
+    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeTagsTypeDescribeTagsPaginateTypeDef,
+    DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingOutputTypeDef,
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = Session()
     client: AutoScalingClient = session.client("autoscaling")
 
     describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")
     describe_auto_scaling_instances_paginator: DescribeAutoScalingInstancesPaginator = client.get_paginator("describe_auto_scaling_instances")
@@ -29,28 +30,30 @@
     describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
     describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
     describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from .client import AutoScalingClient
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
     DescribeAutoScalingInstancesPaginator,
     DescribeLaunchConfigurationsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 Client = AutoScalingClient
 
 
 __all__ = (
     "AutoScalingClient",
@@ -61,8 +64,9 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = Session()
     client: AutoScalingClient = session.client("autoscaling")
 
     describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")
     describe_auto_scaling_instances_paginator: DescribeAutoScalingInstancesPaginator = client.get_paginator("describe_auto_scaling_instances")
@@ -29,28 +30,30 @@
     describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
     describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
     describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from .client import AutoScalingClient
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
     DescribeAutoScalingInstancesPaginator,
     DescribeLaunchConfigurationsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 Client = AutoScalingClient
 
 __all__ = (
     "AutoScalingClient",
     "Client",
@@ -60,8 +63,9 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        "Type annotations for boto3.AutoScaling 1.28.13\nVersion:         1.28.13\nBuilder version:"
         " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.13")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 from .type_defs import (
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
@@ -889,15 +890,15 @@
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#resume_processes)
         """
 
     def rollback_instance_refresh(
-        self, *, AutoScalingGroupName: str = ...
+        self, *, AutoScalingGroupName: str
     ) -> RollbackInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh that is in progress and rolls back any changes that
         it made.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#rollback_instance_refresh)
@@ -1086,7 +1087,16 @@
 
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_warm_pool"]
+    ) -> DescribeWarmPoolPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 from .type_defs import (
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
@@ -824,15 +825,15 @@
         Resumes the specified suspended auto scaling processes, or all suspended
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#resume_processes)
         """
     def rollback_instance_refresh(
-        self, *, AutoScalingGroupName: str = ...
+        self, *, AutoScalingGroupName: str
     ) -> RollbackInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh that is in progress and rolls back any changes that
         it made.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#rollback_instance_refresh)
@@ -1004,7 +1005,15 @@
         """
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_warm_pool"]
+    ) -> DescribeWarmPoolPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "DescribeLoadBalancerTargetGroupsPaginatorName",
     "DescribeLoadBalancersPaginatorName",
     "DescribeNotificationConfigurationsPaginatorName",
     "DescribePoliciesPaginatorName",
     "DescribeScalingActivitiesPaginatorName",
     "DescribeScheduledActionsPaginatorName",
     "DescribeTagsPaginatorName",
+    "DescribeWarmPoolPaginatorName",
     "InstanceGenerationType",
     "InstanceMetadataEndpointStateType",
     "InstanceMetadataHttpTokensStateType",
     "InstanceRefreshStatusType",
     "LifecycleStateType",
     "LocalStorageType",
     "LocalStorageTypeType",
@@ -76,14 +77,15 @@
 DescribeLoadBalancerTargetGroupsPaginatorName = Literal["describe_load_balancer_target_groups"]
 DescribeLoadBalancersPaginatorName = Literal["describe_load_balancers"]
 DescribeNotificationConfigurationsPaginatorName = Literal["describe_notification_configurations"]
 DescribePoliciesPaginatorName = Literal["describe_policies"]
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
+DescribeWarmPoolPaginatorName = Literal["describe_warm_pool"]
 InstanceGenerationType = Literal["current", "previous"]
 InstanceMetadataEndpointStateType = Literal["disabled", "enabled"]
 InstanceMetadataHttpTokensStateType = Literal["optional", "required"]
 InstanceRefreshStatusType = Literal[
     "Cancelled",
     "Cancelling",
     "Failed",
@@ -540,14 +542,15 @@
     "describe_load_balancer_target_groups",
     "describe_load_balancers",
     "describe_notification_configurations",
     "describe_policies",
     "describe_scaling_activities",
     "describe_scheduled_actions",
     "describe_tags",
+    "describe_warm_pool",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "DescribeLoadBalancerTargetGroupsPaginatorName",
     "DescribeLoadBalancersPaginatorName",
     "DescribeNotificationConfigurationsPaginatorName",
     "DescribePoliciesPaginatorName",
     "DescribeScalingActivitiesPaginatorName",
     "DescribeScheduledActionsPaginatorName",
     "DescribeTagsPaginatorName",
+    "DescribeWarmPoolPaginatorName",
     "InstanceGenerationType",
     "InstanceMetadataEndpointStateType",
     "InstanceMetadataHttpTokensStateType",
     "InstanceRefreshStatusType",
     "LifecycleStateType",
     "LocalStorageType",
     "LocalStorageTypeType",
@@ -74,14 +75,15 @@
 DescribeLoadBalancerTargetGroupsPaginatorName = Literal["describe_load_balancer_target_groups"]
 DescribeLoadBalancersPaginatorName = Literal["describe_load_balancers"]
 DescribeNotificationConfigurationsPaginatorName = Literal["describe_notification_configurations"]
 DescribePoliciesPaginatorName = Literal["describe_policies"]
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
+DescribeWarmPoolPaginatorName = Literal["describe_warm_pool"]
 InstanceGenerationType = Literal["current", "previous"]
 InstanceMetadataEndpointStateType = Literal["disabled", "enabled"]
 InstanceMetadataHttpTokensStateType = Literal["optional", "required"]
 InstanceRefreshStatusType = Literal[
     "Cancelled",
     "Cancelling",
     "Failed",
@@ -538,14 +540,15 @@
     "describe_load_balancer_target_groups",
     "describe_load_balancers",
     "describe_notification_configurations",
     "describe_policies",
     "describe_scaling_activities",
     "describe_scheduled_actions",
     "describe_tags",
+    "describe_warm_pool",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = Session()
     client: AutoScalingClient = session.client("autoscaling")
 
     describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")
     describe_auto_scaling_instances_paginator: DescribeAutoScalingInstancesPaginator = client.get_paginator("describe_auto_scaling_instances")
@@ -31,28 +32,30 @@
     describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
     describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
     describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeWarmPoolAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
 )
@@ -64,197 +67,200 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeAutoScalingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinggroupspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AutoScalingGroupsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
-
 class DescribeAutoScalingInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AutoScalingInstancesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
         """
 
-
 class DescribeLaunchConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
-
 class DescribeLoadBalancerTargetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLoadBalancerTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
         """
 
-
 class DescribeLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLoadBalancersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
         """
 
-
 class DescribeNotificationConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
-
 class DescribePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describepoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describepoliciespaginator)
         """
 
-
 class DescribeScalingActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescalingactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
-
 class DescribeScheduledActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
-
 class DescribeTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
         """
+
+class DescribeWarmPoolPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describewarmpoolpaginator)
+    """
+
+    def paginate(
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[DescribeWarmPoolAnswerTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describewarmpoolpaginator)
+        """
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = Session()
     client: AutoScalingClient = session.client("autoscaling")
 
     describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")
     describe_auto_scaling_instances_paginator: DescribeAutoScalingInstancesPaginator = client.get_paginator("describe_auto_scaling_instances")
@@ -31,28 +32,30 @@
     describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
     describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
     describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeWarmPoolAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
 )
@@ -64,185 +67,213 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeAutoScalingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinggroupspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AutoScalingGroupsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
+
 class DescribeAutoScalingInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AutoScalingInstancesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
         """
 
+
 class DescribeLaunchConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
+
 class DescribeLoadBalancerTargetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLoadBalancerTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
         """
 
+
 class DescribeLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLoadBalancersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
         """
 
+
 class DescribeNotificationConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
+
 class DescribePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describepoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describepoliciespaginator)
         """
 
+
 class DescribeScalingActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescalingactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
+
 class DescribeScheduledActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
+
 class DescribeTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
         """
+
+
+class DescribeWarmPoolPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describewarmpoolpaginator)
+    """
+
+    def paginate(
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[DescribeWarmPoolAnswerTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describewarmpoolpaginator)
+        """
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,34 +54,35 @@
 
 __all__ = (
     "AcceleratorCountRequestOutputTypeDef",
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
+    "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationOutputTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "TrafficSourceIdentifierOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsOutputTypeDef",
     "EbsTypeDef",
-    "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
@@ -90,48 +91,36 @@
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
-    "DescribeAccountLimitsAnswerTypeDef",
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
     "DescribeInstanceRefreshesTypeRequestTypeDef",
-    "DescribeLifecycleHookTypesAnswerTypeDef",
     "LifecycleHookTypeDef",
     "DescribeLifecycleHooksTypeRequestTypeDef",
-    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     "LoadBalancerTargetGroupStateTypeDef",
-    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeLoadBalancersRequestRequestTypeDef",
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsTypeRequestTypeDef",
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DescribeTrafficSourcesRequestRequestTypeDef",
     "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceMetadataOptionsOutputTypeDef",
     "InstanceMonitoringOutputTypeDef",
@@ -151,17 +140,15 @@
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyOutputTypeDef",
     "InstanceReusePolicyTypeDef",
     "InstancesDistributionOutputTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "PredictiveScalingPredefinedLoadMetricOutputTypeDef",
     "PredictiveScalingPredefinedMetricPairOutputTypeDef",
     "PredictiveScalingPredefinedScalingMetricOutputTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
@@ -169,38 +156,52 @@
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
     "RefreshPreferencesTypeDef",
-    "ResponseMetadataTypeDef",
-    "RollbackInstanceRefreshAnswerTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "StepAdjustmentOutputTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
-    "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
     "ActivityTypeTypeDef",
+    "CancelInstanceRefreshAnswerTypeDef",
+    "DescribeAccountLimitsAnswerTypeDef",
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DetachInstancesAnswerTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
+    "RollbackInstanceRefreshAnswerTypeDef",
+    "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
-    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     "DescribeTagsTypeRequestTypeDef",
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
+    "DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingOutputTypeDef",
@@ -333,14 +334,25 @@
 )
 
 
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
 
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
 AdjustmentTypeTypeDef = TypedDict(
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
@@ -417,14 +429,24 @@
     {
         "Name": str,
         "Values": Sequence[str],
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
 EnabledMetricTypeDef = TypedDict(
     "EnabledMetricTypeDef",
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
@@ -583,22 +605,14 @@
         "Iops": int,
         "Encrypted": bool,
         "Throughput": int,
     },
     total=False,
 )
 
-CancelInstanceRefreshAnswerTypeDef = TypedDict(
-    "CancelInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelInstanceRefreshTypeRequestTypeDef = TypedDict(
     "CancelInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -811,52 +825,24 @@
 
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
 
-DescribeAccountLimitsAnswerTypeDef = TypedDict(
-    "DescribeAccountLimitsAnswerTypeDef",
-    {
-        "MaxNumberOfAutoScalingGroups": int,
-        "MaxNumberOfLaunchConfigurations": int,
-        "NumberOfAutoScalingGroups": int,
-        "NumberOfLaunchConfigurations": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    {
-        "AutoScalingNotificationTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceRefreshesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
@@ -873,22 +859,14 @@
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
 
-DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    {
-        "LifecycleHookTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -919,36 +897,14 @@
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
-    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -973,36 +929,14 @@
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
 )
 
-_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
-    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
@@ -1053,112 +987,61 @@
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationType": str,
     },
     total=False,
 )
 
-DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
-    {
-        "AutoScalingGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeNotificationConfigurationsTypeRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyNames": Sequence[str],
-        "PolicyTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePoliciesTypeRequestTypeDef = TypedDict(
     "DescribePoliciesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyNames": Sequence[str],
         "PolicyTypes": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ActivityIds": Sequence[str],
-        "AutoScalingGroupName": str,
-        "IncludeDeletedGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeScalingActivitiesTypeRequestTypeDef = TypedDict(
     "DescribeScalingActivitiesTypeRequestTypeDef",
     {
         "ActivityIds": Sequence[str],
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
     "DescribeScheduledActionsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
-    {
-        "TerminationPolicyTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
@@ -1268,21 +1151,14 @@
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1627,43 +1503,24 @@
 LaunchConfigurationNameTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNameTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 
-LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
-    {
-        "LaunchConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 LaunchConfigurationNamesTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeRequestTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
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
 _RequiredPredefinedMetricSpecificationOutputTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationOutputTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationOutputTypeDef = TypedDict(
@@ -1963,39 +1820,19 @@
         "AutoRollback": bool,
         "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
         "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
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
-RollbackInstanceRefreshAnswerTypeDef = TypedDict(
-    "RollbackInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
-    total=False,
 )
 
 _RequiredStepAdjustmentOutputTypeDef = TypedDict(
     "_RequiredStepAdjustmentOutputTypeDef",
     {
         "ScalingAdjustment": int,
     },
@@ -2104,85 +1941,143 @@
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
 )
 
-StartInstanceRefreshAnswerTypeDef = TypedDict(
-    "StartInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TerminateInstanceInAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     {
         "InstanceId": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
 
 ActivitiesTypeTypeDef = TypedDict(
     "ActivitiesTypeTypeDef",
     {
         "Activities": List[ActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeTypeDef = TypedDict(
     "ActivityTypeTypeDef",
     {
         "Activity": ActivityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelInstanceRefreshAnswerTypeDef = TypedDict(
+    "CancelInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsAnswerTypeDef = TypedDict(
+    "DescribeAccountLimitsAnswerTypeDef",
+    {
+        "MaxNumberOfAutoScalingGroups": int,
+        "MaxNumberOfLaunchConfigurations": int,
+        "NumberOfAutoScalingGroups": int,
+        "NumberOfLaunchConfigurations": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    {
+        "AutoScalingNotificationTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    {
+        "LifecycleHookTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    {
+        "TerminationPolicyTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachInstancesAnswerTypeDef = TypedDict(
     "DetachInstancesAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnterStandbyAnswerTypeDef = TypedDict(
     "EnterStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExitStandbyAnswerTypeDef = TypedDict(
     "ExitStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackInstanceRefreshAnswerTypeDef = TypedDict(
+    "RollbackInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartInstanceRefreshAnswerTypeDef = TypedDict(
+    "StartInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAdjustmentTypesAnswerTypeDef = TypedDict(
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachTrafficSourcesTypeRequestTypeDef = TypedDict(
     "AttachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -2194,50 +2089,177 @@
     "DetachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
 )
 
-AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
+        "NextToken": str,
+        "MaxRecords": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeRequestTypeDef",
+DescribeTagsTypeRequestTypeDef = TypedDict(
+    "DescribeTagsTypeRequestTypeDef",
     {
-        "AutoScalingGroupNames": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxRecords": int,
+    },
+    total=False,
+)
+
+AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
+    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
+    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+):
+    pass
+
+
+DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyNames": Sequence[str],
+        "PolicyTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ActivityIds": Sequence[str],
+        "AutoScalingGroupName": str,
+        "IncludeDeletedGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsTypeRequestTypeDef = TypedDict(
-    "DescribeTagsTypeRequestTypeDef",
+_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "NextToken": str,
-        "MaxRecords": int,
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef(
+    _RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+    _OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+):
+    pass
+
+
+LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+    {
+        "LaunchConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_RequiredAutoScalingInstanceDetailsTypeDef",
     {
@@ -2294,31 +2316,31 @@
 
 
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteScheduledActionAnswerTypeDef = TypedDict(
     "BatchDeleteScheduledActionAnswerTypeDef",
     {
         "FailedScheduledActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutScheduledUpdateGroupActionAnswerTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -2426,60 +2448,60 @@
     pass
 
 
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerTargetGroupsResponseTypeDef = TypedDict(
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     {
         "LoadBalancerTargetGroups": List[LoadBalancerTargetGroupStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersResponseTypeDef = TypedDict(
     "DescribeLoadBalancersResponseTypeDef",
     {
         "LoadBalancers": List[LoadBalancerStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMetricCollectionTypesAnswerTypeDef = TypedDict(
     "DescribeMetricCollectionTypesAnswerTypeDef",
     {
         "Metrics": List[MetricCollectionTypeTypeDef],
         "Granularities": List[MetricGranularityTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationConfigurationsAnswerTypeDef = TypedDict(
     "DescribeNotificationConfigurationsAnswerTypeDef",
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrafficSourcesResponseTypeDef = TypedDict(
     "DescribeTrafficSourcesResponseTypeDef",
     {
         "TrafficSources": List[TrafficSourceStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshProgressDetailsTypeDef = TypedDict(
     "InstanceRefreshProgressDetailsTypeDef",
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
@@ -2608,33 +2630,33 @@
     pass
 
 
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredLaunchConfigurationTypeDef = TypedDict(
     "_RequiredLaunchConfigurationTypeDef",
     {
         "LaunchConfigurationName": str,
@@ -2832,24 +2854,24 @@
 
 DescribeWarmPoolAnswerTypeDef = TypedDict(
     "DescribeWarmPoolAnswerTypeDef",
     {
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LaunchConfigurationsTypeTypeDef = TypedDict(
     "LaunchConfigurationsTypeTypeDef",
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredMetricDataQueryOutputTypeDef",
     {
         "Id": str,
@@ -3371,15 +3393,15 @@
 
 
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshTypeDef = TypedDict(
     "InstanceRefreshTypeDef",
     {
         "InstanceRefreshId": str,
@@ -3423,15 +3445,15 @@
 
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScalingPolicyTypeDef = TypedDict(
     "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -3488,19 +3510,19 @@
 
 
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeTypeDef = TypedDict(
     "PoliciesTypeTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,34 +53,35 @@
 
 __all__ = (
     "AcceleratorCountRequestOutputTypeDef",
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
+    "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationOutputTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "TrafficSourceIdentifierOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsOutputTypeDef",
     "EbsTypeDef",
-    "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
@@ -89,48 +90,36 @@
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
-    "DescribeAccountLimitsAnswerTypeDef",
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
     "DescribeInstanceRefreshesTypeRequestTypeDef",
-    "DescribeLifecycleHookTypesAnswerTypeDef",
     "LifecycleHookTypeDef",
     "DescribeLifecycleHooksTypeRequestTypeDef",
-    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     "LoadBalancerTargetGroupStateTypeDef",
-    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeLoadBalancersRequestRequestTypeDef",
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsTypeRequestTypeDef",
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DescribeTrafficSourcesRequestRequestTypeDef",
     "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceMetadataOptionsOutputTypeDef",
     "InstanceMonitoringOutputTypeDef",
@@ -150,17 +139,15 @@
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyOutputTypeDef",
     "InstanceReusePolicyTypeDef",
     "InstancesDistributionOutputTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "PredictiveScalingPredefinedLoadMetricOutputTypeDef",
     "PredictiveScalingPredefinedMetricPairOutputTypeDef",
     "PredictiveScalingPredefinedScalingMetricOutputTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
@@ -168,38 +155,52 @@
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
     "RefreshPreferencesTypeDef",
-    "ResponseMetadataTypeDef",
-    "RollbackInstanceRefreshAnswerTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "StepAdjustmentOutputTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
-    "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
     "ActivityTypeTypeDef",
+    "CancelInstanceRefreshAnswerTypeDef",
+    "DescribeAccountLimitsAnswerTypeDef",
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DetachInstancesAnswerTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
+    "RollbackInstanceRefreshAnswerTypeDef",
+    "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
-    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     "DescribeTagsTypeRequestTypeDef",
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
+    "DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingOutputTypeDef",
@@ -330,14 +331,25 @@
     },
     total=False,
 )
 
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
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
 AdjustmentTypeTypeDef = TypedDict(
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
@@ -410,14 +422,24 @@
     {
         "Name": str,
         "Values": Sequence[str],
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
 EnabledMetricTypeDef = TypedDict(
     "EnabledMetricTypeDef",
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
@@ -570,22 +592,14 @@
         "Iops": int,
         "Encrypted": bool,
         "Throughput": int,
     },
     total=False,
 )
 
-CancelInstanceRefreshAnswerTypeDef = TypedDict(
-    "CancelInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelInstanceRefreshTypeRequestTypeDef = TypedDict(
     "CancelInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -786,52 +800,24 @@
 )
 
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
-DescribeAccountLimitsAnswerTypeDef = TypedDict(
-    "DescribeAccountLimitsAnswerTypeDef",
-    {
-        "MaxNumberOfAutoScalingGroups": int,
-        "MaxNumberOfLaunchConfigurations": int,
-        "NumberOfAutoScalingGroups": int,
-        "NumberOfLaunchConfigurations": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    {
-        "AutoScalingNotificationTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceRefreshesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
@@ -846,22 +832,14 @@
 
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
-DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    {
-        "LifecycleHookTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -890,34 +868,14 @@
 
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
-    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -940,34 +898,14 @@
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
 )
 
-_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
-    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
@@ -1016,112 +954,61 @@
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationType": str,
     },
     total=False,
 )
 
-DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
-    {
-        "AutoScalingGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeNotificationConfigurationsTypeRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyNames": Sequence[str],
-        "PolicyTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePoliciesTypeRequestTypeDef = TypedDict(
     "DescribePoliciesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyNames": Sequence[str],
         "PolicyTypes": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ActivityIds": Sequence[str],
-        "AutoScalingGroupName": str,
-        "IncludeDeletedGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeScalingActivitiesTypeRequestTypeDef = TypedDict(
     "DescribeScalingActivitiesTypeRequestTypeDef",
     {
         "ActivityIds": Sequence[str],
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
     "DescribeScheduledActionsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
-    {
-        "TerminationPolicyTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
@@ -1223,21 +1110,14 @@
 
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1566,43 +1446,24 @@
 LaunchConfigurationNameTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNameTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 
-LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
-    {
-        "LaunchConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 LaunchConfigurationNamesTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeRequestTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
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
 _RequiredPredefinedMetricSpecificationOutputTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationOutputTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationOutputTypeDef = TypedDict(
@@ -1878,39 +1739,19 @@
         "AutoRollback": bool,
         "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
         "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
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
-RollbackInstanceRefreshAnswerTypeDef = TypedDict(
-    "RollbackInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
-    total=False,
 )
 
 _RequiredStepAdjustmentOutputTypeDef = TypedDict(
     "_RequiredStepAdjustmentOutputTypeDef",
     {
         "ScalingAdjustment": int,
     },
@@ -2011,85 +1852,143 @@
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
 )
 
-StartInstanceRefreshAnswerTypeDef = TypedDict(
-    "StartInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TerminateInstanceInAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     {
         "InstanceId": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
 
 ActivitiesTypeTypeDef = TypedDict(
     "ActivitiesTypeTypeDef",
     {
         "Activities": List[ActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeTypeDef = TypedDict(
     "ActivityTypeTypeDef",
     {
         "Activity": ActivityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelInstanceRefreshAnswerTypeDef = TypedDict(
+    "CancelInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsAnswerTypeDef = TypedDict(
+    "DescribeAccountLimitsAnswerTypeDef",
+    {
+        "MaxNumberOfAutoScalingGroups": int,
+        "MaxNumberOfLaunchConfigurations": int,
+        "NumberOfAutoScalingGroups": int,
+        "NumberOfLaunchConfigurations": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    {
+        "AutoScalingNotificationTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    {
+        "LifecycleHookTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    {
+        "TerminationPolicyTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachInstancesAnswerTypeDef = TypedDict(
     "DetachInstancesAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnterStandbyAnswerTypeDef = TypedDict(
     "EnterStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExitStandbyAnswerTypeDef = TypedDict(
     "ExitStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackInstanceRefreshAnswerTypeDef = TypedDict(
+    "RollbackInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartInstanceRefreshAnswerTypeDef = TypedDict(
+    "StartInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAdjustmentTypesAnswerTypeDef = TypedDict(
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachTrafficSourcesTypeRequestTypeDef = TypedDict(
     "AttachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -2101,50 +2000,171 @@
     "DetachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
 )
 
-AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
+        "NextToken": str,
+        "MaxRecords": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeRequestTypeDef",
+DescribeTagsTypeRequestTypeDef = TypedDict(
+    "DescribeTagsTypeRequestTypeDef",
     {
-        "AutoScalingGroupNames": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxRecords": int,
+    },
+    total=False,
+)
+
+AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
+    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
+    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+):
+    pass
+
+DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyNames": Sequence[str],
+        "PolicyTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ActivityIds": Sequence[str],
+        "AutoScalingGroupName": str,
+        "IncludeDeletedGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsTypeRequestTypeDef = TypedDict(
-    "DescribeTagsTypeRequestTypeDef",
+_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "NextToken": str,
-        "MaxRecords": int,
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef(
+    _RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+    _OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+):
+    pass
+
+LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+    {
+        "LaunchConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_RequiredAutoScalingInstanceDetailsTypeDef",
     {
@@ -2197,31 +2217,31 @@
     pass
 
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteScheduledActionAnswerTypeDef = TypedDict(
     "BatchDeleteScheduledActionAnswerTypeDef",
     {
         "FailedScheduledActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutScheduledUpdateGroupActionAnswerTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -2321,60 +2341,60 @@
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerTargetGroupsResponseTypeDef = TypedDict(
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     {
         "LoadBalancerTargetGroups": List[LoadBalancerTargetGroupStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersResponseTypeDef = TypedDict(
     "DescribeLoadBalancersResponseTypeDef",
     {
         "LoadBalancers": List[LoadBalancerStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMetricCollectionTypesAnswerTypeDef = TypedDict(
     "DescribeMetricCollectionTypesAnswerTypeDef",
     {
         "Metrics": List[MetricCollectionTypeTypeDef],
         "Granularities": List[MetricGranularityTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationConfigurationsAnswerTypeDef = TypedDict(
     "DescribeNotificationConfigurationsAnswerTypeDef",
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrafficSourcesResponseTypeDef = TypedDict(
     "DescribeTrafficSourcesResponseTypeDef",
     {
         "TrafficSources": List[TrafficSourceStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshProgressDetailsTypeDef = TypedDict(
     "InstanceRefreshProgressDetailsTypeDef",
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
@@ -2497,33 +2517,33 @@
 ):
     pass
 
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredLaunchConfigurationTypeDef = TypedDict(
     "_RequiredLaunchConfigurationTypeDef",
     {
         "LaunchConfigurationName": str,
@@ -2709,24 +2729,24 @@
 
 DescribeWarmPoolAnswerTypeDef = TypedDict(
     "DescribeWarmPoolAnswerTypeDef",
     {
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LaunchConfigurationsTypeTypeDef = TypedDict(
     "LaunchConfigurationsTypeTypeDef",
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredMetricDataQueryOutputTypeDef",
     {
         "Id": str,
@@ -3222,15 +3242,15 @@
     pass
 
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshTypeDef = TypedDict(
     "InstanceRefreshTypeDef",
     {
         "InstanceRefreshId": str,
@@ -3272,15 +3292,15 @@
 
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScalingPolicyTypeDef = TypedDict(
     "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -3335,19 +3355,19 @@
     pass
 
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeTypeDef = TypedDict(
     "PoliciesTypeTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.12
-Summary: Type annotations for boto3.AutoScaling 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.13
+Summary: Type annotations for boto3.AutoScaling 1.28.13 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -289,14 +289,15 @@
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 client: AutoScalingClient = Session().client("autoscaling")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator(
@@ -321,14 +322,15 @@
 describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator(
     "describe_scaling_activities"
 )
 describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator(
     "describe_scheduled_actions"
 )
 describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_autoscaling.literals` module contains literals extracted from
@@ -348,14 +350,15 @@
     DescribeLoadBalancerTargetGroupsPaginatorName,
     DescribeLoadBalancersPaginatorName,
     DescribeNotificationConfigurationsPaginatorName,
     DescribePoliciesPaginatorName,
     DescribeScalingActivitiesPaginatorName,
     DescribeScheduledActionsPaginatorName,
     DescribeTagsPaginatorName,
+    DescribeWarmPoolPaginatorName,
     InstanceGenerationType,
     InstanceMetadataEndpointStateType,
     InstanceMetadataHttpTokensStateType,
     InstanceRefreshStatusType,
     LifecycleStateType,
     LocalStorageType,
     LocalStorageTypeType,
@@ -394,34 +397,35 @@
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
+    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationOutputTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     TrafficSourceIdentifierOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     EbsOutputTypeDef,
     EbsTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
@@ -430,48 +434,36 @@
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsTypeRequestTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceMetadataOptionsOutputTypeDef,
     InstanceMonitoringOutputTypeDef,
@@ -491,17 +483,15 @@
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricOutputTypeDef,
     PredictiveScalingPredefinedMetricPairOutputTypeDef,
     PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
@@ -509,38 +499,52 @@
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RefreshPreferencesTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackInstanceRefreshAnswerTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
-    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeTagsTypeRequestTypeDef,
+    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeTagsTypeDescribeTagsPaginateTypeDef,
+    DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingOutputTypeDef,
```

### Comparing `mypy-boto3-autoscaling-1.28.12/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.12/setup.py` & `mypy-boto3-autoscaling-1.28.13/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.28.12",
+    version="1.28.13",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScaling 1.28.12 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.AutoScaling 1.28.13 service generated with mypy-boto3-builder"
         " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

