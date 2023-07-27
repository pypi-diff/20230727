# Comparing `tmp/mypy-boto3-cloudformation-1.28.10.tar.gz` & `tmp/mypy-boto3-cloudformation-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudformation-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
```

## Comparing `mypy-boto3-cloudformation-1.28.10.tar` & `mypy-boto3-cloudformation-1.28.12.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30369 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28854 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66147 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66048 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    91414 2023-07-24 19:47:04.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    91321 2023-07-24 19:47:03.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-24 19:47:02.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30369 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 19:49:46.000000 mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:49:46.296631 mypy-boto3-cloudformation-1.28.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-24 19:47:01.000000 mypy-boto3-cloudformation-1.28.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.012562 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66147 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66048 2023-07-27 05:18:31.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17308 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    95531 2023-07-27 05:18:35.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95414 2023-07-27 05:18:33.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudformation-1.28.10/LICENSE` & `mypy-boto3-cloudformation-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/PKG-INFO` & `mypy-boto3-cloudformation-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.10
-Summary: Type annotations for boto3.CloudFormation 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudFormation 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudformation"></a>
 
 # mypy-boto3-cloudformation
 
 [![PyPI - mypy-boto3-cloudformation](https://img.shields.io/pypi/v/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudformation?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -580,175 +580,175 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ActivateTypeOutputTypeDef,
     AutoDeploymentOutputTypeDef,
     AutoDeploymentTypeDef,
     TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
+    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
+    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
+    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
     DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
     ParameterOutputTypeDef,
     TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
+    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
     LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
+    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
+    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
+    GetTemplateOutputTypeDef,
     TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
     WarningsTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
+    ListImportsOutputTypeDef,
     ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
     ManagedExecutionOutputTypeDef,
+    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
+    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
+    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
+    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
+    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
+    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
+    StackResourceDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
     StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    UpdateTerminationProtectionInputRequestTypeDef,
-    ValidateTemplateInputRequestTypeDef,
-    StackSetOperationResultSummaryTypeDef,
-    ActivateTypeInputRequestTypeDef,
-    RegisterTypeInputRequestTypeDef,
-    ActivateTypeOutputTypeDef,
-    CreateChangeSetOutputTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
-    CreateStackSetOutputTypeDef,
-    DeleteStackInstancesOutputTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
-    DescribePublisherOutputTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
-    DetectStackDriftOutputTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
-    GetStackPolicyOutputTypeDef,
-    GetTemplateOutputTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListImportsOutputTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
-    PublishTypeOutputTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
-    RollbackStackOutputTypeDef,
-    SetTypeConfigurationOutputTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     TestTypeOutputTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionInputRequestTypeDef,
     UpdateTerminationProtectionOutputTypeDef,
+    ValidateTemplateInputRequestTypeDef,
+    StackSetOperationResultSummaryTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    ActivateTypeInputRequestTypeDef,
+    RegisterTypeInputRequestTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
     UpdateStackSetInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.10/README.md` & `mypy-boto3-cloudformation-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudformation"></a>
 
 # mypy-boto3-cloudformation
 
 [![PyPI - mypy-boto3-cloudformation](https://img.shields.io/pypi/v/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudformation?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -548,175 +548,175 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ActivateTypeOutputTypeDef,
     AutoDeploymentOutputTypeDef,
     AutoDeploymentTypeDef,
     TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
+    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
+    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
+    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
     DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
     ParameterOutputTypeDef,
     TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
+    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
     LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
+    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
+    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
+    GetTemplateOutputTypeDef,
     TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
     WarningsTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
+    ListImportsOutputTypeDef,
     ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
     ManagedExecutionOutputTypeDef,
+    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
+    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
+    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
+    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
+    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
+    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
+    StackResourceDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
     StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    UpdateTerminationProtectionInputRequestTypeDef,
-    ValidateTemplateInputRequestTypeDef,
-    StackSetOperationResultSummaryTypeDef,
-    ActivateTypeInputRequestTypeDef,
-    RegisterTypeInputRequestTypeDef,
-    ActivateTypeOutputTypeDef,
-    CreateChangeSetOutputTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
-    CreateStackSetOutputTypeDef,
-    DeleteStackInstancesOutputTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
-    DescribePublisherOutputTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
-    DetectStackDriftOutputTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
-    GetStackPolicyOutputTypeDef,
-    GetTemplateOutputTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListImportsOutputTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
-    PublishTypeOutputTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
-    RollbackStackOutputTypeDef,
-    SetTypeConfigurationOutputTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     TestTypeOutputTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionInputRequestTypeDef,
     UpdateTerminationProtectionOutputTypeDef,
+    ValidateTemplateInputRequestTypeDef,
+    StackSetOperationResultSummaryTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    ActivateTypeInputRequestTypeDef,
+    RegisterTypeInputRequestTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
     UpdateStackSetInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__init__.pyi` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/__main__.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFormation 1.28.10\nVersion:         1.28.10\nBuilder"
-        " version: 7.15.1\nDocs:           "
+        "Type annotations for boto3.CloudFormation 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.10")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/client.pyi` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.pyi`

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
     "AccountFilterTypeType",
     "AccountGateStatusType",
     "CallAsType",
     "CapabilityType",
     "CategoryType",
     "ChangeActionType",
@@ -101,15 +100,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AccountFilterTypeType = Literal["DIFFERENCE", "INTERSECTION", "NONE", "UNION"]
 AccountGateStatusType = Literal["FAILED", "SKIPPED", "SUCCEEDED"]
 CallAsType = Literal["DELEGATED_ADMIN", "SELF"]
 CapabilityType = Literal["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"]
 CategoryType = Literal["ACTIVATED", "AWS_TYPES", "REGISTERED", "THIRD_PARTY"]
 ChangeActionType = Literal["Add", "Dynamic", "Import", "Modify", "Remove"]
 ChangeSetCreateCompleteWaiterName = Literal["change_set_create_complete"]
@@ -408,14 +406,15 @@
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
@@ -494,14 +493,15 @@
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
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/literals.pyi` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AccountFilterTypeType",
     "AccountGateStatusType",
     "CallAsType",
     "CapabilityType",
     "CategoryType",
     "ChangeActionType",
@@ -100,14 +101,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AccountFilterTypeType = Literal["DIFFERENCE", "INTERSECTION", "NONE", "UNION"]
 AccountGateStatusType = Literal["FAILED", "SKIPPED", "SUCCEEDED"]
 CallAsType = Literal["DELEGATED_ADMIN", "SELF"]
 CapabilityType = Literal["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"]
 CategoryType = Literal["ACTIVATED", "AWS_TYPES", "REGISTERED", "THIRD_PARTY"]
 ChangeActionType = Literal["Add", "Dynamic", "Import", "Modify", "Remove"]
 ChangeSetCreateCompleteWaiterName = Literal["change_set_create_complete"]
@@ -406,14 +408,15 @@
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
@@ -492,14 +495,15 @@
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
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
 
@@ -129,90 +129,90 @@
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
 
 class DescribeStackEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
         """
 
 
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
 
 class ListChangeSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
         """
 
 
 class ListExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
         """
 
 
 class ListImportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
         """
 
 
@@ -226,30 +226,30 @@
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
         """
 
 
 class ListStackResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
         """
 
 
@@ -262,15 +262,15 @@
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
 
@@ -281,15 +281,15 @@
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 
@@ -300,15 +300,15 @@
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
         """
 
 
@@ -318,15 +318,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
         """
 
 
@@ -340,13 +340,13 @@
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/paginator.pyi` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeChangeSetPaginator(Paginator):
@@ -125,85 +125,85 @@
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
 class DescribeStackEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
         """
 
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
 class ListChangeSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
         """
 
 class ListExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
         """
 
 class ListImportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
         """
 
 class ListStackInstancesPaginator(Paginator):
@@ -216,29 +216,29 @@
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
         """
 
 class ListStackResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
         """
 
 class ListStackSetOperationResultsPaginator(Paginator):
@@ -250,15 +250,15 @@
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
 class ListStackSetOperationsPaginator(Paginator):
@@ -268,15 +268,15 @@
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 class ListStackSetsPaginator(Paginator):
@@ -286,15 +286,15 @@
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
         """
 
 class ListStacksPaginator(Paginator):
@@ -303,15 +303,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
         """
 
 class ListTypesPaginator(Paginator):
@@ -324,13 +324,13 @@
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/service_resource.pyi` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,175 +79,175 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActivateTypeOutputTypeDef",
     "AutoDeploymentOutputTypeDef",
     "AutoDeploymentTypeDef",
     "TypeConfigurationIdentifierOutputTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
+    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
+    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
     "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
     "ParameterOutputTypeDef",
     "TagOutputTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
+    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
     "LoggingConfigOutputTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
+    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
+    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
+    "GetTemplateOutputTypeDef",
     "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
     "WarningsTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListChangeSetsInputRequestTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListImportsOutputTypeDef",
     "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
     "ManagedExecutionOutputTypeDef",
+    "ModuleInfoResponseMetadataTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
+    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
+    "ResponseMetadataTypeDef",
     "RollbackTriggerOutputTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
+    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
+    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
     "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "UpdateTerminationProtectionInputRequestTypeDef",
-    "ValidateTemplateInputRequestTypeDef",
-    "StackSetOperationResultSummaryTypeDef",
-    "ActivateTypeInputRequestTypeDef",
-    "RegisterTypeInputRequestTypeDef",
-    "ActivateTypeOutputTypeDef",
-    "CreateChangeSetOutputTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
-    "CreateStackSetOutputTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
-    "DescribePublisherOutputTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
-    "DetectStackDriftOutputTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
-    "GetStackPolicyOutputTypeDef",
-    "GetTemplateOutputTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListImportsOutputTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
-    "PublishTypeOutputTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
-    "RollbackStackOutputTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "TestTypeOutputTypeDef",
     "UpdateStackInstancesOutputTypeDef",
     "UpdateStackOutputTypeDef",
     "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionInputRequestTypeDef",
     "UpdateTerminationProtectionOutputTypeDef",
+    "ValidateTemplateInputRequestTypeDef",
+    "StackSetOperationResultSummaryTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "ActivateTypeInputRequestTypeDef",
+    "RegisterTypeInputRequestTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
     "UpdateStackSetInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
@@ -314,49 +314,49 @@
 
 AccountGateResultTypeDef = TypedDict(
     "AccountGateResultTypeDef",
     {
         "Status": AccountGateStatusType,
         "StatusReason": str,
     },
+    total=False,
 )
 
 AccountLimitTypeDef = TypedDict(
     "AccountLimitTypeDef",
     {
         "Name": str,
         "Value": int,
     },
+    total=False,
 )
 
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoDeploymentOutputTypeDef = TypedDict(
     "AutoDeploymentOutputTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
     },
+    total=False,
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
@@ -369,14 +369,15 @@
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
         "TypeConfigurationArn": str,
         "Type": ThirdPartyTypeType,
         "TypeName": str,
     },
+    total=False,
 )
 
 TypeConfigurationIdentifierTypeDef = TypedDict(
     "TypeConfigurationIdentifierTypeDef",
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
@@ -394,14 +395,15 @@
         "Alias": str,
         "Configuration": str,
         "LastUpdated": datetime,
         "TypeArn": str,
         "TypeName": str,
         "IsDefaultConfiguration": bool,
     },
+    total=False,
 )
 
 _RequiredCancelUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredCancelUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -432,14 +434,15 @@
 ChangeSetHookResourceTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookResourceTargetDetailsTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "ResourceAction": ChangeActionType,
     },
