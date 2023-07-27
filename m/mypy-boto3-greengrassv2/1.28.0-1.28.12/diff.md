# Comparing `tmp/mypy-boto3-greengrassv2-1.28.0.tar.gz` & `tmp/mypy-boto3-greengrassv2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrassv2-1.28.0.tar", last modified: Thu Jul  6 20:59:40 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrassv2-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
```

## Comparing `mypy-boto3-greengrassv2-1.28.0.tar` & `mypy-boto3-greengrassv2-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.686314 mypy-boto3-greengrassv2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-07-06 20:59:40.678314 mypy-boto3-greengrassv2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.674314 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-07-06 20:42:21.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-07-06 20:42:21.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-06 20:42:21.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-06 20:42:21.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-06 20:42:21.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-06 20:42:21.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37210 2023-07-06 20:42:22.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-07-06 20:42:22.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.678314 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-07-06 20:59:40.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:40.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:40.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:40.000000 mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:40.686314 mypy-boto3-greengrassv2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:42:20.000000 mypy-boto3-greengrassv2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41680 2023-07-27 05:23:09.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41647 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/setup.py
```

### Comparing `mypy-boto3-greengrassv2-1.28.0/LICENSE` & `mypy-boto3-greengrassv2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/PKG-INFO` & `mypy-boto3-greengrassv2-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.28.0
-Summary: Type annotations for boto3.GreengrassV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GreengrassV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrassv2?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrassv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,27 +377,34 @@
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
     CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
+    ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
+    ComponentPlatformOutputTypeDef,
     ComponentPlatformTypeDef,
+    SystemResourceLimitsOutputTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
     CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
+    DeploymentComponentUpdatePolicyOutputTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
+    DeploymentConfigurationValidationPolicyOutputTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
+    IoTJobTimeoutConfigOutputTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
@@ -406,15 +413,17 @@
     GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
     GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
+    IoTJobAbortCriteriaOutputTypeDef,
     IoTJobAbortCriteriaTypeDef,
+    IoTJobRateIncreaseCriteriaOutputTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
@@ -442,37 +451,44 @@
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
+    ComponentRunWithOutputTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
+    DeploymentPoliciesOutputTypeDef,
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
+    IoTJobAbortConfigOutputTypeDef,
     IoTJobAbortConfigTypeDef,
+    IoTJobExponentialRolloutRateOutputTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
+    ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
+    IoTJobExecutionsRolloutConfigOutputTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
+    DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
-    CreateDeploymentRequestRequestTypeDef,
     GetDeploymentResponseTypeDef,
+    CreateDeploymentRequestRequestTypeDef,
     LambdaFunctionRecipeSourceTypeDef,
     CreateComponentVersionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-greengrassv2-1.28.0/README.md` & `mypy-boto3-greengrassv2-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrassv2?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrassv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,27 +345,34 @@
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
     CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
+    ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
+    ComponentPlatformOutputTypeDef,
     ComponentPlatformTypeDef,
+    SystemResourceLimitsOutputTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
     CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
+    DeploymentComponentUpdatePolicyOutputTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
+    DeploymentConfigurationValidationPolicyOutputTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
+    IoTJobTimeoutConfigOutputTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
@@ -374,15 +381,17 @@
     GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
     GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
+    IoTJobAbortCriteriaOutputTypeDef,
     IoTJobAbortCriteriaTypeDef,
+    IoTJobRateIncreaseCriteriaOutputTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
@@ -410,37 +419,44 @@
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
+    ComponentRunWithOutputTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
+    DeploymentPoliciesOutputTypeDef,
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
+    IoTJobAbortConfigOutputTypeDef,
     IoTJobAbortConfigTypeDef,
+    IoTJobExponentialRolloutRateOutputTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
+    ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
+    IoTJobExecutionsRolloutConfigOutputTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
+    DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
-    CreateDeploymentRequestRequestTypeDef,
     GetDeploymentResponseTypeDef,
+    CreateDeploymentRequestRequestTypeDef,
     LambdaFunctionRecipeSourceTypeDef,
     CreateComponentVersionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/__init__.py` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/__init__.pyi` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/__main__.py` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GreengrassV2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.GreengrassV2 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
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

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/client.py` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/client.pyi` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/literals.py` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CloudComponentStateType",
     "ComponentDependencyTypeType",
     "ComponentVisibilityScopeType",
     "CoreDeviceStatusType",
     "DeploymentComponentUpdatePolicyActionType",
     "DeploymentFailureHandlingPolicyType",
@@ -49,15 +48,14 @@
     "GreengrassV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CloudComponentStateType = Literal["DEPLOYABLE", "DEPRECATED", "FAILED", "INITIATED", "REQUESTED"]
 ComponentDependencyTypeType = Literal["HARD", "SOFT"]
 ComponentVisibilityScopeType = Literal["PRIVATE", "PUBLIC"]
 CoreDeviceStatusType = Literal["HEALTHY", "UNHEALTHY"]
 DeploymentComponentUpdatePolicyActionType = Literal["NOTIFY_COMPONENTS", "SKIP_NOTIFY_COMPONENTS"]
 DeploymentFailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK"]
 DeploymentHistoryFilterType = Literal["ALL", "LATEST_ONLY"]
