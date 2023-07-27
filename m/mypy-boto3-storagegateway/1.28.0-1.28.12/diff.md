# Comparing `tmp/mypy-boto3-storagegateway-1.28.0.tar.gz` & `tmp/mypy-boto3-storagegateway-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-storagegateway-1.28.0.tar", last modified: Thu Jul  6 21:00:44 2023, max compression
+gzip compressed data, was "mypy-boto3-storagegateway-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
```

## Comparing `mypy-boto3-storagegateway-1.28.0.tar` & `mypy-boto3-storagegateway-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:44.322445 mypy-boto3-storagegateway-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-06 21:00:44.314445 mypy-boto3-storagegateway-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:44.302445 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68220 2023-07-06 20:56:50.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68112 2023-07-06 20:56:50.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-06 20:56:50.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-07-06 20:56:50.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-07-06 20:56:50.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-07-06 20:56:50.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76928 2023-07-06 20:56:56.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    76851 2023-07-06 20:56:51.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:44.314445 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-06 21:00:44.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:44.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:44.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:44.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:44.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:44.000000 mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:44.322445 mypy-boto3-storagegateway-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:56:49.000000 mypy-boto3-storagegateway-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24276 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22761 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68220 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68112 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-27 11:47:45.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-07-27 11:47:46.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79123 2023-07-27 11:47:45.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24276 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:47:41.000000 mypy-boto3-storagegateway-1.28.12/setup.py
```

### Comparing `mypy-boto3-storagegateway-1.28.0/LICENSE` & `mypy-boto3-storagegateway-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.0/PKG-INFO` & `mypy-boto3-storagegateway-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.0
-Summary: Type annotations for boto3.StorageGateway 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.StorageGateway 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-storagegateway"></a>
 
 # mypy-boto3-storagegateway
 
 [![PyPI - mypy-boto3-storagegateway](https://img.shields.io/pypi/v/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-storagegateway?color=blue)](https://pypistats.org/packages/mypy-boto3-storagegateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,236 +374,243 @@
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
-    ActivateGatewayOutputTypeDef,
+    ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
-    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
-    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
-    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
-    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AttachVolumeOutputTypeDef,
+    AutomaticTapeCreationRuleOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
+    CacheAttributesOutputTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
-    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
-    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
-    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
-    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
-    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
-    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
-    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
+    TagOutputTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
-    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
-    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
-    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
-    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
+    NFSFileShareDefaultsOutputTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
-    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
-    ResetCacheOutputTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
+    SMBLocalGroupsTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
-    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
-    DescribeSnapshotScheduleOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     UpdateSnapshotScheduleInputRequestTypeDef,
+    ActivateGatewayOutputTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
+    AddUploadBufferOutputTypeDef,
+    AddWorkingStorageOutputTypeDef,
+    AssignTapePoolOutputTypeDef,
+    AssociateFileSystemOutputTypeDef,
+    AttachVolumeOutputTypeDef,
+    CancelArchivalOutputTypeDef,
+    CancelRetrievalOutputTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
+    DeleteFileShareOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
+    DeleteTapeOutputTypeDef,
+    DeleteTapePoolOutputTypeDef,
+    DeleteVolumeOutputTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
+    DescribeCacheOutputTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
+    DetachVolumeOutputTypeDef,
+    DisableGatewayOutputTypeDef,
+    DisassociateFileSystemOutputTypeDef,
+    JoinDomainOutputTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    RefreshCacheOutputTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
+    ResetCacheOutputTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
+    ShutdownGatewayOutputTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
-    SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
     UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
-    NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
+    DescribeSnapshotScheduleOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    SMBFileShareInfoTypeDef,
     DescribeSMBSettingsOutputTypeDef,
-    UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
-    DescribeSMBFileSharesOutputTypeDef,
+    NFSFileShareInfoTypeDef,
+    UpdateSMBLocalGroupsInputRequestTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
-    DescribeNFSFileSharesOutputTypeDef,
+    DescribeSMBFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
+    DescribeNFSFileSharesOutputTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-storagegateway-1.28.0/README.md` & `mypy-boto3-storagegateway-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-storagegateway"></a>
 
 # mypy-boto3-storagegateway
 
 [![PyPI - mypy-boto3-storagegateway](https://img.shields.io/pypi/v/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-storagegateway?color=blue)](https://pypistats.org/packages/mypy-boto3-storagegateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,236 +342,243 @@
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
-    ActivateGatewayOutputTypeDef,
+    ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
-    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
-    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
-    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
-    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AttachVolumeOutputTypeDef,
+    AutomaticTapeCreationRuleOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
+    CacheAttributesOutputTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
-    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
-    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
-    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
-    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
-    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
-    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
-    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
+    TagOutputTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
-    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
-    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
-    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
-    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
+    NFSFileShareDefaultsOutputTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
-    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
-    ResetCacheOutputTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
+    SMBLocalGroupsTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
-    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
-    DescribeSnapshotScheduleOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     UpdateSnapshotScheduleInputRequestTypeDef,
+    ActivateGatewayOutputTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
+    AddUploadBufferOutputTypeDef,
+    AddWorkingStorageOutputTypeDef,
+    AssignTapePoolOutputTypeDef,
+    AssociateFileSystemOutputTypeDef,
+    AttachVolumeOutputTypeDef,
+    CancelArchivalOutputTypeDef,
+    CancelRetrievalOutputTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
+    DeleteFileShareOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
+    DeleteTapeOutputTypeDef,
+    DeleteTapePoolOutputTypeDef,
+    DeleteVolumeOutputTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
+    DescribeCacheOutputTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
+    DetachVolumeOutputTypeDef,
+    DisableGatewayOutputTypeDef,
+    DisassociateFileSystemOutputTypeDef,
+    JoinDomainOutputTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    RefreshCacheOutputTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
+    ResetCacheOutputTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
+    ShutdownGatewayOutputTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
-    SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
     UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
-    NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
+    DescribeSnapshotScheduleOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    SMBFileShareInfoTypeDef,
     DescribeSMBSettingsOutputTypeDef,
-    UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
-    DescribeSMBFileSharesOutputTypeDef,
+    NFSFileShareInfoTypeDef,
+    UpdateSMBLocalGroupsInputRequestTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
-    DescribeNFSFileSharesOutputTypeDef,
+    DescribeSMBFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
+    DescribeNFSFileSharesOutputTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/__init__.py` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/__init__.pyi` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/__main__.py` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.StorageGateway 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.StorageGateway 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/client.py` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/client.pyi` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/literals.py` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
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
@@ -284,26 +285,28 @@
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

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/literals.pyi` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
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
@@ -282,26 +283,28 @@
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

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/paginator.py` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,30 +86,30 @@
 class DescribeTapeArchivesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTapeArchivesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
         """
 
 
 class DescribeTapeRecoveryPointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTapeRecoveryPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
         """
 
 
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapespaginator)
         """
 
 
@@ -139,118 +139,118 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describevtldevicespaginator)
         """
 
 
 class ListFileSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFileSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
         """
 
 
 class ListFileSystemAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFileSystemAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
         """
 
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTapePoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
     """
 
     def paginate(
-        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTapePoolsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
         """
 
 
 class ListTapesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
         """
 
 
 class ListVolumesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVolumesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
         """
```

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/paginator.pyi` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -83,29 +83,29 @@
 class DescribeTapeArchivesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTapeArchivesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
         """
 
 class DescribeTapeRecoveryPointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTapeRecoveryPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
         """
 
 class DescribeTapesPaginator(Paginator):
@@ -115,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapespaginator)
         """
 
 class DescribeVTLDevicesPaginator(Paginator):
@@ -133,111 +133,111 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describevtldevicespaginator)
         """
 
 class ListFileSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFileSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
         """
 
 class ListFileSystemAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFileSystemAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
         """
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTapePoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
     """
 
     def paginate(
-        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTapePoolsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
         """
 
 class ListTapesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
         """
 
 class ListVolumesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVolumesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
         """
```

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/type_defs.py` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,310 +33,288 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "ActivateGatewayOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCacheInputRequestTypeDef",
-    "AddCacheOutputTypeDef",
-    "AddTagsToResourceOutputTypeDef",
     "AddUploadBufferInputRequestTypeDef",
-    "AddUploadBufferOutputTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
-    "AddWorkingStorageOutputTypeDef",
     "AssignTapePoolInputRequestTypeDef",
-    "AssignTapePoolOutputTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
-    "AssociateFileSystemOutputTypeDef",
     "AttachVolumeInputRequestTypeDef",
-    "AttachVolumeOutputTypeDef",
+    "AutomaticTapeCreationRuleOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
+    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
+    "CacheAttributesOutputTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
-    "CancelArchivalOutputTypeDef",
     "CancelRetrievalInputRequestTypeDef",
-    "CancelRetrievalOutputTypeDef",
     "ChapInfoTypeDef",
-    "CreateCachediSCSIVolumeOutputTypeDef",
     "NFSFileShareDefaultsTypeDef",
-    "CreateNFSFileShareOutputTypeDef",
-    "CreateSMBFileShareOutputTypeDef",
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    "CreateSnapshotOutputTypeDef",
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    "CreateTapePoolOutputTypeDef",
-    "CreateTapeWithBarcodeOutputTypeDef",
-    "CreateTapesOutputTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
-    "DeleteBandwidthRateLimitOutputTypeDef",
     "DeleteChapCredentialsInputRequestTypeDef",
-    "DeleteChapCredentialsOutputTypeDef",
     "DeleteFileShareInputRequestTypeDef",
-    "DeleteFileShareOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
-    "DeleteGatewayOutputTypeDef",
     "DeleteSnapshotScheduleInputRequestTypeDef",
-    "DeleteSnapshotScheduleOutputTypeDef",
     "DeleteTapeArchiveInputRequestTypeDef",
-    "DeleteTapeArchiveOutputTypeDef",
     "DeleteTapeInputRequestTypeDef",
-    "DeleteTapeOutputTypeDef",
     "DeleteTapePoolInputRequestTypeDef",
-    "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeInputRequestTypeDef",
-    "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitInputRequestTypeDef",
-    "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
-    "DescribeCacheOutputTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
+    "TagOutputTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
-    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
+    "SMBLocalGroupsOutputTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
-    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
-    "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeTapesInputRequestTypeDef",
     "TapeTypeDef",
     "DescribeUploadBufferInputRequestTypeDef",
-    "DescribeUploadBufferOutputTypeDef",
-    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
-    "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeInputRequestTypeDef",
-    "DetachVolumeOutputTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
-    "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
-    "DisassociateFileSystemOutputTypeDef",
     "DiskTypeDef",
+    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
-    "JoinDomainOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSharesInputRequestTypeDef",
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListFileSystemAssociationsInputRequestTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
     "ListLocalDisksInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
     "ListTapePoolsInputRequestTypeDef",
     "PoolInfoTypeDef",
-    "ListTapesInputListTapesPaginateTypeDef",
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
-    "ListVolumeInitiatorsOutputTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
-    "ListVolumesInputListVolumesPaginateTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
+    "NFSFileShareDefaultsOutputTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
-    "NotifyWhenUploadedOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshCacheInputRequestTypeDef",
-    "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
-    "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheInputRequestTypeDef",
-    "ResetCacheOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
-    "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
-    "SetLocalConsolePasswordOutputTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
-    "SetSMBGuestPasswordOutputTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
-    "ShutdownGatewayOutputTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
-    "StartAvailabilityMonitorTestOutputTypeDef",
     "StartGatewayInputRequestTypeDef",
-    "StartGatewayOutputTypeDef",
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
-    "UpdateChapCredentialsOutputTypeDef",
-    "UpdateFileSystemAssociationOutputTypeDef",
     "UpdateGatewayInformationInputRequestTypeDef",
-    "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
-    "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateMaintenanceStartTimeInputRequestTypeDef",
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    "UpdateNFSFileShareOutputTypeDef",
-    "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeInputRequestTypeDef",
-    "UpdateVTLDeviceTypeOutputTypeDef",
     "ActivateGatewayInputRequestTypeDef",
     "AddTagsToResourceInputRequestTypeDef",
     "CreateCachediSCSIVolumeInputRequestTypeDef",
     "CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "CreateStorediSCSIVolumeInputRequestTypeDef",
     "CreateTapePoolInputRequestTypeDef",
     "CreateTapeWithBarcodeInputRequestTypeDef",
     "CreateTapesInputRequestTypeDef",
-    "DescribeSnapshotScheduleOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "UpdateSnapshotScheduleInputRequestTypeDef",
+    "ActivateGatewayOutputTypeDef",
+    "AddCacheOutputTypeDef",
+    "AddTagsToResourceOutputTypeDef",
+    "AddUploadBufferOutputTypeDef",
+    "AddWorkingStorageOutputTypeDef",
+    "AssignTapePoolOutputTypeDef",
+    "AssociateFileSystemOutputTypeDef",
+    "AttachVolumeOutputTypeDef",
+    "CancelArchivalOutputTypeDef",
+    "CancelRetrievalOutputTypeDef",
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    "CreateNFSFileShareOutputTypeDef",
+    "CreateSMBFileShareOutputTypeDef",
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    "CreateSnapshotOutputTypeDef",
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    "CreateTapePoolOutputTypeDef",
+    "CreateTapeWithBarcodeOutputTypeDef",
+    "CreateTapesOutputTypeDef",
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    "DeleteChapCredentialsOutputTypeDef",
+    "DeleteFileShareOutputTypeDef",
+    "DeleteGatewayOutputTypeDef",
+    "DeleteSnapshotScheduleOutputTypeDef",
+    "DeleteTapeArchiveOutputTypeDef",
+    "DeleteTapeOutputTypeDef",
+    "DeleteTapePoolOutputTypeDef",
+    "DeleteVolumeOutputTypeDef",
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    "DescribeCacheOutputTypeDef",
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    "DescribeUploadBufferOutputTypeDef",
+    "DescribeWorkingStorageOutputTypeDef",
+    "DetachVolumeOutputTypeDef",
+    "DisableGatewayOutputTypeDef",
+    "DisassociateFileSystemOutputTypeDef",
+    "JoinDomainOutputTypeDef",
+    "ListVolumeInitiatorsOutputTypeDef",
+    "NotifyWhenUploadedOutputTypeDef",
+    "RefreshCacheOutputTypeDef",
+    "RemoveTagsFromResourceOutputTypeDef",
+    "ResetCacheOutputTypeDef",
+    "RetrieveTapeArchiveOutputTypeDef",
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SetLocalConsolePasswordOutputTypeDef",
+    "SetSMBGuestPasswordOutputTypeDef",
+    "ShutdownGatewayOutputTypeDef",
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    "StartGatewayOutputTypeDef",
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    "UpdateChapCredentialsOutputTypeDef",
+    "UpdateFileSystemAssociationOutputTypeDef",
+    "UpdateGatewayInformationOutputTypeDef",
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    "UpdateNFSFileShareOutputTypeDef",
+    "UpdateSMBFileShareOutputTypeDef",
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    "UpdateSnapshotScheduleOutputTypeDef",
+    "UpdateVTLDeviceTypeOutputTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
-    "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
-    "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
+    "DescribeSnapshotScheduleOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "SMBFileShareInfoTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    "DescribeTapesInputDescribeTapesPaginateTypeDef",
+    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    "ListTapesInputListTapesPaginateTypeDef",
+    "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "DescribeSMBFileSharesOutputTypeDef",
+    "NFSFileShareInfoTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
-    "DescribeNFSFileSharesOutputTypeDef",
+    "DescribeSMBFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
+    "DescribeNFSFileSharesOutputTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ActivateGatewayOutputTypeDef = TypedDict(
-    "ActivateGatewayOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddCacheOutputTypeDef = TypedDict(
-    "AddCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddTagsToResourceOutputTypeDef = TypedDict(
-    "AddTagsToResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddUploadBufferInputRequestTypeDef = TypedDict(
     "AddUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddUploadBufferOutputTypeDef = TypedDict(
-    "AddUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddWorkingStorageInputRequestTypeDef = TypedDict(
     "AddWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddWorkingStorageOutputTypeDef = TypedDict(
-    "AddWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssignTapePoolInputRequestTypeDef = TypedDict(
     "_RequiredAssignTapePoolInputRequestTypeDef",
     {
         "TapeARN": str,
         "PoolId": str,
     },
 )
@@ -351,22 +329,14 @@
 
 class AssignTapePoolInputRequestTypeDef(
     _RequiredAssignTapePoolInputRequestTypeDef, _OptionalAssignTapePoolInputRequestTypeDef
 ):
     pass
 
 
-AssignTapePoolOutputTypeDef = TypedDict(
-    "AssignTapePoolOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheAttributesTypeDef = TypedDict(
     "CacheAttributesTypeDef",
     {
         "CacheStaleTimeoutInSeconds": int,
     },
     total=False,
 )
@@ -375,22 +345,14 @@
     "EndpointNetworkConfigurationTypeDef",
     {
         "IpAddresses": Sequence[str],
     },
     total=False,
 )
 