+    total=False,
 )
 
 ChangeSetSummaryTypeDef = TypedDict(
     "ChangeSetSummaryTypeDef",
     {
         "StackId": str,
         "StackName": str,
@@ -450,14 +453,15 @@
         "StatusReason": str,
         "CreationTime": datetime,
         "Description": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
     },
+    total=False,
 )
 
 _RequiredContinueUpdateRollbackInputRequestTypeDef = TypedDict(
     "_RequiredContinueUpdateRollbackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -504,14 +508,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -528,22 +541,46 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -600,14 +637,22 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
@@ -629,33 +674,32 @@
     "DeploymentTargetsOutputTypeDef",
     {
         "Accounts": List[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": List[str],
         "AccountFilterType": AccountFilterTypeType,
     },
+    total=False,
 )
 
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -693,14 +737,37 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -723,14 +790,15 @@
     "ParameterOutputTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
         "UsePreviousValue": bool,
         "ResolvedValue": str,
     },
+    total=False,
 )
 
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -741,60 +809,113 @@
     "DescribeOrganizationsAccessInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePublisherInputRequestTypeDef = TypedDict(
     "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
     },
     total=False,
 )
 
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-StackEventTypeDef = TypedDict(
-    "StackEventTypeDef",
+_RequiredStackEventTypeDef = TypedDict(
+    "_RequiredStackEventTypeDef",
     {
         "StackId": str,
         "EventId": str,
         "StackName": str,
+        "Timestamp": datetime,
+    },
+)
+_OptionalStackEventTypeDef = TypedDict(
+    "_OptionalStackEventTypeDef",
+    {
         "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "ResourceType": str,
-        "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
         "ResourceStatusReason": str,
         "ResourceProperties": str,
         "ClientRequestToken": str,
         "HookType": str,
         "HookStatus": HookStatusType,
         "HookStatusReason": str,
         "HookInvocationPoint": Literal["PRE_PROVISION"],
         "HookFailureMode": HookFailureModeType,
     },
+    total=False,
 )
 
+
+class StackEventTypeDef(_RequiredStackEventTypeDef, _OptionalStackEventTypeDef):
+    pass
+
+
 _RequiredDescribeStackInstanceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackInstanceInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
     },