@@ -202,14 +200,15 @@
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
@@ -288,26 +287,28 @@
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

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/literals.pyi` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.py`

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
     "CloudComponentStateType",
     "ComponentDependencyTypeType",
     "ComponentVisibilityScopeType",
     "CoreDeviceStatusType",
     "DeploymentComponentUpdatePolicyActionType",
     "DeploymentFailureHandlingPolicyType",
@@ -48,14 +49,15 @@
     "GreengrassV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CloudComponentStateType = Literal["DEPLOYABLE", "DEPRECATED", "FAILED", "INITIATED", "REQUESTED"]
 ComponentDependencyTypeType = Literal["HARD", "SOFT"]
 ComponentVisibilityScopeType = Literal["PRIVATE", "PUBLIC"]
 CoreDeviceStatusType = Literal["HEALTHY", "UNHEALTHY"]
 DeploymentComponentUpdatePolicyActionType = Literal["NOTIFY_COMPONENTS", "SKIP_NOTIFY_COMPONENTS"]
 DeploymentFailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK"]
 DeploymentHistoryFilterType = Literal["ALL", "LATEST_ONLY"]
@@ -200,14 +202,15 @@
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
@@ -286,26 +289,28 @@
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

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/paginator.py` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/paginator.pyi` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/type_defs.py` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -43,40 +43,46 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "AssociateServiceRoleToAccountResponseTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CancelDeploymentResponseTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
+    "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
+    "ComponentPlatformOutputTypeDef",
     "ComponentPlatformTypeDef",
+    "SystemResourceLimitsOutputTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
+    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
     "CreateDeploymentResponseTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
+    "DeploymentComponentUpdatePolicyOutputTypeDef",
     "DeploymentComponentUpdatePolicyTypeDef",
+    "DeploymentConfigurationValidationPolicyOutputTypeDef",
     "DeploymentConfigurationValidationPolicyTypeDef",
+    "IoTJobTimeoutConfigOutputTypeDef",
     "IoTJobTimeoutConfigTypeDef",
     "DeploymentTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EffectiveDeploymentStatusDetailsTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetComponentRequestRequestTypeDef",
@@ -85,15 +91,17 @@
     "GetComponentVersionArtifactResponseTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetCoreDeviceRequestRequestTypeDef",
     "GetCoreDeviceResponseTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetServiceRoleForAccountResponseTypeDef",
     "InstalledComponentTypeDef",
+    "IoTJobAbortCriteriaOutputTypeDef",
     "IoTJobAbortCriteriaTypeDef",
+    "IoTJobRateIncreaseCriteriaOutputTypeDef",
     "IoTJobRateIncreaseCriteriaTypeDef",
     "LambdaDeviceMountTypeDef",
     "LambdaVolumeMountTypeDef",
     "LambdaEventSourceTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
@@ -121,37 +129,44 @@
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
+    "ComponentRunWithOutputTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
+    "DeploymentPoliciesOutputTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
+    "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
+    "IoTJobExponentialRolloutRateOutputTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
+    "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
+    "IoTJobExecutionsRolloutConfigOutputTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
+    "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
-    "CreateDeploymentRequestRequestTypeDef",
     "GetDeploymentResponseTypeDef",
+    "CreateDeploymentRequestRequestTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -243,14 +258,23 @@
         "componentName": str,
         "componentVersion": str,
         "versionRequirements": Mapping[str, str],
     },
     total=False,
 )
 
+ComponentConfigurationUpdateOutputTypeDef = TypedDict(
+    "ComponentConfigurationUpdateOutputTypeDef",
+    {
+        "merge": str,
+        "reset": List[str],
+    },
+    total=False,
+)
+
 ComponentConfigurationUpdateTypeDef = TypedDict(
     "ComponentConfigurationUpdateTypeDef",
     {
         "merge": str,
         "reset": Sequence[str],
     },
     total=False,
@@ -261,23 +285,41 @@
     {
         "versionRequirement": str,
         "dependencyType": ComponentDependencyTypeType,
     },
     total=False,
 )
 
+ComponentPlatformOutputTypeDef = TypedDict(
+    "ComponentPlatformOutputTypeDef",
+    {
+        "name": str,
+        "attributes": Dict[str, str],
+    },
+    total=False,
+)
+
 ComponentPlatformTypeDef = TypedDict(
     "ComponentPlatformTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
+SystemResourceLimitsOutputTypeDef = TypedDict(
+    "SystemResourceLimitsOutputTypeDef",
+    {
+        "memory": int,
+        "cpus": float,
+    },
+    total=False,
+)
+
 SystemResourceLimitsTypeDef = TypedDict(
     "SystemResourceLimitsTypeDef",
     {
         "memory": int,
         "cpus": float,
     },
     total=False,
@@ -289,14 +331,25 @@
         "componentName": str,
         "componentVersion": str,
         "arn": str,
     },
     total=False,
 )
 
+ConnectivityInfoOutputTypeDef = TypedDict(
+    "ConnectivityInfoOutputTypeDef",
+    {
+        "id": str,
+        "hostAddress": str,
+        "portNumber": int,
+        "metadata": str,
+    },
+    total=False,
+)
+
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "id": str,
         "hostAddress": str,
         "portNumber": int,
         "metadata": str,
@@ -341,31 +394,56 @@
 DeleteDeploymentRequestRequestTypeDef = TypedDict(
     "DeleteDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
+DeploymentComponentUpdatePolicyOutputTypeDef = TypedDict(
+    "DeploymentComponentUpdatePolicyOutputTypeDef",
+    {
+        "timeoutInSeconds": int,
+        "action": DeploymentComponentUpdatePolicyActionType,
+    },
+    total=False,
+)
+
 DeploymentComponentUpdatePolicyTypeDef = TypedDict(
     "DeploymentComponentUpdatePolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "action": DeploymentComponentUpdatePolicyActionType,
     },
     total=False,
 )
 
+DeploymentConfigurationValidationPolicyOutputTypeDef = TypedDict(
+    "DeploymentConfigurationValidationPolicyOutputTypeDef",
+    {
+        "timeoutInSeconds": int,
+    },
+    total=False,
+)
+
 DeploymentConfigurationValidationPolicyTypeDef = TypedDict(
     "DeploymentConfigurationValidationPolicyTypeDef",
     {
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
+IoTJobTimeoutConfigOutputTypeDef = TypedDict(
+    "IoTJobTimeoutConfigOutputTypeDef",
+    {
+        "inProgressTimeoutInMinutes": int,
+    },
+    total=False,
+)
+
 IoTJobTimeoutConfigTypeDef = TypedDict(
     "IoTJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
@@ -426,21 +504,19 @@
     "_OptionalGetComponentRequestRequestTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
     },
     total=False,
 )
 
-
 class GetComponentRequestRequestTypeDef(
     _RequiredGetComponentRequestRequestTypeDef, _OptionalGetComponentRequestRequestTypeDef
 ):
     pass
 
-
 GetComponentResponseTypeDef = TypedDict(
     "GetComponentResponseTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
         "recipe": bytes,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -519,24 +595,43 @@
         "lastReportedTimestamp": datetime,
         "lastInstallationSource": str,
         "lifecycleStatusCodes": List[str],
     },
     total=False,
 )
 
+IoTJobAbortCriteriaOutputTypeDef = TypedDict(
+    "IoTJobAbortCriteriaOutputTypeDef",
+    {
+        "failureType": IoTJobExecutionFailureTypeType,
+        "action": Literal["CANCEL"],
+        "thresholdPercentage": float,
+        "minNumberOfExecutedThings": int,
+    },
+)
+
 IoTJobAbortCriteriaTypeDef = TypedDict(
     "IoTJobAbortCriteriaTypeDef",
     {
         "failureType": IoTJobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
+IoTJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
+    "IoTJobRateIncreaseCriteriaOutputTypeDef",
+    {
+        "numberOfNotifiedThings": int,
+        "numberOfSucceededThings": int,
+    },
+    total=False,
+)
+
 IoTJobRateIncreaseCriteriaTypeDef = TypedDict(
     "IoTJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
@@ -553,21 +648,19 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
-
 class LambdaDeviceMountTypeDef(
     _RequiredLambdaDeviceMountTypeDef, _OptionalLambdaDeviceMountTypeDef
 ):
     pass
 
-
 _RequiredLambdaVolumeMountTypeDef = TypedDict(
     "_RequiredLambdaVolumeMountTypeDef",
     {
         "sourcePath": str,
         "destinationPath": str,
     },
 )
@@ -576,21 +669,19 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
-
 class LambdaVolumeMountTypeDef(
     _RequiredLambdaVolumeMountTypeDef, _OptionalLambdaVolumeMountTypeDef
 ):
     pass
 
-
 LambdaEventSourceTypeDef = TypedDict(
     "LambdaEventSourceTypeDef",
     {
         "topic": str,
         "type": LambdaEventSourceTypeType,
     },
 )
@@ -605,22 +696,20 @@
     "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
@@ -628,44 +717,40 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
     "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
     _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListComponentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListComponentVersionsRequestRequestTypeDef = TypedDict(
@@ -673,22 +758,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListComponentVersionsRequestRequestTypeDef(
     _RequiredListComponentVersionsRequestRequestTypeDef,
     _OptionalListComponentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
     "ListComponentsRequestListComponentsPaginateTypeDef",
     {
         "scope": ComponentVisibilityScopeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -758,22 +841,20 @@
     "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
     _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListEffectiveDeploymentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
@@ -781,22 +862,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEffectiveDeploymentsRequestRequestTypeDef(
     _RequiredListEffectiveDeploymentsRequestRequestTypeDef,
     _OptionalListEffectiveDeploymentsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
@@ -804,22 +883,20 @@
     {
         "topologyFilter": InstalledComponentTopologyFilterType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
     _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstalledComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListInstalledComponentsRequestRequestTypeDef = TypedDict(
@@ -828,22 +905,20 @@
         "maxResults": int,
         "nextToken": str,
         "topologyFilter": InstalledComponentTopologyFilterType,
     },
     total=False,
 )
 
-
 class ListInstalledComponentsRequestRequestTypeDef(
     _RequiredListInstalledComponentsRequestRequestTypeDef,
     _OptionalListInstalledComponentsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -924,22 +999,20 @@
     "_OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
-
 class BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef(
     _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
     _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef = TypedDict(
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -963,22 +1036,20 @@
     "_OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
-
 class BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef(
     _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     _OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef = TypedDict(
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -999,44 +1070,54 @@
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "description": str,
         "publisher": str,
-        "platforms": List[ComponentPlatformTypeDef],
+        "platforms": List[ComponentPlatformOutputTypeDef],
     },
     total=False,
 )
 
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
-        "platforms": List[ComponentPlatformTypeDef],
+        "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
 )
 
+ComponentRunWithOutputTypeDef = TypedDict(
+    "ComponentRunWithOutputTypeDef",
+    {
+        "posixUser": str,
+        "systemResourceLimits": SystemResourceLimitsOutputTypeDef,
+        "windowsUser": str,
+    },
+    total=False,
+)
+
 ComponentRunWithTypeDef = TypedDict(
     "ComponentRunWithTypeDef",
     {
         "posixUser": str,
         "systemResourceLimits": SystemResourceLimitsTypeDef,
         "windowsUser": str,
     },
@@ -1051,15 +1132,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "connectivityInfo": List[ConnectivityInfoTypeDef],
+        "connectivityInfo": List[ConnectivityInfoOutputTypeDef],
         "message": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityInfoRequestRequestTypeDef",
@@ -1074,14 +1155,24 @@
     {
         "coreDevices": List[CoreDeviceTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentPoliciesOutputTypeDef = TypedDict(
+    "DeploymentPoliciesOutputTypeDef",
+    {
+        "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
+        "componentUpdatePolicy": DeploymentComponentUpdatePolicyOutputTypeDef,
+        "configurationValidationPolicy": DeploymentConfigurationValidationPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentPoliciesTypeDef = TypedDict(
     "DeploymentPoliciesTypeDef",
     {
         "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
         "componentUpdatePolicy": DeploymentComponentUpdatePolicyTypeDef,
         "configurationValidationPolicy": DeploymentConfigurationValidationPolicyTypeDef,
     },
@@ -1116,37 +1207,51 @@
         "description": str,
         "reason": str,
         "statusDetails": EffectiveDeploymentStatusDetailsTypeDef,
     },
     total=False,
 )
 
-
 class EffectiveDeploymentTypeDef(
     _RequiredEffectiveDeploymentTypeDef, _OptionalEffectiveDeploymentTypeDef
 ):
     pass
 
-
 ListInstalledComponentsResponseTypeDef = TypedDict(
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IoTJobAbortConfigOutputTypeDef = TypedDict(
+    "IoTJobAbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[IoTJobAbortCriteriaOutputTypeDef],
+    },
+)
+
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 
+IoTJobExponentialRolloutRateOutputTypeDef = TypedDict(
+    "IoTJobExponentialRolloutRateOutputTypeDef",
+    {
+        "baseRatePerMinute": int,
+        "incrementFactor": float,
+        "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaOutputTypeDef,
+    },
+)
+
 IoTJobExponentialRolloutRateTypeDef = TypedDict(
     "IoTJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaTypeDef,
     },
@@ -1177,14 +1282,24 @@
         "arn": str,
         "componentName": str,
         "latestVersion": ComponentLatestVersionTypeDef,
     },
     total=False,
 )
 
+ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
+    "ComponentDeploymentSpecificationOutputTypeDef",
+    {
+        "componentVersion": str,
+        "configurationUpdate": ComponentConfigurationUpdateOutputTypeDef,
+        "runWith": ComponentRunWithOutputTypeDef,
+    },
+    total=False,
+)
+
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
         "componentVersion": str,
         "configurationUpdate": ComponentConfigurationUpdateTypeDef,
         "runWith": ComponentRunWithTypeDef,
     },
@@ -1196,14 +1311,23 @@
     {
         "effectiveDeployments": List[EffectiveDeploymentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IoTJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
+    "IoTJobExecutionsRolloutConfigOutputTypeDef",
+    {
+        "exponentialRate": IoTJobExponentialRolloutRateOutputTypeDef,
+        "maximumPerMinute": int,
+    },
+    total=False,
+)
+
 IoTJobExecutionsRolloutConfigTypeDef = TypedDict(
     "IoTJobExecutionsRolloutConfigTypeDef",
     {
         "exponentialRate": IoTJobExponentialRolloutRateTypeDef,
         "maximumPerMinute": int,
     },
     total=False,
@@ -1223,14 +1347,24 @@
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
+    "DeploymentIoTJobConfigurationOutputTypeDef",
+    {
+        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigOutputTypeDef,
+        "abortConfig": IoTJobAbortConfigOutputTypeDef,
+        "timeoutConfig": IoTJobTimeoutConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigTypeDef,
         "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
@@ -1251,14 +1385,35 @@
         "execArgs": Sequence[str],
         "environmentVariables": Mapping[str, str],
         "linuxProcessParams": LambdaLinuxProcessParamsTypeDef,
     },
     total=False,
 )
 
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "targetArn": str,
+        "revisionId": str,
+        "deploymentId": str,
+        "deploymentName": str,
+        "deploymentStatus": DeploymentStatusType,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
+        "deploymentPolicies": DeploymentPoliciesOutputTypeDef,
+        "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
+        "creationTimestamp": datetime,
+        "isLatestForTarget": bool,
+        "parentTargetArn": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "targetArn": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
@@ -1271,42 +1426,19 @@
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "targetArn": str,
-        "revisionId": str,
-        "deploymentId": str,
-        "deploymentName": str,
-        "deploymentStatus": DeploymentStatusType,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
-        "deploymentPolicies": DeploymentPoliciesTypeDef,
-        "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
-        "creationTimestamp": datetime,
-        "isLatestForTarget": bool,
-        "parentTargetArn": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
 _OptionalLambdaFunctionRecipeSourceTypeDef = TypedDict(
@@ -1317,21 +1449,19 @@
         "componentPlatforms": Sequence[ComponentPlatformTypeDef],
         "componentDependencies": Mapping[str, ComponentDependencyRequirementTypeDef],
         "componentLambdaParameters": LambdaExecutionParametersTypeDef,
     },
     total=False,
 )
 
-
 class LambdaFunctionRecipeSourceTypeDef(
     _RequiredLambdaFunctionRecipeSourceTypeDef, _OptionalLambdaFunctionRecipeSourceTypeDef
 ):
     pass
 
-
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
         "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
```

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2/type_defs.pyi` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,39 +43,47 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "AssociateServiceRoleToAccountResponseTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CancelDeploymentResponseTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
+    "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
+    "ComponentPlatformOutputTypeDef",
     "ComponentPlatformTypeDef",
+    "SystemResourceLimitsOutputTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
+    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
     "CreateDeploymentResponseTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
+    "DeploymentComponentUpdatePolicyOutputTypeDef",
     "DeploymentComponentUpdatePolicyTypeDef",
+    "DeploymentConfigurationValidationPolicyOutputTypeDef",
     "DeploymentConfigurationValidationPolicyTypeDef",
+    "IoTJobTimeoutConfigOutputTypeDef",
     "IoTJobTimeoutConfigTypeDef",
     "DeploymentTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EffectiveDeploymentStatusDetailsTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetComponentRequestRequestTypeDef",
@@ -84,15 +92,17 @@
     "GetComponentVersionArtifactResponseTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetCoreDeviceRequestRequestTypeDef",
     "GetCoreDeviceResponseTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetServiceRoleForAccountResponseTypeDef",
     "InstalledComponentTypeDef",
+    "IoTJobAbortCriteriaOutputTypeDef",
     "IoTJobAbortCriteriaTypeDef",
+    "IoTJobRateIncreaseCriteriaOutputTypeDef",
     "IoTJobRateIncreaseCriteriaTypeDef",
     "LambdaDeviceMountTypeDef",
     "LambdaVolumeMountTypeDef",
     "LambdaEventSourceTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
@@ -120,37 +130,44 @@
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
+    "ComponentRunWithOutputTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
+    "DeploymentPoliciesOutputTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
+    "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
+    "IoTJobExponentialRolloutRateOutputTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
+    "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
+    "IoTJobExecutionsRolloutConfigOutputTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
+    "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
-    "CreateDeploymentRequestRequestTypeDef",
     "GetDeploymentResponseTypeDef",
+    "CreateDeploymentRequestRequestTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -242,14 +259,23 @@
         "componentName": str,
         "componentVersion": str,
         "versionRequirements": Mapping[str, str],
     },
     total=False,
 )
 
+ComponentConfigurationUpdateOutputTypeDef = TypedDict(
+    "ComponentConfigurationUpdateOutputTypeDef",
+    {
+        "merge": str,
+        "reset": List[str],
+    },
+    total=False,
+)
+
 ComponentConfigurationUpdateTypeDef = TypedDict(
     "ComponentConfigurationUpdateTypeDef",
     {
         "merge": str,
         "reset": Sequence[str],
     },
     total=False,
@@ -260,23 +286,41 @@
     {
         "versionRequirement": str,
         "dependencyType": ComponentDependencyTypeType,
     },
     total=False,
 )
 
+ComponentPlatformOutputTypeDef = TypedDict(
+    "ComponentPlatformOutputTypeDef",
+    {
+        "name": str,
+        "attributes": Dict[str, str],
+    },
+    total=False,
+)
+
 ComponentPlatformTypeDef = TypedDict(
     "ComponentPlatformTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
+SystemResourceLimitsOutputTypeDef = TypedDict(
+    "SystemResourceLimitsOutputTypeDef",
+    {
+        "memory": int,
+        "cpus": float,
+    },
+    total=False,
+)
+
 SystemResourceLimitsTypeDef = TypedDict(
     "SystemResourceLimitsTypeDef",
     {
         "memory": int,
         "cpus": float,
     },
     total=False,
@@ -288,14 +332,25 @@
         "componentName": str,
         "componentVersion": str,
         "arn": str,
     },
     total=False,
 )
 
+ConnectivityInfoOutputTypeDef = TypedDict(
+    "ConnectivityInfoOutputTypeDef",
+    {
+        "id": str,
+        "hostAddress": str,
+        "portNumber": int,
+        "metadata": str,
+    },
+    total=False,
+)
+
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "id": str,
         "hostAddress": str,
         "portNumber": int,
         "metadata": str,
@@ -340,31 +395,56 @@
 DeleteDeploymentRequestRequestTypeDef = TypedDict(
     "DeleteDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
+DeploymentComponentUpdatePolicyOutputTypeDef = TypedDict(
+    "DeploymentComponentUpdatePolicyOutputTypeDef",
+    {
+        "timeoutInSeconds": int,
+        "action": DeploymentComponentUpdatePolicyActionType,
+    },
+    total=False,
+)
+
 DeploymentComponentUpdatePolicyTypeDef = TypedDict(
     "DeploymentComponentUpdatePolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "action": DeploymentComponentUpdatePolicyActionType,
     },
     total=False,
 )
 
+DeploymentConfigurationValidationPolicyOutputTypeDef = TypedDict(
+    "DeploymentConfigurationValidationPolicyOutputTypeDef",
+    {
+        "timeoutInSeconds": int,
+    },
+    total=False,
+)
+
 DeploymentConfigurationValidationPolicyTypeDef = TypedDict(
     "DeploymentConfigurationValidationPolicyTypeDef",
     {
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
+IoTJobTimeoutConfigOutputTypeDef = TypedDict(
+    "IoTJobTimeoutConfigOutputTypeDef",
+    {
+        "inProgressTimeoutInMinutes": int,
+    },
+    total=False,
+)
+
 IoTJobTimeoutConfigTypeDef = TypedDict(
     "IoTJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
@@ -425,19 +505,21 @@
     "_OptionalGetComponentRequestRequestTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
     },
     total=False,
 )
 
+
 class GetComponentRequestRequestTypeDef(
     _RequiredGetComponentRequestRequestTypeDef, _OptionalGetComponentRequestRequestTypeDef
 ):
     pass
 
+
 GetComponentResponseTypeDef = TypedDict(
     "GetComponentResponseTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
         "recipe": bytes,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -516,24 +598,43 @@
         "lastReportedTimestamp": datetime,
         "lastInstallationSource": str,
         "lifecycleStatusCodes": List[str],
     },
     total=False,
 )
 
+IoTJobAbortCriteriaOutputTypeDef = TypedDict(
+    "IoTJobAbortCriteriaOutputTypeDef",
+    {
+        "failureType": IoTJobExecutionFailureTypeType,
+        "action": Literal["CANCEL"],
+        "thresholdPercentage": float,
+        "minNumberOfExecutedThings": int,
+    },
+)
+
 IoTJobAbortCriteriaTypeDef = TypedDict(
     "IoTJobAbortCriteriaTypeDef",
     {
         "failureType": IoTJobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
+IoTJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
+    "IoTJobRateIncreaseCriteriaOutputTypeDef",
+    {
+        "numberOfNotifiedThings": int,
+        "numberOfSucceededThings": int,
+    },
+    total=False,
+)
+
 IoTJobRateIncreaseCriteriaTypeDef = TypedDict(
     "IoTJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
@@ -550,19 +651,21 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
+
 class LambdaDeviceMountTypeDef(
     _RequiredLambdaDeviceMountTypeDef, _OptionalLambdaDeviceMountTypeDef
 ):
     pass
 
+
 _RequiredLambdaVolumeMountTypeDef = TypedDict(
     "_RequiredLambdaVolumeMountTypeDef",
     {
         "sourcePath": str,
         "destinationPath": str,
     },
 )
@@ -571,19 +674,21 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
+
 class LambdaVolumeMountTypeDef(
     _RequiredLambdaVolumeMountTypeDef, _OptionalLambdaVolumeMountTypeDef
 ):
     pass
 
+
 LambdaEventSourceTypeDef = TypedDict(
     "LambdaEventSourceTypeDef",
     {
         "topic": str,
         "type": LambdaEventSourceTypeType,
     },
 )
@@ -598,20 +703,22 @@
     "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
 ):
     pass
 
+
 _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
@@ -619,40 +726,44 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
     "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
     _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListComponentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListComponentVersionsRequestRequestTypeDef = TypedDict(
@@ -660,20 +771,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListComponentVersionsRequestRequestTypeDef(
     _RequiredListComponentVersionsRequestRequestTypeDef,
     _OptionalListComponentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
     "ListComponentsRequestListComponentsPaginateTypeDef",
     {
         "scope": ComponentVisibilityScopeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -743,20 +856,22 @@
     "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
     _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListEffectiveDeploymentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
@@ -764,20 +879,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEffectiveDeploymentsRequestRequestTypeDef(
     _RequiredListEffectiveDeploymentsRequestRequestTypeDef,
     _OptionalListEffectiveDeploymentsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
@@ -785,20 +902,22 @@
     {
         "topologyFilter": InstalledComponentTopologyFilterType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
     _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstalledComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListInstalledComponentsRequestRequestTypeDef = TypedDict(
@@ -807,20 +926,22 @@
         "maxResults": int,
         "nextToken": str,
         "topologyFilter": InstalledComponentTopologyFilterType,
     },
     total=False,
 )
 
+
 class ListInstalledComponentsRequestRequestTypeDef(
     _RequiredListInstalledComponentsRequestRequestTypeDef,
     _OptionalListInstalledComponentsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -901,20 +1022,22 @@
     "_OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
+
 class BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef(
     _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
     _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef = TypedDict(
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -938,20 +1061,22 @@
     "_OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
+
 class BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef(
     _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     _OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef = TypedDict(
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -972,44 +1097,54 @@
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "description": str,
         "publisher": str,
-        "platforms": List[ComponentPlatformTypeDef],
+        "platforms": List[ComponentPlatformOutputTypeDef],
     },
     total=False,
 )
 
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
-        "platforms": List[ComponentPlatformTypeDef],
+        "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
 )
 
+ComponentRunWithOutputTypeDef = TypedDict(
+    "ComponentRunWithOutputTypeDef",
+    {
+        "posixUser": str,
+        "systemResourceLimits": SystemResourceLimitsOutputTypeDef,
+        "windowsUser": str,
+    },
+    total=False,
+)
+
 ComponentRunWithTypeDef = TypedDict(
     "ComponentRunWithTypeDef",
     {
         "posixUser": str,
         "systemResourceLimits": SystemResourceLimitsTypeDef,
         "windowsUser": str,
     },
@@ -1024,15 +1159,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "connectivityInfo": List[ConnectivityInfoTypeDef],
+        "connectivityInfo": List[ConnectivityInfoOutputTypeDef],
         "message": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityInfoRequestRequestTypeDef",
@@ -1047,14 +1182,24 @@
     {
         "coreDevices": List[CoreDeviceTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentPoliciesOutputTypeDef = TypedDict(
+    "DeploymentPoliciesOutputTypeDef",
+    {
+        "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
+        "componentUpdatePolicy": DeploymentComponentUpdatePolicyOutputTypeDef,
+        "configurationValidationPolicy": DeploymentConfigurationValidationPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentPoliciesTypeDef = TypedDict(
     "DeploymentPoliciesTypeDef",
     {
         "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
         "componentUpdatePolicy": DeploymentComponentUpdatePolicyTypeDef,
         "configurationValidationPolicy": DeploymentConfigurationValidationPolicyTypeDef,
     },
@@ -1089,35 +1234,53 @@
         "description": str,
         "reason": str,
         "statusDetails": EffectiveDeploymentStatusDetailsTypeDef,
     },
     total=False,
 )
 
+
 class EffectiveDeploymentTypeDef(
     _RequiredEffectiveDeploymentTypeDef, _OptionalEffectiveDeploymentTypeDef
 ):
     pass
 
+
 ListInstalledComponentsResponseTypeDef = TypedDict(
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IoTJobAbortConfigOutputTypeDef = TypedDict(
+    "IoTJobAbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[IoTJobAbortCriteriaOutputTypeDef],
+    },
+)
+
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 
+IoTJobExponentialRolloutRateOutputTypeDef = TypedDict(
+    "IoTJobExponentialRolloutRateOutputTypeDef",
+    {
+        "baseRatePerMinute": int,
+        "incrementFactor": float,
+        "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaOutputTypeDef,
+    },
+)
+
 IoTJobExponentialRolloutRateTypeDef = TypedDict(
     "IoTJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaTypeDef,
     },
@@ -1148,14 +1311,24 @@
         "arn": str,
         "componentName": str,
         "latestVersion": ComponentLatestVersionTypeDef,
     },
     total=False,
 )
 
+ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
+    "ComponentDeploymentSpecificationOutputTypeDef",
+    {
+        "componentVersion": str,
+        "configurationUpdate": ComponentConfigurationUpdateOutputTypeDef,
+        "runWith": ComponentRunWithOutputTypeDef,
+    },
+    total=False,
+)
+
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
         "componentVersion": str,
         "configurationUpdate": ComponentConfigurationUpdateTypeDef,
         "runWith": ComponentRunWithTypeDef,
     },
@@ -1167,14 +1340,23 @@
     {
         "effectiveDeployments": List[EffectiveDeploymentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IoTJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
+    "IoTJobExecutionsRolloutConfigOutputTypeDef",
+    {
+        "exponentialRate": IoTJobExponentialRolloutRateOutputTypeDef,
+        "maximumPerMinute": int,
+    },
+    total=False,
+)
+
 IoTJobExecutionsRolloutConfigTypeDef = TypedDict(
     "IoTJobExecutionsRolloutConfigTypeDef",
     {
         "exponentialRate": IoTJobExponentialRolloutRateTypeDef,
         "maximumPerMinute": int,
     },
     total=False,
@@ -1194,14 +1376,24 @@
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
+    "DeploymentIoTJobConfigurationOutputTypeDef",
+    {
+        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigOutputTypeDef,
+        "abortConfig": IoTJobAbortConfigOutputTypeDef,
+        "timeoutConfig": IoTJobTimeoutConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigTypeDef,
         "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
@@ -1222,14 +1414,35 @@
         "execArgs": Sequence[str],
         "environmentVariables": Mapping[str, str],
         "linuxProcessParams": LambdaLinuxProcessParamsTypeDef,
     },
     total=False,
 )
 
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "targetArn": str,
+        "revisionId": str,
+        "deploymentId": str,
+        "deploymentName": str,
+        "deploymentStatus": DeploymentStatusType,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
+        "deploymentPolicies": DeploymentPoliciesOutputTypeDef,
+        "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
+        "creationTimestamp": datetime,
+        "isLatestForTarget": bool,
+        "parentTargetArn": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "targetArn": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
@@ -1242,39 +1455,20 @@
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "targetArn": str,
-        "revisionId": str,
-        "deploymentId": str,
-        "deploymentName": str,
-        "deploymentStatus": DeploymentStatusType,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
-        "deploymentPolicies": DeploymentPoliciesTypeDef,
-        "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
-        "creationTimestamp": datetime,
-        "isLatestForTarget": bool,
-        "parentTargetArn": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
@@ -1286,19 +1480,21 @@
         "componentPlatforms": Sequence[ComponentPlatformTypeDef],
         "componentDependencies": Mapping[str, ComponentDependencyRequirementTypeDef],
         "componentLambdaParameters": LambdaExecutionParametersTypeDef,
     },
     total=False,
 )
 
+
 class LambdaFunctionRecipeSourceTypeDef(
     _RequiredLambdaFunctionRecipeSourceTypeDef, _OptionalLambdaFunctionRecipeSourceTypeDef
 ):
     pass
 
+
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
         "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
```

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/PKG-INFO` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.28.0
-Summary: Type annotations for boto3.GreengrassV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GreengrassV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrassv2?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrassv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,27 +377,34 @@
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
     CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
+    ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
+    ComponentPlatformOutputTypeDef,
     ComponentPlatformTypeDef,
+    SystemResourceLimitsOutputTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
     CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
+    DeploymentComponentUpdatePolicyOutputTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
+    DeploymentConfigurationValidationPolicyOutputTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
+    IoTJobTimeoutConfigOutputTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
@@ -406,15 +413,17 @@
     GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
     GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
+    IoTJobAbortCriteriaOutputTypeDef,
     IoTJobAbortCriteriaTypeDef,
+    IoTJobRateIncreaseCriteriaOutputTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
@@ -442,37 +451,44 @@
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
+    ComponentRunWithOutputTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
+    DeploymentPoliciesOutputTypeDef,
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
+    IoTJobAbortConfigOutputTypeDef,
     IoTJobAbortConfigTypeDef,
+    IoTJobExponentialRolloutRateOutputTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
+    ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
+    IoTJobExecutionsRolloutConfigOutputTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
+    DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
-    CreateDeploymentRequestRequestTypeDef,
     GetDeploymentResponseTypeDef,
+    CreateDeploymentRequestRequestTypeDef,
     LambdaFunctionRecipeSourceTypeDef,
     CreateComponentVersionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-greengrassv2-1.28.0/mypy_boto3_greengrassv2.egg-info/SOURCES.txt` & `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.0/setup.py` & `mypy-boto3-greengrassv2-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrassv2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GreengrassV2 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.GreengrassV2 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