-AssociateFileSystemOutputTypeDef = TypedDict(
-    "AssociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAttachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredAttachVolumeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "VolumeARN": str,
         "NetworkInterfaceId": str,
     },
@@ -407,22 +369,37 @@
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
 
-AttachVolumeOutputTypeDef = TypedDict(
-    "AttachVolumeOutputTypeDef",
+_RequiredAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
+    "_RequiredAutomaticTapeCreationRuleOutputTypeDef",
     {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TapeBarcodePrefix": str,
+        "PoolId": str,
+        "TapeSizeInBytes": int,
+        "MinimumNumTapes": int,
     },
 )
+_OptionalAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
+    "_OptionalAutomaticTapeCreationRuleOutputTypeDef",
+    {
+        "Worm": bool,
+    },
+    total=False,
+)
+
+
+class AutomaticTapeCreationRuleOutputTypeDef(
+    _RequiredAutomaticTapeCreationRuleOutputTypeDef, _OptionalAutomaticTapeCreationRuleOutputTypeDef
+):
+    pass
+
 
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
@@ -440,22 +417,49 @@
 
 class AutomaticTapeCreationRuleTypeDef(
     _RequiredAutomaticTapeCreationRuleTypeDef, _OptionalAutomaticTapeCreationRuleTypeDef
 ):
     pass
 
 
+_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "StartHourOfDay": int,
+        "StartMinuteOfHour": int,
+        "EndHourOfDay": int,
+        "EndMinuteOfHour": int,
+        "DaysOfWeek": List[int],
+    },
+)
+_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+    },
+    total=False,
+)
+
+
+class BandwidthRateLimitIntervalOutputTypeDef(
+    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
+    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
+):
+    pass
+
+
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
+        "DaysOfWeek": Sequence[int],
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
         "AverageDownloadRateLimitInBitsPerSec": int,
@@ -466,14 +470,22 @@
 
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
 
+CacheAttributesOutputTypeDef = TypedDict(
+    "CacheAttributesOutputTypeDef",
+    {
+        "CacheStaleTimeoutInSeconds": int,
+    },
+    total=False,
+)
+
 VolumeiSCSIAttributesTypeDef = TypedDict(
     "VolumeiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "LunNumber": int,
@@ -486,186 +498,67 @@
     "CancelArchivalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelArchivalOutputTypeDef = TypedDict(
-    "CancelArchivalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelRetrievalInputRequestTypeDef = TypedDict(
     "CancelRetrievalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelRetrievalOutputTypeDef = TypedDict(
-    "CancelRetrievalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChapInfoTypeDef = TypedDict(
     "ChapInfoTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
         "SecretToAuthenticateTarget": str,
     },
     total=False,
 )
 
-CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NFSFileShareDefaultsTypeDef = TypedDict(
     "NFSFileShareDefaultsTypeDef",
     {
         "FileMode": str,
         "DirectoryMode": str,
         "GroupId": int,
         "OwnerId": int,
     },
     total=False,
 )
 
-CreateNFSFileShareOutputTypeDef = TypedDict(
-    "CreateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSMBFileShareOutputTypeDef = TypedDict(
-    "CreateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeARN": str,
-        "VolumeRecoveryPointTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotOutputTypeDef = TypedDict(
-    "CreateSnapshotOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "VolumeSizeInBytes": int,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapePoolOutputTypeDef = TypedDict(
-    "CreateTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapeWithBarcodeOutputTypeDef = TypedDict(
-    "CreateTapeWithBarcodeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapesOutputTypeDef = TypedDict(
-    "CreateTapesOutputTypeDef",
-    {
-        "TapeARNs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DeleteBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
         "BandwidthType": str,
     },
 )
 
-DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChapCredentialsInputRequestTypeDef = TypedDict(
     "DeleteChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "InitiatorName": str,
     },
 )
 