@@ -897,14 +1018,23 @@
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
 
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -935,23 +1065,35 @@
     "RequiredActivatedTypeTypeDef",
     {
         "TypeNameAlias": str,
         "OriginalTypeName": str,
         "PublisherId": str,
         "SupportedMajorVersions": List[int],
     },
+    total=False,
 )
 
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
@@ -965,22 +1107,53 @@
 
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
 
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
@@ -1003,33 +1176,51 @@
 ExportTypeDef = TypedDict(
     "ExportTypeDef",
     {
         "ExportingStackId": str,
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": str,
+        "StagesAvailable": List[TemplateStageType],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TemplateSummaryConfigTypeDef = TypedDict(
     "TemplateSummaryConfigTypeDef",
     {
         "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
@@ -1037,22 +1228,54 @@
 ResourceIdentifierSummaryTypeDef = TypedDict(
     "ResourceIdentifierSummaryTypeDef",
     {
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
+    total=False,
 )
 
 WarningsTypeDef = TypedDict(
     "WarningsTypeDef",
     {
         "UnrecognizedResourceTypes": List[str],
     },
+    total=False,
+)
+
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
 )
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
 
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
@@ -1067,22 +1290,52 @@
 
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
 
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListImportsInputRequestTypeDef = TypedDict(
     "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
 _OptionalListImportsInputRequestTypeDef = TypedDict(
@@ -1096,14 +1349,23 @@
 
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
 
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
     "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "OperationId": str,
@@ -1133,14 +1395,36 @@
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
@@ -1163,14 +1447,37 @@
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1187,25 +1494,44 @@
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
 
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1220,14 +1546,23 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1246,14 +1581,15 @@
         "VersionId": str,
         "IsDefaultVersion": bool,
         "Arn": str,
         "TimeCreated": datetime,
         "Description": str,
         "PublicVersionNumber": str,
     },
+    total=False,
 )
 
 TypeFiltersTypeDef = TypedDict(
     "TypeFiltersTypeDef",
     {
         "Category": CategoryType,
         "PublisherId": str,
@@ -1275,46 +1611,70 @@
         "OriginalTypeName": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
+    total=False,
 )
 
 ManagedExecutionOutputTypeDef = TypedDict(
     "ManagedExecutionOutputTypeDef",
     {
         "Active": bool,
     },
+    total=False,
+)
+
+ModuleInfoResponseMetadataTypeDef = TypedDict(
+    "ModuleInfoResponseMetadataTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
+    total=False,
 )
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
     },
+    total=False,
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
 )
 
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
+    total=False,
 )
 
 PhysicalResourceIdContextKeyValuePairTypeDef = TypedDict(
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1338,14 +1698,22 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1374,21 +1742,49 @@
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
     },
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
+    },
 )
 
 RollbackTriggerOutputTypeDef = TypedDict(
     "RollbackTriggerOutputTypeDef",
     {
         "Arn": str,
         "Type": str,
@@ -1421,14 +1817,22 @@
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
 
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalSetStackPolicyInputRequestTypeDef = TypedDict(
@@ -1468,14 +1872,22 @@
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
 
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1489,84 +1901,168 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationSummaryTypeDef = TypedDict(
-    "StackDriftInformationSummaryTypeDef",
+StackDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackDriftInformationResponseMetadataTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
         "LastCheckTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StackDriftInformationTypeDef = TypedDict(
-    "StackDriftInformationTypeDef",
+_RequiredStackDriftInformationSummaryTypeDef = TypedDict(
+    "_RequiredStackDriftInformationSummaryTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
+    },
+)
+_OptionalStackDriftInformationSummaryTypeDef = TypedDict(
+    "_OptionalStackDriftInformationSummaryTypeDef",
+    {
+        "LastCheckTimestamp": datetime,
+    },
+    total=False,
+)
+
+
+class StackDriftInformationSummaryTypeDef(
+    _RequiredStackDriftInformationSummaryTypeDef, _OptionalStackDriftInformationSummaryTypeDef
+):
+    pass
+
+
+_RequiredStackDriftInformationTypeDef = TypedDict(
+    "_RequiredStackDriftInformationTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+    },
+)
+_OptionalStackDriftInformationTypeDef = TypedDict(
+    "_OptionalStackDriftInformationTypeDef",
+    {
         "LastCheckTimestamp": datetime,
     },
+    total=False,
 )
 
+
+class StackDriftInformationTypeDef(
+    _RequiredStackDriftInformationTypeDef, _OptionalStackDriftInformationTypeDef
+):
+    pass
+
+
 StackInstanceComprehensiveStatusTypeDef = TypedDict(
     "StackInstanceComprehensiveStatusTypeDef",
     {
         "DetailedStatus": StackInstanceDetailedStatusType,
     },
+    total=False,
 )
 
-StackResourceDriftInformationTypeDef = TypedDict(
-    "StackResourceDriftInformationTypeDef",
+_RequiredStackResourceDriftInformationTypeDef = TypedDict(
+    "_RequiredStackResourceDriftInformationTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
+    },
+)
+_OptionalStackResourceDriftInformationTypeDef = TypedDict(
+    "_OptionalStackResourceDriftInformationTypeDef",
+    {
         "LastCheckTimestamp": datetime,
     },
+    total=False,
 )
 
-StackResourceDriftInformationSummaryTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryTypeDef",
+
+class StackResourceDriftInformationTypeDef(
+    _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
+):
+    pass
+
+
+StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
         "LastCheckTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
+    "_RequiredStackResourceDriftInformationSummaryTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+    },
+)
+_OptionalStackResourceDriftInformationSummaryTypeDef = TypedDict(
+    "_OptionalStackResourceDriftInformationSummaryTypeDef",
+    {
+        "LastCheckTimestamp": datetime,
+    },
+    total=False,
+)
+
+
+class StackResourceDriftInformationSummaryTypeDef(
+    _RequiredStackResourceDriftInformationSummaryTypeDef,
+    _OptionalStackResourceDriftInformationSummaryTypeDef,
+):
+    pass
+
+
 StackSetDriftDetectionDetailsTypeDef = TypedDict(
     "StackSetDriftDetectionDetailsTypeDef",
     {
         "DriftStatus": StackSetDriftStatusType,
         "DriftDetectionStatus": StackSetDriftDetectionStatusType,
         "LastDriftCheckTimestamp": datetime,
         "TotalStackInstancesCount": int,
         "DriftedStackInstancesCount": int,
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
+    total=False,
 )
 
 StackSetOperationPreferencesOutputTypeDef = TypedDict(
     "StackSetOperationPreferencesOutputTypeDef",
     {
         "RegionConcurrencyType": RegionConcurrencyTypeType,
         "RegionOrder": List[str],
         "FailureToleranceCount": int,
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
+    total=False,
 )
 
 StackSetOperationStatusDetailsTypeDef = TypedDict(
     "StackSetOperationStatusDetailsTypeDef",
     {
         "FailedStackInstancesCount": int,
     },
+    total=False,
 )
 
 _RequiredStopStackSetOperationInputRequestTypeDef = TypedDict(
     "_RequiredStopStackSetOperationInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
@@ -1592,36 +2088,77 @@
     "TemplateParameterTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "NoEcho": bool,
         "Description": str,
     },
+    total=False,
 )
 
 TestTypeInputRequestTypeDef = TypedDict(
     "TestTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": ThirdPartyTypeType,
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -1633,14 +2170,24 @@
         "Account": str,
         "Region": str,
         "Status": StackSetOperationResultStatusType,
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
+    total=False,
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
@@ -1677,313 +2224,22 @@
 
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
-    {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
-    {
-        "TemplateBody": str,
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
-    {
-        "Imports": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "TypeConfigurationIdentifier": TypeConfigurationIdentifierOutputTypeDef,
     },
+    total=False,
 )
 
 BatchDescribeTypeConfigurationsInputRequestTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     {
         "TypeConfigurationIdentifiers": Sequence[TypeConfigurationIdentifierTypeDef],
     },
@@ -1991,22 +2247,23 @@
 
 ChangeSetHookTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookTargetDetailsTypeDef",
     {
         "TargetType": Literal["RESOURCE"],
         "ResourceTargetDetails": ChangeSetHookResourceTargetDetailsTypeDef,
     },
+    total=False,
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2218,179 +2475,14 @@
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
-
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
-    {
-        "ExportName": str,
-    },
-)
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
-
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
@@ -2494,15 +2586,15 @@
 
 
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2528,24 +2620,24 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSummaryInputRequestTypeDef = TypedDict(
     "GetTemplateSummaryInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2567,15 +2659,15 @@
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
@@ -2618,15 +2710,15 @@
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
@@ -2662,27 +2754,27 @@
 
 
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2698,15 +2790,15 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StackSetSummaryTypeDef = TypedDict(
     "StackSetSummaryTypeDef",
     {
         "StackSetName": str,
@@ -2715,112 +2807,154 @@
         "Status": StackSetStatusType,
         "AutoDeployment": AutoDeploymentOutputTypeDef,
         "PermissionModel": PermissionModelsType,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "ManagedExecution": ManagedExecutionOutputTypeDef,
     },
+    total=False,
 )
 
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "ParameterType": str,
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
+    total=False,
 )
 
-StackInstanceResourceDriftsSummaryTypeDef = TypedDict(
-    "StackInstanceResourceDriftsSummaryTypeDef",
+_RequiredStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_RequiredStackInstanceResourceDriftsSummaryTypeDef",
     {
         "StackId": str,
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
-        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
         "ResourceType": str,
-        "PropertyDifferences": List[PropertyDifferenceTypeDef],
         "StackResourceDriftStatus": StackResourceDriftStatusType,
         "Timestamp": datetime,
     },
 )
+_OptionalStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_OptionalStackInstanceResourceDriftsSummaryTypeDef",
+    {
+        "PhysicalResourceId": str,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
+    },
+    total=False,
+)
 
-StackResourceDriftTypeDef = TypedDict(
-    "StackResourceDriftTypeDef",
+
+class StackInstanceResourceDriftsSummaryTypeDef(
+    _RequiredStackInstanceResourceDriftsSummaryTypeDef,
+    _OptionalStackInstanceResourceDriftsSummaryTypeDef,
+):
+    pass
+
+
+_RequiredStackResourceDriftTypeDef = TypedDict(
+    "_RequiredStackResourceDriftTypeDef",
     {
         "StackId": str,
         "LogicalResourceId": str,
+        "ResourceType": str,
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "Timestamp": datetime,
+    },
+)
+_OptionalStackResourceDriftTypeDef = TypedDict(
+    "_OptionalStackResourceDriftTypeDef",
+    {
         "PhysicalResourceId": str,
         "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
-        "ResourceType": str,
         "ExpectedProperties": str,
         "ActualProperties": str,
         "PropertyDifferences": List[PropertyDifferenceTypeDef],
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "Timestamp": datetime,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
+
+class StackResourceDriftTypeDef(
+    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
+):
+    pass
+
+
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
+    total=False,
 )
 
 RollbackConfigurationOutputTypeDef = TypedDict(
     "RollbackConfigurationOutputTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
         "MonitoringTimeInMinutes": int,
     },
+    total=False,
 )
 
 RollbackConfigurationResponseMetadataTypeDef = TypedDict(
     "RollbackConfigurationResponseMetadataTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
-StackSummaryTypeDef = TypedDict(
-    "StackSummaryTypeDef",
+_RequiredStackSummaryTypeDef = TypedDict(
+    "_RequiredStackSummaryTypeDef",
     {
-        "StackId": str,
         "StackName": str,
-        "TemplateDescription": str,
         "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackSummaryTypeDef = TypedDict(
+    "_OptionalStackSummaryTypeDef",
+    {
+        "StackId": str,
+        "TemplateDescription": str,
         "LastUpdatedTime": datetime,
         "DeletionTime": datetime,
-        "StackStatus": StackStatusType,
         "StackStatusReason": str,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationSummaryTypeDef,
     },
+    total=False,
 )
 
+
+class StackSummaryTypeDef(_RequiredStackSummaryTypeDef, _OptionalStackSummaryTypeDef):
+    pass
+
+
 StackInstanceSummaryTypeDef = TypedDict(
     "StackInstanceSummaryTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
@@ -2828,14 +2962,15 @@
         "StatusReason": str,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
+    total=False,
 )
 
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "StackSetId": str,
         "Region": str,
@@ -2846,65 +2981,103 @@
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "StatusReason": str,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
+    total=False,
 )
 
-StackResourceDetailTypeDef = TypedDict(
-    "StackResourceDetailTypeDef",
+_RequiredStackResourceDetailTypeDef = TypedDict(
+    "_RequiredStackResourceDetailTypeDef",
     {
-        "StackName": str,
-        "StackId": str,
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceDetailTypeDef = TypedDict(
+    "_OptionalStackResourceDetailTypeDef",
+    {
+        "StackName": str,
+        "StackId": str,
+        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "Metadata": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
-StackResourceTypeDef = TypedDict(
-    "StackResourceTypeDef",
+
+class StackResourceDetailTypeDef(
+    _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
+):
+    pass
+
+
+_RequiredStackResourceTypeDef = TypedDict(
+    "_RequiredStackResourceTypeDef",
     {
-        "StackName": str,
-        "StackId": str,
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
         "ResourceType": str,
         "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceTypeDef = TypedDict(
+    "_OptionalStackResourceTypeDef",
+    {
+        "StackName": str,
+        "StackId": str,
+        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
-StackResourceSummaryTypeDef = TypedDict(
-    "StackResourceSummaryTypeDef",
+
+class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
+    pass
+
+
+_RequiredStackResourceSummaryTypeDef = TypedDict(
+    "_RequiredStackResourceSummaryTypeDef",
     {
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceSummaryTypeDef = TypedDict(
+    "_OptionalStackResourceSummaryTypeDef",
+    {
+        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
+
+class StackResourceSummaryTypeDef(
+    _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
+):
+    pass
+
+
 StackSetTypeDef = TypedDict(
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
@@ -2918,28 +3091,30 @@
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "AutoDeployment": AutoDeploymentOutputTypeDef,
         "PermissionModel": PermissionModelsType,
         "OrganizationalUnitIds": List[str],
         "ManagedExecution": ManagedExecutionOutputTypeDef,
         "Regions": List[str],
     },
+    total=False,
 )
 
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
     {
         "OperationId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
         "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
     },
+    total=False,
 )
 
 StackSetOperationTypeDef = TypedDict(
     "StackSetOperationTypeDef",
     {
         "OperationId": str,
         "StackSetId": str,
@@ -2952,65 +3127,67 @@
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "DeploymentTargets": DeploymentTargetsOutputTypeDef,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
     },
+    total=False,
 )
 
 ValidateTemplateOutputTypeDef = TypedDict(
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
         "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierOutputTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
         "FailureMode": HookFailureModeType,
         "TypeName": str,
         "TypeVersionId": str,
         "TypeConfigurationVersionId": str,
         "TargetDetails": ChangeSetHookTargetDetailsTypeDef,
     },
+    total=False,
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -3019,41 +3196,41 @@
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
         "Warnings": WarningsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
     "ListStackInstanceResourceDriftsOutputTypeDef",
     {
         "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3062,44 +3239,56 @@
         "ResourceType": str,
         "Replacement": ReplacementType,
         "Scope": List[ResourceAttributeType],
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
-StackTypeDef = TypedDict(
-    "StackTypeDef",
+_RequiredStackTypeDef = TypedDict(
+    "_RequiredStackTypeDef",
     {
-        "StackId": str,
         "StackName": str,
+        "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackTypeDef = TypedDict(
+    "_OptionalStackTypeDef",
+    {
+        "StackId": str,
         "ChangeSetId": str,
         "Description": str,
         "Parameters": List[ParameterOutputTypeDef],
-        "CreationTime": datetime,
         "DeletionTime": datetime,
         "LastUpdatedTime": datetime,
         "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
-        "StackStatus": StackStatusType,
         "StackStatusReason": str,
         "DisableRollback": bool,
         "NotificationARNs": List[str],
         "TimeoutInMinutes": int,
         "Capabilities": List[CapabilityType],
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
         "Tags": List[TagOutputTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
     },
+    total=False,
 )
 
+
+class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+    pass
+
+
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
     },
 )
@@ -3266,114 +3455,115 @@
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
         "HookInvocationCount": int,
         "ResourceChange": ResourceChangeTypeDef,
     },
+    total=False,
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
@@ -3392,10 +3582,10 @@
         "Tags": List[TagOutputTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/type_defs.pyi` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -78,175 +78,175 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActivateTypeOutputTypeDef",
     "AutoDeploymentOutputTypeDef",
     "AutoDeploymentTypeDef",
     "TypeConfigurationIdentifierOutputTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
+    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
+    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
     "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
     "ParameterOutputTypeDef",
     "TagOutputTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
+    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
     "LoggingConfigOutputTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
+    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
+    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
+    "GetTemplateOutputTypeDef",
     "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
     "WarningsTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListChangeSetsInputRequestTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListImportsOutputTypeDef",
     "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
     "ManagedExecutionOutputTypeDef",
+    "ModuleInfoResponseMetadataTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
+    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
+    "ResponseMetadataTypeDef",
     "RollbackTriggerOutputTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
+    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
+    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
     "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "UpdateTerminationProtectionInputRequestTypeDef",
-    "ValidateTemplateInputRequestTypeDef",
-    "StackSetOperationResultSummaryTypeDef",
-    "ActivateTypeInputRequestTypeDef",
-    "RegisterTypeInputRequestTypeDef",
-    "ActivateTypeOutputTypeDef",
-    "CreateChangeSetOutputTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
-    "CreateStackSetOutputTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
-    "DescribePublisherOutputTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
-    "DetectStackDriftOutputTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
-    "GetStackPolicyOutputTypeDef",
-    "GetTemplateOutputTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListImportsOutputTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
-    "PublishTypeOutputTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
-    "RollbackStackOutputTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "TestTypeOutputTypeDef",
     "UpdateStackInstancesOutputTypeDef",
     "UpdateStackOutputTypeDef",
     "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionInputRequestTypeDef",
     "UpdateTerminationProtectionOutputTypeDef",
+    "ValidateTemplateInputRequestTypeDef",
+    "StackSetOperationResultSummaryTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "ActivateTypeInputRequestTypeDef",
+    "RegisterTypeInputRequestTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
     "UpdateStackSetInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
@@ -313,49 +313,49 @@
 
 AccountGateResultTypeDef = TypedDict(
     "AccountGateResultTypeDef",
     {
         "Status": AccountGateStatusType,
         "StatusReason": str,
     },
+    total=False,
 )
 
 AccountLimitTypeDef = TypedDict(
     "AccountLimitTypeDef",
     {
         "Name": str,
         "Value": int,
     },
+    total=False,
 )
 
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoDeploymentOutputTypeDef = TypedDict(
     "AutoDeploymentOutputTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
     },
+    total=False,
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
@@ -368,14 +368,15 @@
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
         "TypeConfigurationArn": str,
         "Type": ThirdPartyTypeType,
         "TypeName": str,
     },
+    total=False,
 )
 
 TypeConfigurationIdentifierTypeDef = TypedDict(
     "TypeConfigurationIdentifierTypeDef",
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
@@ -393,14 +394,15 @@
         "Alias": str,
         "Configuration": str,
         "LastUpdated": datetime,
         "TypeArn": str,
         "TypeName": str,
         "IsDefaultConfiguration": bool,
     },
+    total=False,
 )
 
 _RequiredCancelUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredCancelUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -429,14 +431,15 @@
 ChangeSetHookResourceTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookResourceTargetDetailsTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "ResourceAction": ChangeActionType,
     },
+    total=False,
 )
 
 ChangeSetSummaryTypeDef = TypedDict(
     "ChangeSetSummaryTypeDef",
     {
         "StackId": str,
         "StackName": str,
@@ -447,14 +450,15 @@
         "StatusReason": str,
         "CreationTime": datetime,
         "Description": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
     },
+    total=False,
 )
 
 _RequiredContinueUpdateRollbackInputRequestTypeDef = TypedDict(
     "_RequiredContinueUpdateRollbackInputRequestTypeDef",
     {
         "StackName": str,
     },
@@ -499,14 +503,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -523,22 +536,46 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -591,14 +628,22 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
@@ -618,33 +663,32 @@
     "DeploymentTargetsOutputTypeDef",
     {
         "Accounts": List[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": List[str],
         "AccountFilterType": AccountFilterTypeType,
     },
+    total=False,
 )
 
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -680,14 +724,35 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -708,14 +773,15 @@
     "ParameterOutputTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
         "UsePreviousValue": bool,
         "ResolvedValue": str,
     },
+    total=False,
 )
 
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -726,60 +792,111 @@
     "DescribeOrganizationsAccessInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePublisherInputRequestTypeDef = TypedDict(
     "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
     },
     total=False,
 )
 
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-StackEventTypeDef = TypedDict(
-    "StackEventTypeDef",
+_RequiredStackEventTypeDef = TypedDict(
+    "_RequiredStackEventTypeDef",
     {
         "StackId": str,
         "EventId": str,
         "StackName": str,
+        "Timestamp": datetime,
+    },
+)
+_OptionalStackEventTypeDef = TypedDict(
+    "_OptionalStackEventTypeDef",
+    {
         "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "ResourceType": str,
-        "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
         "ResourceStatusReason": str,
         "ResourceProperties": str,
         "ClientRequestToken": str,
         "HookType": str,
         "HookStatus": HookStatusType,
         "HookStatusReason": str,
         "HookInvocationPoint": Literal["PRE_PROVISION"],
         "HookFailureMode": HookFailureModeType,
     },
+    total=False,
 )
 
+class StackEventTypeDef(_RequiredStackEventTypeDef, _OptionalStackEventTypeDef):
+    pass
+
 _RequiredDescribeStackInstanceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackInstanceInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
     },
@@ -874,14 +991,23 @@
 
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -912,23 +1038,35 @@
     "RequiredActivatedTypeTypeDef",
     {
         "TypeNameAlias": str,
         "OriginalTypeName": str,
         "PublisherId": str,
         "SupportedMajorVersions": List[int],
     },
+    total=False,
 )
 
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
@@ -940,22 +1078,53 @@
 )
 
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
@@ -976,33 +1145,51 @@
 ExportTypeDef = TypedDict(
     "ExportTypeDef",
     {
         "ExportingStackId": str,
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": str,
+        "StagesAvailable": List[TemplateStageType],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TemplateSummaryConfigTypeDef = TypedDict(
     "TemplateSummaryConfigTypeDef",
     {
         "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
@@ -1010,23 +1197,53 @@
 ResourceIdentifierSummaryTypeDef = TypedDict(
     "ResourceIdentifierSummaryTypeDef",
     {
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
+    total=False,
 )
 
 WarningsTypeDef = TypedDict(
     "WarningsTypeDef",
     {
         "UnrecognizedResourceTypes": List[str],
     },
+    total=False,
 )
 
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
@@ -1038,22 +1255,50 @@
 )
 
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
 _RequiredListImportsInputRequestTypeDef = TypedDict(
     "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
 _OptionalListImportsInputRequestTypeDef = TypedDict(
@@ -1065,14 +1310,23 @@
 )
 
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
     "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "OperationId": str,
@@ -1100,14 +1354,34 @@
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
@@ -1128,14 +1402,35 @@
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1150,25 +1445,44 @@
 
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1183,14 +1497,23 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1209,14 +1532,15 @@
         "VersionId": str,
         "IsDefaultVersion": bool,
         "Arn": str,
         "TimeCreated": datetime,
         "Description": str,
         "PublicVersionNumber": str,
     },
+    total=False,
 )
 
 TypeFiltersTypeDef = TypedDict(
     "TypeFiltersTypeDef",
     {
         "Category": CategoryType,
         "PublisherId": str,
@@ -1238,46 +1562,70 @@
         "OriginalTypeName": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
+    total=False,
 )
 
 ManagedExecutionOutputTypeDef = TypedDict(
     "ManagedExecutionOutputTypeDef",
     {
         "Active": bool,
     },
+    total=False,
+)
+
+ModuleInfoResponseMetadataTypeDef = TypedDict(
+    "ModuleInfoResponseMetadataTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
+    total=False,
 )
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
     },
+    total=False,
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
 )
 
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
+    total=False,
 )
 
 PhysicalResourceIdContextKeyValuePairTypeDef = TypedDict(
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1301,14 +1649,22 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1335,21 +1691,49 @@
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
     },
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
+    },
 )
 
 RollbackTriggerOutputTypeDef = TypedDict(
     "RollbackTriggerOutputTypeDef",
     {
         "Arn": str,
         "Type": str,
@@ -1380,14 +1764,22 @@
 )
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalSetStackPolicyInputRequestTypeDef = TypedDict(
@@ -1423,14 +1815,22 @@
 
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1444,84 +1844,160 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationSummaryTypeDef = TypedDict(
-    "StackDriftInformationSummaryTypeDef",
+StackDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackDriftInformationResponseMetadataTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
         "LastCheckTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StackDriftInformationTypeDef = TypedDict(
-    "StackDriftInformationTypeDef",
+_RequiredStackDriftInformationSummaryTypeDef = TypedDict(
+    "_RequiredStackDriftInformationSummaryTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+    },
+)
+_OptionalStackDriftInformationSummaryTypeDef = TypedDict(
+    "_OptionalStackDriftInformationSummaryTypeDef",
+    {
+        "LastCheckTimestamp": datetime,
+    },
+    total=False,
+)
+
+class StackDriftInformationSummaryTypeDef(
+    _RequiredStackDriftInformationSummaryTypeDef, _OptionalStackDriftInformationSummaryTypeDef
+):
+    pass
+
+_RequiredStackDriftInformationTypeDef = TypedDict(
+    "_RequiredStackDriftInformationTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
+    },
+)
+_OptionalStackDriftInformationTypeDef = TypedDict(
+    "_OptionalStackDriftInformationTypeDef",
+    {
         "LastCheckTimestamp": datetime,
     },
+    total=False,
 )
 
+class StackDriftInformationTypeDef(
+    _RequiredStackDriftInformationTypeDef, _OptionalStackDriftInformationTypeDef
+):
+    pass
+
 StackInstanceComprehensiveStatusTypeDef = TypedDict(
     "StackInstanceComprehensiveStatusTypeDef",
     {
         "DetailedStatus": StackInstanceDetailedStatusType,
     },
+    total=False,
 )
 
-StackResourceDriftInformationTypeDef = TypedDict(
-    "StackResourceDriftInformationTypeDef",
+_RequiredStackResourceDriftInformationTypeDef = TypedDict(
+    "_RequiredStackResourceDriftInformationTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
+    },
+)
+_OptionalStackResourceDriftInformationTypeDef = TypedDict(
+    "_OptionalStackResourceDriftInformationTypeDef",
+    {
         "LastCheckTimestamp": datetime,
     },
+    total=False,
 )
 
-StackResourceDriftInformationSummaryTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryTypeDef",
+class StackResourceDriftInformationTypeDef(
+    _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
+):
+    pass
+
+StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseMetadataTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
+    "_RequiredStackResourceDriftInformationSummaryTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
+    },
+)
+_OptionalStackResourceDriftInformationSummaryTypeDef = TypedDict(
+    "_OptionalStackResourceDriftInformationSummaryTypeDef",
+    {
         "LastCheckTimestamp": datetime,
     },
+    total=False,
 )
 
+class StackResourceDriftInformationSummaryTypeDef(
+    _RequiredStackResourceDriftInformationSummaryTypeDef,
+    _OptionalStackResourceDriftInformationSummaryTypeDef,
+):
+    pass
+
 StackSetDriftDetectionDetailsTypeDef = TypedDict(
     "StackSetDriftDetectionDetailsTypeDef",
     {
         "DriftStatus": StackSetDriftStatusType,
         "DriftDetectionStatus": StackSetDriftDetectionStatusType,
         "LastDriftCheckTimestamp": datetime,
         "TotalStackInstancesCount": int,
         "DriftedStackInstancesCount": int,
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
+    total=False,
 )
 
 StackSetOperationPreferencesOutputTypeDef = TypedDict(
     "StackSetOperationPreferencesOutputTypeDef",
     {
         "RegionConcurrencyType": RegionConcurrencyTypeType,
         "RegionOrder": List[str],
         "FailureToleranceCount": int,
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
+    total=False,
 )
 
 StackSetOperationStatusDetailsTypeDef = TypedDict(
     "StackSetOperationStatusDetailsTypeDef",
     {
         "FailedStackInstancesCount": int,
     },
+    total=False,
 )
 
 _RequiredStopStackSetOperationInputRequestTypeDef = TypedDict(
     "_RequiredStopStackSetOperationInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
@@ -1545,36 +2021,77 @@
     "TemplateParameterTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "NoEcho": bool,
         "Description": str,
     },
+    total=False,
 )
 
 TestTypeInputRequestTypeDef = TypedDict(
     "TestTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": ThirdPartyTypeType,
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -1586,14 +2103,24 @@
         "Account": str,
         "Region": str,
         "Status": StackSetOperationResultStatusType,
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
+    total=False,
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
@@ -1628,313 +2155,22 @@
 )
 
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
-    {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
-    {
-        "TemplateBody": str,
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
-    {
-        "Imports": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "TypeConfigurationIdentifier": TypeConfigurationIdentifierOutputTypeDef,
     },
+    total=False,
 )
 
 BatchDescribeTypeConfigurationsInputRequestTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     {
         "TypeConfigurationIdentifiers": Sequence[TypeConfigurationIdentifierTypeDef],
     },
@@ -1942,22 +2178,23 @@
 
 ChangeSetHookTargetDetailsTypeDef = TypedDict(
     "ChangeSetHookTargetDetailsTypeDef",
     {
         "TargetType": Literal["RESOURCE"],
         "ResourceTargetDetails": ChangeSetHookResourceTargetDetailsTypeDef,
     },
+    total=False,
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2155,169 +2392,14 @@
 )
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
-    {
-        "ExportName": str,
-    },
-)
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
-):
-    pass
-
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
@@ -2417,15 +2499,15 @@
     pass
 
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2451,24 +2533,24 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSummaryInputRequestTypeDef = TypedDict(
     "GetTemplateSummaryInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2490,15 +2572,15 @@
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
     _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef,
@@ -2537,15 +2619,15 @@
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
@@ -2577,27 +2659,27 @@
     pass
 
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2613,15 +2695,15 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StackSetSummaryTypeDef = TypedDict(
     "StackSetSummaryTypeDef",
     {
         "StackSetName": str,
@@ -2630,112 +2712,148 @@
         "Status": StackSetStatusType,
         "AutoDeployment": AutoDeploymentOutputTypeDef,
         "PermissionModel": PermissionModelsType,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "ManagedExecution": ManagedExecutionOutputTypeDef,
     },
+    total=False,
 )
 
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "ParameterType": str,
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
+    total=False,
 )
 
-StackInstanceResourceDriftsSummaryTypeDef = TypedDict(
-    "StackInstanceResourceDriftsSummaryTypeDef",
+_RequiredStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_RequiredStackInstanceResourceDriftsSummaryTypeDef",
     {
         "StackId": str,
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
-        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
         "ResourceType": str,
-        "PropertyDifferences": List[PropertyDifferenceTypeDef],
         "StackResourceDriftStatus": StackResourceDriftStatusType,
         "Timestamp": datetime,
     },
 )
+_OptionalStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_OptionalStackInstanceResourceDriftsSummaryTypeDef",
+    {
+        "PhysicalResourceId": str,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
+    },
+    total=False,
+)
 
-StackResourceDriftTypeDef = TypedDict(
-    "StackResourceDriftTypeDef",
+class StackInstanceResourceDriftsSummaryTypeDef(
+    _RequiredStackInstanceResourceDriftsSummaryTypeDef,
+    _OptionalStackInstanceResourceDriftsSummaryTypeDef,
+):
+    pass
+
+_RequiredStackResourceDriftTypeDef = TypedDict(
+    "_RequiredStackResourceDriftTypeDef",
     {
         "StackId": str,
         "LogicalResourceId": str,
+        "ResourceType": str,
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "Timestamp": datetime,
+    },
+)
+_OptionalStackResourceDriftTypeDef = TypedDict(
+    "_OptionalStackResourceDriftTypeDef",
+    {
         "PhysicalResourceId": str,
         "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
-        "ResourceType": str,
         "ExpectedProperties": str,
         "ActualProperties": str,
         "PropertyDifferences": List[PropertyDifferenceTypeDef],
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "Timestamp": datetime,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
+class StackResourceDriftTypeDef(
+    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
+):
+    pass
+
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
+    total=False,
 )
 
 RollbackConfigurationOutputTypeDef = TypedDict(
     "RollbackConfigurationOutputTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
         "MonitoringTimeInMinutes": int,
     },
+    total=False,
 )
 
 RollbackConfigurationResponseMetadataTypeDef = TypedDict(
     "RollbackConfigurationResponseMetadataTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
-StackSummaryTypeDef = TypedDict(
-    "StackSummaryTypeDef",
+_RequiredStackSummaryTypeDef = TypedDict(
+    "_RequiredStackSummaryTypeDef",
     {
-        "StackId": str,
         "StackName": str,
-        "TemplateDescription": str,
         "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackSummaryTypeDef = TypedDict(
+    "_OptionalStackSummaryTypeDef",
+    {
+        "StackId": str,
+        "TemplateDescription": str,
         "LastUpdatedTime": datetime,
         "DeletionTime": datetime,
-        "StackStatus": StackStatusType,
         "StackStatusReason": str,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationSummaryTypeDef,
     },
+    total=False,
 )
 
+class StackSummaryTypeDef(_RequiredStackSummaryTypeDef, _OptionalStackSummaryTypeDef):
+    pass
+
 StackInstanceSummaryTypeDef = TypedDict(
     "StackInstanceSummaryTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
@@ -2743,14 +2861,15 @@
         "StatusReason": str,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
+    total=False,
 )
 
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "StackSetId": str,
         "Region": str,
@@ -2761,65 +2880,97 @@
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "StatusReason": str,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
+    total=False,
 )
 
-StackResourceDetailTypeDef = TypedDict(
-    "StackResourceDetailTypeDef",
+_RequiredStackResourceDetailTypeDef = TypedDict(
+    "_RequiredStackResourceDetailTypeDef",
     {
-        "StackName": str,
-        "StackId": str,
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceDetailTypeDef = TypedDict(
+    "_OptionalStackResourceDetailTypeDef",
+    {
+        "StackName": str,
+        "StackId": str,
+        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "Metadata": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
-StackResourceTypeDef = TypedDict(
-    "StackResourceTypeDef",
+class StackResourceDetailTypeDef(
+    _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
+):
+    pass
+
+_RequiredStackResourceTypeDef = TypedDict(
+    "_RequiredStackResourceTypeDef",
     {
-        "StackName": str,
-        "StackId": str,
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
         "ResourceType": str,
         "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceTypeDef = TypedDict(
+    "_OptionalStackResourceTypeDef",
+    {
+        "StackName": str,
+        "StackId": str,
+        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "Description": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
-StackResourceSummaryTypeDef = TypedDict(
-    "StackResourceSummaryTypeDef",
+class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
+    pass
+
+_RequiredStackResourceSummaryTypeDef = TypedDict(
+    "_RequiredStackResourceSummaryTypeDef",
     {
         "LogicalResourceId": str,
-        "PhysicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceSummaryTypeDef = TypedDict(
+    "_OptionalStackResourceSummaryTypeDef",
+    {
+        "PhysicalResourceId": str,
         "ResourceStatusReason": str,
         "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
+class StackResourceSummaryTypeDef(
+    _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
+):
+    pass
+
 StackSetTypeDef = TypedDict(
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
@@ -2833,28 +2984,30 @@
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "AutoDeployment": AutoDeploymentOutputTypeDef,
         "PermissionModel": PermissionModelsType,
         "OrganizationalUnitIds": List[str],
         "ManagedExecution": ManagedExecutionOutputTypeDef,
         "Regions": List[str],
     },
+    total=False,
 )
 
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
     {
         "OperationId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
         "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
     },
+    total=False,
 )
 
 StackSetOperationTypeDef = TypedDict(
     "StackSetOperationTypeDef",
     {
         "OperationId": str,
         "StackSetId": str,
@@ -2867,65 +3020,67 @@
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "DeploymentTargets": DeploymentTargetsOutputTypeDef,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
     },
+    total=False,
 )
 
 ValidateTemplateOutputTypeDef = TypedDict(
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
         "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierOutputTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
         "FailureMode": HookFailureModeType,
         "TypeName": str,
         "TypeVersionId": str,
         "TypeConfigurationVersionId": str,
         "TargetDetails": ChangeSetHookTargetDetailsTypeDef,
     },
+    total=False,
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -2934,41 +3089,41 @@
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
         "Warnings": WarningsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
     "ListStackInstanceResourceDriftsOutputTypeDef",
     {
         "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -2977,44 +3132,54 @@
         "ResourceType": str,
         "Replacement": ReplacementType,
         "Scope": List[ResourceAttributeType],
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
+    total=False,
 )
 
-StackTypeDef = TypedDict(
-    "StackTypeDef",
+_RequiredStackTypeDef = TypedDict(
+    "_RequiredStackTypeDef",
     {
-        "StackId": str,
         "StackName": str,
+        "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackTypeDef = TypedDict(
+    "_OptionalStackTypeDef",
+    {
+        "StackId": str,
         "ChangeSetId": str,
         "Description": str,
         "Parameters": List[ParameterOutputTypeDef],
-        "CreationTime": datetime,
         "DeletionTime": datetime,
         "LastUpdatedTime": datetime,
         "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
-        "StackStatus": StackStatusType,
         "StackStatusReason": str,
         "DisableRollback": bool,
         "NotificationARNs": List[str],
         "TimeoutInMinutes": int,
         "Capabilities": List[CapabilityType],
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
         "Tags": List[TagOutputTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
     },
+    total=False,
 )
 
+class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+    pass
+
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
     },
 )
@@ -3173,114 +3338,115 @@
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
         "HookInvocationCount": int,
         "ResourceChange": ResourceChangeTypeDef,
     },
+    total=False,
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
@@ -3299,10 +3465,10 @@
         "Tags": List[TagOutputTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.py` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation/waiter.pyi` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/PKG-INFO` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.10
-Summary: Type annotations for boto3.CloudFormation 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudFormation 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudformation"></a>
 
 # mypy-boto3-cloudformation
 
 [![PyPI - mypy-boto3-cloudformation](https://img.shields.io/pypi/v/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudformation?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -580,175 +580,175 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ActivateTypeOutputTypeDef,
     AutoDeploymentOutputTypeDef,
     AutoDeploymentTypeDef,
     TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
+    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
+    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
+    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
     DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
     ParameterOutputTypeDef,
     TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
+    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
     LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
+    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
+    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
+    GetTemplateOutputTypeDef,
     TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
     WarningsTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
+    ListImportsOutputTypeDef,
     ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
     ManagedExecutionOutputTypeDef,
+    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
+    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
+    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
+    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
+    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
+    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
+    StackResourceDriftInformationResponseMetadataTypeDef,
+    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
     StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    UpdateTerminationProtectionInputRequestTypeDef,
-    ValidateTemplateInputRequestTypeDef,
-    StackSetOperationResultSummaryTypeDef,
-    ActivateTypeInputRequestTypeDef,
-    RegisterTypeInputRequestTypeDef,
-    ActivateTypeOutputTypeDef,
-    CreateChangeSetOutputTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
-    CreateStackSetOutputTypeDef,
-    DeleteStackInstancesOutputTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
-    DescribePublisherOutputTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
-    DetectStackDriftOutputTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
-    GetStackPolicyOutputTypeDef,
-    GetTemplateOutputTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListImportsOutputTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
-    PublishTypeOutputTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
-    RollbackStackOutputTypeDef,
-    SetTypeConfigurationOutputTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     TestTypeOutputTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionInputRequestTypeDef,
     UpdateTerminationProtectionOutputTypeDef,
+    ValidateTemplateInputRequestTypeDef,
+    StackSetOperationResultSummaryTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    ActivateTypeInputRequestTypeDef,
+    RegisterTypeInputRequestTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
     UpdateStackSetInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.10/mypy_boto3_cloudformation.egg-info/SOURCES.txt` & `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.10/setup.py` & `mypy-boto3-cloudformation-1.28.12/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudformation",
-    version="1.28.10",
+    version="1.28.12",
     packages=["mypy_boto3_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFormation 1.28.10 service generated with"
-        " mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.CloudFormation 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

