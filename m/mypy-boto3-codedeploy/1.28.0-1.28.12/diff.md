# Comparing `tmp/mypy-boto3-codedeploy-1.28.0.tar.gz` & `tmp/mypy-boto3-codedeploy-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codedeploy-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
+gzip compressed data, was "mypy-boto3-codedeploy-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
```

## Comparing `mypy-boto3-codedeploy-1.28.0.tar` & `mypy-boto3-codedeploy-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.822251 mypy-boto3-codedeploy-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-07-06 20:59:12.814252 mypy-boto3-codedeploy-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.794251 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46184 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-06 20:36:00.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-07-06 20:36:00.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50681 2023-07-06 20:36:02.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-07-06 20:36:00.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.814252 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-07-06 20:59:12.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 20:59:12.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:12.000000 mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.822251 mypy-boto3-codedeploy-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:35:59.000000 mypy-boto3-codedeploy-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21208 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.424555 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46184 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-27 05:19:05.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-07-27 05:19:05.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58069 2023-07-27 05:19:06.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58036 2023-07-27 05:19:06.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/setup.py
```

### Comparing `mypy-boto3-codedeploy-1.28.0/LICENSE` & `mypy-boto3-codedeploy-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/PKG-INFO` & `mypy-boto3-codedeploy-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeDeploy 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeDeploy 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codedeploy"></a>
 
 # mypy-boto3-codedeploy
 
 [![PyPI - mypy-boto3-codedeploy](https://img.shields.io/pypi/v/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codedeploy?color=blue)](https://pypistats.org/packages/mypy-boto3-codedeploy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,25 +417,31 @@
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
+    AlarmOutputTypeDef,
     AlarmTypeDef,
+    AppSpecContentOutputTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
+    AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
+    BlueInstanceTerminationOptionOutputTypeDef,
+    DeploymentReadyOptionOutputTypeDef,
+    GreenFleetProvisioningOptionOutputTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
     CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
     CreateDeploymentConfigOutputTypeDef,
@@ -448,34 +454,43 @@
     CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
+    MinimumHealthyHostsOutputTypeDef,
+    DeploymentStyleOutputTypeDef,
+    EC2TagFilterOutputTypeDef,
+    ECSServiceOutputTypeDef,
     LastDeploymentInfoTypeDef,
+    TagFilterOutputTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
-    TargetGroupInfoTypeDef,
+    TargetGroupInfoOutputTypeDef,
+    ELBInfoOutputTypeDef,
     ELBInfoTypeDef,
     EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
+    GitHubLocationOutputTypeDef,
     GitHubLocationTypeDef,
+    TagOutputTypeDef,
     LambdaFunctionInfoTypeDef,
     ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
     ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
     ListApplicationsOutputTypeDef,
     ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
@@ -493,78 +508,93 @@
     TimeRangeTypeDef,
     ListDeploymentsOutputTypeDef,
     ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TargetGroupInfoTypeDef,
     PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    RawStringOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
     StopDeploymentOutputTypeDef,
+    TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
+    TimeBasedCanaryOutputTypeDef,
     TimeBasedCanaryTypeDef,
+    TimeBasedLinearOutputTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
-    InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
     GetApplicationOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
+    BlueGreenDeploymentConfigurationOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
     EC2TagSetTypeDef,
     ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
     OnPremisesTagSetTypeDef,
+    EC2TagSetOutputTypeDef,
+    OnPremisesTagSetOutputTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
+    InstanceInfoTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
+    RevisionLocationOutputTypeDef,
     RevisionLocationTypeDef,
+    TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
+    TrafficRoutingConfigOutputTypeDef,
     TrafficRoutingConfigTypeDef,
-    BatchGetOnPremisesInstancesOutputTypeDef,
-    GetOnPremisesInstanceOutputTypeDef,
     TargetInstancesTypeDef,
+    TargetInstancesOutputTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
-    BatchGetApplicationRevisionsInputRequestTypeDef,
-    GetApplicationRevisionInputRequestTypeDef,
+    BatchGetOnPremisesInstancesOutputTypeDef,
+    GetOnPremisesInstanceOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     ListApplicationRevisionsOutputTypeDef,
-    RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
+    BatchGetApplicationRevisionsInputRequestTypeDef,
+    GetApplicationRevisionInputRequestTypeDef,
+    RegisterApplicationRevisionInputRequestTypeDef,
+    LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
-    CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    CreateDeploymentConfigInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
-    CreateDeploymentGroupInputRequestTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
+    CreateDeploymentGroupInputRequestTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
```

### Comparing `mypy-boto3-codedeploy-1.28.0/README.md` & `mypy-boto3-codedeploy-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codedeploy"></a>
 
 # mypy-boto3-codedeploy
 
 [![PyPI - mypy-boto3-codedeploy](https://img.shields.io/pypi/v/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codedeploy?color=blue)](https://pypistats.org/packages/mypy-boto3-codedeploy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,25 +385,31 @@
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
+    AlarmOutputTypeDef,
     AlarmTypeDef,
+    AppSpecContentOutputTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
+    AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
+    BlueInstanceTerminationOptionOutputTypeDef,
+    DeploymentReadyOptionOutputTypeDef,
+    GreenFleetProvisioningOptionOutputTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
     CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
     CreateDeploymentConfigOutputTypeDef,
@@ -416,34 +422,43 @@
     CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
+    MinimumHealthyHostsOutputTypeDef,
+    DeploymentStyleOutputTypeDef,
+    EC2TagFilterOutputTypeDef,
+    ECSServiceOutputTypeDef,
     LastDeploymentInfoTypeDef,
+    TagFilterOutputTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
-    TargetGroupInfoTypeDef,
+    TargetGroupInfoOutputTypeDef,
+    ELBInfoOutputTypeDef,
     ELBInfoTypeDef,
     EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
+    GitHubLocationOutputTypeDef,
     GitHubLocationTypeDef,
+    TagOutputTypeDef,
     LambdaFunctionInfoTypeDef,
     ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
     ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
     ListApplicationsOutputTypeDef,
     ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
@@ -461,78 +476,93 @@
     TimeRangeTypeDef,
     ListDeploymentsOutputTypeDef,
     ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TargetGroupInfoTypeDef,
     PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    RawStringOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
     StopDeploymentOutputTypeDef,
+    TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
+    TimeBasedCanaryOutputTypeDef,
     TimeBasedCanaryTypeDef,
+    TimeBasedLinearOutputTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
-    InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
     GetApplicationOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
+    BlueGreenDeploymentConfigurationOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
     EC2TagSetTypeDef,
     ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
     OnPremisesTagSetTypeDef,
+    EC2TagSetOutputTypeDef,
+    OnPremisesTagSetOutputTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
+    InstanceInfoTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
+    RevisionLocationOutputTypeDef,
     RevisionLocationTypeDef,
+    TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
+    TrafficRoutingConfigOutputTypeDef,
     TrafficRoutingConfigTypeDef,
-    BatchGetOnPremisesInstancesOutputTypeDef,
-    GetOnPremisesInstanceOutputTypeDef,
     TargetInstancesTypeDef,
+    TargetInstancesOutputTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
-    BatchGetApplicationRevisionsInputRequestTypeDef,
-    GetApplicationRevisionInputRequestTypeDef,
+    BatchGetOnPremisesInstancesOutputTypeDef,
+    GetOnPremisesInstanceOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     ListApplicationRevisionsOutputTypeDef,
-    RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
+    BatchGetApplicationRevisionsInputRequestTypeDef,
+    GetApplicationRevisionInputRequestTypeDef,
+    RegisterApplicationRevisionInputRequestTypeDef,
+    LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
-    CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    CreateDeploymentConfigInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
-    CreateDeploymentGroupInputRequestTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
+    CreateDeploymentGroupInputRequestTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
```

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/__init__.py` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/__init__.pyi` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/__main__.py` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeDeploy 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeDeploy 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/client.py` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/client.pyi` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/literals.py` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,15 @@
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
@@ -390,26 +391,28 @@
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

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/literals.pyi` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,15 @@
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
@@ -388,26 +389,28 @@
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

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/paginator.py` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/paginator.pyi` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/type_defs.py` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,31 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
+    "AlarmOutputTypeDef",
     "AlarmTypeDef",
+    "AppSpecContentOutputTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
+    "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
+    "BlueInstanceTerminationOptionOutputTypeDef",
+    "DeploymentReadyOptionOutputTypeDef",
+    "GreenFleetProvisioningOptionOutputTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
     "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
     "CreateDeploymentConfigOutputTypeDef",
@@ -86,34 +92,43 @@
     "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
+    "MinimumHealthyHostsOutputTypeDef",
+    "DeploymentStyleOutputTypeDef",
+    "EC2TagFilterOutputTypeDef",
+    "ECSServiceOutputTypeDef",
     "LastDeploymentInfoTypeDef",
+    "TagFilterOutputTypeDef",
+    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
-    "TargetGroupInfoTypeDef",
+    "TargetGroupInfoOutputTypeDef",
+    "ELBInfoOutputTypeDef",
     "ELBInfoTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
+    "GitHubLocationOutputTypeDef",
     "GitHubLocationTypeDef",
+    "TagOutputTypeDef",
     "LambdaFunctionInfoTypeDef",
     "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
     "ListApplicationsOutputTypeDef",
     "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
@@ -131,78 +146,93 @@
     "TimeRangeTypeDef",
     "ListDeploymentsOutputTypeDef",
     "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     "ListGitHubAccountTokenNamesOutputTypeDef",
     "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TargetGroupInfoTypeDef",
     "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    "RawStringOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
     "StopDeploymentOutputTypeDef",
+    "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
+    "TimeBasedCanaryOutputTypeDef",
     "TimeBasedCanaryTypeDef",
+    "TimeBasedLinearOutputTypeDef",
     "TimeBasedLinearTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
-    "InstanceInfoTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
     "BatchGetApplicationsOutputTypeDef",
     "GetApplicationOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
+    "BlueGreenDeploymentConfigurationOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
     "EC2TagSetTypeDef",
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
     "OnPremisesTagSetTypeDef",
+    "EC2TagSetOutputTypeDef",
+    "OnPremisesTagSetOutputTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
+    "InstanceInfoTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
+    "RevisionLocationOutputTypeDef",
     "RevisionLocationTypeDef",
+    "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
+    "TrafficRoutingConfigOutputTypeDef",
     "TrafficRoutingConfigTypeDef",
-    "BatchGetOnPremisesInstancesOutputTypeDef",
-    "GetOnPremisesInstanceOutputTypeDef",
     "TargetInstancesTypeDef",
+    "TargetInstancesOutputTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
-    "BatchGetApplicationRevisionsInputRequestTypeDef",
-    "GetApplicationRevisionInputRequestTypeDef",
+    "BatchGetOnPremisesInstancesOutputTypeDef",
+    "GetOnPremisesInstanceOutputTypeDef",
     "GetApplicationRevisionOutputTypeDef",
     "ListApplicationRevisionsOutputTypeDef",
-    "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
+    "BatchGetApplicationRevisionsInputRequestTypeDef",
+    "GetApplicationRevisionInputRequestTypeDef",
+    "RegisterApplicationRevisionInputRequestTypeDef",
+    "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
-    "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
+    "CreateDeploymentConfigInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
-    "CreateDeploymentGroupInputRequestTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
+    "CreateDeploymentGroupInputRequestTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -214,22 +244,39 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+AlarmOutputTypeDef = TypedDict(
+    "AlarmOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
+AppSpecContentOutputTypeDef = TypedDict(
+    "AppSpecContentOutputTypeDef",
+    {
+        "content": str,
+        "sha256": str,
+    },
+    total=False,
+)
+
 AppSpecContentTypeDef = TypedDict(
     "AppSpecContentTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -244,19 +291,28 @@
         "linkedToGitHub": bool,
         "gitHubAccountName": str,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
+AutoRollbackConfigurationOutputTypeDef = TypedDict(
+    "AutoRollbackConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "events": List[AutoRollbackEventType],
+    },
+    total=False,
+)
+
 AutoRollbackConfigurationTypeDef = TypedDict(
     "AutoRollbackConfigurationTypeDef",
     {
         "enabled": bool,
-        "events": List[AutoRollbackEventType],
+        "events": Sequence[AutoRollbackEventType],
     },
     total=False,
 )
 
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
@@ -308,14 +364,40 @@
 BatchGetOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     {
         "instanceNames": Sequence[str],
     },
 )
 
+BlueInstanceTerminationOptionOutputTypeDef = TypedDict(
+    "BlueInstanceTerminationOptionOutputTypeDef",
+    {
+        "action": InstanceActionType,
+        "terminationWaitTimeInMinutes": int,
+    },
+    total=False,
+)
+
+DeploymentReadyOptionOutputTypeDef = TypedDict(
+    "DeploymentReadyOptionOutputTypeDef",
+    {
+        "actionOnTimeout": DeploymentReadyActionType,
+        "waitTimeInMinutes": int,
+    },
+    total=False,
+)
+
+GreenFleetProvisioningOptionOutputTypeDef = TypedDict(
+    "GreenFleetProvisioningOptionOutputTypeDef",
+    {
+        "action": GreenFleetProvisioningActionType,
+    },
+    total=False,
+)
+
 BlueInstanceTerminationOptionTypeDef = TypedDict(
     "BlueInstanceTerminationOptionTypeDef",
     {
         "action": InstanceActionType,
         "terminationWaitTimeInMinutes": int,
     },
     total=False,
@@ -411,15 +493,15 @@
 )
 
 TriggerConfigTypeDef = TypedDict(
     "TriggerConfigTypeDef",
     {
         "triggerName": str,
         "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
+        "triggerEvents": Sequence[TriggerEventTypeType],
     },
     total=False,
 )
 
 CreateDeploymentGroupOutputTypeDef = TypedDict(
     "CreateDeploymentGroupOutputTypeDef",
     {
@@ -478,25 +560,82 @@
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
+MinimumHealthyHostsOutputTypeDef = TypedDict(
+    "MinimumHealthyHostsOutputTypeDef",
+    {
+        "type": MinimumHealthyHostsTypeType,
+        "value": int,
+    },
+    total=False,
+)
+
+DeploymentStyleOutputTypeDef = TypedDict(
+    "DeploymentStyleOutputTypeDef",
+    {
+        "deploymentType": DeploymentTypeType,
+        "deploymentOption": DeploymentOptionType,
+    },
+    total=False,
+)
+
+EC2TagFilterOutputTypeDef = TypedDict(
+    "EC2TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "Type": EC2TagFilterTypeType,
+    },
+    total=False,
+)
+
+ECSServiceOutputTypeDef = TypedDict(
+    "ECSServiceOutputTypeDef",
+    {
+        "serviceName": str,
+        "clusterName": str,
+    },
+    total=False,
+)
+
 LastDeploymentInfoTypeDef = TypedDict(
     "LastDeploymentInfoTypeDef",
     {
         "deploymentId": str,
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
+TagFilterOutputTypeDef = TypedDict(
+    "TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "Type": TagFilterTypeType,
+    },
+    total=False,
+)
+
+TriggerConfigOutputTypeDef = TypedDict(
+    "TriggerConfigOutputTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -548,16 +687,24 @@
         "scriptName": str,
         "message": str,
         "logTail": str,
     },
     total=False,
 )
 
-TargetGroupInfoTypeDef = TypedDict(
-    "TargetGroupInfoTypeDef",
+TargetGroupInfoOutputTypeDef = TypedDict(
+    "TargetGroupInfoOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
+ELBInfoOutputTypeDef = TypedDict(
+    "ELBInfoOutputTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
 ELBInfoTypeDef = TypedDict(
@@ -645,23 +792,41 @@
 GetOnPremisesInstanceInputRequestTypeDef = TypedDict(
     "GetOnPremisesInstanceInputRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
+GitHubLocationOutputTypeDef = TypedDict(
+    "GitHubLocationOutputTypeDef",
+    {
+        "repository": str,
+        "commitId": str,
+    },
+    total=False,
+)
+
 GitHubLocationTypeDef = TypedDict(
     "GitHubLocationTypeDef",
     {
         "repository": str,
         "commitId": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 LambdaFunctionInfoTypeDef = TypedDict(
     "LambdaFunctionInfoTypeDef",
     {
         "functionName": str,
         "functionAlias": str,
         "currentVersion": str,
         "targetVersion": str,
@@ -983,14 +1148,22 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
+TargetGroupInfoTypeDef = TypedDict(
+    "TargetGroupInfoTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1011,14 +1184,23 @@
     "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     {
         "lifecycleEventHookExecutionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RawStringOutputTypeDef = TypedDict(
+    "RawStringOutputTypeDef",
+    {
+        "content": str,
+        "sha256": str,
+    },
+    total=False,
+)
+
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -1054,14 +1236,26 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+        "bundleType": BundleTypeType,
+        "version": str,
+        "eTag": str,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -1104,31 +1298,57 @@
     {
         "status": StopStatusType,
         "statusMessage": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TrafficRouteOutputTypeDef = TypedDict(
+    "TrafficRouteOutputTypeDef",
+    {
+        "listenerArns": List[str],
+    },
+    total=False,
+)
+
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
-        "listenerArns": List[str],
+        "listenerArns": Sequence[str],
+    },
+    total=False,
+)
+
+TimeBasedCanaryOutputTypeDef = TypedDict(
+    "TimeBasedCanaryOutputTypeDef",
+    {
+        "canaryPercentage": int,
+        "canaryInterval": int,
     },
     total=False,
 )
 
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
         "canaryPercentage": int,
         "canaryInterval": int,
     },
     total=False,
 )
 
+TimeBasedLinearOutputTypeDef = TypedDict(
+    "TimeBasedLinearOutputTypeDef",
+    {
+        "linearPercentage": int,
+        "linearInterval": int,
+    },
+    total=False,
+)
+
 TimeBasedLinearTypeDef = TypedDict(
     "TimeBasedLinearTypeDef",
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
@@ -1177,37 +1397,14 @@
 
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
 
-InstanceInfoTypeDef = TypedDict(
-    "InstanceInfoTypeDef",
-    {
-        "instanceName": str,
-        "iamSessionArn": str,
-        "iamUserArn": str,
-        "instanceArn": str,
-        "registerTime": datetime,
-        "deregisterTime": datetime,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
 )
@@ -1216,20 +1413,30 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AlarmConfigurationOutputTypeDef = TypedDict(
+    "AlarmConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "ignorePollAlarmFailure": bool,
+        "alarms": List[AlarmOutputTypeDef],
+    },
+    total=False,
+)
+
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmTypeDef],
+        "alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
@@ -1258,28 +1465,38 @@
     "UpdateDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BlueGreenDeploymentConfigurationOutputTypeDef = TypedDict(
+    "BlueGreenDeploymentConfigurationOutputTypeDef",
+    {
+        "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionOutputTypeDef,
+        "deploymentReadyOption": DeploymentReadyOptionOutputTypeDef,
+        "greenFleetProvisioningOption": GreenFleetProvisioningOptionOutputTypeDef,
+    },
+    total=False,
+)
+
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
 EC2TagSetTypeDef = TypedDict(
     "EC2TagSetTypeDef",
     {
-        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
+        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     {
@@ -1299,15 +1516,31 @@
     },
     total=False,
 )
 
 OnPremisesTagSetTypeDef = TypedDict(
     "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
+        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
+    },
+    total=False,
+)
+
+EC2TagSetOutputTypeDef = TypedDict(
+    "EC2TagSetOutputTypeDef",
+    {
+        "ec2TagSetList": List[List[EC2TagFilterOutputTypeDef]],
+    },
+    total=False,
+)
+
+OnPremisesTagSetOutputTypeDef = TypedDict(
+    "OnPremisesTagSetOutputTypeDef",
+    {
+        "onPremisesTagSetList": List[List[TagFilterOutputTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1325,15 +1558,15 @@
     {
         "identifer": str,
         "desiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "status": str,
         "trafficWeight": float,
-        "targetGroup": TargetGroupInfoTypeDef,
+        "targetGroup": TargetGroupInfoOutputTypeDef,
         "taskSetLabel": TargetLabelType,
     },
     total=False,
 )
 
 _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef = TypedDict(
     "_RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
@@ -1353,14 +1586,37 @@
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
 
+InstanceInfoTypeDef = TypedDict(
+    "InstanceInfoTypeDef",
+    {
+        "instanceName": str,
+        "iamSessionArn": str,
+        "iamUserArn": str,
+        "instanceArn": str,
+        "registerTime": datetime,
+        "deregisterTime": datetime,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "externalId": str,
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
@@ -1379,68 +1635,94 @@
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
         "nextToken": str,
     },
     total=False,
 )
 
+RevisionLocationOutputTypeDef = TypedDict(
+    "RevisionLocationOutputTypeDef",
+    {
+        "revisionType": RevisionLocationTypeType,
+        "s3Location": S3LocationOutputTypeDef,
+        "gitHubLocation": GitHubLocationOutputTypeDef,
+        "string": RawStringOutputTypeDef,
+        "appSpecContent": AppSpecContentOutputTypeDef,
+    },
+    total=False,
+)
+
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
         "revisionType": RevisionLocationTypeType,
         "s3Location": S3LocationTypeDef,
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
         "appSpecContent": AppSpecContentTypeDef,
     },
     total=False,
 )
 
+TargetGroupPairInfoOutputTypeDef = TypedDict(
+    "TargetGroupPairInfoOutputTypeDef",
+    {
+        "targetGroups": List[TargetGroupInfoOutputTypeDef],
+        "prodTrafficRoute": TrafficRouteOutputTypeDef,
+        "testTrafficRoute": TrafficRouteOutputTypeDef,
+    },
+    total=False,
+)
+
 TargetGroupPairInfoTypeDef = TypedDict(
     "TargetGroupPairInfoTypeDef",
     {
-        "targetGroups": List[TargetGroupInfoTypeDef],
+        "targetGroups": Sequence[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
-TrafficRoutingConfigTypeDef = TypedDict(
-    "TrafficRoutingConfigTypeDef",
+TrafficRoutingConfigOutputTypeDef = TypedDict(
+    "TrafficRoutingConfigOutputTypeDef",
     {
         "type": TrafficRoutingTypeType,
-        "timeBasedCanary": TimeBasedCanaryTypeDef,
-        "timeBasedLinear": TimeBasedLinearTypeDef,
+        "timeBasedCanary": TimeBasedCanaryOutputTypeDef,
+        "timeBasedLinear": TimeBasedLinearOutputTypeDef,
     },
     total=False,
 )
 
-BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
-    "BatchGetOnPremisesInstancesOutputTypeDef",
+TrafficRoutingConfigTypeDef = TypedDict(
+    "TrafficRoutingConfigTypeDef",
     {
-        "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "type": TrafficRoutingTypeType,
+        "timeBasedCanary": TimeBasedCanaryTypeDef,
+        "timeBasedLinear": TimeBasedLinearTypeDef,
     },
+    total=False,
 )
 
-GetOnPremisesInstanceOutputTypeDef = TypedDict(
-    "GetOnPremisesInstanceOutputTypeDef",
+TargetInstancesTypeDef = TypedDict(
+    "TargetInstancesTypeDef",
     {
-        "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tagFilters": Sequence[EC2TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "ec2TagSet": EC2TagSetTypeDef,
     },
+    total=False,
 )
 
-TargetInstancesTypeDef = TypedDict(
-    "TargetInstancesTypeDef",
+TargetInstancesOutputTypeDef = TypedDict(
+    "TargetInstancesOutputTypeDef",
     {
-        "tagFilters": List[EC2TagFilterTypeDef],
+        "tagFilters": List[EC2TagFilterOutputTypeDef],
         "autoScalingGroups": List[str],
-        "ec2TagSet": EC2TagSetTypeDef,
+        "ec2TagSet": EC2TagSetOutputTypeDef,
     },
     total=False,
 )
 
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
@@ -1506,49 +1788,74 @@
         "lifecycleEvents": List[LifecycleEventTypeDef],
         "status": TargetStatusType,
         "taskSetsInfo": List[ECSTaskSetTypeDef],
     },
     total=False,
 )
 
-BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
-    "BatchGetApplicationRevisionsInputRequestTypeDef",
+BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
+    "BatchGetOnPremisesInstancesOutputTypeDef",
     {
-        "applicationName": str,
-        "revisions": Sequence[RevisionLocationTypeDef],
+        "instanceInfos": List[InstanceInfoTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApplicationRevisionInputRequestTypeDef = TypedDict(
-    "GetApplicationRevisionInputRequestTypeDef",
+GetOnPremisesInstanceOutputTypeDef = TypedDict(
+    "GetOnPremisesInstanceOutputTypeDef",
     {
-        "applicationName": str,
-        "revision": RevisionLocationTypeDef,
+        "instanceInfo": InstanceInfoTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
-        "revision": RevisionLocationTypeDef,
+        "revision": RevisionLocationOutputTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
-        "revisions": List[RevisionLocationTypeDef],
+        "revisions": List[RevisionLocationOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RevisionInfoTypeDef = TypedDict(
+    "RevisionInfoTypeDef",
+    {
+        "revisionLocation": RevisionLocationOutputTypeDef,
+        "genericRevisionInfo": GenericRevisionInfoTypeDef,
+    },
+    total=False,
+)
+
+BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
+    "BatchGetApplicationRevisionsInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "revisions": Sequence[RevisionLocationTypeDef],
+    },
+)
+
+GetApplicationRevisionInputRequestTypeDef = TypedDict(
+    "GetApplicationRevisionInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "revision": RevisionLocationTypeDef,
+    },
+)
+
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
         "revision": RevisionLocationTypeDef,
     },
 )
@@ -1564,29 +1871,43 @@
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
 
-RevisionInfoTypeDef = TypedDict(
-    "RevisionInfoTypeDef",
+LoadBalancerInfoOutputTypeDef = TypedDict(
+    "LoadBalancerInfoOutputTypeDef",
     {
-        "revisionLocation": RevisionLocationTypeDef,
-        "genericRevisionInfo": GenericRevisionInfoTypeDef,
+        "elbInfoList": List[ELBInfoOutputTypeDef],
+        "targetGroupInfoList": List[TargetGroupInfoOutputTypeDef],
+        "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
     },
     total=False,
 )
 
 LoadBalancerInfoTypeDef = TypedDict(
     "LoadBalancerInfoTypeDef",
     {
-        "elbInfoList": List[ELBInfoTypeDef],
-        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": List[TargetGroupPairInfoTypeDef],
+        "elbInfoList": Sequence[ELBInfoTypeDef],
+        "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
+        "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
+    },
+    total=False,
+)
+
+DeploymentConfigInfoTypeDef = TypedDict(
+    "DeploymentConfigInfoTypeDef",
+    {
+        "deploymentConfigId": str,
+        "deploymentConfigName": str,
+        "minimumHealthyHosts": MinimumHealthyHostsOutputTypeDef,
+        "createTime": datetime,
+        "computePlatform": ComputePlatformType,
+        "trafficRoutingConfig": TrafficRoutingConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
@@ -1607,27 +1928,14 @@
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
 
-DeploymentConfigInfoTypeDef = TypedDict(
-    "DeploymentConfigInfoTypeDef",
-    {
-        "deploymentConfigId": str,
-        "deploymentConfigName": str,
-        "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
-        "createTime": datetime,
-        "computePlatform": ComputePlatformType,
-        "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalCreateDeploymentInputRequestTypeDef = TypedDict(
@@ -1689,118 +1997,118 @@
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "serviceRoleArn": str,
-    },
-)
-_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "deploymentConfigName": str,
-        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "ecsServices": Sequence[ECSServiceTypeDef],
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateDeploymentGroupInputRequestTypeDef(
-    _RequiredCreateDeploymentGroupInputRequestTypeDef,
-    _OptionalCreateDeploymentGroupInputRequestTypeDef,
-):
-    pass
-
-
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
-        "ec2TagFilters": List[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
+        "ec2TagFilters": List[EC2TagFilterOutputTypeDef],
+        "onPremisesInstanceTagFilters": List[TagFilterOutputTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
-        "targetRevision": RevisionLocationTypeDef,
-        "triggerConfigurations": List[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "deploymentStyle": DeploymentStyleTypeDef,
+        "targetRevision": RevisionLocationOutputTypeDef,
+        "triggerConfigurations": List[TriggerConfigOutputTypeDef],
+        "alarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
+        "deploymentStyle": DeploymentStyleOutputTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "ec2TagSet": EC2TagSetOutputTypeDef,
+        "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
         "computePlatform": ComputePlatformType,
-        "ecsServices": List[ECSServiceTypeDef],
+        "ecsServices": List[ECSServiceOutputTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
     "DeploymentInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "deploymentId": str,
-        "previousRevision": RevisionLocationTypeDef,
-        "revision": RevisionLocationTypeDef,
+        "previousRevision": RevisionLocationOutputTypeDef,
+        "revision": RevisionLocationOutputTypeDef,
         "status": DeploymentStatusType,
         "errorInformation": ErrorInformationTypeDef,
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "targetInstances": TargetInstancesTypeDef,
+        "deploymentStyle": DeploymentStyleOutputTypeDef,
+        "targetInstances": TargetInstancesOutputTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
-        "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
+        "overrideAlarmConfiguration": AlarmConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "serviceRoleArn": str,
+    },
+)
+_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "deploymentConfigName": str,
+        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
+        "deploymentStyle": DeploymentStyleTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "ecsServices": Sequence[ECSServiceTypeDef],
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
+class CreateDeploymentGroupInputRequestTypeDef(
+    _RequiredCreateDeploymentGroupInputRequestTypeDef,
+    _OptionalCreateDeploymentGroupInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/type_defs.pyi` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -54,25 +54,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
+    "AlarmOutputTypeDef",
     "AlarmTypeDef",
+    "AppSpecContentOutputTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
+    "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
+    "BlueInstanceTerminationOptionOutputTypeDef",
+    "DeploymentReadyOptionOutputTypeDef",
+    "GreenFleetProvisioningOptionOutputTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
     "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
     "CreateDeploymentConfigOutputTypeDef",
@@ -85,34 +91,43 @@
     "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
+    "MinimumHealthyHostsOutputTypeDef",
+    "DeploymentStyleOutputTypeDef",
+    "EC2TagFilterOutputTypeDef",
+    "ECSServiceOutputTypeDef",
     "LastDeploymentInfoTypeDef",
+    "TagFilterOutputTypeDef",
+    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
-    "TargetGroupInfoTypeDef",
+    "TargetGroupInfoOutputTypeDef",
+    "ELBInfoOutputTypeDef",
     "ELBInfoTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
+    "GitHubLocationOutputTypeDef",
     "GitHubLocationTypeDef",
+    "TagOutputTypeDef",
     "LambdaFunctionInfoTypeDef",
     "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
     "ListApplicationsOutputTypeDef",
     "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
@@ -130,78 +145,93 @@
     "TimeRangeTypeDef",
     "ListDeploymentsOutputTypeDef",
     "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     "ListGitHubAccountTokenNamesOutputTypeDef",
     "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TargetGroupInfoTypeDef",
     "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    "RawStringOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
     "StopDeploymentOutputTypeDef",
+    "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
+    "TimeBasedCanaryOutputTypeDef",
     "TimeBasedCanaryTypeDef",
+    "TimeBasedLinearOutputTypeDef",
     "TimeBasedLinearTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
-    "InstanceInfoTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
     "BatchGetApplicationsOutputTypeDef",
     "GetApplicationOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
+    "BlueGreenDeploymentConfigurationOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
     "EC2TagSetTypeDef",
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
     "OnPremisesTagSetTypeDef",
+    "EC2TagSetOutputTypeDef",
+    "OnPremisesTagSetOutputTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
+    "InstanceInfoTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
+    "RevisionLocationOutputTypeDef",
     "RevisionLocationTypeDef",
+    "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
+    "TrafficRoutingConfigOutputTypeDef",
     "TrafficRoutingConfigTypeDef",
-    "BatchGetOnPremisesInstancesOutputTypeDef",
-    "GetOnPremisesInstanceOutputTypeDef",
     "TargetInstancesTypeDef",
+    "TargetInstancesOutputTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
-    "BatchGetApplicationRevisionsInputRequestTypeDef",
-    "GetApplicationRevisionInputRequestTypeDef",
+    "BatchGetOnPremisesInstancesOutputTypeDef",
+    "GetOnPremisesInstanceOutputTypeDef",
     "GetApplicationRevisionOutputTypeDef",
     "ListApplicationRevisionsOutputTypeDef",
-    "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
+    "BatchGetApplicationRevisionsInputRequestTypeDef",
+    "GetApplicationRevisionInputRequestTypeDef",
+    "RegisterApplicationRevisionInputRequestTypeDef",
+    "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
-    "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
+    "CreateDeploymentConfigInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
-    "CreateDeploymentGroupInputRequestTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
+    "CreateDeploymentGroupInputRequestTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -213,22 +243,39 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+AlarmOutputTypeDef = TypedDict(
+    "AlarmOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
+AppSpecContentOutputTypeDef = TypedDict(
+    "AppSpecContentOutputTypeDef",
+    {
+        "content": str,
+        "sha256": str,
+    },
+    total=False,
+)
+
 AppSpecContentTypeDef = TypedDict(
     "AppSpecContentTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -243,19 +290,28 @@
         "linkedToGitHub": bool,
         "gitHubAccountName": str,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
+AutoRollbackConfigurationOutputTypeDef = TypedDict(
+    "AutoRollbackConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "events": List[AutoRollbackEventType],
+    },
+    total=False,
+)
+
 AutoRollbackConfigurationTypeDef = TypedDict(
     "AutoRollbackConfigurationTypeDef",
     {
         "enabled": bool,
-        "events": List[AutoRollbackEventType],
+        "events": Sequence[AutoRollbackEventType],
     },
     total=False,
 )
 
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
@@ -307,14 +363,40 @@
 BatchGetOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     {
         "instanceNames": Sequence[str],
     },
 )
 
+BlueInstanceTerminationOptionOutputTypeDef = TypedDict(
+    "BlueInstanceTerminationOptionOutputTypeDef",
+    {
+        "action": InstanceActionType,
+        "terminationWaitTimeInMinutes": int,
+    },
+    total=False,
+)
+
+DeploymentReadyOptionOutputTypeDef = TypedDict(
+    "DeploymentReadyOptionOutputTypeDef",
+    {
+        "actionOnTimeout": DeploymentReadyActionType,
+        "waitTimeInMinutes": int,
+    },
+    total=False,
+)
+
+GreenFleetProvisioningOptionOutputTypeDef = TypedDict(
+    "GreenFleetProvisioningOptionOutputTypeDef",
+    {
+        "action": GreenFleetProvisioningActionType,
+    },
+    total=False,
+)
+
 BlueInstanceTerminationOptionTypeDef = TypedDict(
     "BlueInstanceTerminationOptionTypeDef",
     {
         "action": InstanceActionType,
         "terminationWaitTimeInMinutes": int,
     },
     total=False,
@@ -410,15 +492,15 @@
 )
 
 TriggerConfigTypeDef = TypedDict(
     "TriggerConfigTypeDef",
     {
         "triggerName": str,
         "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
+        "triggerEvents": Sequence[TriggerEventTypeType],
     },
     total=False,
 )
 
 CreateDeploymentGroupOutputTypeDef = TypedDict(
     "CreateDeploymentGroupOutputTypeDef",
     {
@@ -477,25 +559,82 @@
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
+MinimumHealthyHostsOutputTypeDef = TypedDict(
+    "MinimumHealthyHostsOutputTypeDef",
+    {
+        "type": MinimumHealthyHostsTypeType,
+        "value": int,
+    },
+    total=False,
+)
+
+DeploymentStyleOutputTypeDef = TypedDict(
+    "DeploymentStyleOutputTypeDef",
+    {
+        "deploymentType": DeploymentTypeType,
+        "deploymentOption": DeploymentOptionType,
+    },
+    total=False,
+)
+
+EC2TagFilterOutputTypeDef = TypedDict(
+    "EC2TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "Type": EC2TagFilterTypeType,
+    },
+    total=False,
+)
+
+ECSServiceOutputTypeDef = TypedDict(
+    "ECSServiceOutputTypeDef",
+    {
+        "serviceName": str,
+        "clusterName": str,
+    },
+    total=False,
+)
+
 LastDeploymentInfoTypeDef = TypedDict(
     "LastDeploymentInfoTypeDef",
     {
         "deploymentId": str,
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
+TagFilterOutputTypeDef = TypedDict(
+    "TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "Type": TagFilterTypeType,
+    },
+    total=False,
+)
+
+TriggerConfigOutputTypeDef = TypedDict(
+    "TriggerConfigOutputTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -547,16 +686,24 @@
         "scriptName": str,
         "message": str,
         "logTail": str,
     },
     total=False,
 )
 
-TargetGroupInfoTypeDef = TypedDict(
-    "TargetGroupInfoTypeDef",
+TargetGroupInfoOutputTypeDef = TypedDict(
+    "TargetGroupInfoOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
+ELBInfoOutputTypeDef = TypedDict(
+    "ELBInfoOutputTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
 ELBInfoTypeDef = TypedDict(
@@ -644,23 +791,41 @@
 GetOnPremisesInstanceInputRequestTypeDef = TypedDict(
     "GetOnPremisesInstanceInputRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
+GitHubLocationOutputTypeDef = TypedDict(
+    "GitHubLocationOutputTypeDef",
+    {
+        "repository": str,
+        "commitId": str,
+    },
+    total=False,
+)
+
 GitHubLocationTypeDef = TypedDict(
     "GitHubLocationTypeDef",
     {
         "repository": str,
         "commitId": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 LambdaFunctionInfoTypeDef = TypedDict(
     "LambdaFunctionInfoTypeDef",
     {
         "functionName": str,
         "functionAlias": str,
         "currentVersion": str,
         "targetVersion": str,
@@ -968,14 +1133,22 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+TargetGroupInfoTypeDef = TypedDict(
+    "TargetGroupInfoTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -996,14 +1169,23 @@
     "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     {
         "lifecycleEventHookExecutionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RawStringOutputTypeDef = TypedDict(
+    "RawStringOutputTypeDef",
+    {
+        "content": str,
+        "sha256": str,
+    },
+    total=False,
+)
+
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -1037,14 +1219,26 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+        "bundleType": BundleTypeType,
+        "version": str,
+        "eTag": str,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -1085,31 +1279,57 @@
     {
         "status": StopStatusType,
         "statusMessage": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TrafficRouteOutputTypeDef = TypedDict(
+    "TrafficRouteOutputTypeDef",
+    {
+        "listenerArns": List[str],
+    },
+    total=False,
+)
+
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
-        "listenerArns": List[str],
+        "listenerArns": Sequence[str],
+    },
+    total=False,
+)
+
+TimeBasedCanaryOutputTypeDef = TypedDict(
+    "TimeBasedCanaryOutputTypeDef",
+    {
+        "canaryPercentage": int,
+        "canaryInterval": int,
     },
     total=False,
 )
 
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
         "canaryPercentage": int,
         "canaryInterval": int,
     },
     total=False,
 )
 
+TimeBasedLinearOutputTypeDef = TypedDict(
+    "TimeBasedLinearOutputTypeDef",
+    {
+        "linearPercentage": int,
+        "linearInterval": int,
+    },
+    total=False,
+)
+
 TimeBasedLinearTypeDef = TypedDict(
     "TimeBasedLinearTypeDef",
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
@@ -1156,37 +1376,14 @@
 )
 
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
-InstanceInfoTypeDef = TypedDict(
-    "InstanceInfoTypeDef",
-    {
-        "instanceName": str,
-        "iamSessionArn": str,
-        "iamUserArn": str,
-        "instanceArn": str,
-        "registerTime": datetime,
-        "deregisterTime": datetime,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
 )
@@ -1195,20 +1392,30 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AlarmConfigurationOutputTypeDef = TypedDict(
+    "AlarmConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "ignorePollAlarmFailure": bool,
+        "alarms": List[AlarmOutputTypeDef],
+    },
+    total=False,
+)
+
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmTypeDef],
+        "alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
@@ -1237,28 +1444,38 @@
     "UpdateDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BlueGreenDeploymentConfigurationOutputTypeDef = TypedDict(
+    "BlueGreenDeploymentConfigurationOutputTypeDef",
+    {
+        "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionOutputTypeDef,
+        "deploymentReadyOption": DeploymentReadyOptionOutputTypeDef,
+        "greenFleetProvisioningOption": GreenFleetProvisioningOptionOutputTypeDef,
+    },
+    total=False,
+)
+
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
 EC2TagSetTypeDef = TypedDict(
     "EC2TagSetTypeDef",
     {
-        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
+        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     {
@@ -1278,15 +1495,31 @@
     },
     total=False,
 )
 
 OnPremisesTagSetTypeDef = TypedDict(
     "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
+        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
+    },
+    total=False,
+)
+
+EC2TagSetOutputTypeDef = TypedDict(
+    "EC2TagSetOutputTypeDef",
+    {
+        "ec2TagSetList": List[List[EC2TagFilterOutputTypeDef]],
+    },
+    total=False,
+)
+
+OnPremisesTagSetOutputTypeDef = TypedDict(
+    "OnPremisesTagSetOutputTypeDef",
+    {
+        "onPremisesTagSetList": List[List[TagFilterOutputTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1304,15 +1537,15 @@
     {
         "identifer": str,
         "desiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "status": str,
         "trafficWeight": float,
-        "targetGroup": TargetGroupInfoTypeDef,
+        "targetGroup": TargetGroupInfoOutputTypeDef,
         "taskSetLabel": TargetLabelType,
     },
     total=False,
 )
 
 _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef = TypedDict(
     "_RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
@@ -1330,14 +1563,37 @@
 
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
+InstanceInfoTypeDef = TypedDict(
+    "InstanceInfoTypeDef",
+    {
+        "instanceName": str,
+        "iamSessionArn": str,
+        "iamUserArn": str,
+        "instanceArn": str,
+        "registerTime": datetime,
+        "deregisterTime": datetime,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "externalId": str,
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
@@ -1356,68 +1612,94 @@
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
         "nextToken": str,
     },
     total=False,
 )
 
+RevisionLocationOutputTypeDef = TypedDict(
+    "RevisionLocationOutputTypeDef",
+    {
+        "revisionType": RevisionLocationTypeType,
+        "s3Location": S3LocationOutputTypeDef,
+        "gitHubLocation": GitHubLocationOutputTypeDef,
+        "string": RawStringOutputTypeDef,
+        "appSpecContent": AppSpecContentOutputTypeDef,
+    },
+    total=False,
+)
+
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
         "revisionType": RevisionLocationTypeType,
         "s3Location": S3LocationTypeDef,
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
         "appSpecContent": AppSpecContentTypeDef,
     },
     total=False,
 )
 
+TargetGroupPairInfoOutputTypeDef = TypedDict(
+    "TargetGroupPairInfoOutputTypeDef",
+    {
+        "targetGroups": List[TargetGroupInfoOutputTypeDef],
+        "prodTrafficRoute": TrafficRouteOutputTypeDef,
+        "testTrafficRoute": TrafficRouteOutputTypeDef,
+    },
+    total=False,
+)
+
 TargetGroupPairInfoTypeDef = TypedDict(
     "TargetGroupPairInfoTypeDef",
     {
-        "targetGroups": List[TargetGroupInfoTypeDef],
+        "targetGroups": Sequence[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
-TrafficRoutingConfigTypeDef = TypedDict(
-    "TrafficRoutingConfigTypeDef",
+TrafficRoutingConfigOutputTypeDef = TypedDict(
+    "TrafficRoutingConfigOutputTypeDef",
     {
         "type": TrafficRoutingTypeType,
-        "timeBasedCanary": TimeBasedCanaryTypeDef,
-        "timeBasedLinear": TimeBasedLinearTypeDef,
+        "timeBasedCanary": TimeBasedCanaryOutputTypeDef,
+        "timeBasedLinear": TimeBasedLinearOutputTypeDef,
     },
     total=False,
 )
 
-BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
-    "BatchGetOnPremisesInstancesOutputTypeDef",
+TrafficRoutingConfigTypeDef = TypedDict(
+    "TrafficRoutingConfigTypeDef",
     {
-        "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "type": TrafficRoutingTypeType,
+        "timeBasedCanary": TimeBasedCanaryTypeDef,
+        "timeBasedLinear": TimeBasedLinearTypeDef,
     },
+    total=False,
 )
 
-GetOnPremisesInstanceOutputTypeDef = TypedDict(
-    "GetOnPremisesInstanceOutputTypeDef",
+TargetInstancesTypeDef = TypedDict(
+    "TargetInstancesTypeDef",
     {
-        "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tagFilters": Sequence[EC2TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "ec2TagSet": EC2TagSetTypeDef,
     },
+    total=False,
 )
 
-TargetInstancesTypeDef = TypedDict(
-    "TargetInstancesTypeDef",
+TargetInstancesOutputTypeDef = TypedDict(
+    "TargetInstancesOutputTypeDef",
     {
-        "tagFilters": List[EC2TagFilterTypeDef],
+        "tagFilters": List[EC2TagFilterOutputTypeDef],
         "autoScalingGroups": List[str],
-        "ec2TagSet": EC2TagSetTypeDef,
+        "ec2TagSet": EC2TagSetOutputTypeDef,
     },
     total=False,
 )
 
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
@@ -1483,49 +1765,74 @@
         "lifecycleEvents": List[LifecycleEventTypeDef],
         "status": TargetStatusType,
         "taskSetsInfo": List[ECSTaskSetTypeDef],
     },
     total=False,
 )
 
-BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
-    "BatchGetApplicationRevisionsInputRequestTypeDef",
+BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
+    "BatchGetOnPremisesInstancesOutputTypeDef",
     {
-        "applicationName": str,
-        "revisions": Sequence[RevisionLocationTypeDef],
+        "instanceInfos": List[InstanceInfoTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApplicationRevisionInputRequestTypeDef = TypedDict(
-    "GetApplicationRevisionInputRequestTypeDef",
+GetOnPremisesInstanceOutputTypeDef = TypedDict(
+    "GetOnPremisesInstanceOutputTypeDef",
     {
-        "applicationName": str,
-        "revision": RevisionLocationTypeDef,
+        "instanceInfo": InstanceInfoTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
-        "revision": RevisionLocationTypeDef,
+        "revision": RevisionLocationOutputTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
-        "revisions": List[RevisionLocationTypeDef],
+        "revisions": List[RevisionLocationOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RevisionInfoTypeDef = TypedDict(
+    "RevisionInfoTypeDef",
+    {
+        "revisionLocation": RevisionLocationOutputTypeDef,
+        "genericRevisionInfo": GenericRevisionInfoTypeDef,
+    },
+    total=False,
+)
+
+BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
+    "BatchGetApplicationRevisionsInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "revisions": Sequence[RevisionLocationTypeDef],
+    },
+)
+
+GetApplicationRevisionInputRequestTypeDef = TypedDict(
+    "GetApplicationRevisionInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "revision": RevisionLocationTypeDef,
+    },
+)
+
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
         "revision": RevisionLocationTypeDef,
     },
 )
@@ -1539,29 +1846,43 @@
 
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
-RevisionInfoTypeDef = TypedDict(
-    "RevisionInfoTypeDef",
+LoadBalancerInfoOutputTypeDef = TypedDict(
+    "LoadBalancerInfoOutputTypeDef",
     {
-        "revisionLocation": RevisionLocationTypeDef,
-        "genericRevisionInfo": GenericRevisionInfoTypeDef,
+        "elbInfoList": List[ELBInfoOutputTypeDef],
+        "targetGroupInfoList": List[TargetGroupInfoOutputTypeDef],
+        "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
     },
     total=False,
 )
 
 LoadBalancerInfoTypeDef = TypedDict(
     "LoadBalancerInfoTypeDef",
     {
-        "elbInfoList": List[ELBInfoTypeDef],
-        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": List[TargetGroupPairInfoTypeDef],
+        "elbInfoList": Sequence[ELBInfoTypeDef],
+        "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
+        "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
+    },
+    total=False,
+)
+
+DeploymentConfigInfoTypeDef = TypedDict(
+    "DeploymentConfigInfoTypeDef",
+    {
+        "deploymentConfigId": str,
+        "deploymentConfigName": str,
+        "minimumHealthyHosts": MinimumHealthyHostsOutputTypeDef,
+        "createTime": datetime,
+        "computePlatform": ComputePlatformType,
+        "trafficRoutingConfig": TrafficRoutingConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
@@ -1580,27 +1901,14 @@
 
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
-DeploymentConfigInfoTypeDef = TypedDict(
-    "DeploymentConfigInfoTypeDef",
-    {
-        "deploymentConfigId": str,
-        "deploymentConfigName": str,
-        "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
-        "createTime": datetime,
-        "computePlatform": ComputePlatformType,
-        "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalCreateDeploymentInputRequestTypeDef = TypedDict(
@@ -1660,116 +1968,116 @@
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "serviceRoleArn": str,
-    },
-)
-_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "deploymentConfigName": str,
-        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "ecsServices": Sequence[ECSServiceTypeDef],
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateDeploymentGroupInputRequestTypeDef(
-    _RequiredCreateDeploymentGroupInputRequestTypeDef,
-    _OptionalCreateDeploymentGroupInputRequestTypeDef,
-):
-    pass
-
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
-        "ec2TagFilters": List[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
+        "ec2TagFilters": List[EC2TagFilterOutputTypeDef],
+        "onPremisesInstanceTagFilters": List[TagFilterOutputTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
-        "targetRevision": RevisionLocationTypeDef,
-        "triggerConfigurations": List[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "deploymentStyle": DeploymentStyleTypeDef,
+        "targetRevision": RevisionLocationOutputTypeDef,
+        "triggerConfigurations": List[TriggerConfigOutputTypeDef],
+        "alarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
+        "deploymentStyle": DeploymentStyleOutputTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "ec2TagSet": EC2TagSetOutputTypeDef,
+        "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
         "computePlatform": ComputePlatformType,
-        "ecsServices": List[ECSServiceTypeDef],
+        "ecsServices": List[ECSServiceOutputTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
     "DeploymentInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "deploymentId": str,
-        "previousRevision": RevisionLocationTypeDef,
-        "revision": RevisionLocationTypeDef,
+        "previousRevision": RevisionLocationOutputTypeDef,
+        "revision": RevisionLocationOutputTypeDef,
         "status": DeploymentStatusType,
         "errorInformation": ErrorInformationTypeDef,
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "targetInstances": TargetInstancesTypeDef,
+        "deploymentStyle": DeploymentStyleOutputTypeDef,
+        "targetInstances": TargetInstancesOutputTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
-        "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
+        "overrideAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "serviceRoleArn": str,
+    },
+)
+_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "deploymentConfigName": str,
+        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
+        "deploymentStyle": DeploymentStyleTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "ecsServices": Sequence[ECSServiceTypeDef],
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDeploymentGroupInputRequestTypeDef(
+    _RequiredCreateDeploymentGroupInputRequestTypeDef,
+    _OptionalCreateDeploymentGroupInputRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/waiter.py` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy/waiter.pyi` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/PKG-INFO` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeDeploy 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeDeploy 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codedeploy"></a>
 
 # mypy-boto3-codedeploy
 
 [![PyPI - mypy-boto3-codedeploy](https://img.shields.io/pypi/v/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codedeploy?color=blue)](https://pypistats.org/packages/mypy-boto3-codedeploy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,25 +417,31 @@
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
+    AlarmOutputTypeDef,
     AlarmTypeDef,
+    AppSpecContentOutputTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
+    AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
+    BlueInstanceTerminationOptionOutputTypeDef,
+    DeploymentReadyOptionOutputTypeDef,
+    GreenFleetProvisioningOptionOutputTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
     CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
     CreateDeploymentConfigOutputTypeDef,
@@ -448,34 +454,43 @@
     CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
+    MinimumHealthyHostsOutputTypeDef,
+    DeploymentStyleOutputTypeDef,
+    EC2TagFilterOutputTypeDef,
+    ECSServiceOutputTypeDef,
     LastDeploymentInfoTypeDef,
+    TagFilterOutputTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
-    TargetGroupInfoTypeDef,
+    TargetGroupInfoOutputTypeDef,
+    ELBInfoOutputTypeDef,
     ELBInfoTypeDef,
     EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
+    GitHubLocationOutputTypeDef,
     GitHubLocationTypeDef,
+    TagOutputTypeDef,
     LambdaFunctionInfoTypeDef,
     ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
     ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
     ListApplicationsOutputTypeDef,
     ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
@@ -493,78 +508,93 @@
     TimeRangeTypeDef,
     ListDeploymentsOutputTypeDef,
     ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TargetGroupInfoTypeDef,
     PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    RawStringOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
     StopDeploymentOutputTypeDef,
+    TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
+    TimeBasedCanaryOutputTypeDef,
     TimeBasedCanaryTypeDef,
+    TimeBasedLinearOutputTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
-    InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
     GetApplicationOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
+    BlueGreenDeploymentConfigurationOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
     EC2TagSetTypeDef,
     ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
     OnPremisesTagSetTypeDef,
+    EC2TagSetOutputTypeDef,
+    OnPremisesTagSetOutputTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
+    InstanceInfoTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
+    RevisionLocationOutputTypeDef,
     RevisionLocationTypeDef,
+    TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
+    TrafficRoutingConfigOutputTypeDef,
     TrafficRoutingConfigTypeDef,
-    BatchGetOnPremisesInstancesOutputTypeDef,
-    GetOnPremisesInstanceOutputTypeDef,
     TargetInstancesTypeDef,
+    TargetInstancesOutputTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
-    BatchGetApplicationRevisionsInputRequestTypeDef,
-    GetApplicationRevisionInputRequestTypeDef,
+    BatchGetOnPremisesInstancesOutputTypeDef,
+    GetOnPremisesInstanceOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     ListApplicationRevisionsOutputTypeDef,
-    RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
+    BatchGetApplicationRevisionsInputRequestTypeDef,
+    GetApplicationRevisionInputRequestTypeDef,
+    RegisterApplicationRevisionInputRequestTypeDef,
+    LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
-    CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    CreateDeploymentConfigInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
-    CreateDeploymentGroupInputRequestTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
+    CreateDeploymentGroupInputRequestTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
```

### Comparing `mypy-boto3-codedeploy-1.28.0/mypy_boto3_codedeploy.egg-info/SOURCES.txt` & `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.0/setup.py` & `mypy-boto3-codedeploy-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codedeploy",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeDeploy 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CodeDeploy 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