-DeleteChapCredentialsOutputTypeDef = TypedDict(
-    "DeleteChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteFileShareInputRequestTypeDef = TypedDict(
     "_RequiredDeleteFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalDeleteFileShareInputRequestTypeDef = TypedDict(
@@ -679,52 +572,28 @@
 
 class DeleteFileShareInputRequestTypeDef(
     _RequiredDeleteFileShareInputRequestTypeDef, _OptionalDeleteFileShareInputRequestTypeDef
 ):
     pass
 
 
-DeleteFileShareOutputTypeDef = TypedDict(
-    "DeleteFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DeleteSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteSnapshotScheduleOutputTypeDef = TypedDict(
-    "DeleteSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeArchiveInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
     },
 )
 _OptionalDeleteTapeArchiveInputRequestTypeDef = TypedDict(
@@ -738,22 +607,14 @@
 
 class DeleteTapeArchiveInputRequestTypeDef(
     _RequiredDeleteTapeArchiveInputRequestTypeDef, _OptionalDeleteTapeArchiveInputRequestTypeDef
 ):
     pass
 
 
-DeleteTapeArchiveOutputTypeDef = TypedDict(
-    "DeleteTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
@@ -768,114 +629,56 @@
 
 class DeleteTapeInputRequestTypeDef(
     _RequiredDeleteTapeInputRequestTypeDef, _OptionalDeleteTapeInputRequestTypeDef
 ):
     pass
 
 
-DeleteTapeOutputTypeDef = TypedDict(
-    "DeleteTapeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTapePoolInputRequestTypeDef = TypedDict(
     "DeleteTapePoolInputRequestTypeDef",
     {
         "PoolARN": str,
     },
 )
 
-DeleteTapePoolOutputTypeDef = TypedDict(
-    "DeleteTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVolumeInputRequestTypeDef = TypedDict(
     "DeleteVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteVolumeOutputTypeDef = TypedDict(
-    "DeleteVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "Status": AvailabilityMonitorTestStatusType,
-        "StartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
 DescribeCacheInputRequestTypeDef = TypedDict(
     "DescribeCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeCacheOutputTypeDef = TypedDict(
-    "DescribeCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "CacheAllocatedInBytes": int,
-        "CacheUsedPercentage": float,
-        "CacheDirtyPercentage": float,
-        "CacheHitPercentage": float,
-        "CacheMissPercentage": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCachediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
@@ -906,31 +709,26 @@
         "Ipv4Address": str,
         "MacAddress": str,
         "Ipv6Address": str,
     },
     total=False,
 )
 
-DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeInputRequestTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "GatewayARN": str,
+        "Key": str,
+        "Value": str,
     },
 )
 
-DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeOutputTypeDef",
+DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-        "DayOfWeek": int,
-        "DayOfMonth": int,
-        "Timezone": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNFSFileSharesInputRequestTypeDef = TypedDict(
     "DescribeNFSFileSharesInputRequestTypeDef",
     {
         "FileShareARNList": Sequence[str],
@@ -947,16 +745,16 @@
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
+SMBLocalGroupsOutputTypeDef = TypedDict(
+    "SMBLocalGroupsOutputTypeDef",
     {
         "GatewayAdmins": List[str],
     },
     total=False,
 )
 
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
@@ -969,19 +767,20 @@
 DescribeStorediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
-DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeTapeArchivesInputRequestTypeDef = TypedDict(
     "DescribeTapeArchivesInputRequestTypeDef",
     {
@@ -1008,36 +807,14 @@
         "Worm": bool,
         "RetentionStartDate": datetime,
         "PoolEntryDate": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
-    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
@@ -1064,37 +841,14 @@
         "TapeRecoveryPointTime": datetime,
         "TapeSizeInBytes": int,
         "TapeStatus": str,
     },
     total=False,
 )
 
-_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeTapesInputDescribeTapesPaginateTypeDef(
-    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
-    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTapesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapesInputRequestTypeDef = TypedDict(
@@ -1137,48 +891,14 @@
 DescribeUploadBufferInputRequestTypeDef = TypedDict(
     "DescribeUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeUploadBufferOutputTypeDef = TypedDict(
-    "DescribeUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "UploadBufferUsedInBytes": int,
-        "UploadBufferAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "VTLDeviceARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
-    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeVTLDevicesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVTLDevicesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeVTLDevicesInputRequestTypeDef = TypedDict(
@@ -1201,25 +921,14 @@
 DescribeWorkingStorageInputRequestTypeDef = TypedDict(
     "DescribeWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeWorkingStorageOutputTypeDef = TypedDict(
-    "DescribeWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "WorkingStorageUsedInBytes": int,
-        "WorkingStorageAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredDetachVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 _OptionalDetachVolumeInputRequestTypeDef = TypedDict(
@@ -1233,22 +942,14 @@
 
 class DetachVolumeInputRequestTypeDef(
     _RequiredDetachVolumeInputRequestTypeDef, _OptionalDetachVolumeInputRequestTypeDef
 ):
     pass
 
 
-DetachVolumeOutputTypeDef = TypedDict(
-    "DetachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceiSCSIAttributesTypeDef = TypedDict(
     "DeviceiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "ChapEnabled": bool,
@@ -1259,22 +960,14 @@
 DisableGatewayInputRequestTypeDef = TypedDict(
     "DisableGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DisableGatewayOutputTypeDef = TypedDict(
-    "DisableGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateFileSystemInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateFileSystemInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalDisassociateFileSystemInputRequestTypeDef = TypedDict(
@@ -1289,22 +982,14 @@
 class DisassociateFileSystemInputRequestTypeDef(
     _RequiredDisassociateFileSystemInputRequestTypeDef,
     _OptionalDisassociateFileSystemInputRequestTypeDef,
 ):
     pass
 
 
-DisassociateFileSystemOutputTypeDef = TypedDict(
-    "DisassociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "DiskId": str,
         "DiskPath": str,
         "DiskNode": str,
         "DiskStatus": str,
@@ -1312,14 +997,22 @@
         "DiskAllocationType": str,
         "DiskAllocationResource": str,
         "DiskAttributeList": List[str],
     },
     total=False,
 )
 
+EndpointNetworkConfigurationOutputTypeDef = TypedDict(
+    "EndpointNetworkConfigurationOutputTypeDef",
+    {
+        "IpAddresses": List[str],
+    },
+    total=False,
+)
+
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": FileShareTypeType,
         "FileShareARN": str,
         "FileShareId": str,
         "FileShareStatus": str,
@@ -1385,77 +1078,42 @@
 
 class JoinDomainInputRequestTypeDef(
     _RequiredJoinDomainInputRequestTypeDef, _OptionalJoinDomainInputRequestTypeDef
 ):
     pass
 
 
-JoinDomainOutputTypeDef = TypedDict(
-    "JoinDomainOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAutomaticTapeCreationPoliciesInputRequestTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
     total=False,
 )
 
-ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSharesInputRequestTypeDef = TypedDict(
     "ListFileSharesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSystemAssociationsInputRequestTypeDef = TypedDict(
     "ListFileSystemAssociationsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
@@ -1464,36 +1122,14 @@
 ListLocalDisksInputRequestTypeDef = TypedDict(
     "ListLocalDisksInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1508,23 +1144,14 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    {
-        "PoolARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapePoolsInputRequestTypeDef = TypedDict(
     "ListTapePoolsInputRequestTypeDef",
     {
         "PoolARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1540,23 +1167,14 @@
         "RetentionLockType": RetentionLockTypeType,
         "RetentionLockTimeInDays": int,
         "PoolStatus": PoolStatusType,
     },
     total=False,
 )
 
-ListTapesInputListTapesPaginateTypeDef = TypedDict(
-    "ListTapesInputListTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapesInputRequestTypeDef = TypedDict(
     "ListTapesInputRequestTypeDef",
     {
         "TapeARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1581,22 +1199,14 @@
 ListVolumeInitiatorsInputRequestTypeDef = TypedDict(
     "ListVolumeInitiatorsInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-ListVolumeInitiatorsOutputTypeDef = TypedDict(
-    "ListVolumeInitiatorsOutputTypeDef",
-    {
-        "Initiators": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVolumeRecoveryPointsInputRequestTypeDef = TypedDict(
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1607,23 +1217,14 @@
         "VolumeSizeInBytes": int,
         "VolumeUsageInBytes": int,
         "VolumeRecoveryPointTime": str,
     },
     total=False,
 )
 
-ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
-    "ListVolumesInputListVolumesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVolumesInputRequestTypeDef = TypedDict(
     "ListVolumesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "Limit": int,
     },
@@ -1640,40 +1241,32 @@
         "VolumeType": str,
         "VolumeSizeInBytes": int,
         "VolumeAttachmentStatus": str,
     },
     total=False,
 )
 
-NotifyWhenUploadedInputRequestTypeDef = TypedDict(
-    "NotifyWhenUploadedInputRequestTypeDef",
+NFSFileShareDefaultsOutputTypeDef = TypedDict(
+    "NFSFileShareDefaultsOutputTypeDef",
     {
-        "FileShareARN": str,
+        "FileMode": str,
+        "DirectoryMode": str,
+        "GroupId": int,
+        "OwnerId": int,
     },
+    total=False,
 )
 
-NotifyWhenUploadedOutputTypeDef = TypedDict(
-    "NotifyWhenUploadedOutputTypeDef",
+NotifyWhenUploadedInputRequestTypeDef = TypedDict(
+    "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
 _RequiredRefreshCacheInputRequestTypeDef = TypedDict(
     "_RequiredRefreshCacheInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalRefreshCacheInputRequestTypeDef = TypedDict(
@@ -1688,182 +1281,90 @@
 
 class RefreshCacheInputRequestTypeDef(
     _RequiredRefreshCacheInputRequestTypeDef, _OptionalRefreshCacheInputRequestTypeDef
 ):
     pass
 
 
-RefreshCacheOutputTypeDef = TypedDict(
-    "RefreshCacheOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceInputRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-RemoveTagsFromResourceOutputTypeDef = TypedDict(
-    "RemoveTagsFromResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResetCacheInputRequestTypeDef = TypedDict(
     "ResetCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ResetCacheOutputTypeDef = TypedDict(
-    "ResetCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
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
 RetrieveTapeArchiveInputRequestTypeDef = TypedDict(
     "RetrieveTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeArchiveOutputTypeDef = TypedDict(
-    "RetrieveTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "GatewayAdmins": Sequence[str],
     },
+    total=False,
 )
 
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
 
-SetLocalConsolePasswordOutputTypeDef = TypedDict(
-    "SetLocalConsolePasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSMBGuestPasswordInputRequestTypeDef = TypedDict(
     "SetSMBGuestPasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Password": str,
     },
 )
 
-SetSMBGuestPasswordOutputTypeDef = TypedDict(
-    "SetSMBGuestPasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ShutdownGatewayInputRequestTypeDef = TypedDict(
     "ShutdownGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ShutdownGatewayOutputTypeDef = TypedDict(
-    "ShutdownGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartGatewayInputRequestTypeDef = TypedDict(
     "StartGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartGatewayOutputTypeDef = TypedDict(
-    "StartGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
@@ -1879,30 +1380,14 @@
 class UpdateBandwidthRateLimitInputRequestTypeDef(
     _RequiredUpdateBandwidthRateLimitInputRequestTypeDef,
     _OptionalUpdateBandwidthRateLimitInputRequestTypeDef,
 ):
     pass
 
 
-UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChapCredentialsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
     },
@@ -1919,31 +1404,14 @@
 class UpdateChapCredentialsInputRequestTypeDef(
     _RequiredUpdateChapCredentialsInputRequestTypeDef,
     _OptionalUpdateChapCredentialsInputRequestTypeDef,
 ):
     pass
 
 
-UpdateChapCredentialsOutputTypeDef = TypedDict(
-    "UpdateChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFileSystemAssociationOutputTypeDef = TypedDict(
-    "UpdateFileSystemAssociationOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
@@ -1961,38 +1429,21 @@
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
 
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "GatewayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -2010,102 +1461,38 @@
 class UpdateMaintenanceStartTimeInputRequestTypeDef(
     _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef,
     _OptionalUpdateMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
 
-UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateNFSFileShareOutputTypeDef = TypedDict(
-    "UpdateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBFileShareOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBFileShareVisibilityInputRequestTypeDef = TypedDict(
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
     {
         "GatewayARN": str,
         "FileSharesVisible": bool,
     },
 )
 
-UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBSecurityStrategyInputRequestTypeDef = TypedDict(
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
     },
 )
 
-UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSnapshotScheduleOutputTypeDef = TypedDict(
-    "UpdateSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateVTLDeviceTypeInputRequestTypeDef = TypedDict(
     "UpdateVTLDeviceTypeInputRequestTypeDef",
     {
         "VTLDeviceARN": str,
         "DeviceType": str,
     },
 )
 
-UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
-    "UpdateVTLDeviceTypeOutputTypeDef",
-    {
-        "VTLDeviceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredActivateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayName": str,
         "GatewayTimezone": str,
         "GatewayRegion": str,
@@ -2318,37 +1705,14 @@
 
 class CreateTapesInputRequestTypeDef(
     _RequiredCreateTapesInputRequestTypeDef, _OptionalCreateTapesInputRequestTypeDef
 ):
     pass
 
 
-DescribeSnapshotScheduleOutputTypeDef = TypedDict(
-    "DescribeSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
-        "Description": str,
-        "Timezone": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "Marker": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
         "StartAt": int,
         "RecurrenceInHours": int,
     },
@@ -2366,14 +1730,576 @@
 class UpdateSnapshotScheduleInputRequestTypeDef(
     _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
     _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
 ):
     pass
 
 
+ActivateGatewayOutputTypeDef = TypedDict(
+    "ActivateGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddCacheOutputTypeDef = TypedDict(
+    "AddCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddTagsToResourceOutputTypeDef = TypedDict(
+    "AddTagsToResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddUploadBufferOutputTypeDef = TypedDict(
+    "AddUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddWorkingStorageOutputTypeDef = TypedDict(
+    "AddWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssignTapePoolOutputTypeDef = TypedDict(
+    "AssignTapePoolOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateFileSystemOutputTypeDef = TypedDict(
+    "AssociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachVolumeOutputTypeDef = TypedDict(
+    "AttachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelArchivalOutputTypeDef = TypedDict(
+    "CancelArchivalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelRetrievalOutputTypeDef = TypedDict(
+    "CancelRetrievalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNFSFileShareOutputTypeDef = TypedDict(
+    "CreateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSMBFileShareOutputTypeDef = TypedDict(
+    "CreateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeARN": str,
+        "VolumeRecoveryPointTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotOutputTypeDef = TypedDict(
+    "CreateSnapshotOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "VolumeSizeInBytes": int,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapePoolOutputTypeDef = TypedDict(
+    "CreateTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapeWithBarcodeOutputTypeDef = TypedDict(
+    "CreateTapeWithBarcodeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapesOutputTypeDef = TypedDict(
+    "CreateTapesOutputTypeDef",
+    {
+        "TapeARNs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteChapCredentialsOutputTypeDef = TypedDict(
+    "DeleteChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileShareOutputTypeDef = TypedDict(
+    "DeleteFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotScheduleOutputTypeDef = TypedDict(
+    "DeleteSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeArchiveOutputTypeDef = TypedDict(
+    "DeleteTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeOutputTypeDef = TypedDict(
+    "DeleteTapeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapePoolOutputTypeDef = TypedDict(
+    "DeleteTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVolumeOutputTypeDef = TypedDict(
+    "DeleteVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "Status": AvailabilityMonitorTestStatusType,
+        "StartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCacheOutputTypeDef = TypedDict(
+    "DescribeCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "CacheAllocatedInBytes": int,
+        "CacheUsedPercentage": float,
+        "CacheDirtyPercentage": float,
+        "CacheHitPercentage": float,
+        "CacheMissPercentage": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+        "DayOfWeek": int,
+        "DayOfMonth": int,
+        "Timezone": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUploadBufferOutputTypeDef = TypedDict(
+    "DescribeUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "UploadBufferUsedInBytes": int,
+        "UploadBufferAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkingStorageOutputTypeDef = TypedDict(
+    "DescribeWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "WorkingStorageUsedInBytes": int,
+        "WorkingStorageAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachVolumeOutputTypeDef = TypedDict(
+    "DetachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableGatewayOutputTypeDef = TypedDict(
+    "DisableGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateFileSystemOutputTypeDef = TypedDict(
+    "DisassociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JoinDomainOutputTypeDef = TypedDict(
+    "JoinDomainOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVolumeInitiatorsOutputTypeDef = TypedDict(
+    "ListVolumeInitiatorsOutputTypeDef",
+    {
+        "Initiators": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+NotifyWhenUploadedOutputTypeDef = TypedDict(
+    "NotifyWhenUploadedOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RefreshCacheOutputTypeDef = TypedDict(
+    "RefreshCacheOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveTagsFromResourceOutputTypeDef = TypedDict(
+    "RemoveTagsFromResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetCacheOutputTypeDef = TypedDict(
+    "ResetCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeArchiveOutputTypeDef = TypedDict(
+    "RetrieveTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetLocalConsolePasswordOutputTypeDef = TypedDict(
+    "SetLocalConsolePasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetSMBGuestPasswordOutputTypeDef = TypedDict(
+    "SetSMBGuestPasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShutdownGatewayOutputTypeDef = TypedDict(
+    "ShutdownGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGatewayOutputTypeDef = TypedDict(
+    "StartGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChapCredentialsOutputTypeDef = TypedDict(
+    "UpdateChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFileSystemAssociationOutputTypeDef = TypedDict(
+    "UpdateFileSystemAssociationOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "GatewayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateNFSFileShareOutputTypeDef = TypedDict(
+    "UpdateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSnapshotScheduleOutputTypeDef = TypedDict(
+    "UpdateSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
+    "UpdateVTLDeviceTypeOutputTypeDef",
+    {
+        "VTLDeviceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateSMBFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateSMBFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
         "GatewayARN": str,
         "Role": str,
         "LocationARN": str,
@@ -2411,50 +2337,14 @@
 
 class CreateSMBFileShareInputRequestTypeDef(
     _RequiredCreateSMBFileShareInputRequestTypeDef, _OptionalCreateSMBFileShareInputRequestTypeDef
 ):
     pass
 
 
-SMBFileShareInfoTypeDef = TypedDict(
-    "SMBFileShareInfoTypeDef",
-    {
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
-        "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "SMBACLEnabled": bool,
-        "AccessBasedEnumeration": bool,
-        "AdminUserList": List[str],
-        "ValidUserList": List[str],
-        "InvalidUserList": List[str],
-        "AuditDestinationARN": str,
-        "Authentication": str,
-        "CaseSensitivity": CaseSensitivityType,
-        "Tags": List[TagTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "OplocksEnabled": bool,
-    },
-    total=False,
-)
-
 _RequiredUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemAssociationInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
@@ -2541,15 +2431,15 @@
 ):
     pass
 
 
 AutomaticTapeCreationPolicyInfoTypeDef = TypedDict(
     "AutomaticTapeCreationPolicyInfoTypeDef",
     {
-        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleTypeDef],
+        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleOutputTypeDef],
         "GatewayARN": str,
     },
     total=False,
 )
 
 UpdateAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -2559,16 +2449,16 @@
     },
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
@@ -2618,15 +2508,15 @@
     total=False,
 )
 
 DescribeChapCredentialsOutputTypeDef = TypedDict(
     "DescribeChapCredentialsOutputTypeDef",
     {
         "ChapCredentials": List[ChapInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateNFSFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
@@ -2662,45 +2552,14 @@
 
 class CreateNFSFileShareInputRequestTypeDef(
     _RequiredCreateNFSFileShareInputRequestTypeDef, _OptionalCreateNFSFileShareInputRequestTypeDef
 ):
     pass
 
 
-NFSFileShareInfoTypeDef = TypedDict(
-    "NFSFileShareInfoTypeDef",
-    {
-        "NFSFileShareDefaults": NFSFileShareDefaultsTypeDef,
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
-        "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ClientList": List[str],
-        "Squash": str,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "Tags": List[TagTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "AuditDestinationARN": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNFSFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalUpdateNFSFileShareInputRequestTypeDef = TypedDict(
@@ -2741,75 +2600,278 @@
         "GatewayState": str,
         "GatewayNetworkInterfaces": List[NetworkInterfaceTypeDef],
         "GatewayType": str,
         "NextUpdateAvailabilityDate": str,
         "LastSoftwareUpdate": str,
         "Ec2InstanceId": str,
         "Ec2InstanceRegion": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "VPCEndpoint": str,
         "CloudWatchLogGroupARN": str,
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeSnapshotScheduleOutputTypeDef = TypedDict(
+    "DescribeSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "StartAt": int,
+        "RecurrenceInHours": int,
+        "Description": str,
+        "Timezone": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Marker": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SMBFileShareInfoTypeDef = TypedDict(
+    "SMBFileShareInfoTypeDef",
+    {
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "SMBACLEnabled": bool,
+        "AccessBasedEnumeration": bool,
+        "AdminUserList": List[str],
+        "ValidUserList": List[str],
+        "InvalidUserList": List[str],
+        "AuditDestinationARN": str,
+        "Authentication": str,
+        "CaseSensitivity": CaseSensitivityType,
+        "Tags": List[TagOutputTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "OplocksEnabled": bool,
+    },
+    total=False,
+)
+
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     {
         "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
+_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
+    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTapesInputDescribeTapesPaginateTypeDef(
+    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
+    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "VTLDeviceARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
+    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+):
+    pass
+
+
+ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    {
+        "PoolARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTapesInputListTapesPaginateTypeDef = TypedDict(
+    "ListTapesInputListTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
+    "ListVolumesInputListVolumesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 DescribeTapeArchivesOutputTypeDef = TypedDict(
     "DescribeTapeArchivesOutputTypeDef",
     {
         "TapeArchives": List[TapeArchiveTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapeRecoveryPointsOutputTypeDef = TypedDict(
     "DescribeTapeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "TapeRecoveryPointInfos": List[TapeRecoveryPointInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapesOutputTypeDef = TypedDict(
     "DescribeTapesOutputTypeDef",
     {
         "Tapes": List[TapeTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VTLDeviceTypeDef = TypedDict(
     "VTLDeviceTypeDef",
     {
         "VTLDeviceARN": str,
@@ -2822,150 +2884,189 @@
 )
 
 ListLocalDisksOutputTypeDef = TypedDict(
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FileSystemAssociationInfoTypeDef = TypedDict(
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
-        "Tags": List[TagTypeDef],
-        "CacheAttributes": CacheAttributesTypeDef,
-        "EndpointNetworkConfiguration": EndpointNetworkConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileSystemAssociationSummaryList": List[FileSystemAssociationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapePoolsOutputTypeDef = TypedDict(
     "ListTapePoolsOutputTypeDef",
     {
         "PoolInfos": List[PoolInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapesOutputTypeDef = TypedDict(
     "ListTapesOutputTypeDef",
     {
         "TapeInfos": List[TapeInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumeRecoveryPointsOutputTypeDef = TypedDict(
     "ListVolumeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "VolumeRecoveryPointInfos": List[VolumeRecoveryPointInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumesOutputTypeDef = TypedDict(
     "ListVolumesOutputTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSMBFileSharesOutputTypeDef = TypedDict(
-    "DescribeSMBFileSharesOutputTypeDef",
+NFSFileShareInfoTypeDef = TypedDict(
+    "NFSFileShareInfoTypeDef",
     {
-        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NFSFileShareDefaults": NFSFileShareDefaultsOutputTypeDef,
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ClientList": List[str],
+        "Squash": str,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "Tags": List[TagOutputTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "AuditDestinationARN": str,
+    },
+    total=False,
+)
+
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStorediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeNFSFileSharesOutputTypeDef = TypedDict(
-    "DescribeNFSFileSharesOutputTypeDef",
+DescribeSMBFileSharesOutputTypeDef = TypedDict(
+    "DescribeSMBFileSharesOutputTypeDef",
     {
-        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
         "GatewayARN": str,
         "VTLDevices": List[VTLDeviceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNFSFileSharesOutputTypeDef = TypedDict(
+    "DescribeNFSFileSharesOutputTypeDef",
+    {
+        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway/type_defs.pyi` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,310 +32,288 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "ActivateGatewayOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCacheInputRequestTypeDef",
-    "AddCacheOutputTypeDef",
-    "AddTagsToResourceOutputTypeDef",
     "AddUploadBufferInputRequestTypeDef",
-    "AddUploadBufferOutputTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
-    "AddWorkingStorageOutputTypeDef",
     "AssignTapePoolInputRequestTypeDef",
-    "AssignTapePoolOutputTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
-    "AssociateFileSystemOutputTypeDef",
     "AttachVolumeInputRequestTypeDef",
-    "AttachVolumeOutputTypeDef",
+    "AutomaticTapeCreationRuleOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
+    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
+    "CacheAttributesOutputTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
-    "CancelArchivalOutputTypeDef",
     "CancelRetrievalInputRequestTypeDef",
-    "CancelRetrievalOutputTypeDef",
     "ChapInfoTypeDef",
-    "CreateCachediSCSIVolumeOutputTypeDef",
     "NFSFileShareDefaultsTypeDef",
-    "CreateNFSFileShareOutputTypeDef",
-    "CreateSMBFileShareOutputTypeDef",
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    "CreateSnapshotOutputTypeDef",
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    "CreateTapePoolOutputTypeDef",
-    "CreateTapeWithBarcodeOutputTypeDef",
-    "CreateTapesOutputTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
-    "DeleteBandwidthRateLimitOutputTypeDef",
     "DeleteChapCredentialsInputRequestTypeDef",
-    "DeleteChapCredentialsOutputTypeDef",
     "DeleteFileShareInputRequestTypeDef",
-    "DeleteFileShareOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
-    "DeleteGatewayOutputTypeDef",
     "DeleteSnapshotScheduleInputRequestTypeDef",
-    "DeleteSnapshotScheduleOutputTypeDef",
     "DeleteTapeArchiveInputRequestTypeDef",
-    "DeleteTapeArchiveOutputTypeDef",
     "DeleteTapeInputRequestTypeDef",
-    "DeleteTapeOutputTypeDef",
     "DeleteTapePoolInputRequestTypeDef",
-    "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeInputRequestTypeDef",
-    "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitInputRequestTypeDef",
-    "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
-    "DescribeCacheOutputTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
+    "TagOutputTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
-    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
+    "SMBLocalGroupsOutputTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
-    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
-    "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeTapesInputRequestTypeDef",
     "TapeTypeDef",
     "DescribeUploadBufferInputRequestTypeDef",
-    "DescribeUploadBufferOutputTypeDef",
-    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
-    "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeInputRequestTypeDef",
-    "DetachVolumeOutputTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
-    "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
-    "DisassociateFileSystemOutputTypeDef",
     "DiskTypeDef",
+    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
-    "JoinDomainOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSharesInputRequestTypeDef",
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListFileSystemAssociationsInputRequestTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
     "ListLocalDisksInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
     "ListTapePoolsInputRequestTypeDef",
     "PoolInfoTypeDef",
-    "ListTapesInputListTapesPaginateTypeDef",
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
-    "ListVolumeInitiatorsOutputTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
-    "ListVolumesInputListVolumesPaginateTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
+    "NFSFileShareDefaultsOutputTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
-    "NotifyWhenUploadedOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshCacheInputRequestTypeDef",
-    "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
-    "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheInputRequestTypeDef",
-    "ResetCacheOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
-    "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
-    "SetLocalConsolePasswordOutputTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
-    "SetSMBGuestPasswordOutputTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
-    "ShutdownGatewayOutputTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
-    "StartAvailabilityMonitorTestOutputTypeDef",
     "StartGatewayInputRequestTypeDef",
-    "StartGatewayOutputTypeDef",
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
-    "UpdateChapCredentialsOutputTypeDef",
-    "UpdateFileSystemAssociationOutputTypeDef",
     "UpdateGatewayInformationInputRequestTypeDef",
-    "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
-    "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateMaintenanceStartTimeInputRequestTypeDef",
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    "UpdateNFSFileShareOutputTypeDef",
-    "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeInputRequestTypeDef",
-    "UpdateVTLDeviceTypeOutputTypeDef",
     "ActivateGatewayInputRequestTypeDef",
     "AddTagsToResourceInputRequestTypeDef",
     "CreateCachediSCSIVolumeInputRequestTypeDef",
     "CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "CreateStorediSCSIVolumeInputRequestTypeDef",
     "CreateTapePoolInputRequestTypeDef",
     "CreateTapeWithBarcodeInputRequestTypeDef",
     "CreateTapesInputRequestTypeDef",
-    "DescribeSnapshotScheduleOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "UpdateSnapshotScheduleInputRequestTypeDef",
+    "ActivateGatewayOutputTypeDef",
+    "AddCacheOutputTypeDef",
+    "AddTagsToResourceOutputTypeDef",
+    "AddUploadBufferOutputTypeDef",
+    "AddWorkingStorageOutputTypeDef",
+    "AssignTapePoolOutputTypeDef",
+    "AssociateFileSystemOutputTypeDef",
+    "AttachVolumeOutputTypeDef",
+    "CancelArchivalOutputTypeDef",
+    "CancelRetrievalOutputTypeDef",
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    "CreateNFSFileShareOutputTypeDef",
+    "CreateSMBFileShareOutputTypeDef",
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    "CreateSnapshotOutputTypeDef",
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    "CreateTapePoolOutputTypeDef",
+    "CreateTapeWithBarcodeOutputTypeDef",
+    "CreateTapesOutputTypeDef",
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    "DeleteChapCredentialsOutputTypeDef",
+    "DeleteFileShareOutputTypeDef",
+    "DeleteGatewayOutputTypeDef",
+    "DeleteSnapshotScheduleOutputTypeDef",
+    "DeleteTapeArchiveOutputTypeDef",
+    "DeleteTapeOutputTypeDef",
+    "DeleteTapePoolOutputTypeDef",
+    "DeleteVolumeOutputTypeDef",
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    "DescribeCacheOutputTypeDef",
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    "DescribeUploadBufferOutputTypeDef",
+    "DescribeWorkingStorageOutputTypeDef",
+    "DetachVolumeOutputTypeDef",
+    "DisableGatewayOutputTypeDef",
+    "DisassociateFileSystemOutputTypeDef",
+    "JoinDomainOutputTypeDef",
+    "ListVolumeInitiatorsOutputTypeDef",
+    "NotifyWhenUploadedOutputTypeDef",
+    "RefreshCacheOutputTypeDef",
+    "RemoveTagsFromResourceOutputTypeDef",
+    "ResetCacheOutputTypeDef",
+    "RetrieveTapeArchiveOutputTypeDef",
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SetLocalConsolePasswordOutputTypeDef",
+    "SetSMBGuestPasswordOutputTypeDef",
+    "ShutdownGatewayOutputTypeDef",
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    "StartGatewayOutputTypeDef",
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    "UpdateChapCredentialsOutputTypeDef",
+    "UpdateFileSystemAssociationOutputTypeDef",
+    "UpdateGatewayInformationOutputTypeDef",
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    "UpdateNFSFileShareOutputTypeDef",
+    "UpdateSMBFileShareOutputTypeDef",
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    "UpdateSnapshotScheduleOutputTypeDef",
+    "UpdateVTLDeviceTypeOutputTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
-    "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
-    "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
+    "DescribeSnapshotScheduleOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "SMBFileShareInfoTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    "DescribeTapesInputDescribeTapesPaginateTypeDef",
+    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    "ListTapesInputListTapesPaginateTypeDef",
+    "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "DescribeSMBFileSharesOutputTypeDef",
+    "NFSFileShareInfoTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
-    "DescribeNFSFileSharesOutputTypeDef",
+    "DescribeSMBFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
+    "DescribeNFSFileSharesOutputTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ActivateGatewayOutputTypeDef = TypedDict(
-    "ActivateGatewayOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddCacheOutputTypeDef = TypedDict(
-    "AddCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddTagsToResourceOutputTypeDef = TypedDict(
-    "AddTagsToResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddUploadBufferInputRequestTypeDef = TypedDict(
     "AddUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddUploadBufferOutputTypeDef = TypedDict(
-    "AddUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddWorkingStorageInputRequestTypeDef = TypedDict(
     "AddWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddWorkingStorageOutputTypeDef = TypedDict(
-    "AddWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssignTapePoolInputRequestTypeDef = TypedDict(
     "_RequiredAssignTapePoolInputRequestTypeDef",
     {
         "TapeARN": str,
         "PoolId": str,
     },
 )
@@ -348,22 +326,14 @@
 )
 
 class AssignTapePoolInputRequestTypeDef(
     _RequiredAssignTapePoolInputRequestTypeDef, _OptionalAssignTapePoolInputRequestTypeDef
 ):
     pass
 
-AssignTapePoolOutputTypeDef = TypedDict(
-    "AssignTapePoolOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheAttributesTypeDef = TypedDict(
     "CacheAttributesTypeDef",
     {
         "CacheStaleTimeoutInSeconds": int,
     },
     total=False,
 )
@@ -372,22 +342,14 @@
     "EndpointNetworkConfigurationTypeDef",
     {
         "IpAddresses": Sequence[str],
     },
     total=False,
 )
 
-AssociateFileSystemOutputTypeDef = TypedDict(
-    "AssociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAttachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredAttachVolumeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "VolumeARN": str,
         "NetworkInterfaceId": str,
     },
@@ -402,22 +364,35 @@
 )
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
-AttachVolumeOutputTypeDef = TypedDict(
-    "AttachVolumeOutputTypeDef",
+_RequiredAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
+    "_RequiredAutomaticTapeCreationRuleOutputTypeDef",
     {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TapeBarcodePrefix": str,
+        "PoolId": str,
+        "TapeSizeInBytes": int,
+        "MinimumNumTapes": int,
     },
 )
+_OptionalAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
+    "_OptionalAutomaticTapeCreationRuleOutputTypeDef",
+    {
+        "Worm": bool,
+    },
+    total=False,
+)
+
+class AutomaticTapeCreationRuleOutputTypeDef(
+    _RequiredAutomaticTapeCreationRuleOutputTypeDef, _OptionalAutomaticTapeCreationRuleOutputTypeDef
+):
+    pass
 
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
@@ -433,22 +408,47 @@
 )
 
 class AutomaticTapeCreationRuleTypeDef(
     _RequiredAutomaticTapeCreationRuleTypeDef, _OptionalAutomaticTapeCreationRuleTypeDef
 ):
     pass
 
+_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "StartHourOfDay": int,
+        "StartMinuteOfHour": int,
+        "EndHourOfDay": int,
+        "EndMinuteOfHour": int,
+        "DaysOfWeek": List[int],
+    },
+)
+_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+    },
+    total=False,
+)
+
+class BandwidthRateLimitIntervalOutputTypeDef(
+    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
+    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
+):
+    pass
+
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
+        "DaysOfWeek": Sequence[int],
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
         "AverageDownloadRateLimitInBitsPerSec": int,
@@ -457,14 +457,22 @@
 )
 
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
+CacheAttributesOutputTypeDef = TypedDict(
+    "CacheAttributesOutputTypeDef",
+    {
+        "CacheStaleTimeoutInSeconds": int,
+    },
+    total=False,
+)
+
 VolumeiSCSIAttributesTypeDef = TypedDict(
     "VolumeiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "LunNumber": int,
@@ -477,186 +485,67 @@
     "CancelArchivalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelArchivalOutputTypeDef = TypedDict(
-    "CancelArchivalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelRetrievalInputRequestTypeDef = TypedDict(
     "CancelRetrievalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelRetrievalOutputTypeDef = TypedDict(
-    "CancelRetrievalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChapInfoTypeDef = TypedDict(
     "ChapInfoTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
         "SecretToAuthenticateTarget": str,
     },
     total=False,
 )
 
-CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NFSFileShareDefaultsTypeDef = TypedDict(
     "NFSFileShareDefaultsTypeDef",
     {
         "FileMode": str,
         "DirectoryMode": str,
         "GroupId": int,
         "OwnerId": int,
     },
     total=False,
 )
 
-CreateNFSFileShareOutputTypeDef = TypedDict(
-    "CreateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSMBFileShareOutputTypeDef = TypedDict(
-    "CreateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeARN": str,
-        "VolumeRecoveryPointTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotOutputTypeDef = TypedDict(
-    "CreateSnapshotOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "VolumeSizeInBytes": int,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapePoolOutputTypeDef = TypedDict(
-    "CreateTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapeWithBarcodeOutputTypeDef = TypedDict(
-    "CreateTapeWithBarcodeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapesOutputTypeDef = TypedDict(
-    "CreateTapesOutputTypeDef",
-    {
-        "TapeARNs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DeleteBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
         "BandwidthType": str,
     },
 )
 
-DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChapCredentialsInputRequestTypeDef = TypedDict(
     "DeleteChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "InitiatorName": str,
     },
 )
 
-DeleteChapCredentialsOutputTypeDef = TypedDict(
-    "DeleteChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteFileShareInputRequestTypeDef = TypedDict(
     "_RequiredDeleteFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalDeleteFileShareInputRequestTypeDef = TypedDict(
@@ -668,52 +557,28 @@
 )
 
 class DeleteFileShareInputRequestTypeDef(
     _RequiredDeleteFileShareInputRequestTypeDef, _OptionalDeleteFileShareInputRequestTypeDef
 ):
     pass
 
-DeleteFileShareOutputTypeDef = TypedDict(
-    "DeleteFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DeleteSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteSnapshotScheduleOutputTypeDef = TypedDict(
-    "DeleteSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeArchiveInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
     },
 )
 _OptionalDeleteTapeArchiveInputRequestTypeDef = TypedDict(
@@ -725,22 +590,14 @@
 )
 
 class DeleteTapeArchiveInputRequestTypeDef(
     _RequiredDeleteTapeArchiveInputRequestTypeDef, _OptionalDeleteTapeArchiveInputRequestTypeDef
 ):
     pass
 
-DeleteTapeArchiveOutputTypeDef = TypedDict(
-    "DeleteTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
@@ -753,114 +610,56 @@
 )
 
 class DeleteTapeInputRequestTypeDef(
     _RequiredDeleteTapeInputRequestTypeDef, _OptionalDeleteTapeInputRequestTypeDef
 ):
     pass
 
-DeleteTapeOutputTypeDef = TypedDict(
-    "DeleteTapeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTapePoolInputRequestTypeDef = TypedDict(
     "DeleteTapePoolInputRequestTypeDef",
     {
         "PoolARN": str,
     },
 )
 
-DeleteTapePoolOutputTypeDef = TypedDict(
-    "DeleteTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVolumeInputRequestTypeDef = TypedDict(
     "DeleteVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteVolumeOutputTypeDef = TypedDict(
-    "DeleteVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "Status": AvailabilityMonitorTestStatusType,
-        "StartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
 DescribeCacheInputRequestTypeDef = TypedDict(
     "DescribeCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeCacheOutputTypeDef = TypedDict(
-    "DescribeCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "CacheAllocatedInBytes": int,
-        "CacheUsedPercentage": float,
-        "CacheDirtyPercentage": float,
-        "CacheHitPercentage": float,
-        "CacheMissPercentage": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCachediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
@@ -891,31 +690,26 @@
         "Ipv4Address": str,
         "MacAddress": str,
         "Ipv6Address": str,
     },
     total=False,
 )
 
-DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeInputRequestTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "GatewayARN": str,
+        "Key": str,
+        "Value": str,
     },
 )
 
-DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeOutputTypeDef",
+DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-        "DayOfWeek": int,
-        "DayOfMonth": int,
-        "Timezone": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNFSFileSharesInputRequestTypeDef = TypedDict(
     "DescribeNFSFileSharesInputRequestTypeDef",
     {
         "FileShareARNList": Sequence[str],
@@ -932,16 +726,16 @@
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
+SMBLocalGroupsOutputTypeDef = TypedDict(
+    "SMBLocalGroupsOutputTypeDef",
     {
         "GatewayAdmins": List[str],
     },
     total=False,
 )
 
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
@@ -954,19 +748,20 @@
 DescribeStorediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
-DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeTapeArchivesInputRequestTypeDef = TypedDict(
     "DescribeTapeArchivesInputRequestTypeDef",
     {
@@ -993,34 +788,14 @@
         "Worm": bool,
         "RetentionStartDate": datetime,
         "PoolEntryDate": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
-    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
@@ -1045,35 +820,14 @@
         "TapeRecoveryPointTime": datetime,
         "TapeSizeInBytes": int,
         "TapeStatus": str,
     },
     total=False,
 )
 
-_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeTapesInputDescribeTapesPaginateTypeDef(
-    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
-    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTapesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapesInputRequestTypeDef = TypedDict(
@@ -1114,46 +868,14 @@
 DescribeUploadBufferInputRequestTypeDef = TypedDict(
     "DescribeUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeUploadBufferOutputTypeDef = TypedDict(
-    "DescribeUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "UploadBufferUsedInBytes": int,
-        "UploadBufferAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "VTLDeviceARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
-    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeVTLDevicesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVTLDevicesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeVTLDevicesInputRequestTypeDef = TypedDict(
@@ -1174,25 +896,14 @@
 DescribeWorkingStorageInputRequestTypeDef = TypedDict(
     "DescribeWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeWorkingStorageOutputTypeDef = TypedDict(
-    "DescribeWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "WorkingStorageUsedInBytes": int,
-        "WorkingStorageAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredDetachVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 _OptionalDetachVolumeInputRequestTypeDef = TypedDict(
@@ -1204,22 +915,14 @@
 )
 
 class DetachVolumeInputRequestTypeDef(
     _RequiredDetachVolumeInputRequestTypeDef, _OptionalDetachVolumeInputRequestTypeDef
 ):
     pass
 
-DetachVolumeOutputTypeDef = TypedDict(
-    "DetachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceiSCSIAttributesTypeDef = TypedDict(
     "DeviceiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "ChapEnabled": bool,
@@ -1230,22 +933,14 @@
 DisableGatewayInputRequestTypeDef = TypedDict(
     "DisableGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DisableGatewayOutputTypeDef = TypedDict(
-    "DisableGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateFileSystemInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateFileSystemInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalDisassociateFileSystemInputRequestTypeDef = TypedDict(
@@ -1258,22 +953,14 @@
 
 class DisassociateFileSystemInputRequestTypeDef(
     _RequiredDisassociateFileSystemInputRequestTypeDef,
     _OptionalDisassociateFileSystemInputRequestTypeDef,
 ):
     pass
 
-DisassociateFileSystemOutputTypeDef = TypedDict(
-    "DisassociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "DiskId": str,
         "DiskPath": str,
         "DiskNode": str,
         "DiskStatus": str,
@@ -1281,14 +968,22 @@
         "DiskAllocationType": str,
         "DiskAllocationResource": str,
         "DiskAttributeList": List[str],
     },
     total=False,
 )
 
+EndpointNetworkConfigurationOutputTypeDef = TypedDict(
+    "EndpointNetworkConfigurationOutputTypeDef",
+    {
+        "IpAddresses": List[str],
+    },
+    total=False,
+)
+
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": FileShareTypeType,
         "FileShareARN": str,
         "FileShareId": str,
         "FileShareStatus": str,
@@ -1352,77 +1047,42 @@
 )
 
 class JoinDomainInputRequestTypeDef(
     _RequiredJoinDomainInputRequestTypeDef, _OptionalJoinDomainInputRequestTypeDef
 ):
     pass
 
-JoinDomainOutputTypeDef = TypedDict(
-    "JoinDomainOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAutomaticTapeCreationPoliciesInputRequestTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
     total=False,
 )
 
-ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSharesInputRequestTypeDef = TypedDict(
     "ListFileSharesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSystemAssociationsInputRequestTypeDef = TypedDict(
     "ListFileSystemAssociationsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
@@ -1431,34 +1091,14 @@
 ListLocalDisksInputRequestTypeDef = TypedDict(
     "ListLocalDisksInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1471,23 +1111,14 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    {
-        "PoolARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapePoolsInputRequestTypeDef = TypedDict(
     "ListTapePoolsInputRequestTypeDef",
     {
         "PoolARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1503,23 +1134,14 @@
         "RetentionLockType": RetentionLockTypeType,
         "RetentionLockTimeInDays": int,
         "PoolStatus": PoolStatusType,
     },
     total=False,
 )
 
-ListTapesInputListTapesPaginateTypeDef = TypedDict(
-    "ListTapesInputListTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapesInputRequestTypeDef = TypedDict(
     "ListTapesInputRequestTypeDef",
     {
         "TapeARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1544,22 +1166,14 @@
 ListVolumeInitiatorsInputRequestTypeDef = TypedDict(
     "ListVolumeInitiatorsInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-ListVolumeInitiatorsOutputTypeDef = TypedDict(
-    "ListVolumeInitiatorsOutputTypeDef",
-    {
-        "Initiators": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVolumeRecoveryPointsInputRequestTypeDef = TypedDict(
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1570,23 +1184,14 @@
         "VolumeSizeInBytes": int,
         "VolumeUsageInBytes": int,
         "VolumeRecoveryPointTime": str,
     },
     total=False,
 )
 
-ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
-    "ListVolumesInputListVolumesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVolumesInputRequestTypeDef = TypedDict(
     "ListVolumesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "Limit": int,
     },
@@ -1603,40 +1208,32 @@
         "VolumeType": str,
         "VolumeSizeInBytes": int,
         "VolumeAttachmentStatus": str,
     },
     total=False,
 )
 
-NotifyWhenUploadedInputRequestTypeDef = TypedDict(
-    "NotifyWhenUploadedInputRequestTypeDef",
+NFSFileShareDefaultsOutputTypeDef = TypedDict(
+    "NFSFileShareDefaultsOutputTypeDef",
     {
-        "FileShareARN": str,
+        "FileMode": str,
+        "DirectoryMode": str,
+        "GroupId": int,
+        "OwnerId": int,
     },
+    total=False,
 )
 
-NotifyWhenUploadedOutputTypeDef = TypedDict(
-    "NotifyWhenUploadedOutputTypeDef",
+NotifyWhenUploadedInputRequestTypeDef = TypedDict(
+    "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
 _RequiredRefreshCacheInputRequestTypeDef = TypedDict(
     "_RequiredRefreshCacheInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalRefreshCacheInputRequestTypeDef = TypedDict(
@@ -1649,182 +1246,90 @@
 )
 
 class RefreshCacheInputRequestTypeDef(
     _RequiredRefreshCacheInputRequestTypeDef, _OptionalRefreshCacheInputRequestTypeDef
 ):
     pass
 
-RefreshCacheOutputTypeDef = TypedDict(
-    "RefreshCacheOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceInputRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-RemoveTagsFromResourceOutputTypeDef = TypedDict(
-    "RemoveTagsFromResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResetCacheInputRequestTypeDef = TypedDict(
     "ResetCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ResetCacheOutputTypeDef = TypedDict(
-    "ResetCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
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
 RetrieveTapeArchiveInputRequestTypeDef = TypedDict(
     "RetrieveTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeArchiveOutputTypeDef = TypedDict(
-    "RetrieveTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "GatewayAdmins": Sequence[str],
     },
+    total=False,
 )
 
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
 
-SetLocalConsolePasswordOutputTypeDef = TypedDict(
-    "SetLocalConsolePasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSMBGuestPasswordInputRequestTypeDef = TypedDict(
     "SetSMBGuestPasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Password": str,
     },
 )
 
-SetSMBGuestPasswordOutputTypeDef = TypedDict(
-    "SetSMBGuestPasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ShutdownGatewayInputRequestTypeDef = TypedDict(
     "ShutdownGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ShutdownGatewayOutputTypeDef = TypedDict(
-    "ShutdownGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartGatewayInputRequestTypeDef = TypedDict(
     "StartGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartGatewayOutputTypeDef = TypedDict(
-    "StartGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
@@ -1838,30 +1343,14 @@
 
 class UpdateBandwidthRateLimitInputRequestTypeDef(
     _RequiredUpdateBandwidthRateLimitInputRequestTypeDef,
     _OptionalUpdateBandwidthRateLimitInputRequestTypeDef,
 ):
     pass
 
-UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChapCredentialsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
     },
@@ -1876,31 +1365,14 @@
 
 class UpdateChapCredentialsInputRequestTypeDef(
     _RequiredUpdateChapCredentialsInputRequestTypeDef,
     _OptionalUpdateChapCredentialsInputRequestTypeDef,
 ):
     pass
 
-UpdateChapCredentialsOutputTypeDef = TypedDict(
-    "UpdateChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFileSystemAssociationOutputTypeDef = TypedDict(
-    "UpdateFileSystemAssociationOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
@@ -1916,38 +1388,21 @@
 
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "GatewayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -1963,102 +1418,38 @@
 
 class UpdateMaintenanceStartTimeInputRequestTypeDef(
     _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef,
     _OptionalUpdateMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
-UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateNFSFileShareOutputTypeDef = TypedDict(
-    "UpdateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBFileShareOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBFileShareVisibilityInputRequestTypeDef = TypedDict(
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
     {
         "GatewayARN": str,
         "FileSharesVisible": bool,
     },
 )
 
-UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBSecurityStrategyInputRequestTypeDef = TypedDict(
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
     },
 )
 
-UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSnapshotScheduleOutputTypeDef = TypedDict(
-    "UpdateSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateVTLDeviceTypeInputRequestTypeDef = TypedDict(
     "UpdateVTLDeviceTypeInputRequestTypeDef",
     {
         "VTLDeviceARN": str,
         "DeviceType": str,
     },
 )
 
-UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
-    "UpdateVTLDeviceTypeOutputTypeDef",
-    {
-        "VTLDeviceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredActivateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayName": str,
         "GatewayTimezone": str,
         "GatewayRegion": str,
@@ -2255,37 +1646,14 @@
 )
 
 class CreateTapesInputRequestTypeDef(
     _RequiredCreateTapesInputRequestTypeDef, _OptionalCreateTapesInputRequestTypeDef
 ):
     pass
 
-DescribeSnapshotScheduleOutputTypeDef = TypedDict(
-    "DescribeSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
-        "Description": str,
-        "Timezone": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "Marker": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
         "StartAt": int,
         "RecurrenceInHours": int,
     },
@@ -2301,14 +1669,576 @@
 
 class UpdateSnapshotScheduleInputRequestTypeDef(
     _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
     _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
 ):
     pass
 
+ActivateGatewayOutputTypeDef = TypedDict(
+    "ActivateGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddCacheOutputTypeDef = TypedDict(
+    "AddCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddTagsToResourceOutputTypeDef = TypedDict(
+    "AddTagsToResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddUploadBufferOutputTypeDef = TypedDict(
+    "AddUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddWorkingStorageOutputTypeDef = TypedDict(
+    "AddWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssignTapePoolOutputTypeDef = TypedDict(
+    "AssignTapePoolOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateFileSystemOutputTypeDef = TypedDict(
+    "AssociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachVolumeOutputTypeDef = TypedDict(
+    "AttachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelArchivalOutputTypeDef = TypedDict(
+    "CancelArchivalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelRetrievalOutputTypeDef = TypedDict(
+    "CancelRetrievalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNFSFileShareOutputTypeDef = TypedDict(
+    "CreateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSMBFileShareOutputTypeDef = TypedDict(
+    "CreateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeARN": str,
+        "VolumeRecoveryPointTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotOutputTypeDef = TypedDict(
+    "CreateSnapshotOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "VolumeSizeInBytes": int,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapePoolOutputTypeDef = TypedDict(
+    "CreateTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapeWithBarcodeOutputTypeDef = TypedDict(
+    "CreateTapeWithBarcodeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapesOutputTypeDef = TypedDict(
+    "CreateTapesOutputTypeDef",
+    {
+        "TapeARNs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteChapCredentialsOutputTypeDef = TypedDict(
+    "DeleteChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileShareOutputTypeDef = TypedDict(
+    "DeleteFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotScheduleOutputTypeDef = TypedDict(
+    "DeleteSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeArchiveOutputTypeDef = TypedDict(
+    "DeleteTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeOutputTypeDef = TypedDict(
+    "DeleteTapeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapePoolOutputTypeDef = TypedDict(
+    "DeleteTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVolumeOutputTypeDef = TypedDict(
+    "DeleteVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "Status": AvailabilityMonitorTestStatusType,
+        "StartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCacheOutputTypeDef = TypedDict(
+    "DescribeCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "CacheAllocatedInBytes": int,
+        "CacheUsedPercentage": float,
+        "CacheDirtyPercentage": float,
+        "CacheHitPercentage": float,
+        "CacheMissPercentage": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+        "DayOfWeek": int,
+        "DayOfMonth": int,
+        "Timezone": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUploadBufferOutputTypeDef = TypedDict(
+    "DescribeUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "UploadBufferUsedInBytes": int,
+        "UploadBufferAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkingStorageOutputTypeDef = TypedDict(
+    "DescribeWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "WorkingStorageUsedInBytes": int,
+        "WorkingStorageAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachVolumeOutputTypeDef = TypedDict(
+    "DetachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableGatewayOutputTypeDef = TypedDict(
+    "DisableGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateFileSystemOutputTypeDef = TypedDict(
+    "DisassociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JoinDomainOutputTypeDef = TypedDict(
+    "JoinDomainOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVolumeInitiatorsOutputTypeDef = TypedDict(
+    "ListVolumeInitiatorsOutputTypeDef",
+    {
+        "Initiators": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+NotifyWhenUploadedOutputTypeDef = TypedDict(
+    "NotifyWhenUploadedOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RefreshCacheOutputTypeDef = TypedDict(
+    "RefreshCacheOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveTagsFromResourceOutputTypeDef = TypedDict(
+    "RemoveTagsFromResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetCacheOutputTypeDef = TypedDict(
+    "ResetCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeArchiveOutputTypeDef = TypedDict(
+    "RetrieveTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetLocalConsolePasswordOutputTypeDef = TypedDict(
+    "SetLocalConsolePasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetSMBGuestPasswordOutputTypeDef = TypedDict(
+    "SetSMBGuestPasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShutdownGatewayOutputTypeDef = TypedDict(
+    "ShutdownGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGatewayOutputTypeDef = TypedDict(
+    "StartGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChapCredentialsOutputTypeDef = TypedDict(
+    "UpdateChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFileSystemAssociationOutputTypeDef = TypedDict(
+    "UpdateFileSystemAssociationOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "GatewayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateNFSFileShareOutputTypeDef = TypedDict(
+    "UpdateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSnapshotScheduleOutputTypeDef = TypedDict(
+    "UpdateSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
+    "UpdateVTLDeviceTypeOutputTypeDef",
+    {
+        "VTLDeviceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateSMBFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateSMBFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
         "GatewayARN": str,
         "Role": str,
         "LocationARN": str,
@@ -2344,50 +2274,14 @@
 )
 
 class CreateSMBFileShareInputRequestTypeDef(
     _RequiredCreateSMBFileShareInputRequestTypeDef, _OptionalCreateSMBFileShareInputRequestTypeDef
 ):
     pass
 
-SMBFileShareInfoTypeDef = TypedDict(
-    "SMBFileShareInfoTypeDef",
-    {
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
-        "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "SMBACLEnabled": bool,
-        "AccessBasedEnumeration": bool,
-        "AdminUserList": List[str],
-        "ValidUserList": List[str],
-        "InvalidUserList": List[str],
-        "AuditDestinationARN": str,
-        "Authentication": str,
-        "CaseSensitivity": CaseSensitivityType,
-        "Tags": List[TagTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "OplocksEnabled": bool,
-    },
-    total=False,
-)
-
 _RequiredUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemAssociationInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
@@ -2468,15 +2362,15 @@
     _RequiredAssociateFileSystemInputRequestTypeDef, _OptionalAssociateFileSystemInputRequestTypeDef
 ):
     pass
 
 AutomaticTapeCreationPolicyInfoTypeDef = TypedDict(
     "AutomaticTapeCreationPolicyInfoTypeDef",
     {
-        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleTypeDef],
+        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleOutputTypeDef],
         "GatewayARN": str,
     },
     total=False,
 )
 
 UpdateAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -2486,16 +2380,16 @@
     },
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
@@ -2545,15 +2439,15 @@
     total=False,
 )
 
 DescribeChapCredentialsOutputTypeDef = TypedDict(
     "DescribeChapCredentialsOutputTypeDef",
     {
         "ChapCredentials": List[ChapInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateNFSFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
@@ -2587,45 +2481,14 @@
 )
 
 class CreateNFSFileShareInputRequestTypeDef(
     _RequiredCreateNFSFileShareInputRequestTypeDef, _OptionalCreateNFSFileShareInputRequestTypeDef
 ):
     pass
 
-NFSFileShareInfoTypeDef = TypedDict(
-    "NFSFileShareInfoTypeDef",
-    {
-        "NFSFileShareDefaults": NFSFileShareDefaultsTypeDef,
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
-        "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ClientList": List[str],
-        "Squash": str,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "Tags": List[TagTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "AuditDestinationARN": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNFSFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalUpdateNFSFileShareInputRequestTypeDef = TypedDict(
@@ -2664,75 +2527,270 @@
         "GatewayState": str,
         "GatewayNetworkInterfaces": List[NetworkInterfaceTypeDef],
         "GatewayType": str,
         "NextUpdateAvailabilityDate": str,
         "LastSoftwareUpdate": str,
         "Ec2InstanceId": str,
         "Ec2InstanceRegion": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "VPCEndpoint": str,
         "CloudWatchLogGroupARN": str,
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotScheduleOutputTypeDef = TypedDict(
+    "DescribeSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "StartAt": int,
+        "RecurrenceInHours": int,
+        "Description": str,
+        "Timezone": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Marker": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SMBFileShareInfoTypeDef = TypedDict(
+    "SMBFileShareInfoTypeDef",
+    {
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "SMBACLEnabled": bool,
+        "AccessBasedEnumeration": bool,
+        "AdminUserList": List[str],
+        "ValidUserList": List[str],
+        "InvalidUserList": List[str],
+        "AuditDestinationARN": str,
+        "Authentication": str,
+        "CaseSensitivity": CaseSensitivityType,
+        "Tags": List[TagOutputTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "OplocksEnabled": bool,
     },
+    total=False,
 )
 
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
+    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
     {
         "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
+_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTapesInputDescribeTapesPaginateTypeDef(
+    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
+    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "VTLDeviceARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
+    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+):
+    pass
+
+ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    {
+        "PoolARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTapesInputListTapesPaginateTypeDef = TypedDict(
+    "ListTapesInputListTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
+    "ListVolumesInputListVolumesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 DescribeTapeArchivesOutputTypeDef = TypedDict(
     "DescribeTapeArchivesOutputTypeDef",
     {
         "TapeArchives": List[TapeArchiveTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapeRecoveryPointsOutputTypeDef = TypedDict(
     "DescribeTapeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "TapeRecoveryPointInfos": List[TapeRecoveryPointInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapesOutputTypeDef = TypedDict(
     "DescribeTapesOutputTypeDef",
     {
         "Tapes": List[TapeTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VTLDeviceTypeDef = TypedDict(
     "VTLDeviceTypeDef",
     {
         "VTLDeviceARN": str,
@@ -2745,150 +2803,189 @@
 )
 
 ListLocalDisksOutputTypeDef = TypedDict(
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FileSystemAssociationInfoTypeDef = TypedDict(
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
-        "Tags": List[TagTypeDef],
-        "CacheAttributes": CacheAttributesTypeDef,
-        "EndpointNetworkConfiguration": EndpointNetworkConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileSystemAssociationSummaryList": List[FileSystemAssociationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapePoolsOutputTypeDef = TypedDict(
     "ListTapePoolsOutputTypeDef",
     {
         "PoolInfos": List[PoolInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapesOutputTypeDef = TypedDict(
     "ListTapesOutputTypeDef",
     {
         "TapeInfos": List[TapeInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumeRecoveryPointsOutputTypeDef = TypedDict(
     "ListVolumeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "VolumeRecoveryPointInfos": List[VolumeRecoveryPointInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumesOutputTypeDef = TypedDict(
     "ListVolumesOutputTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSMBFileSharesOutputTypeDef = TypedDict(
-    "DescribeSMBFileSharesOutputTypeDef",
+NFSFileShareInfoTypeDef = TypedDict(
+    "NFSFileShareInfoTypeDef",
     {
-        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NFSFileShareDefaults": NFSFileShareDefaultsOutputTypeDef,
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ClientList": List[str],
+        "Squash": str,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "Tags": List[TagOutputTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "AuditDestinationARN": str,
+    },
+    total=False,
+)
+
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStorediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeNFSFileSharesOutputTypeDef = TypedDict(
-    "DescribeNFSFileSharesOutputTypeDef",
+DescribeSMBFileSharesOutputTypeDef = TypedDict(
+    "DescribeSMBFileSharesOutputTypeDef",
     {
-        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
         "GatewayARN": str,
         "VTLDevices": List[VTLDeviceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNFSFileSharesOutputTypeDef = TypedDict(
+    "DescribeNFSFileSharesOutputTypeDef",
+    {
+        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/PKG-INFO` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.0
-Summary: Type annotations for boto3.StorageGateway 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.StorageGateway 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-storagegateway"></a>
 
 # mypy-boto3-storagegateway
 
 [![PyPI - mypy-boto3-storagegateway](https://img.shields.io/pypi/v/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-storagegateway?color=blue)](https://pypistats.org/packages/mypy-boto3-storagegateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,236 +374,243 @@
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
-    ActivateGatewayOutputTypeDef,
+    ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
-    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
-    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
-    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
-    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AttachVolumeOutputTypeDef,
+    AutomaticTapeCreationRuleOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
+    CacheAttributesOutputTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
-    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
-    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
-    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
-    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
-    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
-    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
-    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
+    TagOutputTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
-    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
-    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
-    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
-    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
+    NFSFileShareDefaultsOutputTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
-    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
-    ResetCacheOutputTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
+    SMBLocalGroupsTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
-    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
-    DescribeSnapshotScheduleOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     UpdateSnapshotScheduleInputRequestTypeDef,
+    ActivateGatewayOutputTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
+    AddUploadBufferOutputTypeDef,
+    AddWorkingStorageOutputTypeDef,
+    AssignTapePoolOutputTypeDef,
+    AssociateFileSystemOutputTypeDef,
+    AttachVolumeOutputTypeDef,
+    CancelArchivalOutputTypeDef,
+    CancelRetrievalOutputTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
+    DeleteFileShareOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
+    DeleteTapeOutputTypeDef,
+    DeleteTapePoolOutputTypeDef,
+    DeleteVolumeOutputTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
+    DescribeCacheOutputTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
+    DetachVolumeOutputTypeDef,
+    DisableGatewayOutputTypeDef,
+    DisassociateFileSystemOutputTypeDef,
+    JoinDomainOutputTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    RefreshCacheOutputTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
+    ResetCacheOutputTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
+    ShutdownGatewayOutputTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
-    SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
     UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
-    NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
+    DescribeSnapshotScheduleOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    SMBFileShareInfoTypeDef,
     DescribeSMBSettingsOutputTypeDef,
-    UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
-    DescribeSMBFileSharesOutputTypeDef,
+    NFSFileShareInfoTypeDef,
+    UpdateSMBLocalGroupsInputRequestTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
-    DescribeNFSFileSharesOutputTypeDef,
+    DescribeSMBFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
+    DescribeNFSFileSharesOutputTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-storagegateway-1.28.0/mypy_boto3_storagegateway.egg-info/SOURCES.txt` & `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.0/setup.py` & `mypy-boto3-storagegateway-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-storagegateway",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.StorageGateway 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.StorageGateway 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

