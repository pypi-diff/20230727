# Comparing `tmp/mypy-boto3-ssm-1.28.0.tar.gz` & `tmp/mypy-boto3-ssm-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-1.28.0.tar", last modified: Thu Jul  6 21:00:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-1.28.12.tar", last modified: Thu Jul 27 11:49:42 2023, max compression
```

## Comparing `mypy-boto3-ssm-1.28.0.tar` & `mypy-boto3-ssm-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.630441 mypy-boto3-ssm-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46020 2023-07-06 21:00:42.630441 mypy-boto3-ssm-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44551 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.614441 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131264 2023-07-06 20:56:21.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   131071 2023-07-06 20:56:20.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28094 2023-07-06 20:56:22.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28092 2023-07-06 20:56:21.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59280 2023-07-06 20:56:21.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    59231 2023-07-06 20:56:21.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   204479 2023-07-06 20:56:31.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   204251 2023-07-06 20:56:28.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-06 20:56:21.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-06 20:56:21.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.630441 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46020 2023-07-06 21:00:42.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 21:00:42.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:42.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:42.000000 mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:42.630441 mypy-boto3-ssm-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:56:19.000000 mypy-boto3-ssm-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47440 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    45969 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.693330 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131264 2023-07-27 11:47:18.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131071 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-27 11:47:21.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-07-27 11:47:21.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59186 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59137 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   217858 2023-07-27 11:47:28.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   217610 2023-07-27 11:47:23.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47440 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:16.000000 mypy-boto3-ssm-1.28.12/setup.py
```

### Comparing `mypy-boto3-ssm-1.28.0/LICENSE` & `mypy-boto3-ssm-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/PKG-INFO` & `mypy-boto3-ssm-1.28.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.0
-Summary: Type annotations for boto3.SSM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ssm"></a>
 
 # mypy-boto3-ssm
 
 [![PyPI - mypy-boto3-ssm](https://img.shields.io/pypi/v/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -643,288 +643,307 @@
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    AlarmOutputTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
-    AssociationStatusTypeDef,
-    TargetTypeDef,
+    AssociationStatusOutputTypeDef,
+    TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    AssociationStatusTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
+    CloudWatchOutputConfigOutputTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
-    NotificationConfigTypeDef,
+    NotificationConfigOutputTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
-    CreateActivationResultTypeDef,
+    TargetTypeDef,
     DocumentRequiresTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
-    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
-    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
-    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
-    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
+    DocumentRequiresOutputTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
+    DocumentReviewCommentSourceOutputTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
-    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
-    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
-    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
-    LoggingInfoTypeDef,
+    LoggingInfoOutputTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
+    MetadataValueOutputTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
+    S3OutputLocationOutputTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
-    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LoggingInfoTypeDef,
+    MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
+    MaintenanceWindowLambdaParametersOutputTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
+    NotificationConfigTypeDef,
+    MaintenanceWindowStepFunctionsParametersOutputTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
+    OpsItemDataValueOutputTypeDef,
     OpsItemIdentityTypeDef,
-    PaginatorConfigTypeDef,
+    OpsItemNotificationOutputTypeDef,
+    RelatedOpsItemOutputTypeDef,
     ParameterInlinePolicyTypeDef,
+    PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
+    ResourceDataSyncOrganizationalUnitOutputTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
+    ResourceDataSyncDestinationDataSharingOutputTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
-    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
-    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
-    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
-    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
+    CreateActivationResultTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
+    CreateOpsItemResponseTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
+    DeleteParametersResultTypeDef,
+    DeletePatchBaselineResultTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesResultTypeDef,
+    GetCalendarStateResponseTypeDef,
+    GetConnectionStatusResponseTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
+    GetMaintenanceWindowResultTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListInventoryEntriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
+    ResumeSessionResponseTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
+    StartSessionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
+    UnlabelParameterVersionResultTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     AssociationTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
     UpdateDocumentRequestRequestTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
     GetCommandInvocationResultTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
-    MaintenanceWindowRunCommandParametersTypeDef,
+    MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
     PutComplianceItemsRequestRequestTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
-    DocumentIdentifierTypeDef,
-    GetDocumentResultTypeDef,
-    OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
-    OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
-    GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeActivationsRequestRequestTypeDef,
+    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
     DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
@@ -966,142 +985,158 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribePatchBaselinesResultTypeDef,
     PatchGroupPatchBaselineMappingTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
+    DocumentIdentifierTypeDef,
+    GetDocumentResultTypeDef,
     DocumentDescriptionTypeDef,
     ListDocumentsRequestListDocumentsPaginateTypeDef,
     ListDocumentsRequestRequestTypeDef,
     DocumentReviewerResponseSourceTypeDef,
     DocumentReviewsTypeDef,
     ListDocumentVersionsResultTypeDef,
     EffectivePatchTypeDef,
     GetCommandInvocationRequestCommandExecutedWaitTypeDef,
     InventoryGroupTypeDef,
     ListInventoryEntriesRequestRequestTypeDef,
     GetInventoryRequestGetInventoryPaginateTypeDef,
     GetInventoryRequestRequestTypeDef,
+    GetOpsMetadataResultTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
+    InstanceAssociationOutputLocationOutputTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
     InventoryItemSchemaTypeDef,
     PutInventoryRequestRequestTypeDef,
     InventoryResultEntityTypeDef,
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
+    MaintenanceWindowRunCommandParametersTypeDef,
     OpsEntityTypeDef,
+    OpsItemSummaryTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
+    OpsItemTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
+    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
+    ResourceDataSyncS3DestinationOutputTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
+    TargetLocationOutputTypeDef,
     SendCommandRequestRequestTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
-    ListDocumentsResultTypeDef,
-    DescribeOpsItemsResponseTypeDef,
-    GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
+    ListDocumentsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
     DocumentMetadataResponseInfoTypeDef,
     UpdateDocumentMetadataRequestRequestTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     InventoryAggregatorTypeDef,
     DescribeInstanceInformationResultTypeDef,
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
+    DescribeOpsItemsResponseTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
+    GetOpsItemResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
+    PatchRuleOutputTypeDef,
     PatchRuleTypeDef,
-    ResourceDataSyncSourceTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
+    ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
+    RunbookOutputTypeDef,
+    StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
     CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
     StartAutomationExecutionRequestRequestTypeDef,
-    StepExecutionTypeDef,
     UpdateAssociationRequestRequestTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
-    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
-    ResourceDataSyncItemTypeDef,
     CreateAssociationResultTypeDef,
     DescribeAssociationResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
+    GetPatchBaselineResultTypeDef,
+    UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
-    GetPatchBaselineResultTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
-    UpdatePatchBaselineResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-1.28.0/README.md` & `mypy-boto3-ssm-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ssm"></a>
 
 # mypy-boto3-ssm
 
 [![PyPI - mypy-boto3-ssm](https://img.shields.io/pypi/v/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -611,288 +611,307 @@
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    AlarmOutputTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
-    AssociationStatusTypeDef,
-    TargetTypeDef,
+    AssociationStatusOutputTypeDef,
+    TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    AssociationStatusTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
+    CloudWatchOutputConfigOutputTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
-    NotificationConfigTypeDef,
+    NotificationConfigOutputTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
-    CreateActivationResultTypeDef,
+    TargetTypeDef,
     DocumentRequiresTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
-    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
-    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
-    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
-    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
+    DocumentRequiresOutputTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
+    DocumentReviewCommentSourceOutputTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
-    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
-    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
-    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
-    LoggingInfoTypeDef,
+    LoggingInfoOutputTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
+    MetadataValueOutputTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
+    S3OutputLocationOutputTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
-    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LoggingInfoTypeDef,
+    MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
+    MaintenanceWindowLambdaParametersOutputTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
+    NotificationConfigTypeDef,
+    MaintenanceWindowStepFunctionsParametersOutputTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
+    OpsItemDataValueOutputTypeDef,
     OpsItemIdentityTypeDef,
-    PaginatorConfigTypeDef,
+    OpsItemNotificationOutputTypeDef,
+    RelatedOpsItemOutputTypeDef,
     ParameterInlinePolicyTypeDef,
+    PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
+    ResourceDataSyncOrganizationalUnitOutputTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
+    ResourceDataSyncDestinationDataSharingOutputTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
-    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
-    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
-    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
-    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
+    CreateActivationResultTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
+    CreateOpsItemResponseTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
+    DeleteParametersResultTypeDef,
+    DeletePatchBaselineResultTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesResultTypeDef,
+    GetCalendarStateResponseTypeDef,
+    GetConnectionStatusResponseTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
+    GetMaintenanceWindowResultTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListInventoryEntriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
+    ResumeSessionResponseTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
+    StartSessionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
+    UnlabelParameterVersionResultTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     AssociationTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
     UpdateDocumentRequestRequestTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
     GetCommandInvocationResultTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
-    MaintenanceWindowRunCommandParametersTypeDef,
+    MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
     PutComplianceItemsRequestRequestTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
-    DocumentIdentifierTypeDef,
-    GetDocumentResultTypeDef,
-    OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
-    OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
-    GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeActivationsRequestRequestTypeDef,
+    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
     DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
@@ -934,142 +953,158 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribePatchBaselinesResultTypeDef,
     PatchGroupPatchBaselineMappingTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
+    DocumentIdentifierTypeDef,
+    GetDocumentResultTypeDef,
     DocumentDescriptionTypeDef,
     ListDocumentsRequestListDocumentsPaginateTypeDef,
     ListDocumentsRequestRequestTypeDef,
     DocumentReviewerResponseSourceTypeDef,
     DocumentReviewsTypeDef,
     ListDocumentVersionsResultTypeDef,
     EffectivePatchTypeDef,
     GetCommandInvocationRequestCommandExecutedWaitTypeDef,
     InventoryGroupTypeDef,
     ListInventoryEntriesRequestRequestTypeDef,
     GetInventoryRequestGetInventoryPaginateTypeDef,
     GetInventoryRequestRequestTypeDef,
+    GetOpsMetadataResultTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
+    InstanceAssociationOutputLocationOutputTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
     InventoryItemSchemaTypeDef,
     PutInventoryRequestRequestTypeDef,
     InventoryResultEntityTypeDef,
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
+    MaintenanceWindowRunCommandParametersTypeDef,
     OpsEntityTypeDef,
+    OpsItemSummaryTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
+    OpsItemTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
+    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
+    ResourceDataSyncS3DestinationOutputTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
+    TargetLocationOutputTypeDef,
     SendCommandRequestRequestTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
-    ListDocumentsResultTypeDef,
-    DescribeOpsItemsResponseTypeDef,
-    GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
+    ListDocumentsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
     DocumentMetadataResponseInfoTypeDef,
     UpdateDocumentMetadataRequestRequestTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     InventoryAggregatorTypeDef,
     DescribeInstanceInformationResultTypeDef,
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
+    DescribeOpsItemsResponseTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
+    GetOpsItemResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
+    PatchRuleOutputTypeDef,
     PatchRuleTypeDef,
-    ResourceDataSyncSourceTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
+    ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
+    RunbookOutputTypeDef,
+    StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
     CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
     StartAutomationExecutionRequestRequestTypeDef,
-    StepExecutionTypeDef,
     UpdateAssociationRequestRequestTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
-    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
-    ResourceDataSyncItemTypeDef,
     CreateAssociationResultTypeDef,
     DescribeAssociationResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
+    GetPatchBaselineResultTypeDef,
+    UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
-    GetPatchBaselineResultTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
-    UpdatePatchBaselineResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/__init__.py` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/__init__.pyi` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/__main__.py` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSM 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SSM 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/client.py` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/client.pyi` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/literals.py` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -634,14 +634,15 @@
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
@@ -720,26 +721,28 @@
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

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/literals.pyi` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -632,14 +632,15 @@
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
@@ -718,26 +719,28 @@
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

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/paginator.py` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
         """
 
 
@@ -289,15 +289,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 
@@ -308,15 +308,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAssociationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 
@@ -326,15 +326,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAutomationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 
@@ -346,15 +346,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAutomationStepExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 
@@ -364,60 +364,60 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 
 class DescribeEffectiveInstanceAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEffectiveInstanceAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
         """
 
 
 class DescribeEffectivePatchesForPatchBaselinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
     """
 
     def paginate(
-        self, *, BaselineId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BaselineId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEffectivePatchesForPatchBaselineResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
         """
 
 
 class DescribeInstanceAssociationsStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstanceAssociationsStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
         """
 
 
@@ -428,30 +428,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 
 class DescribeInstancePatchStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstancePatchStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
         """
 
 
@@ -462,15 +462,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 
@@ -481,30 +481,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 
 class DescribeInventoryDeletionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
-        self, *, DeletionId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeletionId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInventoryDeletionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
         """
 
 
@@ -516,15 +516,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 
@@ -535,15 +535,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 
@@ -554,15 +554,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 
@@ -575,15 +575,15 @@
     def paginate(
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 
@@ -594,15 +594,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 
@@ -613,15 +613,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 
@@ -631,15 +631,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 
@@ -650,15 +650,15 @@
     """
 
     def paginate(
         self,
         *,
         Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 
@@ -668,15 +668,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
         """
 
 
@@ -687,15 +687,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeparameterspaginator)
         """
 
 
@@ -705,15 +705,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 
@@ -723,15 +723,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
         """
 
 
@@ -743,15 +743,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 
@@ -762,15 +762,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describesessionspaginator)
         """
 
 
@@ -782,15 +782,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventorypaginator)
         """
 
 
@@ -802,15 +802,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventoryschemapaginator)
         """
 
 
@@ -823,15 +823,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getopssummarypaginator)
         """
 
 
@@ -842,15 +842,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparameterhistorypaginator)
         """
 
 
@@ -863,45 +863,45 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparametersbypathpaginator)
         """
 
 
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
         """
 
 
 class ListAssociationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
     """
 
     def paginate(
-        self, *, AssociationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AssociationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
         """
 
 
@@ -911,15 +911,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
         """
 
 
@@ -932,15 +932,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 
@@ -952,15 +952,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCommandsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandspaginator)
         """
 
 
@@ -972,15 +972,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 
@@ -990,30 +990,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 
 class ListDocumentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
         """
 
 
@@ -1024,15 +1024,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentspaginator)
         """
 
 
@@ -1042,15 +1042,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
         """
 
 
@@ -1061,15 +1061,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 
@@ -1079,15 +1079,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
         """
 
 
@@ -1097,28 +1097,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
 
 
 class ListResourceDataSyncPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
     """
 
     def paginate(
-        self, *, SyncType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SyncType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDataSyncResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/paginator.pyi` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
         """
 
 class DescribeAssociationExecutionTargetsPaginator(Paginator):
@@ -285,15 +285,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 class DescribeAssociationExecutionsPaginator(Paginator):
@@ -303,15 +303,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAssociationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 class DescribeAutomationExecutionsPaginator(Paginator):
@@ -320,15 +320,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAutomationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 class DescribeAutomationStepExecutionsPaginator(Paginator):
@@ -339,15 +339,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAutomationStepExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 class DescribeAvailablePatchesPaginator(Paginator):
@@ -356,57 +356,57 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 class DescribeEffectiveInstanceAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEffectiveInstanceAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
         """
 
 class DescribeEffectivePatchesForPatchBaselinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
     """
 
     def paginate(
-        self, *, BaselineId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BaselineId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEffectivePatchesForPatchBaselineResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
         """
 
 class DescribeInstanceAssociationsStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstanceAssociationsStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
         """
 
 class DescribeInstanceInformationPaginator(Paginator):
@@ -416,29 +416,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 class DescribeInstancePatchStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstancePatchStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
         """
 
 class DescribeInstancePatchStatesForPatchGroupPaginator(Paginator):
@@ -448,15 +448,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 class DescribeInstancePatchesPaginator(Paginator):
@@ -466,29 +466,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 class DescribeInventoryDeletionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
-        self, *, DeletionId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeletionId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeInventoryDeletionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionTaskInvocationsPaginator(Paginator):
@@ -499,15 +499,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionTasksPaginator(Paginator):
@@ -517,15 +517,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionsPaginator(Paginator):
@@ -535,15 +535,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 class DescribeMaintenanceWindowSchedulePaginator(Paginator):
@@ -555,15 +555,15 @@
     def paginate(
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 class DescribeMaintenanceWindowTargetsPaginator(Paginator):
@@ -573,15 +573,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 class DescribeMaintenanceWindowTasksPaginator(Paginator):
@@ -591,15 +591,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 class DescribeMaintenanceWindowsPaginator(Paginator):
@@ -608,15 +608,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 class DescribeMaintenanceWindowsForTargetPaginator(Paginator):
@@ -626,15 +626,15 @@
     """
 
     def paginate(
         self,
         *,
         Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 class DescribeOpsItemsPaginator(Paginator):
@@ -643,15 +643,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
         """
 
 class DescribeParametersPaginator(Paginator):
@@ -661,15 +661,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeparameterspaginator)
         """
 
 class DescribePatchBaselinesPaginator(Paginator):
@@ -678,15 +678,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 class DescribePatchGroupsPaginator(Paginator):
@@ -695,15 +695,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
         """
 
 class DescribePatchPropertiesPaginator(Paginator):
@@ -714,15 +714,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 class DescribeSessionsPaginator(Paginator):
@@ -732,15 +732,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describesessionspaginator)
         """
 
 class GetInventoryPaginator(Paginator):
@@ -751,15 +751,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventorypaginator)
         """
 
 class GetInventorySchemaPaginator(Paginator):
@@ -770,15 +770,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventoryschemapaginator)
         """
 
 class GetOpsSummaryPaginator(Paginator):
@@ -790,15 +790,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getopssummarypaginator)
         """
 
 class GetParameterHistoryPaginator(Paginator):
@@ -808,15 +808,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparameterhistorypaginator)
         """
 
 class GetParametersByPathPaginator(Paginator):
@@ -828,43 +828,43 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparametersbypathpaginator)
         """
 
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
         """
 
 class ListAssociationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
     """
 
     def paginate(
-        self, *, AssociationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AssociationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
         """
 
 class ListAssociationsPaginator(Paginator):
@@ -873,15 +873,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
         """
 
 class ListCommandInvocationsPaginator(Paginator):
@@ -893,15 +893,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 class ListCommandsPaginator(Paginator):
@@ -912,15 +912,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCommandsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandspaginator)
         """
 
 class ListComplianceItemsPaginator(Paginator):
@@ -931,15 +931,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 class ListComplianceSummariesPaginator(Paginator):
@@ -948,29 +948,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 class ListDocumentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
         """
 
 class ListDocumentsPaginator(Paginator):
@@ -980,15 +980,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentspaginator)
         """
 
 class ListOpsItemEventsPaginator(Paginator):
@@ -997,15 +997,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
         """
 
 class ListOpsItemRelatedItemsPaginator(Paginator):
@@ -1015,15 +1015,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 class ListOpsMetadataPaginator(Paginator):
@@ -1032,15 +1032,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
         """
 
 class ListResourceComplianceSummariesPaginator(Paginator):
@@ -1049,27 +1049,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
 
 class ListResourceDataSyncPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
     """
 
     def paginate(
-        self, *, SyncType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SyncType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDataSyncResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/type_defs.py` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     from mypy_boto3_ssm.type_defs import AccountSharingInfoTypeDef
 
     data: AccountSharingInfoTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationExecutionFilterKeyType,
     AssociationExecutionTargetsFilterKeyType,
     AssociationFilterKeyType,
     AssociationFilterOperatorTypeType,
@@ -99,291 +101,309 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSharingInfoTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
+    "AlarmOutputTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
-    "AssociationStatusTypeDef",
-    "TargetTypeDef",
+    "AssociationStatusOutputTypeDef",
+    "TargetOutputTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
+    "AssociationStatusTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
-    "CancelMaintenanceWindowExecutionResultTypeDef",
+    "CloudWatchOutputConfigOutputTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
-    "NotificationConfigTypeDef",
+    "NotificationConfigOutputTypeDef",
+    "ComplianceExecutionSummaryOutputTypeDef",
     "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
-    "CreateActivationResultTypeDef",
+    "TargetTypeDef",
     "DocumentRequiresTypeDef",
-    "CreateMaintenanceWindowResultTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
-    "CreateOpsItemResponseTypeDef",
     "MetadataValueTypeDef",
-    "CreateOpsMetadataResultTypeDef",
-    "CreatePatchBaselineResultTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
-    "DeleteMaintenanceWindowResultTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
     "DeleteParametersRequestRequestTypeDef",
-    "DeleteParametersResultTypeDef",
     "DeletePatchBaselineRequestRequestTypeDef",
-    "DeletePatchBaselineResultTypeDef",
     "DeleteResourceDataSyncRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeregisterManagedInstanceRequestRequestTypeDef",
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
     "DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     "DescribeActivationsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAssociationRequestRequestTypeDef",
     "StepExecutionFilterTypeDef",
     "PatchOrchestratorFilterTypeDef",
     "PatchTypeDef",
     "DescribeDocumentPermissionRequestRequestTypeDef",
     "DescribeDocumentRequestRequestTypeDef",
-    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     "InstanceAssociationTypeDef",
-    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
-    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
-    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
     "OpsItemFilterTypeDef",
     "ParameterStringFilterTypeDef",
     "ParametersFilterTypeDef",
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
-    "DescribePatchGroupStateResultTypeDef",
-    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
-    "DescribePatchPropertiesResultTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
+    "DocumentRequiresOutputTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
+    "DocumentReviewCommentSourceOutputTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
-    "GetCalendarStateResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetCommandInvocationRequestRequestTypeDef",
     "GetConnectionStatusRequestRequestTypeDef",
-    "GetConnectionStatusResponseTypeDef",
     "GetDefaultPatchBaselineRequestRequestTypeDef",
-    "GetDefaultPatchBaselineResultTypeDef",
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionResultTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
-    "GetMaintenanceWindowResultTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
-    "LoggingInfoTypeDef",
+    "LoggingInfoOutputTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
+    "MetadataValueOutputTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
-    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "GetPatchBaselineForPatchGroupResultTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
+    "S3OutputLocationOutputTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
-    "LabelParameterVersionResultTypeDef",
-    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationVersionsRequestRequestTypeDef",
     "ListDocumentMetadataHistoryRequestRequestTypeDef",
-    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     "ListDocumentVersionsRequestRequestTypeDef",
-    "ListInventoryEntriesResultTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LoggingInfoTypeDef",
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
     "MaintenanceWindowLambdaParametersTypeDef",
+    "NotificationConfigTypeDef",
+    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
+    "OpsItemDataValueOutputTypeDef",
     "OpsItemIdentityTypeDef",
-    "PaginatorConfigTypeDef",
+    "OpsItemNotificationOutputTypeDef",
+    "RelatedOpsItemOutputTypeDef",
     "ParameterInlinePolicyTypeDef",
+    "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
-    "PutInventoryResultTypeDef",
-    "PutParameterResultTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
-    "RegisterDefaultPatchBaselineResultTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
+    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
+    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeSessionRequestRequestTypeDef",
-    "ResumeSessionResponseTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
-    "StartAutomationExecutionResultTypeDef",
-    "StartChangeRequestExecutionResultTypeDef",
     "StartSessionRequestRequestTypeDef",
-    "StartSessionResponseTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionRequestRequestTypeDef",
-    "UnlabelParameterVersionResultTypeDef",
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     "UpdateMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowResultTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
-    "UpdateOpsMetadataResultTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
-    "DescribeDocumentPermissionResponseTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "PutParameterRequestRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
+    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "CancelMaintenanceWindowExecutionResultTypeDef",
+    "CreateActivationResultTypeDef",
+    "CreateMaintenanceWindowResultTypeDef",
+    "CreateOpsItemResponseTypeDef",
+    "CreateOpsMetadataResultTypeDef",
+    "CreatePatchBaselineResultTypeDef",
+    "DeleteMaintenanceWindowResultTypeDef",
+    "DeleteParametersResultTypeDef",
+    "DeletePatchBaselineResultTypeDef",
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
+    "DescribeDocumentPermissionResponseTypeDef",
+    "DescribePatchGroupStateResultTypeDef",
+    "DescribePatchPropertiesResultTypeDef",
+    "GetCalendarStateResponseTypeDef",
+    "GetConnectionStatusResponseTypeDef",
+    "GetDefaultPatchBaselineResultTypeDef",
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    "GetMaintenanceWindowResultTypeDef",
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    "LabelParameterVersionResultTypeDef",
+    "ListInventoryEntriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PutInventoryResultTypeDef",
+    "PutParameterResultTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
+    "ResumeSessionResponseTypeDef",
+    "StartAutomationExecutionResultTypeDef",
+    "StartChangeRequestExecutionResultTypeDef",
+    "StartSessionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
+    "UnlabelParameterVersionResultTypeDef",
+    "UpdateMaintenanceWindowResultTypeDef",
+    "UpdateOpsMetadataResultTypeDef",
     "AssociationTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
-    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
-    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListAssociationsRequestRequestTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     "GetCommandInvocationResultTypeDef",
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
-    "ListCommandsRequestListCommandsPaginateTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
-    "MaintenanceWindowRunCommandParametersTypeDef",
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     "ComplianceItemTypeDef",
     "PutComplianceItemsRequestRequestTypeDef",
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "CreateDocumentRequestRequestTypeDef",
-    "DocumentIdentifierTypeDef",
-    "GetDocumentResultTypeDef",
-    "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
-    "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
-    "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
-    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     "DescribeActivationsRequestRequestTypeDef",
+    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
+    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
     "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
@@ -425,142 +445,158 @@
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribePatchBaselinesResultTypeDef",
     "PatchGroupPatchBaselineMappingTypeDef",
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
     "UpdateDocumentDefaultVersionResultTypeDef",
+    "DocumentIdentifierTypeDef",
+    "GetDocumentResultTypeDef",
     "DocumentDescriptionTypeDef",
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     "ListDocumentsRequestRequestTypeDef",
     "DocumentReviewerResponseSourceTypeDef",
     "DocumentReviewsTypeDef",
     "ListDocumentVersionsResultTypeDef",
     "EffectivePatchTypeDef",
     "GetCommandInvocationRequestCommandExecutedWaitTypeDef",
     "InventoryGroupTypeDef",
     "ListInventoryEntriesRequestRequestTypeDef",
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     "GetInventoryRequestRequestTypeDef",
+    "GetOpsMetadataResultTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
+    "InstanceAssociationOutputLocationOutputTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
     "InventoryItemSchemaTypeDef",
     "PutInventoryRequestRequestTypeDef",
     "InventoryResultEntityTypeDef",
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
+    "MaintenanceWindowRunCommandParametersTypeDef",
     "OpsEntityTypeDef",
+    "OpsItemSummaryTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
+    "OpsItemTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
+    "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
+    "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
+    "ResourceDataSyncS3DestinationOutputTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
+    "TargetLocationOutputTypeDef",
     "SendCommandRequestRequestTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
     "ListCommandInvocationsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
-    "ListDocumentsResultTypeDef",
-    "DescribeOpsItemsResponseTypeDef",
-    "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
+    "ListDocumentsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
     "DocumentMetadataResponseInfoTypeDef",
     "UpdateDocumentMetadataRequestRequestTypeDef",
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     "InventoryAggregatorTypeDef",
     "DescribeInstanceInformationResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
+    "DescribeOpsItemsResponseTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
+    "GetOpsItemResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
+    "PatchRuleOutputTypeDef",
     "PatchRuleTypeDef",
-    "ResourceDataSyncSourceTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
+    "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
+    "CreateAssociationBatchRequestEntryOutputTypeDef",
+    "RunbookOutputTypeDef",
+    "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
     "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
     "StartAutomationExecutionRequestRequestTypeDef",
-    "StepExecutionTypeDef",
     "UpdateAssociationRequestRequestTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
+    "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
-    "ResourceDataSyncItemTypeDef",
     "CreateAssociationResultTypeDef",
     "DescribeAssociationResultTypeDef",
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
+    "GetPatchBaselineResultTypeDef",
+    "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
-    "GetPatchBaselineResultTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
-    "UpdatePatchBaselineResultTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
@@ -569,22 +605,37 @@
     {
         "AccountId": str,
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+AlarmOutputTypeDef = TypedDict(
+    "AlarmOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -602,60 +653,61 @@
         "OpsItemId": str,
         "AssociationType": str,
         "ResourceType": str,
         "ResourceUri": str,
     },
 )
 
-AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AssociationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociationOverviewTypeDef = TypedDict(
     "AssociationOverviewTypeDef",
     {
         "Status": str,
         "DetailedStatus": str,
         "AssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
+_RequiredAssociationStatusOutputTypeDef = TypedDict(
+    "_RequiredAssociationStatusOutputTypeDef",
     {
         "Date": datetime,
         "Name": AssociationStatusNameType,
         "Message": str,
     },
 )
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
+_OptionalAssociationStatusOutputTypeDef = TypedDict(
+    "_OptionalAssociationStatusOutputTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
-
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+class AssociationStatusOutputTypeDef(
+    _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
 ):
     pass
 
-
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
     total=False,
 )
 
 AssociationExecutionFilterTypeDef = TypedDict(
     "AssociationExecutionFilterTypeDef",
     {
@@ -686,14 +738,35 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
+    {
+        "Date": Union[datetime, str],
+        "Name": AssociationStatusNameType,
+        "Message": str,
+    },
+)
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
+    {
+        "AdditionalInfo": str,
+    },
+    total=False,
+)
+
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+):
+    pass
+
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -768,34 +841,33 @@
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
-
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "CancelMaintenanceWindowExecutionResultTypeDef",
+CloudWatchOutputConfigOutputTypeDef = TypedDict(
+    "CloudWatchOutputConfigOutputTypeDef",
     {
-        "WindowExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CloudWatchLogGroupName": str,
+        "CloudWatchOutputEnabled": bool,
     },
+    total=False,
 )
 
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
@@ -826,46 +898,65 @@
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
     total=False,
 )
 
-NotificationConfigTypeDef = TypedDict(
-    "NotificationConfigTypeDef",
+NotificationConfigOutputTypeDef = TypedDict(
+    "NotificationConfigOutputTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": List[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
+_RequiredComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryOutputTypeDef",
+    {
+        "ExecutionTime": datetime,
+    },
+)
+_OptionalComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryOutputTypeDef",
+    {
+        "ExecutionId": str,
+        "ExecutionType": str,
+    },
+    total=False,
+)
+
+class ComplianceExecutionSummaryOutputTypeDef(
+    _RequiredComplianceExecutionSummaryOutputTypeDef,
+    _OptionalComplianceExecutionSummaryOutputTypeDef,
+):
+    pass
+
 _RequiredComplianceExecutionSummaryTypeDef = TypedDict(
     "_RequiredComplianceExecutionSummaryTypeDef",
     {
-        "ExecutionTime": datetime,
+        "ExecutionTime": Union[datetime, str],
     },
 )
 _OptionalComplianceExecutionSummaryTypeDef = TypedDict(
     "_OptionalComplianceExecutionSummaryTypeDef",
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
-
 class ComplianceExecutionSummaryTypeDef(
     _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
 ):
     pass
 
-
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
 )
@@ -875,21 +966,19 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
-
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -913,21 +1002,21 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateActivationResultTypeDef = TypedDict(
-    "CreateActivationResultTypeDef",
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
-        "ActivationId": str,
-        "ActivationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Values": Sequence[str],
     },
+    total=False,
 )
 
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
@@ -938,27 +1027,17 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
-
-CreateMaintenanceWindowResultTypeDef = TypedDict(
-    "CreateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -975,47 +1054,22 @@
 RelatedOpsItemTypeDef = TypedDict(
     "RelatedOpsItemTypeDef",
     {
         "OpsItemId": str,
     },
 )
 
-CreateOpsItemResponseTypeDef = TypedDict(
-    "CreateOpsItemResponseTypeDef",
-    {
-        "OpsItemId": str,
-        "OpsItemArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetadataValueTypeDef = TypedDict(
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-CreateOpsMetadataResultTypeDef = TypedDict(
-    "CreateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePatchBaselineResultTypeDef = TypedDict(
-    "CreatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1041,21 +1095,19 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
-
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1064,36 +1116,26 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
-
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-DeleteMaintenanceWindowResultTypeDef = TypedDict(
-    "DeleteMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOpsMetadataRequestRequestTypeDef = TypedDict(
     "DeleteOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 
@@ -1107,60 +1149,41 @@
 DeleteParametersRequestRequestTypeDef = TypedDict(
     "DeleteParametersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
-DeleteParametersResultTypeDef = TypedDict(
-    "DeleteParametersResultTypeDef",
-    {
-        "DeletedParameters": List[str],
-        "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePatchBaselineRequestRequestTypeDef = TypedDict(
     "DeletePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-DeletePatchBaselineResultTypeDef = TypedDict(
-    "DeletePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
-
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1177,23 +1200,14 @@
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
@@ -1201,57 +1215,47 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
-
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
-DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeActivationsFilterTypeDef = TypedDict(
     "DescribeActivationsFilterTypeDef",
     {
         "FilterKey": DescribeActivationsFilterKeysType,
         "FilterValues": Sequence[str],
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
 DescribeAssociationRequestRequestTypeDef = TypedDict(
     "DescribeAssociationRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationId": str,
         "AssociationVersion": str,
@@ -1318,22 +1322,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1341,43 +1343,19 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
-    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1385,55 +1363,31 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
     },
     total=False,
 )
 
-_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "BaselineId": str,
-    },
-)
-_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
-    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
@@ -1441,44 +1395,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
-    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1486,22 +1416,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1553,43 +1481,19 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
-
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
-
-_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-    },
-)
-_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
-    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1597,22 +1501,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1624,30 +1526,19 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
-
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
-
-DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    {
-        "DeletionId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1753,21 +1644,19 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
-
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1787,57 +1676,14 @@
 DescribePatchGroupStateRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupStateRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 
-DescribePatchGroupStateResultTypeDef = TypedDict(
-    "DescribePatchGroupStateResultTypeDef",
-    {
-        "Instances": int,
-        "InstancesWithInstalledPatches": int,
-        "InstancesWithInstalledOtherPatches": int,
-        "InstancesWithInstalledPendingRebootPatches": int,
-        "InstancesWithInstalledRejectedPatches": int,
-        "InstancesWithMissingPatches": int,
-        "InstancesWithFailedPatches": int,
-        "InstancesWithNotApplicablePatches": int,
-        "InstancesWithUnreportedNotApplicablePatches": int,
-        "InstancesWithCriticalNonCompliantPatches": int,
-        "InstancesWithSecurityNonCompliantPatches": int,
-        "InstancesWithOtherNonCompliantPatches": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "OperatingSystem": OperatingSystemType,
-        "Property": PatchPropertyType,
-    },
-)
-_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "PatchSet": PatchSetType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
-    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribePatchPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -1847,31 +1693,20 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
-
-DescribePatchPropertiesResultTypeDef = TypedDict(
-    "DescribePatchPropertiesResultTypeDef",
-    {
-        "Properties": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1901,14 +1736,35 @@
         "Type": DocumentParameterTypeType,
         "Description": str,
         "DefaultValue": str,
     },
     total=False,
 )
 
+_RequiredDocumentRequiresOutputTypeDef = TypedDict(
+    "_RequiredDocumentRequiresOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalDocumentRequiresOutputTypeDef = TypedDict(
+    "_OptionalDocumentRequiresOutputTypeDef",
+    {
+        "Version": str,
+        "RequireType": str,
+        "VersionName": str,
+    },
+    total=False,
+)
+
+class DocumentRequiresOutputTypeDef(
+    _RequiredDocumentRequiresOutputTypeDef, _OptionalDocumentRequiresOutputTypeDef
+):
+    pass
+
 ReviewInformationTypeDef = TypedDict(
     "ReviewInformationTypeDef",
     {
         "ReviewedTime": datetime,
         "Status": ReviewStatusType,
         "Reviewer": str,
     },
@@ -1928,14 +1784,23 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+DocumentReviewCommentSourceOutputTypeDef = TypedDict(
+    "DocumentReviewCommentSourceOutputTypeDef",
+    {
+        "Type": Literal["Comment"],
+        "Content": str,
+    },
+    total=False,
+)
+
 DocumentReviewCommentSourceTypeDef = TypedDict(
     "DocumentReviewCommentSourceTypeDef",
     {
         "Type": Literal["Comment"],
         "Content": str,
     },
     total=False,
@@ -1995,31 +1860,19 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
-
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
-
-GetCalendarStateResponseTypeDef = TypedDict(
-    "GetCalendarStateResponseTypeDef",
-    {
-        "State": CalendarStateType,
-        "AtTime": str,
-        "NextTransitionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -2036,66 +1889,35 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
-
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
-GetConnectionStatusResponseTypeDef = TypedDict(
-    "GetConnectionStatusResponseTypeDef",
-    {
-        "Target": str,
-        "Status": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetDefaultPatchBaselineRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-GetDefaultPatchBaselineResultTypeDef = TypedDict(
-    "GetDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": str,
-        "SnapshotDownloadUrl": str,
-        "Product": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -2104,21 +1926,19 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
-
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2126,37 +1946,24 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
-
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
-
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    {
-        "TypeName": str,
-        "Aggregator": bool,
-        "SubType": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInventorySchemaRequestRequestTypeDef = TypedDict(
     "GetInventorySchemaRequestRequestTypeDef",
     {
         "TypeName": str,
         "NextToken": str,
         "MaxResults": int,
         "Aggregator": bool,
@@ -2168,149 +1975,93 @@
 GetMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskIds": List[str],
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "InvocationId": str,
     },
 )
 
-GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskExecutionId": str,
-        "InvocationId": str,
-        "ExecutionId": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "Parameters": str,
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "OwnerInformation": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 
-MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+MaintenanceWindowTaskParameterValueExpressionOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-GetMaintenanceWindowResultTypeDef = TypedDict(
-    "GetMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "NextExecutionTime": str,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-_RequiredLoggingInfoTypeDef = TypedDict(
-    "_RequiredLoggingInfoTypeDef",
+_RequiredLoggingInfoOutputTypeDef = TypedDict(
+    "_RequiredLoggingInfoOutputTypeDef",
     {
         "S3BucketName": str,
         "S3Region": str,
     },
 )
-_OptionalLoggingInfoTypeDef = TypedDict(
-    "_OptionalLoggingInfoTypeDef",
+_OptionalLoggingInfoOutputTypeDef = TypedDict(
+    "_OptionalLoggingInfoOutputTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
-class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
+class LoggingInfoOutputTypeDef(
+    _RequiredLoggingInfoOutputTypeDef, _OptionalLoggingInfoOutputTypeDef
+):
     pass
 
-
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -2318,20 +2069,26 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+MetadataValueOutputTypeDef = TypedDict(
+    "MetadataValueOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
 
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
@@ -2340,49 +2097,24 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
-
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
-
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
-    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetParameterHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterHistoryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterHistoryRequestRequestTypeDef = TypedDict(
@@ -2391,43 +2123,39 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
-
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2450,81 +2178,54 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
-GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
     {
-        "ResourceArn": str,
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
     },
 )
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
 
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
@@ -2533,22 +2234,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2580,14 +2279,24 @@
     {
         "DetailedStatus": str,
         "InstanceAssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
+S3OutputLocationOutputTypeDef = TypedDict(
+    "S3OutputLocationOutputTypeDef",
+    {
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+    },
+    total=False,
+)
+
 S3OutputLocationTypeDef = TypedDict(
     "S3OutputLocationTypeDef",
     {
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
@@ -2634,19 +2343,17 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
-
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
-
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2656,21 +2363,19 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
-
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
-
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2678,53 +2383,20 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
-
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
-
-LabelParameterVersionResultTypeDef = TypedDict(
-    "LabelParameterVersionResultTypeDef",
-    {
-        "InvalidLabels": List[str],
-        "ParameterVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
-    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2732,22 +2404,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2757,44 +2427,20 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
-    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2802,35 +2448,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListInventoryEntriesResultTypeDef = TypedDict(
-    "ListInventoryEntriesResultTypeDef",
-    {
-        "TypeName": str,
-        "InstanceId": str,
-        "SchemaVersion": str,
-        "CaptureTime": str,
-        "Entries": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2861,23 +2492,14 @@
         "LastModifiedDate": datetime,
         "LastModifiedUser": str,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
-    {
-        "SyncType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceDataSyncRequestRequestTypeDef = TypedDict(
     "ListResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2888,42 +2510,106 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
+_RequiredLoggingInfoTypeDef = TypedDict(
+    "_RequiredLoggingInfoTypeDef",
+    {
+        "S3BucketName": str,
+        "S3Region": str,
+    },
+)
+_OptionalLoggingInfoTypeDef = TypedDict(
+    "_OptionalLoggingInfoTypeDef",
+    {
+        "S3KeyPrefix": str,
+    },
+    total=False,
+)
+
+class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
+    pass
+
+MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Dict[str, List[str]],
+    },
+    total=False,
+)
+
 MaintenanceWindowAutomationParametersTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+MaintenanceWindowLambdaParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
+    {
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": bytes,
     },
     total=False,
 )
 
 MaintenanceWindowLambdaParametersTypeDef = TypedDict(
     "MaintenanceWindowLambdaParametersTypeDef",
     {
         "ClientContext": str,
         "Qualifier": str,
-        "Payload": bytes,
+        "Payload": Union[str, bytes, IO[Any], StreamingBody],
+    },
+    total=False,
+)
+
+NotificationConfigTypeDef = TypedDict(
+    "NotificationConfigTypeDef",
+    {
+        "NotificationArn": str,
+        "NotificationEvents": Sequence[NotificationEventType],
+        "NotificationType": NotificationTypeType,
+    },
+    total=False,
+)
+
+MaintenanceWindowStepFunctionsParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
+    {
+        "Input": str,
+        "Name": str,
     },
     total=False,
 )
 
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
 )
 
+MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    {
+        "Values": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredModifyDocumentPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDocumentPermissionRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionType": Literal["Share"],
     },
 )
@@ -2933,81 +2619,84 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
-
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
 )
 
+OpsItemDataValueOutputTypeDef = TypedDict(
+    "OpsItemDataValueOutputTypeDef",
+    {
+        "Value": str,
+        "Type": OpsItemDataTypeType,
+    },
+    total=False,
+)
+
 OpsItemIdentityTypeDef = TypedDict(
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+OpsItemNotificationOutputTypeDef = TypedDict(
+    "OpsItemNotificationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Arn": str,
     },
     total=False,
 )
 
+RelatedOpsItemOutputTypeDef = TypedDict(
+    "RelatedOpsItemOutputTypeDef",
+    {
+        "OpsItemId": str,
+    },
+)
+
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
     total=False,
 )
 
-PatchFilterTypeDef = TypedDict(
-    "PatchFilterTypeDef",
+PatchFilterOutputTypeDef = TypedDict(
+    "PatchFilterOutputTypeDef",
     {
         "Key": PatchFilterKeyType,
-        "Values": Sequence[str],
-    },
-)
-
-PutInventoryResultTypeDef = TypedDict(
-    "PutInventoryResultTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Values": List[str],
     },
 )
 
-PutParameterResultTypeDef = TypedDict(
-    "PutParameterResultTypeDef",
+PatchFilterTypeDef = TypedDict(
+    "PatchFilterTypeDef",
     {
-        "Version": int,
-        "Tier": ParameterTierType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": PatchFilterKeyType,
+        "Values": Sequence[str],
     },
 )
 
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -3019,78 +2708,34 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyHash": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
@@ -3099,58 +2744,53 @@
 ResetServiceSettingRequestRequestTypeDef = TypedDict(
     "ResetServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
     },
 )
 
+ResourceDataSyncOrganizationalUnitOutputTypeDef = TypedDict(
+    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
+    {
+        "OrganizationalUnitId": str,
+    },
+    total=False,
+)
+
 ResourceDataSyncOrganizationalUnitTypeDef = TypedDict(
     "ResourceDataSyncOrganizationalUnitTypeDef",
     {
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-ResourceDataSyncDestinationDataSharingTypeDef = TypedDict(
-    "ResourceDataSyncDestinationDataSharingTypeDef",
+ResourceDataSyncDestinationDataSharingOutputTypeDef = TypedDict(
+    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
     {
         "DestinationDataSharingType": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResourceDataSyncDestinationDataSharingTypeDef = TypedDict(
+    "ResourceDataSyncDestinationDataSharingTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DestinationDataSharingType": str,
     },
+    total=False,
 )
 
 ResumeSessionRequestRequestTypeDef = TypedDict(
     "ResumeSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-ResumeSessionResponseTypeDef = TypedDict(
-    "ResumeSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendAutomationSignalRequestRequestTypeDef = TypedDict(
     "_RequiredSendAutomationSignalRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
         "SignalType": SignalTypeType,
     },
 )
@@ -3158,22 +2798,20 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
-
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -3182,30 +2820,14 @@
 StartAssociationsOnceRequestRequestTypeDef = TypedDict(
     "StartAssociationsOnceRequestRequestTypeDef",
     {
         "AssociationIds": Sequence[str],
     },
 )
 
-StartAutomationExecutionResultTypeDef = TypedDict(
-    "StartAutomationExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartChangeRequestExecutionResultTypeDef = TypedDict(
-    "StartChangeRequestExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 _OptionalStartSessionRequestRequestTypeDef = TypedDict(
@@ -3214,86 +2836,55 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
-
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnlabelParameterVersionRequestRequestTypeDef = TypedDict(
     "UnlabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "ParameterVersion": int,
         "Labels": Sequence[str],
     },
 )
 
-UnlabelParameterVersionResultTypeDef = TypedDict(
-    "UnlabelParameterVersionResultTypeDef",
-    {
-        "RemovedLabels": List[str],
-        "InvalidLabels": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDocumentDefaultVersionRequestRequestTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
     },
 )
@@ -3319,88 +2910,49 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateMaintenanceWindowResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
 
-UpdateOpsMetadataResultTypeDef = TypedDict(
-    "UpdateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateServiceSettingRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
         "SettingValue": str,
     },
 )
 
-DescribeDocumentPermissionResponseTypeDef = TypedDict(
-    "DescribeDocumentPermissionResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivationTypeDef = TypedDict(
     "ActivationTypeDef",
     {
         "ActivationId": str,
         "Description": str,
         "DefaultInstanceName": str,
         "IamRole": str,
         "RegistrationLimit": int,
         "RegistrationsCount": int,
         "ExpirationDate": datetime,
         "Expired": bool,
         "CreatedDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
@@ -3430,30 +2982,20 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -3469,20 +3011,37 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
-
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
+_RequiredAlarmConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAlarmConfigurationOutputTypeDef",
+    {
+        "Alarms": List[AlarmOutputTypeDef],
+    },
+)
+_OptionalAlarmConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAlarmConfigurationOutputTypeDef",
+    {
+        "IgnorePollAlarmFailure": bool,
+    },
+    total=False,
+)
+
+class AlarmConfigurationOutputTypeDef(
+    _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
@@ -3490,204 +3049,485 @@
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
-
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
-
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
+AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
+        "AssociationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociationTypeDef = TypedDict(
-    "AssociationTypeDef",
+CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "CancelMaintenanceWindowExecutionResultTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationId": str,
-        "AssociationVersion": str,
-        "DocumentVersion": str,
-        "Targets": List[TargetTypeDef],
-        "LastExecutionDate": datetime,
-        "Overview": AssociationOverviewTypeDef,
-        "ScheduleExpression": str,
-        "AssociationName": str,
-        "ScheduleOffset": int,
-        "TargetMaps": List[Dict[str, List[str]]],
+        "WindowExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+CreateActivationResultTypeDef = TypedDict(
+    "CreateActivationResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "ActivationId": str,
+        "ActivationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+
+CreateMaintenanceWindowResultTypeDef = TypedDict(
+    "CreateMaintenanceWindowResultTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateOpsItemResponseTypeDef = TypedDict(
+    "CreateOpsItemResponseTypeDef",
+    {
+        "OpsItemId": str,
+        "OpsItemArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
+CreateOpsMetadataResultTypeDef = TypedDict(
+    "CreateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+CreatePatchBaselineResultTypeDef = TypedDict(
+    "CreatePatchBaselineResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+
+DeleteMaintenanceWindowResultTypeDef = TypedDict(
+    "DeleteMaintenanceWindowResultTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DeleteParametersResultTypeDef = TypedDict(
+    "DeleteParametersResultTypeDef",
+    {
+        "DeletedParameters": List[str],
+        "InvalidParameters": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
+DeletePatchBaselineResultTypeDef = TypedDict(
+    "DeletePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-MaintenanceWindowTargetTypeDef = TypedDict(
-    "MaintenanceWindowTargetTypeDef",
+DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": List[TargetTypeDef],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetTypeDef],
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+
+DescribeDocumentPermissionResponseTypeDef = TypedDict(
+    "DescribeDocumentPermissionResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchGroupStateResultTypeDef = TypedDict(
+    "DescribePatchGroupStateResultTypeDef",
+    {
+        "Instances": int,
+        "InstancesWithInstalledPatches": int,
+        "InstancesWithInstalledOtherPatches": int,
+        "InstancesWithInstalledPendingRebootPatches": int,
+        "InstancesWithInstalledRejectedPatches": int,
+        "InstancesWithMissingPatches": int,
+        "InstancesWithFailedPatches": int,
+        "InstancesWithNotApplicablePatches": int,
+        "InstancesWithUnreportedNotApplicablePatches": int,
+        "InstancesWithCriticalNonCompliantPatches": int,
+        "InstancesWithSecurityNonCompliantPatches": int,
+        "InstancesWithOtherNonCompliantPatches": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchPropertiesResultTypeDef = TypedDict(
+    "DescribePatchPropertiesResultTypeDef",
+    {
+        "Properties": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalendarStateResponseTypeDef = TypedDict(
+    "GetCalendarStateResponseTypeDef",
+    {
+        "State": CalendarStateType,
+        "AtTime": str,
+        "NextTransitionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectionStatusResponseTypeDef = TypedDict(
+    "GetConnectionStatusResponseTypeDef",
+    {
+        "Target": str,
+        "Status": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDefaultPatchBaselineResultTypeDef = TypedDict(
+    "GetDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
     {
+        "InstanceId": str,
+        "SnapshotId": str,
+        "SnapshotDownloadUrl": str,
+        "Product": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskIds": List[str],
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskExecutionId": str,
+        "InvocationId": str,
+        "ExecutionId": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "Parameters": str,
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "OwnerInformation": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowResultTypeDef = TypedDict(
+    "GetMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "ClientToken": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "NextExecutionTime": str,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
+LabelParameterVersionResultTypeDef = TypedDict(
+    "LabelParameterVersionResultTypeDef",
+    {
+        "InvalidLabels": List[str],
+        "ParameterVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListInventoryEntriesResultTypeDef = TypedDict(
+    "ListInventoryEntriesResultTypeDef",
+    {
+        "TypeName": str,
+        "InstanceId": str,
+        "SchemaVersion": str,
+        "CaptureTime": str,
+        "Entries": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutInventoryResultTypeDef = TypedDict(
+    "PutInventoryResultTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutParameterResultTypeDef = TypedDict(
+    "PutParameterResultTypeDef",
+    {
+        "Version": int,
+        "Tier": ParameterTierType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyHash": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
     {
-        "WindowId": str,
         "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+
+RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "OwnerInformation": str,
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResumeSessionResponseTypeDef = TypedDict(
+    "ResumeSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAutomationExecutionResultTypeDef = TypedDict(
+    "StartAutomationExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartChangeRequestExecutionResultTypeDef = TypedDict(
+    "StartChangeRequestExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnlabelParameterVersionResultTypeDef = TypedDict(
+    "UnlabelParameterVersionResultTypeDef",
+    {
+        "RemovedLabels": List[str],
+        "InvalidLabels": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceWindowResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "Replace": bool,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateOpsMetadataResultTypeDef = TypedDict(
+    "UpdateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
+AssociationTypeDef = TypedDict(
+    "AssociationTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationId": str,
+        "AssociationVersion": str,
+        "DocumentVersion": str,
+        "Targets": List[TargetOutputTypeDef],
+        "LastExecutionDate": datetime,
+        "Overview": AssociationOverviewTypeDef,
+        "ScheduleExpression": str,
+        "AssociationName": str,
+        "ScheduleOffset": int,
+        "TargetMaps": List[Dict[str, List[str]]],
+    },
+    total=False,
+)
 
+MaintenanceWindowTargetTypeDef = TypedDict(
+    "MaintenanceWindowTargetTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": List[TargetOutputTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+    },
+    total=False,
+)
 
 UpdateMaintenanceWindowTargetResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTargetResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "AssociationId": str,
-        },
-    )
-)
-_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "Filters": Sequence[AssociationExecutionFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
@@ -3696,22 +3536,20 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3720,38 +3558,14 @@
         "DetailedStatus": str,
         "LastExecutionDate": datetime,
         "OutputSource": OutputSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "AssociationId": str,
-        "ExecutionId": str,
-    },
-)
-_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef",
     {
         "AssociationId": str,
         "ExecutionId": str,
     },
 )
@@ -3761,41 +3575,39 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
-
-ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
-    {
-        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
+    },
+)
+
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3808,30 +3620,19 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
-
-DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
-    {
-        "Filters": Sequence[AutomationExecutionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -3853,55 +3654,32 @@
         "ExecutionEndDateTime": str,
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "Details": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[CommandFilterTypeDef],
         "Details": bool,
     },
     total=False,
 )
 
-ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCommandsRequestRequestTypeDef = TypedDict(
     "ListCommandsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
@@ -3923,29 +3701,29 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
     },
     total=False,
 )
 
-MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersTypeDef",
+MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     {
         "Comment": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
@@ -3957,15 +3735,15 @@
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Id": str,
         "Title": str,
         "Status": ComplianceStatusType,
         "Severity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
 _RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
     "_RequiredPutComplianceItemsRequestRequestTypeDef",
@@ -3982,73 +3760,42 @@
     {
         "ItemContentHash": str,
         "UploadType": ComplianceUploadTypeType,
     },
     total=False,
 )
 
-
 class PutComplianceItemsRequestRequestTypeDef(
     _RequiredPutComplianceItemsRequestRequestTypeDef,
     _OptionalPutComplianceItemsRequestRequestTypeDef,
 ):
     pass
 
-
-ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "ResourceIds": Sequence[str],
-        "ResourceTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -4088,116 +3835,118 @@
         "ExpirationDate": Union[datetime, str],
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
-
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDocumentRequestRequestTypeDef",
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
-        "Content": str,
-        "Name": str,
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
     },
 )
-_OptionalCreateDocumentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDocumentRequestRequestTypeDef",
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
-        "Requires": Sequence[DocumentRequiresTypeDef],
-        "Attachments": Sequence[AttachmentsSourceTypeDef],
-        "DisplayName": str,
-        "VersionName": str,
-        "DocumentType": DocumentTypeType,
-        "DocumentFormat": DocumentFormatType,
-        "TargetType": str,
-        "Tags": Sequence[TagTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-
-class CreateDocumentRequestRequestTypeDef(
-    _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
 ):
     pass
 
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
 
-DocumentIdentifierTypeDef = TypedDict(
-    "DocumentIdentifierTypeDef",
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
     {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "OwnerInformation": str,
         "Name": str,
-        "CreatedDate": datetime,
-        "DisplayName": str,
-        "Owner": str,
-        "VersionName": str,
-        "PlatformTypes": List[PlatformTypeType],
-        "DocumentVersion": str,
-        "DocumentType": DocumentTypeType,
-        "SchemaVersion": str,
-        "DocumentFormat": DocumentFormatType,
-        "TargetType": str,
-        "Tags": List[TagTypeDef],
-        "Requires": List[DocumentRequiresTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "Author": str,
+        "Description": str,
+        "Replace": bool,
     },
     total=False,
 )
 
-GetDocumentResultTypeDef = TypedDict(
-    "GetDocumentResultTypeDef",
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDocumentRequestRequestTypeDef",
     {
+        "Content": str,
         "Name": str,
-        "CreatedDate": datetime,
+    },
+)
+_OptionalCreateDocumentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDocumentRequestRequestTypeDef",
+    {
+        "Requires": Sequence[DocumentRequiresTypeDef],
+        "Attachments": Sequence[AttachmentsSourceTypeDef],
         "DisplayName": str,
         "VersionName": str,
-        "DocumentVersion": str,
-        "Status": DocumentStatusType,
-        "StatusInformation": str,
-        "Content": str,
         "DocumentType": DocumentTypeType,
         "DocumentFormat": DocumentFormatType,
-        "Requires": List[DocumentRequiresTypeDef],
-        "AttachmentsContent": List[AttachmentContentTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OpsItemSummaryTypeDef = TypedDict(
-    "OpsItemSummaryTypeDef",
-    {
-        "CreatedBy": str,
-        "CreatedTime": datetime,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Priority": int,
-        "Source": str,
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Title": str,
-        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
-        "Category": str,
-        "Severity": str,
-        "OpsItemType": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
+        "TargetType": str,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+class CreateDocumentRequestRequestTypeDef(
+    _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsItemRequestRequestTypeDef",
     {
         "Description": str,
         "Source": str,
         "Title": str,
     },
@@ -4218,50 +3967,19 @@
         "PlannedStartTime": Union[datetime, str],
         "PlannedEndTime": Union[datetime, str],
         "AccountId": str,
     },
     total=False,
 )
 
-
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
-OpsItemTypeDef = TypedDict(
-    "OpsItemTypeDef",
-    {
-        "CreatedBy": str,
-        "OpsItemType": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Notifications": List[OpsItemNotificationTypeDef],
-        "Priority": int,
-        "RelatedOpsItems": List[RelatedOpsItemTypeDef],
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Version": str,
-        "Title": str,
-        "Source": str,
-        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
-        "Category": str,
-        "Severity": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
-        "OpsItemArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalUpdateOpsItemRequestRequestTypeDef = TypedDict(
@@ -4282,21 +4000,19 @@
         "PlannedStartTime": Union[datetime, str],
         "PlannedEndTime": Union[datetime, str],
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -4304,31 +4020,19 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
-GetOpsMetadataResultTypeDef = TypedDict(
-    "GetOpsMetadataResultTypeDef",
-    {
-        "ResourceId": str,
-        "Metadata": Dict[str, MetadataValueTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -4336,36 +4040,384 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+DescribeActivationsRequestRequestTypeDef = TypedDict(
+    "DescribeActivationsRequestRequestTypeDef",
+    {
+        "Filters": Sequence[DescribeActivationsFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
 
 DescribeActivationsRequestDescribeActivationsPaginateTypeDef = TypedDict(
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeActivationsRequestRequestTypeDef = TypedDict(
-    "DescribeActivationsRequestRequestTypeDef",
+_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     {
-        "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "AssociationId": str,
+        "ExecutionId": str,
+    },
+)
+_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "AssociationId": str,
+        },
+    )
+)
+_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "Filters": Sequence[AssociationExecutionFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+):
+    pass
+
+DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    {
+        "Filters": Sequence[AutomationExecutionFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
+    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "BaselineId": str,
+    },
+)
+_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
+    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
+    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+    },
+)
+_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
+    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+):
+    pass
+
+DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    {
+        "DeletionId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "OperatingSystem": OperatingSystemType,
+        "Property": PatchPropertyType,
+    },
+)
+_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "PatchSet": PatchSetType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
+    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+):
+    pass
+
+GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    {
+        "TypeName": str,
+        "Aggregator": bool,
+        "SubType": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "WithDecryption": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
+    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
+    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+):
+    pass
+
+ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    {
+        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "Details": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "ResourceIds": Sequence[str],
+        "ResourceTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
+    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    {
+        "SyncType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
@@ -4373,27 +4425,25 @@
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4403,27 +4453,25 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeAvailablePatchesRequestRequestTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestRequestTypeDef",
     {
@@ -4440,27 +4488,25 @@
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4469,31 +4515,29 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
     TypedDict(
         "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
         {
             "WindowId": str,
             "Targets": Sequence[TargetTypeDef],
             "ResourceType": MaintenanceWindowResourceTypeType,
             "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
+            "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
 DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
@@ -4508,15 +4552,15 @@
     total=False,
 )
 
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchBaselinesRequestRequestTypeDef = TypedDict(
     "DescribePatchBaselinesRequestRequestTypeDef",
     {
@@ -4527,15 +4571,15 @@
     total=False,
 )
 
 DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef = TypedDict(
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchGroupsRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupsRequestRequestTypeDef",
     {
@@ -4547,33 +4591,33 @@
 )
 
 DescribeAvailablePatchesResultTypeDef = TypedDict(
     "DescribeAvailablePatchesResultTypeDef",
     {
         "Patches": List[PatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEffectiveInstanceAssociationsResultTypeDef = TypedDict(
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     {
         "Associations": List[InstanceAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef = TypedDict(
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     {
         "InstanceInformationFilterList": Sequence[InstanceInformationFilterTypeDef],
         "Filters": Sequence[InstanceInformationStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeInstanceInformationRequestRequestTypeDef = TypedDict(
     "DescribeInstanceInformationRequestRequestTypeDef",
     {
@@ -4591,27 +4635,25 @@
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4620,73 +4662,69 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchStatesResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchesResultTypeDef = TypedDict(
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4696,45 +4734,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4743,45 +4777,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4790,45 +4820,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4837,45 +4863,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -4884,27 +4906,25 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeMaintenanceWindowsRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestRequestTypeDef",
     {
@@ -4918,59 +4938,59 @@
 DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef",
     {
         "WindowExecutionTaskInvocationIdentities": List[
             MaintenanceWindowExecutionTaskInvocationIdentityTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionsResultTypeDef",
     {
         "WindowExecutions": List[MaintenanceWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowScheduleResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleResultTypeDef",
     {
         "ScheduledWindowExecutions": List[ScheduledWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsForTargetResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsForTargetResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityForTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef = TypedDict(
     "DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef",
     {
         "OpsItemFilters": Sequence[OpsItemFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeOpsItemsRequestRequestTypeDef = TypedDict(
     "DescribeOpsItemsRequestRequestTypeDef",
     {
@@ -4989,27 +5009,25 @@
 )
 _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef = TypedDict(
     "_OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef",
     {
         "Recursive": bool,
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -5020,28 +5038,26 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeParametersRequestRequestTypeDef = TypedDict(
     "DescribeParametersRequestRequestTypeDef",
     {
@@ -5054,15 +5070,15 @@
 )
 
 DescribePatchBaselinesResultTypeDef = TypedDict(
     "DescribePatchBaselinesResultTypeDef",
     {
         "BaselineIdentities": List[PatchBaselineIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PatchGroupPatchBaselineMappingTypeDef = TypedDict(
     "PatchGroupPatchBaselineMappingTypeDef",
     {
         "PatchGroup": str,
@@ -5077,27 +5093,25 @@
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
         "Filters": Sequence[SessionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -5106,26 +5120,66 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
-
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DocumentIdentifierTypeDef = TypedDict(
+    "DocumentIdentifierTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "Owner": str,
+        "VersionName": str,
+        "PlatformTypes": List[PlatformTypeType],
+        "DocumentVersion": str,
+        "DocumentType": DocumentTypeType,
+        "SchemaVersion": str,
+        "DocumentFormat": DocumentFormatType,
+        "TargetType": str,
+        "Tags": List[TagOutputTypeDef],
+        "Requires": List[DocumentRequiresOutputTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "Author": str,
+    },
+    total=False,
+)
+
+GetDocumentResultTypeDef = TypedDict(
+    "GetDocumentResultTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "VersionName": str,
+        "DocumentVersion": str,
+        "Status": DocumentStatusType,
+        "StatusInformation": str,
+        "Content": str,
+        "DocumentType": DocumentTypeType,
+        "DocumentFormat": DocumentFormatType,
+        "Requires": List[DocumentRequiresOutputTypeDef],
+        "AttachmentsContent": List[AttachmentContentTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
@@ -5144,17 +5198,17 @@
         "PlatformTypes": List[PlatformTypeType],
         "DocumentType": DocumentTypeType,
         "SchemaVersion": str,
         "LatestVersion": str,
         "DefaultVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "AttachmentsInformation": List[AttachmentInformationTypeDef],
-        "Requires": List[DocumentRequiresTypeDef],
+        "Requires": List[DocumentRequiresOutputTypeDef],
         "Author": str,
         "ReviewInformation": List[ReviewInformationTypeDef],
         "ApprovedVersion": str,
         "PendingReviewVersion": str,
         "ReviewStatus": ReviewStatusType,
         "Category": List[str],
         "CategoryEnum": List[str],
@@ -5163,15 +5217,15 @@
 )
 
 ListDocumentsRequestListDocumentsPaginateTypeDef = TypedDict(
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     {
         "DocumentFilterList": Sequence[DocumentFilterTypeDef],
         "Filters": Sequence[DocumentKeyValuesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
@@ -5185,15 +5239,15 @@
 
 DocumentReviewerResponseSourceTypeDef = TypedDict(
     "DocumentReviewerResponseSourceTypeDef",
     {
         "CreateTime": datetime,
         "UpdatedTime": datetime,
         "ReviewStatus": ReviewStatusType,
-        "Comment": List[DocumentReviewCommentSourceTypeDef],
+        "Comment": List[DocumentReviewCommentSourceOutputTypeDef],
         "Reviewer": str,
     },
     total=False,
 )
 
 _RequiredDocumentReviewsTypeDef = TypedDict(
     "_RequiredDocumentReviewsTypeDef",
@@ -5205,25 +5259,23 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
-
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
-
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EffectivePatchTypeDef = TypedDict(
     "EffectivePatchTypeDef",
     {
         "Patch": PatchTypeDef,
@@ -5244,22 +5296,20 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
-
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5277,29 +5327,27 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetInventoryRequestRequestTypeDef = TypedDict(
     "GetInventoryRequestRequestTypeDef",
     {
@@ -5308,14 +5356,24 @@
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+GetOpsMetadataResultTypeDef = TypedDict(
+    "GetOpsMetadataResultTypeDef",
+    {
+        "ResourceId": str,
+        "Metadata": Dict[str, MetadataValueOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OpsAggregatorTypeDef = TypedDict(
     "OpsAggregatorTypeDef",
     {
         "AggregatorType": str,
         "TypeName": str,
         "AttributeName": str,
         "Values": Mapping[str, str],
@@ -5328,15 +5386,15 @@
 GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef = TypedDict(
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     {
         "SyncName": str,
         "Filters": Sequence[OpsFilterTypeDef],
         "Aggregators": Sequence["OpsAggregatorTypeDef"],
         "ResultAttributes": Sequence[OpsResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetOpsSummaryRequestRequestTypeDef = TypedDict(
     "GetOpsSummaryRequestRequestTypeDef",
     {
@@ -5350,58 +5408,58 @@
     total=False,
 )
 
 GetParameterResultTypeDef = TypedDict(
     "GetParameterResultTypeDef",
     {
         "Parameter": ParameterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersByPathResultTypeDef = TypedDict(
     "GetParametersByPathResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersResultTypeDef = TypedDict(
     "GetParametersResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceSettingResultTypeDef = TypedDict(
     "GetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetServiceSettingResultTypeDef = TypedDict(
     "ResetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceInformationTypeDef = TypedDict(
     "InstanceInformationTypeDef",
     {
         "InstanceId": str,
@@ -5425,14 +5483,22 @@
         "AssociationOverview": InstanceAggregatedAssociationOverviewTypeDef,
         "SourceId": str,
         "SourceType": SourceTypeType,
     },
     total=False,
 )
 
+InstanceAssociationOutputLocationOutputTypeDef = TypedDict(
+    "InstanceAssociationOutputLocationOutputTypeDef",
+    {
+        "S3Location": S3OutputLocationOutputTypeDef,
+    },
+    total=False,
+)
+
 InstanceAssociationOutputLocationTypeDef = TypedDict(
     "InstanceAssociationOutputLocationTypeDef",
     {
         "S3Location": S3OutputLocationTypeDef,
     },
     total=False,
 )
@@ -5467,21 +5533,19 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
-
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5495,15 +5559,15 @@
     total=False,
 )
 
 ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef = TypedDict(
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     {
         "Filters": Sequence[OpsItemEventFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemEventsRequestRequestTypeDef = TypedDict(
     "ListOpsItemEventsRequestRequestTypeDef",
     {
@@ -5515,15 +5579,15 @@
 )
 
 ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     {
         "OpsItemId": str,
         "Filters": Sequence[OpsItemRelatedItemsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemRelatedItemsRequestRequestTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     {
@@ -5535,15 +5599,15 @@
     total=False,
 )
 
 ListOpsMetadataRequestListOpsMetadataPaginateTypeDef = TypedDict(
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     {
         "Filters": Sequence[OpsMetadataFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsMetadataRequestRequestTypeDef = TypedDict(
     "ListOpsMetadataRequestRequestTypeDef",
     {
@@ -5555,27 +5619,69 @@
 )
 
 ListOpsMetadataResultTypeDef = TypedDict(
     "ListOpsMetadataResultTypeDef",
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersTypeDef",
+    {
+        "Comment": str,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "DocumentVersion": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ServiceRoleArn": str,
+        "TimeoutSeconds": int,
     },
+    total=False,
 )
 
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
 )
 
+OpsItemSummaryTypeDef = TypedDict(
+    "OpsItemSummaryTypeDef",
+    {
+        "CreatedBy": str,
+        "CreatedTime": datetime,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Priority": int,
+        "Source": str,
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Title": str,
+        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
+        "Category": str,
+        "Severity": str,
+        "OpsItemType": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+    },
+    total=False,
+)
+
 OpsItemEventSummaryTypeDef = TypedDict(
     "OpsItemEventSummaryTypeDef",
     {
         "OpsItemId": str,
         "EventId": str,
         "Source": str,
         "DetailType": str,
@@ -5598,14 +5704,43 @@
         "CreatedTime": datetime,
         "LastModifiedBy": OpsItemIdentityTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+OpsItemTypeDef = TypedDict(
+    "OpsItemTypeDef",
+    {
+        "CreatedBy": str,
+        "OpsItemType": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Notifications": List[OpsItemNotificationOutputTypeDef],
+        "Priority": int,
+        "RelatedOpsItems": List[RelatedOpsItemOutputTypeDef],
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Version": str,
+        "Title": str,
+        "Source": str,
+        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
+        "Category": str,
+        "Severity": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+        "OpsItemArn": str,
+    },
+    total=False,
+)
+
 ParameterHistoryTypeDef = TypedDict(
     "ParameterHistoryTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "KeyId": str,
         "LastModifiedDate": datetime,
@@ -5636,42 +5771,91 @@
         "Tier": ParameterTierType,
         "Policies": List[ParameterInlinePolicyTypeDef],
         "DataType": str,
     },
     total=False,
 )
 
+PatchFilterGroupOutputTypeDef = TypedDict(
+    "PatchFilterGroupOutputTypeDef",
+    {
+        "PatchFilters": List[PatchFilterOutputTypeDef],
+    },
+)
+
 PatchFilterGroupTypeDef = TypedDict(
     "PatchFilterGroupTypeDef",
     {
         "PatchFilters": Sequence[PatchFilterTypeDef],
     },
 )
 
+_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationSourceType": str,
+    },
+)
+_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitOutputTypeDef],
+    },
+    total=False,
+)
+
+class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
+    _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+    _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+):
+    pass
+
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
-
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
+_RequiredResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
+    "_RequiredResourceDataSyncS3DestinationOutputTypeDef",
+    {
+        "BucketName": str,
+        "SyncFormat": Literal["JsonSerDe"],
+        "Region": str,
+    },
+)
+_OptionalResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
+    "_OptionalResourceDataSyncS3DestinationOutputTypeDef",
+    {
+        "Prefix": str,
+        "AWSKMSKeyARN": str,
+        "DestinationDataSharing": ResourceDataSyncDestinationDataSharingOutputTypeDef,
+    },
+    total=False,
+)
+
+class ResourceDataSyncS3DestinationOutputTypeDef(
+    _RequiredResourceDataSyncS3DestinationOutputTypeDef,
+    _OptionalResourceDataSyncS3DestinationOutputTypeDef,
+):
+    pass
 
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
@@ -5683,21 +5867,19 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
-
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -5713,30 +5895,30 @@
 )
 
 DescribeActivationsResultTypeDef = TypedDict(
     "DescribeActivationsResultTypeDef",
     {
         "ActivationList": List[ActivationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationExecutionTypeDef = TypedDict(
     "AssociationExecutionTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "Status": str,
         "DetailedStatus": str,
         "CreatedTime": datetime,
         "LastExecutionDate": datetime,
         "ResourceCountByStatus": str,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
@@ -5744,94 +5926,109 @@
         "CommandId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "Comment": str,
         "ExpiresAfter": datetime,
         "Parameters": Dict[str, List[str]],
         "InstanceIds": List[str],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "RequestedDateTime": datetime,
         "Status": CommandStatusType,
         "StatusDetails": str,
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
         "TimeoutSeconds": int,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 GetMaintenanceWindowExecutionTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "TaskArn": str,
         "ServiceRole": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "TaskParameters": List[Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef]],
+        "TaskParameters": List[
+            Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]
+        ],
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 MaintenanceWindowTaskTypeDef = TypedDict(
     "MaintenanceWindowTaskTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "Targets": List[TargetTypeDef],
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "Targets": List[TargetOutputTypeDef],
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "Priority": int,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+TargetLocationOutputTypeDef = TypedDict(
+    "TargetLocationOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "Regions": List[str],
+        "TargetLocationMaxConcurrency": str,
+        "TargetLocationMaxErrors": str,
+        "ExecutionRoleName": str,
+        "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredSendCommandRequestRequestTypeDef = TypedDict(
     "_RequiredSendCommandRequestRequestTypeDef",
     {
@@ -5858,21 +6055,19 @@
         "NotificationConfig": NotificationConfigTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SendCommandRequestRequestTypeDef(
     _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
 ):
     pass
 
-
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -5883,62 +6078,62 @@
 )
 
 ListAssociationsResultTypeDef = TypedDict(
     "ListAssociationsResultTypeDef",
     {
         "Associations": List[AssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTargetsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     {
         "Targets": List[MaintenanceWindowTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionTargetsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionTargetsResultTypeDef",
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     {
-        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersTypeDef,
-        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
+        "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersOutputTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
         "ComplianceItems": List[ComplianceItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryItemTypeDef = TypedDict(
     "ComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
@@ -5952,77 +6147,60 @@
     "ResourceComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Status": ComplianceStatusType,
         "OverallSeverity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
-ListDocumentsResultTypeDef = TypedDict(
-    "ListDocumentsResultTypeDef",
-    {
-        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeOpsItemsResponseTypeDef = TypedDict(
-    "DescribeOpsItemsResponseTypeDef",
+DescribePatchGroupsResultTypeDef = TypedDict(
+    "DescribePatchGroupsResultTypeDef",
     {
+        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
-        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOpsItemResponseTypeDef = TypedDict(
-    "GetOpsItemResponseTypeDef",
-    {
-        "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribePatchGroupsResultTypeDef = TypedDict(
-    "DescribePatchGroupsResultTypeDef",
+ListDocumentsResultTypeDef = TypedDict(
+    "ListDocumentsResultTypeDef",
     {
-        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
+        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDocumentResultTypeDef = TypedDict(
     "DescribeDocumentResultTypeDef",
     {
         "Document": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDocumentResultTypeDef = TypedDict(
     "UpdateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataResponseInfoTypeDef = TypedDict(
     "DocumentMetadataResponseInfoTypeDef",
     {
         "ReviewerResponse": List[DocumentReviewerResponseSourceTypeDef],
@@ -6041,28 +6219,26 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryAggregatorTypeDef = TypedDict(
     "InventoryAggregatorTypeDef",
     {
         "Expression": str,
@@ -6073,15 +6249,15 @@
 )
 
 DescribeInstanceInformationResultTypeDef = TypedDict(
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": str,
@@ -6102,15 +6278,15 @@
 
 DeleteInventoryResultTypeDef = TypedDict(
     "DeleteInventoryResultTypeDef",
     {
         "DeletionId": str,
         "TypeName": str,
         "DeletionSummary": InventoryDeletionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDeletionStatusItemTypeDef = TypedDict(
     "InventoryDeletionStatusItemTypeDef",
     {
         "DeletionId": str,
@@ -6125,72 +6301,120 @@
 )
 
 GetInventorySchemaResultTypeDef = TypedDict(
     "GetInventorySchemaResultTypeDef",
     {
         "Schemas": List[InventoryItemSchemaTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInventoryResultTypeDef = TypedDict(
     "GetInventoryResultTypeDef",
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    {
+        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
+    },
+    total=False,
+)
+
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOpsItemsResponseTypeDef = TypedDict(
+    "DescribeOpsItemsResponseTypeDef",
+    {
+        "NextToken": str,
+        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemRelatedItemsResponseTypeDef = TypedDict(
     "ListOpsItemRelatedItemsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpsItemResponseTypeDef = TypedDict(
+    "GetOpsItemResponseTypeDef",
+    {
+        "OpsItem": OpsItemTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParametersResultTypeDef = TypedDict(
     "DescribeParametersResultTypeDef",
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPatchRuleOutputTypeDef = TypedDict(
+    "_RequiredPatchRuleOutputTypeDef",
+    {
+        "PatchFilterGroup": PatchFilterGroupOutputTypeDef,
+    },
+)
+_OptionalPatchRuleOutputTypeDef = TypedDict(
+    "_OptionalPatchRuleOutputTypeDef",
+    {
+        "ComplianceLevel": PatchComplianceLevelType,
+        "ApproveAfterDays": int,
+        "ApproveUntilDate": str,
+        "EnableNonSecurity": bool,
+    },
+    total=False,
+)
+
+class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
+    pass
+
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
 _OptionalPatchRuleTypeDef = TypedDict(
@@ -6200,18 +6424,29 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
-
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
+ResourceDataSyncSourceWithStateTypeDef = TypedDict(
+    "ResourceDataSyncSourceWithStateTypeDef",
+    {
+        "SourceType": str,
+        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+        "SourceRegions": List[str],
+        "IncludeFutureRegions": bool,
+        "State": str,
+        "EnableAllOpsDataSources": bool,
+    },
+    total=False,
+)
 
 _RequiredResourceDataSyncSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncSourceTypeDef",
     {
         "SourceType": str,
         "SourceRegions": Sequence[str],
     },
@@ -6222,148 +6457,224 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
-
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
-
-ResourceDataSyncSourceWithStateTypeDef = TypedDict(
-    "ResourceDataSyncSourceWithStateTypeDef",
-    {
-        "SourceType": str,
-        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
-        "SourceRegions": List[str],
-        "IncludeFutureRegions": bool,
-        "State": str,
-        "EnableAllOpsDataSources": bool,
-    },
-    total=False,
-)
-
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionsResultTypeDef",
     {
         "AssociationExecutions": List[AssociationExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandsResultTypeDef = TypedDict(
     "ListCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "Command": CommandTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     {
         "WindowExecutionTaskIdentities": List[MaintenanceWindowExecutionTaskIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTasksResultTypeDef",
     {
         "Tasks": List[MaintenanceWindowTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationDescriptionTypeDef = TypedDict(
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationVersion": str,
         "Date": datetime,
         "LastUpdateAssociationDate": datetime,
-        "Status": AssociationStatusTypeDef,
+        "Status": AssociationStatusOutputTypeDef,
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 AssociationVersionInfoTypeDef = TypedDict(
     "AssociationVersionInfoTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
+_RequiredCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryOutputTypeDef",
+    {
+        "InstanceId": str,
+        "Parameters": Dict[str, List[str]],
+        "AutomationTargetParameterName": str,
+        "DocumentVersion": str,
+        "Targets": List[TargetOutputTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "AssociationName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": List[str],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": List[Dict[str, List[str]]],
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateAssociationBatchRequestEntryOutputTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
+):
+    pass
+
+_RequiredRunbookOutputTypeDef = TypedDict(
+    "_RequiredRunbookOutputTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalRunbookOutputTypeDef = TypedDict(
+    "_OptionalRunbookOutputTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Dict[str, List[str]],
+        "TargetParameterName": str,
+        "Targets": List[TargetOutputTypeDef],
+        "TargetMaps": List[Dict[str, List[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": List[TargetLocationOutputTypeDef],
+    },
+    total=False,
+)
+
+class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
+    pass
+
+StepExecutionTypeDef = TypedDict(
+    "StepExecutionTypeDef",
+    {
+        "StepName": str,
+        "Action": str,
+        "TimeoutSeconds": int,
+        "OnFailure": str,
+        "MaxAttempts": int,
+        "ExecutionStartTime": datetime,
+        "ExecutionEndTime": datetime,
+        "StepStatus": AutomationExecutionStatusType,
+        "ResponseCode": str,
+        "Inputs": Dict[str, str],
+        "Outputs": Dict[str, List[str]],
+        "Response": str,
+        "FailureMessage": str,
+        "FailureDetails": FailureDetailsTypeDef,
+        "StepExecutionId": str,
+        "OverriddenParameters": Dict[str, List[str]],
+        "IsEnd": bool,
+        "NextStep": str,
+        "IsCritical": bool,
+        "ValidNextSteps": List[str],
+        "Targets": List[TargetOutputTypeDef],
+        "TargetLocation": TargetLocationOutputTypeDef,
+        "TriggeredAlarms": List[AlarmStateInformationTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
     "_RequiredCreateAssociationBatchRequestEntryTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
@@ -6387,22 +6698,20 @@
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateAssociationBatchRequestEntryTypeDef(
     _RequiredCreateAssociationBatchRequestEntryTypeDef,
     _OptionalCreateAssociationBatchRequestEntryTypeDef,
 ):
     pass
 
-
 _RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssociationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
@@ -6427,47 +6736,43 @@
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateAssociationRequestRequestTypeDef(
     _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredRunbookTypeDef = TypedDict(
     "_RequiredRunbookTypeDef",
     {
         "DocumentName": str,
     },
 )
 _OptionalRunbookTypeDef = TypedDict(
     "_OptionalRunbookTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
-        "TargetMaps": List[Dict[str, List[str]]],
+        "Targets": Sequence[TargetTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": Sequence[TargetLocationTypeDef],
     },
     total=False,
 )
 
-
 class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
-
 _RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartAutomationExecutionRequestRequestTypeDef",
     {
         "DocumentName": str,
     },
 )
 _OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
@@ -6485,52 +6790,20 @@
         "TargetLocations": Sequence[TargetLocationTypeDef],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StartAutomationExecutionRequestRequestTypeDef(
     _RequiredStartAutomationExecutionRequestRequestTypeDef,
     _OptionalStartAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
-
-StepExecutionTypeDef = TypedDict(
-    "StepExecutionTypeDef",
-    {
-        "StepName": str,
-        "Action": str,
-        "TimeoutSeconds": int,
-        "OnFailure": str,
-        "MaxAttempts": int,
-        "ExecutionStartTime": datetime,
-        "ExecutionEndTime": datetime,
-        "StepStatus": AutomationExecutionStatusType,
-        "ResponseCode": str,
-        "Inputs": Dict[str, str],
-        "Outputs": Dict[str, List[str]],
-        "Response": str,
-        "FailureMessage": str,
-        "FailureDetails": FailureDetailsTypeDef,
-        "StepExecutionId": str,
-        "OverriddenParameters": Dict[str, List[str]],
-        "IsEnd": bool,
-        "NextStep": str,
-        "IsCritical": bool,
-        "ValidNextSteps": List[str],
-        "Targets": List[TargetTypeDef],
-        "TargetLocation": TargetLocationTypeDef,
-        "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
@@ -6555,41 +6828,109 @@
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAssociationRequestRequestTypeDef(
     _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
 ):
     pass
 
-
 GetMaintenanceWindowTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowTaskResultTypeDef",
+    {
+        "WindowId": str,
+        "WindowTaskId": str,
+        "Targets": List[TargetOutputTypeDef],
+        "TaskArn": str,
+        "ServiceRoleArn": str,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "Name": str,
+        "Description": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListComplianceSummariesResultTypeDef = TypedDict(
+    "ListComplianceSummariesResultTypeDef",
+    {
+        "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceComplianceSummariesResultTypeDef = TypedDict(
+    "ListResourceComplianceSummariesResultTypeDef",
+    {
+        "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
+    "ListDocumentMetadataHistoryResponseTypeDef",
+    {
+        "Name": str,
+        "DocumentVersion": str,
+        "Author": str,
+        "Metadata": DocumentMetadataResponseInfoTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
+    "DescribeInstanceAssociationsStatusResultTypeDef",
+    {
+        "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInventoryDeletionsResultTypeDef = TypedDict(
+    "DescribeInventoryDeletionsResultTypeDef",
+    {
+        "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
@@ -6613,22 +6954,20 @@
         "ClientToken": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
     _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
     _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -6649,97 +6988,49 @@
         "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowTaskResultTypeDef",
+PatchRuleGroupOutputTypeDef = TypedDict(
+    "PatchRuleGroupOutputTypeDef",
     {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
-        "TaskArn": str,
-        "ServiceRoleArn": str,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PatchRules": List[PatchRuleOutputTypeDef],
     },
 )
 
-ListComplianceSummariesResultTypeDef = TypedDict(
-    "ListComplianceSummariesResultTypeDef",
-    {
-        "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListResourceComplianceSummariesResultTypeDef = TypedDict(
-    "ListResourceComplianceSummariesResultTypeDef",
-    {
-        "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
-    "ListDocumentMetadataHistoryResponseTypeDef",
-    {
-        "Name": str,
-        "DocumentVersion": str,
-        "Author": str,
-        "Metadata": DocumentMetadataResponseInfoTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
-    "DescribeInstanceAssociationsStatusResultTypeDef",
-    {
-        "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeInventoryDeletionsResultTypeDef = TypedDict(
-    "DescribeInventoryDeletionsResultTypeDef",
+PatchRuleGroupTypeDef = TypedDict(
+    "PatchRuleGroupTypeDef",
     {
-        "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PatchRules": Sequence[PatchRuleTypeDef],
     },
 )
 
-PatchRuleGroupTypeDef = TypedDict(
-    "PatchRuleGroupTypeDef",
+ResourceDataSyncItemTypeDef = TypedDict(
+    "ResourceDataSyncItemTypeDef",
     {
-        "PatchRules": Sequence[PatchRuleTypeDef],
+        "SyncName": str,
+        "SyncType": str,
+        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationOutputTypeDef,
+        "LastSyncTime": datetime,
+        "LastSuccessfulSyncTime": datetime,
+        "SyncLastModifiedTime": datetime,
+        "LastStatus": LastResourceDataSyncStatusType,
+        "SyncCreatedTime": datetime,
+        "LastSyncStatusMessage": str,
     },
+    total=False,
 )
 
 _RequiredCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
@@ -6750,100 +7041,74 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
-
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
 )
 
-ResourceDataSyncItemTypeDef = TypedDict(
-    "ResourceDataSyncItemTypeDef",
-    {
-        "SyncName": str,
-        "SyncType": str,
-        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
-        "LastSyncTime": datetime,
-        "LastSuccessfulSyncTime": datetime,
-        "SyncLastModifiedTime": datetime,
-        "LastStatus": LastResourceDataSyncStatusType,
-        "SyncCreatedTime": datetime,
-        "LastSyncStatusMessage": str,
-    },
-    total=False,
-)
-
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationResultTypeDef = TypedDict(
     "DescribeAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationResultTypeDef = TypedDict(
     "UpdateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationStatusResultTypeDef = TypedDict(
     "UpdateAssociationStatusResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociationVersionsResultTypeDef = TypedDict(
     "ListAssociationVersionsResultTypeDef",
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
-    {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedCreateAssociationTypeDef = TypedDict(
     "FailedCreateAssociationTypeDef",
     {
-        "Entry": CreateAssociationBatchRequestEntryTypeDef,
+        "Entry": CreateAssociationBatchRequestEntryOutputTypeDef,
         "Message": str,
         "Fault": FaultType,
     },
     total=False,
 )
 
 AutomationExecutionMetadataTypeDef = TypedDict(
@@ -6860,64 +7125,33 @@
         "Outputs": Dict[str, List[str]],
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "FailureMessage": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
         "AutomationType": AutomationTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-        "Runbooks": Sequence[RunbookTypeDef],
-    },
-)
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "ScheduledTime": Union[datetime, str],
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
-        "ClientToken": str,
-        "AutoApprove": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": Union[datetime, str],
-        "ChangeDetails": str,
-    },
-    total=False,
-)
-
-
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
-):
-    pass
-
-
 AutomationExecutionTypeDef = TypedDict(
     "AutomationExecutionTypeDef",
     {
         "AutomationExecutionId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "ExecutionStartTime": datetime,
@@ -6930,40 +7164,119 @@
         "FailureMessage": str,
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "ExecutedBy": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ProgressCounters": ProgressCountersTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
 DescribeAutomationStepExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationStepExecutionsResultTypeDef",
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+    },
+)
+
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookTypeDef],
+    },
+)
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": Union[datetime, str],
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": Union[datetime, str],
+        "ChangeDetails": str,
+    },
+    total=False,
+)
+
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
+GetPatchBaselineResultTypeDef = TypedDict(
+    "GetPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "PatchGroups": List[str],
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePatchBaselineResultTypeDef = TypedDict(
+    "UpdatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
@@ -7000,44 +7313,20 @@
         "Sources": Sequence[PatchSourceTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
-GetPatchBaselineResultTypeDef = TypedDict(
-    "GetPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "PatchGroups": List[str],
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
@@ -7054,75 +7343,52 @@
         "Description": str,
         "Sources": Sequence[PatchSourceTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
-UpdatePatchBaselineResultTypeDef = TypedDict(
-    "UpdatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssociationBatchResultTypeDef = TypedDict(
     "CreateAssociationBatchResultTypeDef",
     {
         "Successful": List[AssociationDescriptionTypeDef],
         "Failed": List[FailedCreateAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAutomationExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationExecutionsResultTypeDef",
     {
         "AutomationExecutionMetadataList": List[AutomationExecutionMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutomationExecutionResultTypeDef = TypedDict(
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -7133,13 +7399,12 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
-
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/type_defs.pyi` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     from mypy_boto3_ssm.type_defs import AccountSharingInfoTypeDef
 
     data: AccountSharingInfoTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationExecutionFilterKeyType,
     AssociationExecutionTargetsFilterKeyType,
     AssociationFilterKeyType,
     AssociationFilterOperatorTypeType,
@@ -99,290 +101,310 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountSharingInfoTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
+    "AlarmOutputTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
-    "AssociationStatusTypeDef",
-    "TargetTypeDef",
+    "AssociationStatusOutputTypeDef",
+    "TargetOutputTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
+    "AssociationStatusTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
-    "CancelMaintenanceWindowExecutionResultTypeDef",
+    "CloudWatchOutputConfigOutputTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
-    "NotificationConfigTypeDef",
+    "NotificationConfigOutputTypeDef",
+    "ComplianceExecutionSummaryOutputTypeDef",
     "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
-    "CreateActivationResultTypeDef",
+    "TargetTypeDef",
     "DocumentRequiresTypeDef",
-    "CreateMaintenanceWindowResultTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
-    "CreateOpsItemResponseTypeDef",
     "MetadataValueTypeDef",
-    "CreateOpsMetadataResultTypeDef",
-    "CreatePatchBaselineResultTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
-    "DeleteMaintenanceWindowResultTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
     "DeleteParametersRequestRequestTypeDef",
-    "DeleteParametersResultTypeDef",
     "DeletePatchBaselineRequestRequestTypeDef",
-    "DeletePatchBaselineResultTypeDef",
     "DeleteResourceDataSyncRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeregisterManagedInstanceRequestRequestTypeDef",
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
     "DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     "DescribeActivationsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAssociationRequestRequestTypeDef",
     "StepExecutionFilterTypeDef",
     "PatchOrchestratorFilterTypeDef",
     "PatchTypeDef",
     "DescribeDocumentPermissionRequestRequestTypeDef",
     "DescribeDocumentRequestRequestTypeDef",
-    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     "InstanceAssociationTypeDef",
-    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
-    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
-    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
     "OpsItemFilterTypeDef",
     "ParameterStringFilterTypeDef",
     "ParametersFilterTypeDef",
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
-    "DescribePatchGroupStateResultTypeDef",
-    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
-    "DescribePatchPropertiesResultTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
+    "DocumentRequiresOutputTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
+    "DocumentReviewCommentSourceOutputTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
-    "GetCalendarStateResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetCommandInvocationRequestRequestTypeDef",
     "GetConnectionStatusRequestRequestTypeDef",
-    "GetConnectionStatusResponseTypeDef",
     "GetDefaultPatchBaselineRequestRequestTypeDef",
-    "GetDefaultPatchBaselineResultTypeDef",
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionResultTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
-    "GetMaintenanceWindowResultTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
-    "LoggingInfoTypeDef",
+    "LoggingInfoOutputTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
+    "MetadataValueOutputTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
-    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "GetPatchBaselineForPatchGroupResultTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
+    "S3OutputLocationOutputTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
-    "LabelParameterVersionResultTypeDef",
-    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationVersionsRequestRequestTypeDef",
     "ListDocumentMetadataHistoryRequestRequestTypeDef",
-    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     "ListDocumentVersionsRequestRequestTypeDef",
-    "ListInventoryEntriesResultTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LoggingInfoTypeDef",
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
     "MaintenanceWindowLambdaParametersTypeDef",
+    "NotificationConfigTypeDef",
+    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
+    "OpsItemDataValueOutputTypeDef",
     "OpsItemIdentityTypeDef",
-    "PaginatorConfigTypeDef",
+    "OpsItemNotificationOutputTypeDef",
+    "RelatedOpsItemOutputTypeDef",
     "ParameterInlinePolicyTypeDef",
+    "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
-    "PutInventoryResultTypeDef",
-    "PutParameterResultTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
-    "RegisterDefaultPatchBaselineResultTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
+    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
+    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeSessionRequestRequestTypeDef",
-    "ResumeSessionResponseTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
-    "StartAutomationExecutionResultTypeDef",
-    "StartChangeRequestExecutionResultTypeDef",
     "StartSessionRequestRequestTypeDef",
-    "StartSessionResponseTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionRequestRequestTypeDef",
-    "UnlabelParameterVersionResultTypeDef",
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     "UpdateMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowResultTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
-    "UpdateOpsMetadataResultTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
-    "DescribeDocumentPermissionResponseTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "PutParameterRequestRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
+    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "CancelMaintenanceWindowExecutionResultTypeDef",
+    "CreateActivationResultTypeDef",
+    "CreateMaintenanceWindowResultTypeDef",
+    "CreateOpsItemResponseTypeDef",
+    "CreateOpsMetadataResultTypeDef",
+    "CreatePatchBaselineResultTypeDef",
+    "DeleteMaintenanceWindowResultTypeDef",
+    "DeleteParametersResultTypeDef",
+    "DeletePatchBaselineResultTypeDef",
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
+    "DescribeDocumentPermissionResponseTypeDef",
+    "DescribePatchGroupStateResultTypeDef",
+    "DescribePatchPropertiesResultTypeDef",
+    "GetCalendarStateResponseTypeDef",
+    "GetConnectionStatusResponseTypeDef",
+    "GetDefaultPatchBaselineResultTypeDef",
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    "GetMaintenanceWindowResultTypeDef",
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    "LabelParameterVersionResultTypeDef",
+    "ListInventoryEntriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PutInventoryResultTypeDef",
+    "PutParameterResultTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
+    "ResumeSessionResponseTypeDef",
+    "StartAutomationExecutionResultTypeDef",
+    "StartChangeRequestExecutionResultTypeDef",
+    "StartSessionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
+    "UnlabelParameterVersionResultTypeDef",
+    "UpdateMaintenanceWindowResultTypeDef",
+    "UpdateOpsMetadataResultTypeDef",
     "AssociationTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
-    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
-    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListAssociationsRequestRequestTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     "GetCommandInvocationResultTypeDef",
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
-    "ListCommandsRequestListCommandsPaginateTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
-    "MaintenanceWindowRunCommandParametersTypeDef",
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     "ComplianceItemTypeDef",
     "PutComplianceItemsRequestRequestTypeDef",
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "CreateDocumentRequestRequestTypeDef",
-    "DocumentIdentifierTypeDef",
-    "GetDocumentResultTypeDef",
-    "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
-    "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
-    "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
-    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     "DescribeActivationsRequestRequestTypeDef",
+    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
+    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
     "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
@@ -424,142 +446,158 @@
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribePatchBaselinesResultTypeDef",
     "PatchGroupPatchBaselineMappingTypeDef",
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
     "UpdateDocumentDefaultVersionResultTypeDef",
+    "DocumentIdentifierTypeDef",
+    "GetDocumentResultTypeDef",
     "DocumentDescriptionTypeDef",
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     "ListDocumentsRequestRequestTypeDef",
     "DocumentReviewerResponseSourceTypeDef",
     "DocumentReviewsTypeDef",
     "ListDocumentVersionsResultTypeDef",
     "EffectivePatchTypeDef",
     "GetCommandInvocationRequestCommandExecutedWaitTypeDef",
     "InventoryGroupTypeDef",
     "ListInventoryEntriesRequestRequestTypeDef",
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     "GetInventoryRequestRequestTypeDef",
+    "GetOpsMetadataResultTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
+    "InstanceAssociationOutputLocationOutputTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
     "InventoryItemSchemaTypeDef",
     "PutInventoryRequestRequestTypeDef",
     "InventoryResultEntityTypeDef",
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
+    "MaintenanceWindowRunCommandParametersTypeDef",
     "OpsEntityTypeDef",
+    "OpsItemSummaryTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
+    "OpsItemTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
+    "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
+    "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
+    "ResourceDataSyncS3DestinationOutputTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
+    "TargetLocationOutputTypeDef",
     "SendCommandRequestRequestTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
     "ListCommandInvocationsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
-    "ListDocumentsResultTypeDef",
-    "DescribeOpsItemsResponseTypeDef",
-    "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
+    "ListDocumentsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
     "DocumentMetadataResponseInfoTypeDef",
     "UpdateDocumentMetadataRequestRequestTypeDef",
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     "InventoryAggregatorTypeDef",
     "DescribeInstanceInformationResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
+    "DescribeOpsItemsResponseTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
+    "GetOpsItemResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
+    "PatchRuleOutputTypeDef",
     "PatchRuleTypeDef",
-    "ResourceDataSyncSourceTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
+    "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
+    "CreateAssociationBatchRequestEntryOutputTypeDef",
+    "RunbookOutputTypeDef",
+    "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
     "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
     "StartAutomationExecutionRequestRequestTypeDef",
-    "StepExecutionTypeDef",
     "UpdateAssociationRequestRequestTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
+    "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
-    "ResourceDataSyncItemTypeDef",
     "CreateAssociationResultTypeDef",
     "DescribeAssociationResultTypeDef",
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
+    "GetPatchBaselineResultTypeDef",
+    "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
-    "GetPatchBaselineResultTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
-    "UpdatePatchBaselineResultTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
@@ -568,22 +606,37 @@
     {
         "AccountId": str,
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+AlarmOutputTypeDef = TypedDict(
+    "AlarmOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -601,58 +654,63 @@
         "OpsItemId": str,
         "AssociationType": str,
         "ResourceType": str,
         "ResourceUri": str,
     },
 )
 
-AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AssociationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociationOverviewTypeDef = TypedDict(
     "AssociationOverviewTypeDef",
     {
         "Status": str,
         "DetailedStatus": str,
         "AssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
+_RequiredAssociationStatusOutputTypeDef = TypedDict(
+    "_RequiredAssociationStatusOutputTypeDef",
     {
         "Date": datetime,
         "Name": AssociationStatusNameType,
         "Message": str,
     },
 )
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
+_OptionalAssociationStatusOutputTypeDef = TypedDict(
+    "_OptionalAssociationStatusOutputTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+
+class AssociationStatusOutputTypeDef(
+    _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
 ):
     pass
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
+
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
     total=False,
 )
 
 AssociationExecutionFilterTypeDef = TypedDict(
     "AssociationExecutionFilterTypeDef",
     {
@@ -683,14 +741,37 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
+    {
+        "Date": Union[datetime, str],
+        "Name": AssociationStatusNameType,
+        "Message": str,
+    },
+)
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
+    {
+        "AdditionalInfo": str,
+    },
+    total=False,
+)
+
+
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+):
+    pass
+
+
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -765,32 +846,35 @@
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
+
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "CancelMaintenanceWindowExecutionResultTypeDef",
+CloudWatchOutputConfigOutputTypeDef = TypedDict(
+    "CloudWatchOutputConfigOutputTypeDef",
     {
-        "WindowExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CloudWatchLogGroupName": str,
+        "CloudWatchOutputEnabled": bool,
     },
+    total=False,
 )
 
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
@@ -821,44 +905,69 @@
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
     total=False,
 )
 
-NotificationConfigTypeDef = TypedDict(
-    "NotificationConfigTypeDef",
+NotificationConfigOutputTypeDef = TypedDict(
+    "NotificationConfigOutputTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": List[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
+_RequiredComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryOutputTypeDef",
+    {
+        "ExecutionTime": datetime,
+    },
+)
+_OptionalComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryOutputTypeDef",
+    {
+        "ExecutionId": str,
+        "ExecutionType": str,
+    },
+    total=False,
+)
+
+
+class ComplianceExecutionSummaryOutputTypeDef(
+    _RequiredComplianceExecutionSummaryOutputTypeDef,
+    _OptionalComplianceExecutionSummaryOutputTypeDef,
+):
+    pass
+
+
 _RequiredComplianceExecutionSummaryTypeDef = TypedDict(
     "_RequiredComplianceExecutionSummaryTypeDef",
     {
-        "ExecutionTime": datetime,
+        "ExecutionTime": Union[datetime, str],
     },
 )
 _OptionalComplianceExecutionSummaryTypeDef = TypedDict(
     "_OptionalComplianceExecutionSummaryTypeDef",
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
+
 class ComplianceExecutionSummaryTypeDef(
     _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
 ):
     pass
 
+
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
 )
@@ -868,19 +977,21 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
+
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -904,21 +1015,21 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateActivationResultTypeDef = TypedDict(
-    "CreateActivationResultTypeDef",
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
-        "ActivationId": str,
-        "ActivationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Values": Sequence[str],
     },
+    total=False,
 )
 
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
@@ -929,24 +1040,18 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
-CreateMaintenanceWindowResultTypeDef = TypedDict(
-    "CreateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
@@ -964,47 +1069,22 @@
 RelatedOpsItemTypeDef = TypedDict(
     "RelatedOpsItemTypeDef",
     {
         "OpsItemId": str,
     },
 )
 
-CreateOpsItemResponseTypeDef = TypedDict(
-    "CreateOpsItemResponseTypeDef",
-    {
-        "OpsItemId": str,
-        "OpsItemArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetadataValueTypeDef = TypedDict(
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-CreateOpsMetadataResultTypeDef = TypedDict(
-    "CreateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePatchBaselineResultTypeDef = TypedDict(
-    "CreatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1030,19 +1110,21 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
+
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1051,34 +1133,28 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
+
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-DeleteMaintenanceWindowResultTypeDef = TypedDict(
-    "DeleteMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOpsMetadataRequestRequestTypeDef = TypedDict(
     "DeleteOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 
@@ -1092,58 +1168,43 @@
 DeleteParametersRequestRequestTypeDef = TypedDict(
     "DeleteParametersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
-DeleteParametersResultTypeDef = TypedDict(
-    "DeleteParametersResultTypeDef",
-    {
-        "DeletedParameters": List[str],
-        "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePatchBaselineRequestRequestTypeDef = TypedDict(
     "DeletePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-DeletePatchBaselineResultTypeDef = TypedDict(
-    "DeletePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
+
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1160,23 +1221,14 @@
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
@@ -1184,55 +1236,49 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
+
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeActivationsFilterTypeDef = TypedDict(
     "DescribeActivationsFilterTypeDef",
     {
         "FilterKey": DescribeActivationsFilterKeysType,
         "FilterValues": Sequence[str],
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
 DescribeAssociationRequestRequestTypeDef = TypedDict(
     "DescribeAssociationRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationId": str,
         "AssociationVersion": str,
@@ -1299,20 +1345,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1320,38 +1368,20 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
-    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
@@ -1360,51 +1390,33 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
     },
     total=False,
 )
 
-_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "BaselineId": str,
-    },
-)
-_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
-    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
@@ -1412,39 +1424,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
-    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
@@ -1453,20 +1447,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1518,38 +1514,20 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
+
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
-_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-    },
-)
-_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
-    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
@@ -1558,20 +1536,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1583,27 +1563,20 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
+
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
-DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    {
-        "DeletionId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
@@ -1710,19 +1683,21 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
+
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1742,55 +1717,14 @@
 DescribePatchGroupStateRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupStateRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 
-DescribePatchGroupStateResultTypeDef = TypedDict(
-    "DescribePatchGroupStateResultTypeDef",
-    {
-        "Instances": int,
-        "InstancesWithInstalledPatches": int,
-        "InstancesWithInstalledOtherPatches": int,
-        "InstancesWithInstalledPendingRebootPatches": int,
-        "InstancesWithInstalledRejectedPatches": int,
-        "InstancesWithMissingPatches": int,
-        "InstancesWithFailedPatches": int,
-        "InstancesWithNotApplicablePatches": int,
-        "InstancesWithUnreportedNotApplicablePatches": int,
-        "InstancesWithCriticalNonCompliantPatches": int,
-        "InstancesWithSecurityNonCompliantPatches": int,
-        "InstancesWithOtherNonCompliantPatches": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "OperatingSystem": OperatingSystemType,
-        "Property": PatchPropertyType,
-    },
-)
-_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "PatchSet": PatchSetType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
-    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribePatchPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -1800,28 +1734,21 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
-DescribePatchPropertiesResultTypeDef = TypedDict(
-    "DescribePatchPropertiesResultTypeDef",
-    {
-        "Properties": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
@@ -1852,14 +1779,37 @@
         "Type": DocumentParameterTypeType,
         "Description": str,
         "DefaultValue": str,
     },
     total=False,
 )
 
+_RequiredDocumentRequiresOutputTypeDef = TypedDict(
+    "_RequiredDocumentRequiresOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalDocumentRequiresOutputTypeDef = TypedDict(
+    "_OptionalDocumentRequiresOutputTypeDef",
+    {
+        "Version": str,
+        "RequireType": str,
+        "VersionName": str,
+    },
+    total=False,
+)
+
+
+class DocumentRequiresOutputTypeDef(
+    _RequiredDocumentRequiresOutputTypeDef, _OptionalDocumentRequiresOutputTypeDef
+):
+    pass
+
+
 ReviewInformationTypeDef = TypedDict(
     "ReviewInformationTypeDef",
     {
         "ReviewedTime": datetime,
         "Status": ReviewStatusType,
         "Reviewer": str,
     },
@@ -1879,14 +1829,23 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+DocumentReviewCommentSourceOutputTypeDef = TypedDict(
+    "DocumentReviewCommentSourceOutputTypeDef",
+    {
+        "Type": Literal["Comment"],
+        "Content": str,
+    },
+    total=False,
+)
+
 DocumentReviewCommentSourceTypeDef = TypedDict(
     "DocumentReviewCommentSourceTypeDef",
     {
         "Type": Literal["Comment"],
         "Content": str,
     },
     total=False,
@@ -1946,28 +1905,20 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
+
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
-GetCalendarStateResponseTypeDef = TypedDict(
-    "GetCalendarStateResponseTypeDef",
-    {
-        "State": CalendarStateType,
-        "AtTime": str,
-        "NextTransitionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
@@ -1985,64 +1936,37 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
+
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
-GetConnectionStatusResponseTypeDef = TypedDict(
-    "GetConnectionStatusResponseTypeDef",
-    {
-        "Target": str,
-        "Status": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetDefaultPatchBaselineRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-GetDefaultPatchBaselineResultTypeDef = TypedDict(
-    "GetDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": str,
-        "SnapshotDownloadUrl": str,
-        "Product": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -2051,19 +1975,21 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
+
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2071,35 +1997,26 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
+
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
+
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    {
-        "TypeName": str,
-        "Aggregator": bool,
-        "SubType": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInventorySchemaRequestRequestTypeDef = TypedDict(
     "GetInventorySchemaRequestRequestTypeDef",
     {
         "TypeName": str,
         "NextToken": str,
         "MaxResults": int,
         "Aggregator": bool,
@@ -2111,145 +2028,97 @@
 GetMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskIds": List[str],
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "InvocationId": str,
     },
 )
 
-GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskExecutionId": str,
-        "InvocationId": str,
-        "ExecutionId": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "Parameters": str,
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "OwnerInformation": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 
-MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+MaintenanceWindowTaskParameterValueExpressionOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-GetMaintenanceWindowResultTypeDef = TypedDict(
-    "GetMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "NextExecutionTime": str,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-_RequiredLoggingInfoTypeDef = TypedDict(
-    "_RequiredLoggingInfoTypeDef",
+_RequiredLoggingInfoOutputTypeDef = TypedDict(
+    "_RequiredLoggingInfoOutputTypeDef",
     {
         "S3BucketName": str,
         "S3Region": str,
     },
 )
-_OptionalLoggingInfoTypeDef = TypedDict(
-    "_OptionalLoggingInfoTypeDef",
+_OptionalLoggingInfoOutputTypeDef = TypedDict(
+    "_OptionalLoggingInfoOutputTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
+
+class LoggingInfoOutputTypeDef(
+    _RequiredLoggingInfoOutputTypeDef, _OptionalLoggingInfoOutputTypeDef
+):
     pass
 
+
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -2257,19 +2126,29 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
+MetadataValueOutputTypeDef = TypedDict(
+    "MetadataValueOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2277,45 +2156,26 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
+
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
+
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
-    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetParameterHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterHistoryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterHistoryRequestRequestTypeDef = TypedDict(
@@ -2324,39 +2184,43 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
+
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2379,76 +2243,59 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
+
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
     {
-        "ResourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
     },
-    total=False,
 )
 
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2456,20 +2303,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2501,14 +2350,24 @@
     {
         "DetailedStatus": str,
         "InstanceAssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
+S3OutputLocationOutputTypeDef = TypedDict(
+    "S3OutputLocationOutputTypeDef",
+    {
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+    },
+    total=False,
+)
+
 S3OutputLocationTypeDef = TypedDict(
     "S3OutputLocationTypeDef",
     {
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
@@ -2555,17 +2414,19 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
+
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
+
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2575,19 +2436,21 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
+
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
+
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2595,48 +2458,21 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
+
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
-LabelParameterVersionResultTypeDef = TypedDict(
-    "LabelParameterVersionResultTypeDef",
-    {
-        "InvalidLabels": List[str],
-        "ParameterVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
-    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
@@ -2645,20 +2481,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2668,39 +2506,21 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
-    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
@@ -2709,32 +2529,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListInventoryEntriesResultTypeDef = TypedDict(
-    "ListInventoryEntriesResultTypeDef",
-    {
-        "TypeName": str,
-        "InstanceId": str,
-        "SchemaVersion": str,
-        "CaptureTime": str,
-        "Entries": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
@@ -2766,23 +2575,14 @@
         "LastModifiedDate": datetime,
         "LastModifiedUser": str,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
-    {
-        "SyncType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceDataSyncRequestRequestTypeDef = TypedDict(
     "ListResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2793,42 +2593,108 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
+_RequiredLoggingInfoTypeDef = TypedDict(
+    "_RequiredLoggingInfoTypeDef",
+    {
+        "S3BucketName": str,
+        "S3Region": str,
+    },
+)
+_OptionalLoggingInfoTypeDef = TypedDict(
+    "_OptionalLoggingInfoTypeDef",
+    {
+        "S3KeyPrefix": str,
+    },
+    total=False,
+)
+
+
+class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
+    pass
+
+
+MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Dict[str, List[str]],
+    },
+    total=False,
+)
+
 MaintenanceWindowAutomationParametersTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+MaintenanceWindowLambdaParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
+    {
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": bytes,
     },
     total=False,
 )
 
 MaintenanceWindowLambdaParametersTypeDef = TypedDict(
     "MaintenanceWindowLambdaParametersTypeDef",
     {
         "ClientContext": str,
         "Qualifier": str,
-        "Payload": bytes,
+        "Payload": Union[str, bytes, IO[Any], StreamingBody],
+    },
+    total=False,
+)
+
+NotificationConfigTypeDef = TypedDict(
+    "NotificationConfigTypeDef",
+    {
+        "NotificationArn": str,
+        "NotificationEvents": Sequence[NotificationEventType],
+        "NotificationType": NotificationTypeType,
+    },
+    total=False,
+)
+
+MaintenanceWindowStepFunctionsParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
+    {
+        "Input": str,
+        "Name": str,
     },
     total=False,
 )
 
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
 )
 
+MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    {
+        "Values": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredModifyDocumentPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDocumentPermissionRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionType": Literal["Share"],
     },
 )
@@ -2838,79 +2704,86 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
+
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
 )
 
+OpsItemDataValueOutputTypeDef = TypedDict(
+    "OpsItemDataValueOutputTypeDef",
+    {
+        "Value": str,
+        "Type": OpsItemDataTypeType,
+    },
+    total=False,
+)
+
 OpsItemIdentityTypeDef = TypedDict(
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+OpsItemNotificationOutputTypeDef = TypedDict(
+    "OpsItemNotificationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Arn": str,
     },
     total=False,
 )
 
+RelatedOpsItemOutputTypeDef = TypedDict(
+    "RelatedOpsItemOutputTypeDef",
+    {
+        "OpsItemId": str,
+    },
+)
+
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
     total=False,
 )
 
-PatchFilterTypeDef = TypedDict(
-    "PatchFilterTypeDef",
+PatchFilterOutputTypeDef = TypedDict(
+    "PatchFilterOutputTypeDef",
     {
         "Key": PatchFilterKeyType,
-        "Values": Sequence[str],
-    },
-)
-
-PutInventoryResultTypeDef = TypedDict(
-    "PutInventoryResultTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Values": List[str],
     },
 )
 
-PutParameterResultTypeDef = TypedDict(
-    "PutParameterResultTypeDef",
+PatchFilterTypeDef = TypedDict(
+    "PatchFilterTypeDef",
     {
-        "Version": int,
-        "Tier": ParameterTierType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": PatchFilterKeyType,
+        "Values": Sequence[str],
     },
 )
 
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -2922,76 +2795,36 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyHash": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
@@ -3000,58 +2833,53 @@
 ResetServiceSettingRequestRequestTypeDef = TypedDict(
     "ResetServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
     },
 )
 
+ResourceDataSyncOrganizationalUnitOutputTypeDef = TypedDict(
+    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
+    {
+        "OrganizationalUnitId": str,
+    },
+    total=False,
+)
+
 ResourceDataSyncOrganizationalUnitTypeDef = TypedDict(
     "ResourceDataSyncOrganizationalUnitTypeDef",
     {
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-ResourceDataSyncDestinationDataSharingTypeDef = TypedDict(
-    "ResourceDataSyncDestinationDataSharingTypeDef",
+ResourceDataSyncDestinationDataSharingOutputTypeDef = TypedDict(
+    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
     {
         "DestinationDataSharingType": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResourceDataSyncDestinationDataSharingTypeDef = TypedDict(
+    "ResourceDataSyncDestinationDataSharingTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DestinationDataSharingType": str,
     },
+    total=False,
 )
 
 ResumeSessionRequestRequestTypeDef = TypedDict(
     "ResumeSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-ResumeSessionResponseTypeDef = TypedDict(
-    "ResumeSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendAutomationSignalRequestRequestTypeDef = TypedDict(
     "_RequiredSendAutomationSignalRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
         "SignalType": SignalTypeType,
     },
 )
@@ -3059,20 +2887,22 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
+
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -3081,30 +2911,14 @@
 StartAssociationsOnceRequestRequestTypeDef = TypedDict(
     "StartAssociationsOnceRequestRequestTypeDef",
     {
         "AssociationIds": Sequence[str],
     },
 )
 
-StartAutomationExecutionResultTypeDef = TypedDict(
-    "StartAutomationExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartChangeRequestExecutionResultTypeDef = TypedDict(
-    "StartChangeRequestExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 _OptionalStartSessionRequestRequestTypeDef = TypedDict(
@@ -3113,28 +2927,20 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
@@ -3142,53 +2948,38 @@
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
+
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnlabelParameterVersionRequestRequestTypeDef = TypedDict(
     "UnlabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "ParameterVersion": int,
         "Labels": Sequence[str],
     },
 )
 
-UnlabelParameterVersionResultTypeDef = TypedDict(
-    "UnlabelParameterVersionResultTypeDef",
-    {
-        "RemovedLabels": List[str],
-        "InvalidLabels": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDocumentDefaultVersionRequestRequestTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
     },
 )
@@ -3214,86 +3005,51 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-UpdateMaintenanceWindowResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
 
-UpdateOpsMetadataResultTypeDef = TypedDict(
-    "UpdateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateServiceSettingRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
         "SettingValue": str,
     },
 )
 
-DescribeDocumentPermissionResponseTypeDef = TypedDict(
-    "DescribeDocumentPermissionResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivationTypeDef = TypedDict(
     "ActivationTypeDef",
     {
         "ActivationId": str,
         "Description": str,
         "DefaultInstanceName": str,
         "IamRole": str,
         "RegistrationLimit": int,
         "RegistrationsCount": int,
         "ExpirationDate": datetime,
         "Expired": bool,
         "CreatedDate": datetime,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
@@ -3323,27 +3079,21 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
@@ -3360,211 +3110,529 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
+
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredAlarmConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAlarmConfigurationOutputTypeDef",
+    {
+        "Alarms": List[AlarmOutputTypeDef],
+    },
+)
+_OptionalAlarmConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAlarmConfigurationOutputTypeDef",
+    {
+        "IgnorePollAlarmFailure": bool,
+    },
+    total=False,
+)
+
+
+class AlarmConfigurationOutputTypeDef(
+    _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationTypeDef = TypedDict(
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
+
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
+
+AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
+        "AssociationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociationTypeDef = TypedDict(
-    "AssociationTypeDef",
+CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "CancelMaintenanceWindowExecutionResultTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationId": str,
-        "AssociationVersion": str,
-        "DocumentVersion": str,
-        "Targets": List[TargetTypeDef],
-        "LastExecutionDate": datetime,
-        "Overview": AssociationOverviewTypeDef,
-        "ScheduleExpression": str,
-        "AssociationName": str,
-        "ScheduleOffset": int,
-        "TargetMaps": List[Dict[str, List[str]]],
+        "WindowExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+CreateActivationResultTypeDef = TypedDict(
+    "CreateActivationResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "ActivationId": str,
+        "ActivationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+
+CreateMaintenanceWindowResultTypeDef = TypedDict(
+    "CreateMaintenanceWindowResultTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
+CreateOpsItemResponseTypeDef = TypedDict(
+    "CreateOpsItemResponseTypeDef",
+    {
+        "OpsItemId": str,
+        "OpsItemArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+CreateOpsMetadataResultTypeDef = TypedDict(
+    "CreateOpsMetadataResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+
+CreatePatchBaselineResultTypeDef = TypedDict(
+    "CreatePatchBaselineResultTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
+DeleteMaintenanceWindowResultTypeDef = TypedDict(
+    "DeleteMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-MaintenanceWindowTargetTypeDef = TypedDict(
-    "MaintenanceWindowTargetTypeDef",
+DeleteParametersResultTypeDef = TypedDict(
+    "DeleteParametersResultTypeDef",
+    {
+        "DeletedParameters": List[str],
+        "InvalidParameters": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePatchBaselineResultTypeDef = TypedDict(
+    "DeletePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": List[TargetTypeDef],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetTypeDef],
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+
+DescribeDocumentPermissionResponseTypeDef = TypedDict(
+    "DescribeDocumentPermissionResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchGroupStateResultTypeDef = TypedDict(
+    "DescribePatchGroupStateResultTypeDef",
+    {
+        "Instances": int,
+        "InstancesWithInstalledPatches": int,
+        "InstancesWithInstalledOtherPatches": int,
+        "InstancesWithInstalledPendingRebootPatches": int,
+        "InstancesWithInstalledRejectedPatches": int,
+        "InstancesWithMissingPatches": int,
+        "InstancesWithFailedPatches": int,
+        "InstancesWithNotApplicablePatches": int,
+        "InstancesWithUnreportedNotApplicablePatches": int,
+        "InstancesWithCriticalNonCompliantPatches": int,
+        "InstancesWithSecurityNonCompliantPatches": int,
+        "InstancesWithOtherNonCompliantPatches": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchPropertiesResultTypeDef = TypedDict(
+    "DescribePatchPropertiesResultTypeDef",
     {
+        "Properties": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalendarStateResponseTypeDef = TypedDict(
+    "GetCalendarStateResponseTypeDef",
+    {
+        "State": CalendarStateType,
+        "AtTime": str,
+        "NextTransitionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectionStatusResponseTypeDef = TypedDict(
+    "GetConnectionStatusResponseTypeDef",
+    {
+        "Target": str,
+        "Status": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDefaultPatchBaselineResultTypeDef = TypedDict(
+    "GetDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "SnapshotId": str,
+        "SnapshotDownloadUrl": str,
+        "Product": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskIds": List[str],
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskExecutionId": str,
+        "InvocationId": str,
+        "ExecutionId": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "Parameters": str,
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "OwnerInformation": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowResultTypeDef = TypedDict(
+    "GetMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "ClientToken": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "NextExecutionTime": str,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
+GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+LabelParameterVersionResultTypeDef = TypedDict(
+    "LabelParameterVersionResultTypeDef",
+    {
+        "InvalidLabels": List[str],
+        "ParameterVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListInventoryEntriesResultTypeDef = TypedDict(
+    "ListInventoryEntriesResultTypeDef",
+    {
+        "TypeName": str,
+        "InstanceId": str,
+        "SchemaVersion": str,
+        "CaptureTime": str,
+        "Entries": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutInventoryResultTypeDef = TypedDict(
+    "PutInventoryResultTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutParameterResultTypeDef = TypedDict(
+    "PutParameterResultTypeDef",
+    {
+        "Version": int,
+        "Tier": ParameterTierType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyHash": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
     {
-        "WindowId": str,
         "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+
+RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "OwnerInformation": str,
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResumeSessionResponseTypeDef = TypedDict(
+    "ResumeSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAutomationExecutionResultTypeDef = TypedDict(
+    "StartAutomationExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartChangeRequestExecutionResultTypeDef = TypedDict(
+    "StartChangeRequestExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnlabelParameterVersionResultTypeDef = TypedDict(
+    "UnlabelParameterVersionResultTypeDef",
+    {
+        "RemovedLabels": List[str],
+        "InvalidLabels": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceWindowResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "Replace": bool,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateOpsMetadataResultTypeDef = TypedDict(
+    "UpdateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociationTypeDef = TypedDict(
+    "AssociationTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationId": str,
+        "AssociationVersion": str,
+        "DocumentVersion": str,
+        "Targets": List[TargetOutputTypeDef],
+        "LastExecutionDate": datetime,
+        "Overview": AssociationOverviewTypeDef,
+        "ScheduleExpression": str,
+        "AssociationName": str,
+        "ScheduleOffset": int,
+        "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
+MaintenanceWindowTargetTypeDef = TypedDict(
+    "MaintenanceWindowTargetTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": List[TargetOutputTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+    },
+    total=False,
+)
 
 UpdateMaintenanceWindowTargetResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTargetResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "AssociationId": str,
-        },
-    )
-)
-_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "Filters": Sequence[AssociationExecutionFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
@@ -3573,20 +3641,22 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3595,36 +3665,14 @@
         "DetailedStatus": str,
         "LastExecutionDate": datetime,
         "OutputSource": OutputSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "AssociationId": str,
-        "ExecutionId": str,
-    },
-)
-_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef",
     {
         "AssociationId": str,
         "ExecutionId": str,
     },
 )
@@ -3634,39 +3682,41 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
-ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
-    {
-        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
+    },
+)
+
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3679,27 +3729,20 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
-DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
-    {
-        "Filters": Sequence[AutomationExecutionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -3722,29 +3765,17 @@
         "ExecutionEndDateTime": str,
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "Details": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
@@ -3752,25 +3783,14 @@
         "NextToken": str,
         "Filters": Sequence[CommandFilterTypeDef],
         "Details": bool,
     },
     total=False,
 )
 
-ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCommandsRequestRequestTypeDef = TypedDict(
     "ListCommandsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
@@ -3792,29 +3812,29 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
     },
     total=False,
 )
 
-MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersTypeDef",
+MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     {
         "Comment": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
@@ -3826,15 +3846,15 @@
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Id": str,
         "Title": str,
         "Status": ComplianceStatusType,
         "Severity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
 _RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
     "_RequiredPutComplianceItemsRequestRequestTypeDef",
@@ -3851,71 +3871,44 @@
     {
         "ItemContentHash": str,
         "UploadType": ComplianceUploadTypeType,
     },
     total=False,
 )
 
+
 class PutComplianceItemsRequestRequestTypeDef(
     _RequiredPutComplianceItemsRequestRequestTypeDef,
     _OptionalPutComplianceItemsRequestRequestTypeDef,
 ):
     pass
 
-ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "ResourceIds": Sequence[str],
-        "ResourceTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -3955,19 +3948,99 @@
         "ExpirationDate": Union[datetime, str],
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
+
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+    },
+    total=False,
+)
+
+
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3982,84 +4055,20 @@
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
-DocumentIdentifierTypeDef = TypedDict(
-    "DocumentIdentifierTypeDef",
-    {
-        "Name": str,
-        "CreatedDate": datetime,
-        "DisplayName": str,
-        "Owner": str,
-        "VersionName": str,
-        "PlatformTypes": List[PlatformTypeType],
-        "DocumentVersion": str,
-        "DocumentType": DocumentTypeType,
-        "SchemaVersion": str,
-        "DocumentFormat": DocumentFormatType,
-        "TargetType": str,
-        "Tags": List[TagTypeDef],
-        "Requires": List[DocumentRequiresTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "Author": str,
-    },
-    total=False,
-)
-
-GetDocumentResultTypeDef = TypedDict(
-    "GetDocumentResultTypeDef",
-    {
-        "Name": str,
-        "CreatedDate": datetime,
-        "DisplayName": str,
-        "VersionName": str,
-        "DocumentVersion": str,
-        "Status": DocumentStatusType,
-        "StatusInformation": str,
-        "Content": str,
-        "DocumentType": DocumentTypeType,
-        "DocumentFormat": DocumentFormatType,
-        "Requires": List[DocumentRequiresTypeDef],
-        "AttachmentsContent": List[AttachmentContentTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OpsItemSummaryTypeDef = TypedDict(
-    "OpsItemSummaryTypeDef",
-    {
-        "CreatedBy": str,
-        "CreatedTime": datetime,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Priority": int,
-        "Source": str,
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Title": str,
-        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
-        "Category": str,
-        "Severity": str,
-        "OpsItemType": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
-    },
-    total=False,
-)
 
 _RequiredCreateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsItemRequestRequestTypeDef",
     {
         "Description": str,
         "Source": str,
         "Title": str,
@@ -4081,47 +4090,20 @@
         "PlannedStartTime": Union[datetime, str],
         "PlannedEndTime": Union[datetime, str],
         "AccountId": str,
     },
     total=False,
 )
 
+
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
-OpsItemTypeDef = TypedDict(
-    "OpsItemTypeDef",
-    {
-        "CreatedBy": str,
-        "OpsItemType": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Notifications": List[OpsItemNotificationTypeDef],
-        "Priority": int,
-        "RelatedOpsItems": List[RelatedOpsItemTypeDef],
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Version": str,
-        "Title": str,
-        "Source": str,
-        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
-        "Category": str,
-        "Severity": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
-        "OpsItemArn": str,
-    },
-    total=False,
-)
 
 _RequiredUpdateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
@@ -4143,19 +4125,21 @@
         "PlannedStartTime": Union[datetime, str],
         "PlannedEndTime": Union[datetime, str],
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -4163,28 +4147,20 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-GetOpsMetadataResultTypeDef = TypedDict(
-    "GetOpsMetadataResultTypeDef",
-    {
-        "ResourceId": str,
-        "Metadata": Dict[str, MetadataValueTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
@@ -4193,34 +4169,410 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
+DescribeActivationsRequestRequestTypeDef = TypedDict(
+    "DescribeActivationsRequestRequestTypeDef",
+    {
+        "Filters": Sequence[DescribeActivationsFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeActivationsRequestDescribeActivationsPaginateTypeDef = TypedDict(
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeActivationsRequestRequestTypeDef = TypedDict(
-    "DescribeActivationsRequestRequestTypeDef",
+_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     {
-        "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "AssociationId": str,
+        "ExecutionId": str,
+    },
+)
+_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "AssociationId": str,
+        },
+    )
+)
+_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "Filters": Sequence[AssociationExecutionFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+):
+    pass
+
+
+DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    {
+        "Filters": Sequence[AutomationExecutionFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
+    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "BaselineId": str,
+    },
+)
+_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
+    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
+    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+    },
+)
+_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
+    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+):
+    pass
+
+
+DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    {
+        "DeletionId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "OperatingSystem": OperatingSystemType,
+        "Property": PatchPropertyType,
+    },
+)
+_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "PatchSet": PatchSetType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
+    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+):
+    pass
+
+
+GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    {
+        "TypeName": str,
+        "Aggregator": bool,
+        "SubType": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "WithDecryption": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
+    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
+    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    {
+        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "Details": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "ResourceIds": Sequence[str],
+        "ResourceTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
+    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    {
+        "SyncType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
@@ -4228,25 +4580,27 @@
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4256,25 +4610,27 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeAvailablePatchesRequestRequestTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestRequestTypeDef",
     {
@@ -4291,25 +4647,27 @@
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4318,29 +4676,31 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
     TypedDict(
         "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
         {
             "WindowId": str,
             "Targets": Sequence[TargetTypeDef],
             "ResourceType": MaintenanceWindowResourceTypeType,
             "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
+            "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
 DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
@@ -4355,15 +4715,15 @@
     total=False,
 )
 
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchBaselinesRequestRequestTypeDef = TypedDict(
     "DescribePatchBaselinesRequestRequestTypeDef",
     {
@@ -4374,15 +4734,15 @@
     total=False,
 )
 
 DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef = TypedDict(
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchGroupsRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupsRequestRequestTypeDef",
     {
@@ -4394,33 +4754,33 @@
 )
 
 DescribeAvailablePatchesResultTypeDef = TypedDict(
     "DescribeAvailablePatchesResultTypeDef",
     {
         "Patches": List[PatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEffectiveInstanceAssociationsResultTypeDef = TypedDict(
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     {
         "Associations": List[InstanceAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef = TypedDict(
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     {
         "InstanceInformationFilterList": Sequence[InstanceInformationFilterTypeDef],
         "Filters": Sequence[InstanceInformationStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeInstanceInformationRequestRequestTypeDef = TypedDict(
     "DescribeInstanceInformationRequestRequestTypeDef",
     {
@@ -4438,25 +4798,27 @@
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4465,69 +4827,73 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchStatesResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchesResultTypeDef = TypedDict(
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4537,41 +4903,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4580,41 +4950,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4623,41 +4997,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4666,41 +5044,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -4709,25 +5091,27 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeMaintenanceWindowsRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestRequestTypeDef",
     {
@@ -4741,59 +5125,59 @@
 DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef",
     {
         "WindowExecutionTaskInvocationIdentities": List[
             MaintenanceWindowExecutionTaskInvocationIdentityTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionsResultTypeDef",
     {
         "WindowExecutions": List[MaintenanceWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowScheduleResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleResultTypeDef",
     {
         "ScheduledWindowExecutions": List[ScheduledWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsForTargetResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsForTargetResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityForTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef = TypedDict(
     "DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef",
     {
         "OpsItemFilters": Sequence[OpsItemFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeOpsItemsRequestRequestTypeDef = TypedDict(
     "DescribeOpsItemsRequestRequestTypeDef",
     {
@@ -4812,25 +5196,27 @@
 )
 _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef = TypedDict(
     "_OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef",
     {
         "Recursive": bool,
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -4841,26 +5227,28 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeParametersRequestRequestTypeDef = TypedDict(
     "DescribeParametersRequestRequestTypeDef",
     {
@@ -4873,15 +5261,15 @@
 )
 
 DescribePatchBaselinesResultTypeDef = TypedDict(
     "DescribePatchBaselinesResultTypeDef",
     {
         "BaselineIdentities": List[PatchBaselineIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PatchGroupPatchBaselineMappingTypeDef = TypedDict(
     "PatchGroupPatchBaselineMappingTypeDef",
     {
         "PatchGroup": str,
@@ -4896,25 +5284,27 @@
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
         "Filters": Sequence[SessionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -4923,24 +5313,68 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
+
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DocumentIdentifierTypeDef = TypedDict(
+    "DocumentIdentifierTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "Owner": str,
+        "VersionName": str,
+        "PlatformTypes": List[PlatformTypeType],
+        "DocumentVersion": str,
+        "DocumentType": DocumentTypeType,
+        "SchemaVersion": str,
+        "DocumentFormat": DocumentFormatType,
+        "TargetType": str,
+        "Tags": List[TagOutputTypeDef],
+        "Requires": List[DocumentRequiresOutputTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "Author": str,
+    },
+    total=False,
+)
+
+GetDocumentResultTypeDef = TypedDict(
+    "GetDocumentResultTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "VersionName": str,
+        "DocumentVersion": str,
+        "Status": DocumentStatusType,
+        "StatusInformation": str,
+        "Content": str,
+        "DocumentType": DocumentTypeType,
+        "DocumentFormat": DocumentFormatType,
+        "Requires": List[DocumentRequiresOutputTypeDef],
+        "AttachmentsContent": List[AttachmentContentTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
@@ -4959,17 +5393,17 @@
         "PlatformTypes": List[PlatformTypeType],
         "DocumentType": DocumentTypeType,
         "SchemaVersion": str,
         "LatestVersion": str,
         "DefaultVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "AttachmentsInformation": List[AttachmentInformationTypeDef],
-        "Requires": List[DocumentRequiresTypeDef],
+        "Requires": List[DocumentRequiresOutputTypeDef],
         "Author": str,
         "ReviewInformation": List[ReviewInformationTypeDef],
         "ApprovedVersion": str,
         "PendingReviewVersion": str,
         "ReviewStatus": ReviewStatusType,
         "Category": List[str],
         "CategoryEnum": List[str],
@@ -4978,15 +5412,15 @@
 )
 
 ListDocumentsRequestListDocumentsPaginateTypeDef = TypedDict(
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     {
         "DocumentFilterList": Sequence[DocumentFilterTypeDef],
         "Filters": Sequence[DocumentKeyValuesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
@@ -5000,15 +5434,15 @@
 
 DocumentReviewerResponseSourceTypeDef = TypedDict(
     "DocumentReviewerResponseSourceTypeDef",
     {
         "CreateTime": datetime,
         "UpdatedTime": datetime,
         "ReviewStatus": ReviewStatusType,
-        "Comment": List[DocumentReviewCommentSourceTypeDef],
+        "Comment": List[DocumentReviewCommentSourceOutputTypeDef],
         "Reviewer": str,
     },
     total=False,
 )
 
 _RequiredDocumentReviewsTypeDef = TypedDict(
     "_RequiredDocumentReviewsTypeDef",
@@ -5020,23 +5454,25 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
+
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
+
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EffectivePatchTypeDef = TypedDict(
     "EffectivePatchTypeDef",
     {
         "Patch": PatchTypeDef,
@@ -5057,20 +5493,22 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
+
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5088,27 +5526,29 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetInventoryRequestRequestTypeDef = TypedDict(
     "GetInventoryRequestRequestTypeDef",
     {
@@ -5117,14 +5557,24 @@
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+GetOpsMetadataResultTypeDef = TypedDict(
+    "GetOpsMetadataResultTypeDef",
+    {
+        "ResourceId": str,
+        "Metadata": Dict[str, MetadataValueOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OpsAggregatorTypeDef = TypedDict(
     "OpsAggregatorTypeDef",
     {
         "AggregatorType": str,
         "TypeName": str,
         "AttributeName": str,
         "Values": Mapping[str, str],
@@ -5137,15 +5587,15 @@
 GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef = TypedDict(
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     {
         "SyncName": str,
         "Filters": Sequence[OpsFilterTypeDef],
         "Aggregators": Sequence["OpsAggregatorTypeDef"],
         "ResultAttributes": Sequence[OpsResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetOpsSummaryRequestRequestTypeDef = TypedDict(
     "GetOpsSummaryRequestRequestTypeDef",
     {
@@ -5159,58 +5609,58 @@
     total=False,
 )
 
 GetParameterResultTypeDef = TypedDict(
     "GetParameterResultTypeDef",
     {
         "Parameter": ParameterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersByPathResultTypeDef = TypedDict(
     "GetParametersByPathResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersResultTypeDef = TypedDict(
     "GetParametersResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceSettingResultTypeDef = TypedDict(
     "GetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetServiceSettingResultTypeDef = TypedDict(
     "ResetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceInformationTypeDef = TypedDict(
     "InstanceInformationTypeDef",
     {
         "InstanceId": str,
@@ -5234,14 +5684,22 @@
         "AssociationOverview": InstanceAggregatedAssociationOverviewTypeDef,
         "SourceId": str,
         "SourceType": SourceTypeType,
     },
     total=False,
 )
 
+InstanceAssociationOutputLocationOutputTypeDef = TypedDict(
+    "InstanceAssociationOutputLocationOutputTypeDef",
+    {
+        "S3Location": S3OutputLocationOutputTypeDef,
+    },
+    total=False,
+)
+
 InstanceAssociationOutputLocationTypeDef = TypedDict(
     "InstanceAssociationOutputLocationTypeDef",
     {
         "S3Location": S3OutputLocationTypeDef,
     },
     total=False,
 )
@@ -5276,19 +5734,21 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
+
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5302,15 +5762,15 @@
     total=False,
 )
 
 ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef = TypedDict(
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     {
         "Filters": Sequence[OpsItemEventFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemEventsRequestRequestTypeDef = TypedDict(
     "ListOpsItemEventsRequestRequestTypeDef",
     {
@@ -5322,15 +5782,15 @@
 )
 
 ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     {
         "OpsItemId": str,
         "Filters": Sequence[OpsItemRelatedItemsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemRelatedItemsRequestRequestTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     {
@@ -5342,15 +5802,15 @@
     total=False,
 )
 
 ListOpsMetadataRequestListOpsMetadataPaginateTypeDef = TypedDict(
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     {
         "Filters": Sequence[OpsMetadataFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsMetadataRequestRequestTypeDef = TypedDict(
     "ListOpsMetadataRequestRequestTypeDef",
     {
@@ -5362,27 +5822,69 @@
 )
 
 ListOpsMetadataResultTypeDef = TypedDict(
     "ListOpsMetadataResultTypeDef",
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersTypeDef",
+    {
+        "Comment": str,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "DocumentVersion": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ServiceRoleArn": str,
+        "TimeoutSeconds": int,
+    },
+    total=False,
+)
+
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
 )
 
+OpsItemSummaryTypeDef = TypedDict(
+    "OpsItemSummaryTypeDef",
+    {
+        "CreatedBy": str,
+        "CreatedTime": datetime,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Priority": int,
+        "Source": str,
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Title": str,
+        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
+        "Category": str,
+        "Severity": str,
+        "OpsItemType": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+    },
+    total=False,
+)
+
 OpsItemEventSummaryTypeDef = TypedDict(
     "OpsItemEventSummaryTypeDef",
     {
         "OpsItemId": str,
         "EventId": str,
         "Source": str,
         "DetailType": str,
@@ -5405,14 +5907,43 @@
         "CreatedTime": datetime,
         "LastModifiedBy": OpsItemIdentityTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+OpsItemTypeDef = TypedDict(
+    "OpsItemTypeDef",
+    {
+        "CreatedBy": str,
+        "OpsItemType": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Notifications": List[OpsItemNotificationOutputTypeDef],
+        "Priority": int,
+        "RelatedOpsItems": List[RelatedOpsItemOutputTypeDef],
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Version": str,
+        "Title": str,
+        "Source": str,
+        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
+        "Category": str,
+        "Severity": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+        "OpsItemArn": str,
+    },
+    total=False,
+)
+
 ParameterHistoryTypeDef = TypedDict(
     "ParameterHistoryTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "KeyId": str,
         "LastModifiedDate": datetime,
@@ -5443,41 +5974,98 @@
         "Tier": ParameterTierType,
         "Policies": List[ParameterInlinePolicyTypeDef],
         "DataType": str,
     },
     total=False,
 )
 
+PatchFilterGroupOutputTypeDef = TypedDict(
+    "PatchFilterGroupOutputTypeDef",
+    {
+        "PatchFilters": List[PatchFilterOutputTypeDef],
+    },
+)
+
 PatchFilterGroupTypeDef = TypedDict(
     "PatchFilterGroupTypeDef",
     {
         "PatchFilters": Sequence[PatchFilterTypeDef],
     },
 )
 
+_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationSourceType": str,
+    },
+)
+_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
+    _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+    _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+):
+    pass
+
+
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
+
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
+
+_RequiredResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
+    "_RequiredResourceDataSyncS3DestinationOutputTypeDef",
+    {
+        "BucketName": str,
+        "SyncFormat": Literal["JsonSerDe"],
+        "Region": str,
+    },
+)
+_OptionalResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
+    "_OptionalResourceDataSyncS3DestinationOutputTypeDef",
+    {
+        "Prefix": str,
+        "AWSKMSKeyARN": str,
+        "DestinationDataSharing": ResourceDataSyncDestinationDataSharingOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ResourceDataSyncS3DestinationOutputTypeDef(
+    _RequiredResourceDataSyncS3DestinationOutputTypeDef,
+    _OptionalResourceDataSyncS3DestinationOutputTypeDef,
+):
+    pass
+
+
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5488,19 +6076,21 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
+
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -5516,30 +6106,30 @@
 )
 
 DescribeActivationsResultTypeDef = TypedDict(
     "DescribeActivationsResultTypeDef",
     {
         "ActivationList": List[ActivationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationExecutionTypeDef = TypedDict(
     "AssociationExecutionTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "Status": str,
         "DetailedStatus": str,
         "CreatedTime": datetime,
         "LastExecutionDate": datetime,
         "ResourceCountByStatus": str,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
@@ -5547,94 +6137,109 @@
         "CommandId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "Comment": str,
         "ExpiresAfter": datetime,
         "Parameters": Dict[str, List[str]],
         "InstanceIds": List[str],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "RequestedDateTime": datetime,
         "Status": CommandStatusType,
         "StatusDetails": str,
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
         "TimeoutSeconds": int,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 GetMaintenanceWindowExecutionTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "TaskArn": str,
         "ServiceRole": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "TaskParameters": List[Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef]],
+        "TaskParameters": List[
+            Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]
+        ],
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 MaintenanceWindowTaskTypeDef = TypedDict(
     "MaintenanceWindowTaskTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "Targets": List[TargetTypeDef],
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "Targets": List[TargetOutputTypeDef],
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "Priority": int,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+TargetLocationOutputTypeDef = TypedDict(
+    "TargetLocationOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "Regions": List[str],
+        "TargetLocationMaxConcurrency": str,
+        "TargetLocationMaxErrors": str,
+        "ExecutionRoleName": str,
+        "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredSendCommandRequestRequestTypeDef = TypedDict(
     "_RequiredSendCommandRequestRequestTypeDef",
     {
@@ -5661,19 +6266,21 @@
         "NotificationConfig": NotificationConfigTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SendCommandRequestRequestTypeDef(
     _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
 ):
     pass
 
+
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -5684,62 +6291,62 @@
 )
 
 ListAssociationsResultTypeDef = TypedDict(
     "ListAssociationsResultTypeDef",
     {
         "Associations": List[AssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTargetsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     {
         "Targets": List[MaintenanceWindowTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionTargetsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionTargetsResultTypeDef",
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     {
-        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersTypeDef,
-        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
+        "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersOutputTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
         "ComplianceItems": List[ComplianceItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryItemTypeDef = TypedDict(
     "ComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
@@ -5753,77 +6360,60 @@
     "ResourceComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Status": ComplianceStatusType,
         "OverallSeverity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
-ListDocumentsResultTypeDef = TypedDict(
-    "ListDocumentsResultTypeDef",
-    {
-        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeOpsItemsResponseTypeDef = TypedDict(
-    "DescribeOpsItemsResponseTypeDef",
+DescribePatchGroupsResultTypeDef = TypedDict(
+    "DescribePatchGroupsResultTypeDef",
     {
+        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
-        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOpsItemResponseTypeDef = TypedDict(
-    "GetOpsItemResponseTypeDef",
-    {
-        "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribePatchGroupsResultTypeDef = TypedDict(
-    "DescribePatchGroupsResultTypeDef",
+ListDocumentsResultTypeDef = TypedDict(
+    "ListDocumentsResultTypeDef",
     {
-        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
+        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDocumentResultTypeDef = TypedDict(
     "DescribeDocumentResultTypeDef",
     {
         "Document": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDocumentResultTypeDef = TypedDict(
     "UpdateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataResponseInfoTypeDef = TypedDict(
     "DocumentMetadataResponseInfoTypeDef",
     {
         "ReviewerResponse": List[DocumentReviewerResponseSourceTypeDef],
@@ -5842,26 +6432,28 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryAggregatorTypeDef = TypedDict(
     "InventoryAggregatorTypeDef",
     {
         "Expression": str,
@@ -5872,15 +6464,15 @@
 )
 
 DescribeInstanceInformationResultTypeDef = TypedDict(
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": str,
@@ -5901,15 +6493,15 @@
 
 DeleteInventoryResultTypeDef = TypedDict(
     "DeleteInventoryResultTypeDef",
     {
         "DeletionId": str,
         "TypeName": str,
         "DeletionSummary": InventoryDeletionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDeletionStatusItemTypeDef = TypedDict(
     "InventoryDeletionStatusItemTypeDef",
     {
         "DeletionId": str,
@@ -5924,71 +6516,121 @@
 )
 
 GetInventorySchemaResultTypeDef = TypedDict(
     "GetInventorySchemaResultTypeDef",
     {
         "Schemas": List[InventoryItemSchemaTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInventoryResultTypeDef = TypedDict(
     "GetInventoryResultTypeDef",
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    {
+        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
+    },
+    total=False,
+)
+
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOpsItemsResponseTypeDef = TypedDict(
+    "DescribeOpsItemsResponseTypeDef",
+    {
+        "NextToken": str,
+        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemRelatedItemsResponseTypeDef = TypedDict(
     "ListOpsItemRelatedItemsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpsItemResponseTypeDef = TypedDict(
+    "GetOpsItemResponseTypeDef",
+    {
+        "OpsItem": OpsItemTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParametersResultTypeDef = TypedDict(
     "DescribeParametersResultTypeDef",
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPatchRuleOutputTypeDef = TypedDict(
+    "_RequiredPatchRuleOutputTypeDef",
+    {
+        "PatchFilterGroup": PatchFilterGroupOutputTypeDef,
     },
 )
+_OptionalPatchRuleOutputTypeDef = TypedDict(
+    "_OptionalPatchRuleOutputTypeDef",
+    {
+        "ComplianceLevel": PatchComplianceLevelType,
+        "ApproveAfterDays": int,
+        "ApproveUntilDate": str,
+        "EnableNonSecurity": bool,
+    },
+    total=False,
+)
+
+
+class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
+    pass
+
 
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
@@ -5999,17 +6641,32 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
+
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
+
+ResourceDataSyncSourceWithStateTypeDef = TypedDict(
+    "ResourceDataSyncSourceWithStateTypeDef",
+    {
+        "SourceType": str,
+        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+        "SourceRegions": List[str],
+        "IncludeFutureRegions": bool,
+        "State": str,
+        "EnableAllOpsDataSources": bool,
+    },
+    total=False,
+)
+
 _RequiredResourceDataSyncSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncSourceTypeDef",
     {
         "SourceType": str,
         "SourceRegions": Sequence[str],
     },
 )
@@ -6019,146 +6676,230 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
+
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
-ResourceDataSyncSourceWithStateTypeDef = TypedDict(
-    "ResourceDataSyncSourceWithStateTypeDef",
-    {
-        "SourceType": str,
-        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
-        "SourceRegions": List[str],
-        "IncludeFutureRegions": bool,
-        "State": str,
-        "EnableAllOpsDataSources": bool,
-    },
-    total=False,
-)
 
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionsResultTypeDef",
     {
         "AssociationExecutions": List[AssociationExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandsResultTypeDef = TypedDict(
     "ListCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "Command": CommandTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     {
         "WindowExecutionTaskIdentities": List[MaintenanceWindowExecutionTaskIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTasksResultTypeDef",
     {
         "Tasks": List[MaintenanceWindowTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationDescriptionTypeDef = TypedDict(
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationVersion": str,
         "Date": datetime,
         "LastUpdateAssociationDate": datetime,
-        "Status": AssociationStatusTypeDef,
+        "Status": AssociationStatusOutputTypeDef,
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 AssociationVersionInfoTypeDef = TypedDict(
     "AssociationVersionInfoTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
+_RequiredCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryOutputTypeDef",
+    {
+        "InstanceId": str,
+        "Parameters": Dict[str, List[str]],
+        "AutomationTargetParameterName": str,
+        "DocumentVersion": str,
+        "Targets": List[TargetOutputTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "AssociationName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": List[str],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": List[Dict[str, List[str]]],
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAssociationBatchRequestEntryOutputTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
+):
+    pass
+
+
+_RequiredRunbookOutputTypeDef = TypedDict(
+    "_RequiredRunbookOutputTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalRunbookOutputTypeDef = TypedDict(
+    "_OptionalRunbookOutputTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Dict[str, List[str]],
+        "TargetParameterName": str,
+        "Targets": List[TargetOutputTypeDef],
+        "TargetMaps": List[Dict[str, List[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": List[TargetLocationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
+    pass
+
+
+StepExecutionTypeDef = TypedDict(
+    "StepExecutionTypeDef",
+    {
+        "StepName": str,
+        "Action": str,
+        "TimeoutSeconds": int,
+        "OnFailure": str,
+        "MaxAttempts": int,
+        "ExecutionStartTime": datetime,
+        "ExecutionEndTime": datetime,
+        "StepStatus": AutomationExecutionStatusType,
+        "ResponseCode": str,
+        "Inputs": Dict[str, str],
+        "Outputs": Dict[str, List[str]],
+        "Response": str,
+        "FailureMessage": str,
+        "FailureDetails": FailureDetailsTypeDef,
+        "StepExecutionId": str,
+        "OverriddenParameters": Dict[str, List[str]],
+        "IsEnd": bool,
+        "NextStep": str,
+        "IsCritical": bool,
+        "ValidNextSteps": List[str],
+        "Targets": List[TargetOutputTypeDef],
+        "TargetLocation": TargetLocationOutputTypeDef,
+        "TriggeredAlarms": List[AlarmStateInformationTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
     "_RequiredCreateAssociationBatchRequestEntryTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
@@ -6182,20 +6923,22 @@
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateAssociationBatchRequestEntryTypeDef(
     _RequiredCreateAssociationBatchRequestEntryTypeDef,
     _OptionalCreateAssociationBatchRequestEntryTypeDef,
 ):
     pass
 
+
 _RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssociationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
@@ -6220,43 +6963,47 @@
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateAssociationRequestRequestTypeDef(
     _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredRunbookTypeDef = TypedDict(
     "_RequiredRunbookTypeDef",
     {
         "DocumentName": str,
     },
 )
 _OptionalRunbookTypeDef = TypedDict(
     "_OptionalRunbookTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
-        "TargetMaps": List[Dict[str, List[str]]],
+        "Targets": Sequence[TargetTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": Sequence[TargetLocationTypeDef],
     },
     total=False,
 )
 
+
 class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
+
 _RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartAutomationExecutionRequestRequestTypeDef",
     {
         "DocumentName": str,
     },
 )
 _OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
@@ -6274,49 +7021,21 @@
         "TargetLocations": Sequence[TargetLocationTypeDef],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StartAutomationExecutionRequestRequestTypeDef(
     _RequiredStartAutomationExecutionRequestRequestTypeDef,
     _OptionalStartAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
-StepExecutionTypeDef = TypedDict(
-    "StepExecutionTypeDef",
-    {
-        "StepName": str,
-        "Action": str,
-        "TimeoutSeconds": int,
-        "OnFailure": str,
-        "MaxAttempts": int,
-        "ExecutionStartTime": datetime,
-        "ExecutionEndTime": datetime,
-        "StepStatus": AutomationExecutionStatusType,
-        "ResponseCode": str,
-        "Inputs": Dict[str, str],
-        "Outputs": Dict[str, List[str]],
-        "Response": str,
-        "FailureMessage": str,
-        "FailureDetails": FailureDetailsTypeDef,
-        "StepExecutionId": str,
-        "OverriddenParameters": Dict[str, List[str]],
-        "IsEnd": bool,
-        "NextStep": str,
-        "IsCritical": bool,
-        "ValidNextSteps": List[str],
-        "Targets": List[TargetTypeDef],
-        "TargetLocation": TargetLocationTypeDef,
-        "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-    },
-    total=False,
-)
 
 _RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
@@ -6342,39 +7061,111 @@
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAssociationRequestRequestTypeDef(
     _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
 ):
     pass
 
+
 GetMaintenanceWindowTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowTaskResultTypeDef",
+    {
+        "WindowId": str,
+        "WindowTaskId": str,
+        "Targets": List[TargetOutputTypeDef],
+        "TaskArn": str,
+        "ServiceRoleArn": str,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "Name": str,
+        "Description": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListComplianceSummariesResultTypeDef = TypedDict(
+    "ListComplianceSummariesResultTypeDef",
+    {
+        "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceComplianceSummariesResultTypeDef = TypedDict(
+    "ListResourceComplianceSummariesResultTypeDef",
+    {
+        "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
+    "ListDocumentMetadataHistoryResponseTypeDef",
+    {
+        "Name": str,
+        "DocumentVersion": str,
+        "Author": str,
+        "Metadata": DocumentMetadataResponseInfoTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
+    "DescribeInstanceAssociationsStatusResultTypeDef",
+    {
+        "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInventoryDeletionsResultTypeDef = TypedDict(
+    "DescribeInventoryDeletionsResultTypeDef",
+    {
+        "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
@@ -6398,20 +7189,22 @@
         "ClientToken": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
     _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
     _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -6432,95 +7225,51 @@
         "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
 ):
     pass
 
-UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowTaskResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
-        "TaskArn": str,
-        "ServiceRoleArn": str,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-ListComplianceSummariesResultTypeDef = TypedDict(
-    "ListComplianceSummariesResultTypeDef",
+PatchRuleGroupOutputTypeDef = TypedDict(
+    "PatchRuleGroupOutputTypeDef",
     {
-        "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PatchRules": List[PatchRuleOutputTypeDef],
     },
 )
 
-ListResourceComplianceSummariesResultTypeDef = TypedDict(
-    "ListResourceComplianceSummariesResultTypeDef",
-    {
-        "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
-    "ListDocumentMetadataHistoryResponseTypeDef",
-    {
-        "Name": str,
-        "DocumentVersion": str,
-        "Author": str,
-        "Metadata": DocumentMetadataResponseInfoTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
-    "DescribeInstanceAssociationsStatusResultTypeDef",
-    {
-        "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeInventoryDeletionsResultTypeDef = TypedDict(
-    "DescribeInventoryDeletionsResultTypeDef",
+PatchRuleGroupTypeDef = TypedDict(
+    "PatchRuleGroupTypeDef",
     {
-        "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PatchRules": Sequence[PatchRuleTypeDef],
     },
 )
 
-PatchRuleGroupTypeDef = TypedDict(
-    "PatchRuleGroupTypeDef",
+ResourceDataSyncItemTypeDef = TypedDict(
+    "ResourceDataSyncItemTypeDef",
     {
-        "PatchRules": Sequence[PatchRuleTypeDef],
+        "SyncName": str,
+        "SyncType": str,
+        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationOutputTypeDef,
+        "LastSyncTime": datetime,
+        "LastSuccessfulSyncTime": datetime,
+        "SyncLastModifiedTime": datetime,
+        "LastStatus": LastResourceDataSyncStatusType,
+        "SyncCreatedTime": datetime,
+        "LastSyncStatusMessage": str,
     },
+    total=False,
 )
 
 _RequiredCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
@@ -6531,98 +7280,76 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
+
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
 )
 
-ResourceDataSyncItemTypeDef = TypedDict(
-    "ResourceDataSyncItemTypeDef",
-    {
-        "SyncName": str,
-        "SyncType": str,
-        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
-        "LastSyncTime": datetime,
-        "LastSuccessfulSyncTime": datetime,
-        "SyncLastModifiedTime": datetime,
-        "LastStatus": LastResourceDataSyncStatusType,
-        "SyncCreatedTime": datetime,
-        "LastSyncStatusMessage": str,
-    },
-    total=False,
-)
-
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationResultTypeDef = TypedDict(
     "DescribeAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationResultTypeDef = TypedDict(
     "UpdateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationStatusResultTypeDef = TypedDict(
     "UpdateAssociationStatusResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociationVersionsResultTypeDef = TypedDict(
     "ListAssociationVersionsResultTypeDef",
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
-    {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedCreateAssociationTypeDef = TypedDict(
     "FailedCreateAssociationTypeDef",
     {
-        "Entry": CreateAssociationBatchRequestEntryTypeDef,
+        "Entry": CreateAssociationBatchRequestEntryOutputTypeDef,
         "Message": str,
         "Fault": FaultType,
     },
     total=False,
 )
 
 AutomationExecutionMetadataTypeDef = TypedDict(
@@ -6639,62 +7366,33 @@
         "Outputs": Dict[str, List[str]],
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "FailureMessage": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
         "AutomationType": AutomationTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-        "Runbooks": Sequence[RunbookTypeDef],
-    },
-)
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "ScheduledTime": Union[datetime, str],
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
-        "ClientToken": str,
-        "AutoApprove": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": Union[datetime, str],
-        "ChangeDetails": str,
-    },
-    total=False,
-)
-
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
-):
-    pass
-
 AutomationExecutionTypeDef = TypedDict(
     "AutomationExecutionTypeDef",
     {
         "AutomationExecutionId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "ExecutionStartTime": datetime,
@@ -6707,40 +7405,121 @@
         "FailureMessage": str,
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "ExecutedBy": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ProgressCounters": ProgressCountersTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
 DescribeAutomationStepExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationStepExecutionsResultTypeDef",
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+    },
+)
+
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookTypeDef],
+    },
+)
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": Union[datetime, str],
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": Union[datetime, str],
+        "ChangeDetails": str,
+    },
+    total=False,
+)
+
+
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
+
+GetPatchBaselineResultTypeDef = TypedDict(
+    "GetPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "PatchGroups": List[str],
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePatchBaselineResultTypeDef = TypedDict(
+    "UpdatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
@@ -6777,41 +7556,21 @@
         "Sources": Sequence[PatchSourceTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-GetPatchBaselineResultTypeDef = TypedDict(
-    "GetPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "PatchGroups": List[str],
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
@@ -6829,73 +7588,54 @@
         "Description": str,
         "Sources": Sequence[PatchSourceTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-UpdatePatchBaselineResultTypeDef = TypedDict(
-    "UpdatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssociationBatchResultTypeDef = TypedDict(
     "CreateAssociationBatchResultTypeDef",
     {
         "Successful": List[AssociationDescriptionTypeDef],
         "Failed": List[FailedCreateAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAutomationExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationExecutionsResultTypeDef",
     {
         "AutomationExecutionMetadataList": List[AutomationExecutionMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutomationExecutionResultTypeDef = TypedDict(
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -6906,12 +7646,13 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
+
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/waiter.py` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm/waiter.pyi` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/PKG-INFO` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.0
-Summary: Type annotations for boto3.SSM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ssm"></a>
 
 # mypy-boto3-ssm
 
 [![PyPI - mypy-boto3-ssm](https://img.shields.io/pypi/v/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -643,288 +643,307 @@
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    AlarmOutputTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
-    AssociationStatusTypeDef,
-    TargetTypeDef,
+    AssociationStatusOutputTypeDef,
+    TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    AssociationStatusTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
+    CloudWatchOutputConfigOutputTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
-    NotificationConfigTypeDef,
+    NotificationConfigOutputTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
-    CreateActivationResultTypeDef,
+    TargetTypeDef,
     DocumentRequiresTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
-    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
-    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
-    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
-    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
+    DocumentRequiresOutputTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
+    DocumentReviewCommentSourceOutputTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
-    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
-    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
-    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
-    LoggingInfoTypeDef,
+    LoggingInfoOutputTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
+    MetadataValueOutputTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
+    S3OutputLocationOutputTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
-    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LoggingInfoTypeDef,
+    MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
+    MaintenanceWindowLambdaParametersOutputTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
+    NotificationConfigTypeDef,
+    MaintenanceWindowStepFunctionsParametersOutputTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
+    OpsItemDataValueOutputTypeDef,
     OpsItemIdentityTypeDef,
-    PaginatorConfigTypeDef,
+    OpsItemNotificationOutputTypeDef,
+    RelatedOpsItemOutputTypeDef,
     ParameterInlinePolicyTypeDef,
+    PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
+    ResourceDataSyncOrganizationalUnitOutputTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
+    ResourceDataSyncDestinationDataSharingOutputTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
-    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
-    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
-    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
-    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
+    CreateActivationResultTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
+    CreateOpsItemResponseTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
+    DeleteParametersResultTypeDef,
+    DeletePatchBaselineResultTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesResultTypeDef,
+    GetCalendarStateResponseTypeDef,
+    GetConnectionStatusResponseTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
+    GetMaintenanceWindowResultTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListInventoryEntriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
+    ResumeSessionResponseTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
+    StartSessionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
+    UnlabelParameterVersionResultTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     AssociationTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
     UpdateDocumentRequestRequestTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
     GetCommandInvocationResultTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
-    MaintenanceWindowRunCommandParametersTypeDef,
+    MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
     PutComplianceItemsRequestRequestTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
-    DocumentIdentifierTypeDef,
-    GetDocumentResultTypeDef,
-    OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
-    OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
-    GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeActivationsRequestRequestTypeDef,
+    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
     DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
@@ -966,142 +985,158 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribePatchBaselinesResultTypeDef,
     PatchGroupPatchBaselineMappingTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
+    DocumentIdentifierTypeDef,
+    GetDocumentResultTypeDef,
     DocumentDescriptionTypeDef,
     ListDocumentsRequestListDocumentsPaginateTypeDef,
     ListDocumentsRequestRequestTypeDef,
     DocumentReviewerResponseSourceTypeDef,
     DocumentReviewsTypeDef,
     ListDocumentVersionsResultTypeDef,
     EffectivePatchTypeDef,
     GetCommandInvocationRequestCommandExecutedWaitTypeDef,
     InventoryGroupTypeDef,
     ListInventoryEntriesRequestRequestTypeDef,
     GetInventoryRequestGetInventoryPaginateTypeDef,
     GetInventoryRequestRequestTypeDef,
+    GetOpsMetadataResultTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
+    InstanceAssociationOutputLocationOutputTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
     InventoryItemSchemaTypeDef,
     PutInventoryRequestRequestTypeDef,
     InventoryResultEntityTypeDef,
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
+    MaintenanceWindowRunCommandParametersTypeDef,
     OpsEntityTypeDef,
+    OpsItemSummaryTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
+    OpsItemTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
+    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
+    ResourceDataSyncS3DestinationOutputTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
+    TargetLocationOutputTypeDef,
     SendCommandRequestRequestTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
-    ListDocumentsResultTypeDef,
-    DescribeOpsItemsResponseTypeDef,
-    GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
+    ListDocumentsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
     DocumentMetadataResponseInfoTypeDef,
     UpdateDocumentMetadataRequestRequestTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     InventoryAggregatorTypeDef,
     DescribeInstanceInformationResultTypeDef,
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
+    DescribeOpsItemsResponseTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
+    GetOpsItemResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
+    PatchRuleOutputTypeDef,
     PatchRuleTypeDef,
-    ResourceDataSyncSourceTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
+    ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
+    RunbookOutputTypeDef,
+    StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
     CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
     StartAutomationExecutionRequestRequestTypeDef,
-    StepExecutionTypeDef,
     UpdateAssociationRequestRequestTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
-    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
-    ResourceDataSyncItemTypeDef,
     CreateAssociationResultTypeDef,
     DescribeAssociationResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
+    GetPatchBaselineResultTypeDef,
+    UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
-    GetPatchBaselineResultTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
-    UpdatePatchBaselineResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-1.28.0/mypy_boto3_ssm.egg-info/SOURCES.txt` & `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.0/setup.py` & `mypy-boto3-ssm-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSM 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SSM 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

