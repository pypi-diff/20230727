# Comparing `tmp/mypy-boto3-snowball-1.28.12.tar.gz` & `tmp/mypy-boto3-snowball-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-snowball-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
+gzip compressed data, was "mypy-boto3-snowball-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-snowball-1.28.12.tar` & `mypy-boto3-snowball-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.393318 mypy-boto3-snowball-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-27 11:49:41.389318 mypy-boto3-snowball-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16263 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.389318 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35021 2023-07-27 11:47:09.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34998 2023-07-27 11:47:09.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.389318 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-27 11:49:41.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:41.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:41.000000 mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.393318 mypy-boto3-snowball-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:47:08.000000 mypy-boto3-snowball-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.758719 mypy-boto3-snowball-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-18 19:32:41.754719 mypy-boto3-snowball-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34275 2023-07-18 19:32:29.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34254 2023-07-18 19:32:28.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.758719 mypy-boto3-snowball-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/setup.py
```

### Comparing `mypy-boto3-snowball-1.28.12/LICENSE` & `mypy-boto3-snowball-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.12/PKG-INFO` & `mypy-boto3-snowball-1.28.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.28.12
-Summary: Type annotations for boto3.Snowball 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snowball)](https://pepy.tech/project/mypy-boto3-snowball)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,90 +364,90 @@
     AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
     NotificationTypeDef,
     JobListEntryTypeDef,
     PickupDetailsTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     PickupDetailsOutputTypeDef,
     KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     ListPickupLocationsRequestRequestTypeDef,
     NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
     S3OnDeviceServiceConfigurationOutputTypeDef,
     TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    ListPickupLocationsResultTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
     DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
```

### Comparing `mypy-boto3-snowball-1.28.12/README.md` & `mypy-boto3-snowball-1.28.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snowball)](https://pepy.tech/project/mypy-boto3-snowball)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,90 +332,90 @@
     AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
     NotificationTypeDef,
     JobListEntryTypeDef,
     PickupDetailsTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     PickupDetailsOutputTypeDef,
     KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     ListPickupLocationsRequestRequestTypeDef,
     NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
     S3OnDeviceServiceConfigurationOutputTypeDef,
     TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    ListPickupLocationsResultTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
     DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/__init__.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/__init__.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/__main__.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Snowball 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Snowball 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/client.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/client.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/literals.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.pyi`

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
     "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
     "ImpactLevelType",
     "JobStateType",
@@ -45,15 +44,14 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
 ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
@@ -215,15 +213,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -302,28 +299,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/literals.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.py`

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
     "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
     "ImpactLevelType",
     "JobStateType",
@@ -44,14 +45,15 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
 ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
@@ -213,15 +215,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -300,28 +301,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/paginator.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,88 +66,88 @@
 class DescribeAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
         """
 
 
 class ListClusterJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
         """
 
 
 class ListCompatibleImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
         """
 
 
 class ListLongTermPricingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/paginator.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,83 +63,83 @@
 class DescribeAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
         """
 
 class ListClusterJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
         """
 
 class ListCompatibleImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
         """
 
 class ListLongTermPricingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/type_defs.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,90 +47,90 @@
     "AddressOutputTypeDef",
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAddressResultTypeDef",
     "NotificationTypeDef",
     "JobListEntryTypeDef",
     "PickupDetailsTypeDef",
+    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
+    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionOutputTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
     "EKSOnDeviceServiceConfigurationOutputTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceOutputTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionOutputTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
+    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
     "INDTaxDocumentsOutputTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
     "PickupDetailsOutputTypeDef",
     "KeyRangeOutputTypeDef",
     "KeyRangeTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "ListPickupLocationsRequestRequestTypeDef",
     "NFSOnDeviceServiceConfigurationOutputTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
     "S3OnDeviceServiceConfigurationOutputTypeDef",
     "TGWOnDeviceServiceConfigurationOutputTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TargetOnDeviceServiceOutputTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionOutputTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
-    "CreateAddressRequestRequestTypeDef",
-    "CreateAddressResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateLongTermPricingResultTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
-    "GetJobManifestResultTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
+    "ListPickupLocationsResultTypeDef",
+    "CreateAddressRequestRequestTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "ListPickupLocationsResultTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
     "DependentServiceOutputTypeDef",
     "DependentServiceTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsOutputTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationOutputTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
@@ -170,15 +170,14 @@
         "Landmark": str,
         "Country": str,
         "PostalCode": str,
         "PhoneNumber": str,
         "IsRestricted": bool,
         "Type": AddressTypeType,
     },
-    total=False,
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressId": str,
         "Name": str,
@@ -217,45 +216,39 @@
     "ClusterListEntryTypeDef",
     {
         "ClusterId": str,
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 NotificationOutputTypeDef = TypedDict(
     "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
         "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
         "DevicePickupSnsTopicARN": str,
     },
-    total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AddressId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationTypeDef = TypedDict(
     "NotificationTypeDef",
     {
         "SnsTopicARN": str,
@@ -273,15 +266,14 @@
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 PickupDetailsTypeDef = TypedDict(
     "PickupDetailsTypeDef",
     {
         "Name": str,
         "PhoneNumber": str,
@@ -290,14 +282,22 @@
         "IdentificationExpirationDate": Union[datetime, str],
         "IdentificationIssuingOrg": str,
         "DevicePickupId": str,
     },
     total=False,
 )
 
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
         "SnowballType": SnowballTypeType,
     },
 )
@@ -313,14 +313,22 @@
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
 
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -335,31 +343,37 @@
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
 
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
     },
-    total=False,
 )
 
 ServiceVersionOutputTypeDef = TypedDict(
     "ServiceVersionOutputTypeDef",
     {
         "Version": str,
     },
-    total=False,
 )
 
 ServiceVersionTypeDef = TypedDict(
     "ServiceVersionTypeDef",
     {
         "Version": str,
     },
@@ -369,20 +383,18 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -409,53 +421,49 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EKSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationOutputTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
-    total=False,
 )
 
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
 )
 
-_RequiredEc2AmiResourceOutputTypeDef = TypedDict(
-    "_RequiredEc2AmiResourceOutputTypeDef",
+Ec2AmiResourceOutputTypeDef = TypedDict(
+    "Ec2AmiResourceOutputTypeDef",
     {
         "AmiId": str,
-    },
-)
-_OptionalEc2AmiResourceOutputTypeDef = TypedDict(
-    "_OptionalEc2AmiResourceOutputTypeDef",
-    {
         "SnowballAmiId": str,
     },
-    total=False,
 )
 
-
-class Ec2AmiResourceOutputTypeDef(
-    _RequiredEc2AmiResourceOutputTypeDef, _OptionalEc2AmiResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredEc2AmiResourceTypeDef = TypedDict(
     "_RequiredEc2AmiResourceTypeDef",
     {
         "AmiId": str,
     },
 )
 _OptionalEc2AmiResourceTypeDef = TypedDict(
@@ -472,15 +480,14 @@
 
 
 EventTriggerDefinitionOutputTypeDef = TypedDict(
     "EventTriggerDefinitionOutputTypeDef",
     {
         "EventResourceARN": str,
     },
-    total=False,
 )
 
 EventTriggerDefinitionTypeDef = TypedDict(
     "EventTriggerDefinitionTypeDef",
     {
         "EventResourceARN": str,
     },
@@ -490,34 +497,66 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
+    {
+        "UpdatesURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 INDTaxDocumentsOutputTypeDef = TypedDict(
     "INDTaxDocumentsOutputTypeDef",
     {
         "GSTIN": str,
     },
-    total=False,
 )
 
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
@@ -527,49 +566,68 @@
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
-    total=False,
 )
 
 PickupDetailsOutputTypeDef = TypedDict(
     "PickupDetailsOutputTypeDef",
     {
         "Name": str,
         "PhoneNumber": str,
         "Email": str,
         "IdentificationNumber": str,
         "IdentificationExpirationDate": datetime,
         "IdentificationIssuingOrg": str,
         "DevicePickupId": str,
     },
-    total=False,
 )
 
 KeyRangeOutputTypeDef = TypedDict(
     "KeyRangeOutputTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
-    total=False,
 )
 
 KeyRangeTypeDef = TypedDict(
     "KeyRangeTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -584,41 +642,73 @@
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -634,15 +724,14 @@
         "CurrentActiveJob": str,
         "ReplacementJob": str,
         "IsLongTermPricingAutoRenew": bool,
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
-    total=False,
 )
 
 ListPickupLocationsRequestRequestTypeDef = TypedDict(
     "ListPickupLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -652,15 +741,14 @@
 
 NFSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationOutputTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
-    total=False,
 )
 
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
@@ -672,24 +760,22 @@
     "S3OnDeviceServiceConfigurationOutputTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
         "ServiceSize": int,
         "FaultTolerance": int,
     },
-    total=False,
 )
 
 TGWOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "TGWOnDeviceServiceConfigurationOutputTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
-    total=False,
 )
 
 S3OnDeviceServiceConfigurationTypeDef = TypedDict(
     "S3OnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
@@ -704,21 +790,41 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
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
 TargetOnDeviceServiceOutputTypeDef = TypedDict(
     "TargetOnDeviceServiceOutputTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
-    total=False,
 )
 
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
@@ -728,23 +834,21 @@
 
 ShipmentTypeDef = TypedDict(
     "ShipmentTypeDef",
     {
         "Status": str,
         "TrackingNumber": str,
     },
-    total=False,
 )
 
 WirelessConnectionOutputTypeDef = TypedDict(
     "WirelessConnectionOutputTypeDef",
     {
         "IsWifiEnabled": bool,
     },
-    total=False,
 )
 
 WirelessConnectionTypeDef = TypedDict(
     "WirelessConnectionTypeDef",
     {
         "IsWifiEnabled": bool,
     },
@@ -778,254 +882,115 @@
 class UpdateLongTermPricingRequestRequestTypeDef(
     _RequiredUpdateLongTermPricingRequestRequestTypeDef,
     _OptionalUpdateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
 
-CreateAddressRequestRequestTypeDef = TypedDict(
-    "CreateAddressRequestRequestTypeDef",
-    {
-        "Address": AddressTypeDef,
-    },
-)
-
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
-    {
-        "AddressId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
         "Address": AddressOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
         "Addresses": List[AddressOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
     {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Addresses": List[AddressOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
+CreateAddressRequestRequestTypeDef = TypedDict(
+    "CreateAddressRequestRequestTypeDef",
     {
-        "UpdatesURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Address": AddressTypeDef,
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPickupLocationsResultTypeDef = TypedDict(
-    "ListPickupLocationsResultTypeDef",
-    {
-        "Addresses": List[AddressOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClusterJobsResultTypeDef = TypedDict(
     "ListClusterJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DependentServiceOutputTypeDef = TypedDict(
     "DependentServiceOutputTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionOutputTypeDef,
     },
-    total=False,
 )
 
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 LambdaResourceOutputTypeDef = TypedDict(
     "LambdaResourceOutputTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": List[EventTriggerDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
@@ -1034,15 +999,14 @@
 )
 
 TaxDocumentsOutputTypeDef = TypedDict(
     "TaxDocumentsOutputTypeDef",
     {
         "IND": INDTaxDocumentsOutputTypeDef,
     },
-    total=False,
 )
 
 TaxDocumentsTypeDef = TypedDict(
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
@@ -1050,27 +1014,26 @@
 )
 
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "OnDeviceServiceConfigurationOutputTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationOutputTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationOutputTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationOutputTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
@@ -1083,15 +1046,14 @@
 S3ResourceOutputTypeDef = TypedDict(
     "S3ResourceOutputTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeOutputTypeDef,
         "TargetOnDeviceServices": List[TargetOnDeviceServiceOutputTypeDef],
     },
-    total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
@@ -1103,23 +1065,21 @@
 ShippingDetailsTypeDef = TypedDict(
     "ShippingDetailsTypeDef",
     {
         "ShippingOption": ShippingOptionType,
         "InboundShipment": ShipmentTypeDef,
         "OutboundShipment": ShipmentTypeDef,
     },
-    total=False,
 )
 
 SnowconeDeviceConfigurationOutputTypeDef = TypedDict(
     "SnowconeDeviceConfigurationOutputTypeDef",
     {
         "WirelessConnection": WirelessConnectionOutputTypeDef,
     },
-    total=False,
 )
 
 SnowconeDeviceConfigurationTypeDef = TypedDict(
     "SnowconeDeviceConfigurationTypeDef",
     {
         "WirelessConnection": WirelessConnectionTypeDef,
     },
@@ -1129,15 +1089,15 @@
 ListServiceVersionsResultTypeDef = TypedDict(
     "ListServiceVersionsResultTypeDef",
     {
         "ServiceVersions": List[ServiceVersionOutputTypeDef],
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListServiceVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceVersionsRequestRequestTypeDef",
     {
         "ServiceName": ServiceNameType,
@@ -1164,15 +1124,14 @@
 JobResourceOutputTypeDef = TypedDict(
     "JobResourceOutputTypeDef",
     {
         "S3Resources": List[S3ResourceOutputTypeDef],
         "LambdaResources": List[LambdaResourceOutputTypeDef],
         "Ec2AmiResources": List[Ec2AmiResourceOutputTypeDef],
     },
-    total=False,
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
@@ -1182,15 +1141,14 @@
 )
 
 DeviceConfigurationOutputTypeDef = TypedDict(
     "DeviceConfigurationOutputTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 DeviceConfigurationTypeDef = TypedDict(
     "DeviceConfigurationTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationTypeDef,
     },
@@ -1212,15 +1170,14 @@
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsOutputTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "AddressId": str,
@@ -1338,15 +1295,14 @@
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
         "ImpactLevel": ImpactLevelType,
         "PickupDetails": PickupDetailsOutputTypeDef,
         "SnowballId": str,
     },
-    total=False,
 )
 
 CreateJobRequestRequestTypeDef = TypedDict(
     "CreateJobRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "Resources": JobResourceTypeDef,
@@ -1371,19 +1327,19 @@
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball/type_defs.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -46,90 +46,90 @@
     "AddressOutputTypeDef",
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAddressResultTypeDef",
     "NotificationTypeDef",
     "JobListEntryTypeDef",
     "PickupDetailsTypeDef",
+    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
+    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionOutputTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
     "EKSOnDeviceServiceConfigurationOutputTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceOutputTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionOutputTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
+    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
     "INDTaxDocumentsOutputTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
     "PickupDetailsOutputTypeDef",
     "KeyRangeOutputTypeDef",
     "KeyRangeTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "ListPickupLocationsRequestRequestTypeDef",
     "NFSOnDeviceServiceConfigurationOutputTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
     "S3OnDeviceServiceConfigurationOutputTypeDef",
     "TGWOnDeviceServiceConfigurationOutputTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TargetOnDeviceServiceOutputTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionOutputTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
-    "CreateAddressRequestRequestTypeDef",
-    "CreateAddressResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateLongTermPricingResultTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
-    "GetJobManifestResultTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
+    "ListPickupLocationsResultTypeDef",
+    "CreateAddressRequestRequestTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "ListPickupLocationsResultTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
     "DependentServiceOutputTypeDef",
     "DependentServiceTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsOutputTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationOutputTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
@@ -169,15 +169,14 @@
         "Landmark": str,
         "Country": str,
         "PostalCode": str,
         "PhoneNumber": str,
         "IsRestricted": bool,
         "Type": AddressTypeType,
     },
-    total=False,
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressId": str,
         "Name": str,
@@ -216,45 +215,39 @@
     "ClusterListEntryTypeDef",
     {
         "ClusterId": str,
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 NotificationOutputTypeDef = TypedDict(
     "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
         "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
         "DevicePickupSnsTopicARN": str,
     },
-    total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AddressId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationTypeDef = TypedDict(
     "NotificationTypeDef",
     {
         "SnsTopicARN": str,
@@ -272,15 +265,14 @@
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 PickupDetailsTypeDef = TypedDict(
     "PickupDetailsTypeDef",
     {
         "Name": str,
         "PhoneNumber": str,
@@ -289,14 +281,22 @@
         "IdentificationExpirationDate": Union[datetime, str],
         "IdentificationIssuingOrg": str,
         "DevicePickupId": str,
     },
     total=False,
 )
 
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
         "SnowballType": SnowballTypeType,
     },
 )
@@ -310,14 +310,22 @@
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -330,31 +338,37 @@
 
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
     },
-    total=False,
 )
 
 ServiceVersionOutputTypeDef = TypedDict(
     "ServiceVersionOutputTypeDef",
     {
         "Version": str,
     },
-    total=False,
 )
 
 ServiceVersionTypeDef = TypedDict(
     "ServiceVersionTypeDef",
     {
         "Version": str,
     },
@@ -364,20 +378,18 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -404,51 +416,49 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EKSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationOutputTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
-    total=False,
 )
 
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
 )
 
-_RequiredEc2AmiResourceOutputTypeDef = TypedDict(
-    "_RequiredEc2AmiResourceOutputTypeDef",
+Ec2AmiResourceOutputTypeDef = TypedDict(
+    "Ec2AmiResourceOutputTypeDef",
     {
         "AmiId": str,
-    },
-)
-_OptionalEc2AmiResourceOutputTypeDef = TypedDict(
-    "_OptionalEc2AmiResourceOutputTypeDef",
-    {
         "SnowballAmiId": str,
     },
-    total=False,
 )
 
-class Ec2AmiResourceOutputTypeDef(
-    _RequiredEc2AmiResourceOutputTypeDef, _OptionalEc2AmiResourceOutputTypeDef
-):
-    pass
-
 _RequiredEc2AmiResourceTypeDef = TypedDict(
     "_RequiredEc2AmiResourceTypeDef",
     {
         "AmiId": str,
     },
 )
 _OptionalEc2AmiResourceTypeDef = TypedDict(
@@ -463,15 +473,14 @@
     pass
 
 EventTriggerDefinitionOutputTypeDef = TypedDict(
     "EventTriggerDefinitionOutputTypeDef",
     {
         "EventResourceARN": str,
     },
-    total=False,
 )
 
 EventTriggerDefinitionTypeDef = TypedDict(
     "EventTriggerDefinitionTypeDef",
     {
         "EventResourceARN": str,
     },
@@ -481,34 +490,66 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
+    {
+        "UpdatesURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 INDTaxDocumentsOutputTypeDef = TypedDict(
     "INDTaxDocumentsOutputTypeDef",
     {
         "GSTIN": str,
     },
-    total=False,
 )
 
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
@@ -518,49 +559,66 @@
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
-    total=False,
 )
 
 PickupDetailsOutputTypeDef = TypedDict(
     "PickupDetailsOutputTypeDef",
     {
         "Name": str,
         "PhoneNumber": str,
         "Email": str,
         "IdentificationNumber": str,
         "IdentificationExpirationDate": datetime,
         "IdentificationIssuingOrg": str,
         "DevicePickupId": str,
     },
-    total=False,
 )
 
 KeyRangeOutputTypeDef = TypedDict(
     "KeyRangeOutputTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
-    total=False,
 )
 
 KeyRangeTypeDef = TypedDict(
     "KeyRangeTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -573,41 +631,73 @@
 )
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -623,15 +713,14 @@
         "CurrentActiveJob": str,
         "ReplacementJob": str,
         "IsLongTermPricingAutoRenew": bool,
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
-    total=False,
 )
 
 ListPickupLocationsRequestRequestTypeDef = TypedDict(
     "ListPickupLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -641,15 +730,14 @@
 
 NFSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationOutputTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
-    total=False,
 )
 
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
@@ -661,24 +749,22 @@
     "S3OnDeviceServiceConfigurationOutputTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
         "ServiceSize": int,
         "FaultTolerance": int,
     },
-    total=False,
 )
 
 TGWOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "TGWOnDeviceServiceConfigurationOutputTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
-    total=False,
 )
 
 S3OnDeviceServiceConfigurationTypeDef = TypedDict(
     "S3OnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
@@ -693,21 +779,41 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
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
 TargetOnDeviceServiceOutputTypeDef = TypedDict(
     "TargetOnDeviceServiceOutputTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
-    total=False,
 )
 
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
@@ -717,23 +823,21 @@
 
 ShipmentTypeDef = TypedDict(
     "ShipmentTypeDef",
     {
         "Status": str,
         "TrackingNumber": str,
     },
-    total=False,
 )
 
 WirelessConnectionOutputTypeDef = TypedDict(
     "WirelessConnectionOutputTypeDef",
     {
         "IsWifiEnabled": bool,
     },
-    total=False,
 )
 
 WirelessConnectionTypeDef = TypedDict(
     "WirelessConnectionTypeDef",
     {
         "IsWifiEnabled": bool,
     },
@@ -765,252 +869,115 @@
 
 class UpdateLongTermPricingRequestRequestTypeDef(
     _RequiredUpdateLongTermPricingRequestRequestTypeDef,
     _OptionalUpdateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
-CreateAddressRequestRequestTypeDef = TypedDict(
-    "CreateAddressRequestRequestTypeDef",
-    {
-        "Address": AddressTypeDef,
-    },
-)
-
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
-    {
-        "AddressId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
         "Address": AddressOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
         "Addresses": List[AddressOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
     {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Addresses": List[AddressOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
+CreateAddressRequestRequestTypeDef = TypedDict(
+    "CreateAddressRequestRequestTypeDef",
     {
-        "UpdatesURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Address": AddressTypeDef,
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPickupLocationsResultTypeDef = TypedDict(
-    "ListPickupLocationsResultTypeDef",
-    {
-        "Addresses": List[AddressOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClusterJobsResultTypeDef = TypedDict(
     "ListClusterJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DependentServiceOutputTypeDef = TypedDict(
     "DependentServiceOutputTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionOutputTypeDef,
     },
-    total=False,
 )
 
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 LambdaResourceOutputTypeDef = TypedDict(
     "LambdaResourceOutputTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": List[EventTriggerDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
@@ -1019,15 +986,14 @@
 )
 
 TaxDocumentsOutputTypeDef = TypedDict(
     "TaxDocumentsOutputTypeDef",
     {
         "IND": INDTaxDocumentsOutputTypeDef,
     },
-    total=False,
 )
 
 TaxDocumentsTypeDef = TypedDict(
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
@@ -1035,27 +1001,26 @@
 )
 
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
     "OnDeviceServiceConfigurationOutputTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationOutputTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationOutputTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationOutputTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
@@ -1068,15 +1033,14 @@
 S3ResourceOutputTypeDef = TypedDict(
     "S3ResourceOutputTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeOutputTypeDef,
         "TargetOnDeviceServices": List[TargetOnDeviceServiceOutputTypeDef],
     },
-    total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
@@ -1088,23 +1052,21 @@
 ShippingDetailsTypeDef = TypedDict(
     "ShippingDetailsTypeDef",
     {
         "ShippingOption": ShippingOptionType,
         "InboundShipment": ShipmentTypeDef,
         "OutboundShipment": ShipmentTypeDef,
     },
-    total=False,
 )
 
 SnowconeDeviceConfigurationOutputTypeDef = TypedDict(
     "SnowconeDeviceConfigurationOutputTypeDef",
     {
         "WirelessConnection": WirelessConnectionOutputTypeDef,
     },
-    total=False,
 )
 
 SnowconeDeviceConfigurationTypeDef = TypedDict(
     "SnowconeDeviceConfigurationTypeDef",
     {
         "WirelessConnection": WirelessConnectionTypeDef,
     },
@@ -1114,15 +1076,15 @@
 ListServiceVersionsResultTypeDef = TypedDict(
     "ListServiceVersionsResultTypeDef",
     {
         "ServiceVersions": List[ServiceVersionOutputTypeDef],
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListServiceVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceVersionsRequestRequestTypeDef",
     {
         "ServiceName": ServiceNameType,
@@ -1147,15 +1109,14 @@
 JobResourceOutputTypeDef = TypedDict(
     "JobResourceOutputTypeDef",
     {
         "S3Resources": List[S3ResourceOutputTypeDef],
         "LambdaResources": List[LambdaResourceOutputTypeDef],
         "Ec2AmiResources": List[Ec2AmiResourceOutputTypeDef],
     },
-    total=False,
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
@@ -1165,15 +1126,14 @@
 )
 
 DeviceConfigurationOutputTypeDef = TypedDict(
     "DeviceConfigurationOutputTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 DeviceConfigurationTypeDef = TypedDict(
     "DeviceConfigurationTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationTypeDef,
     },
@@ -1195,15 +1155,14 @@
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsOutputTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "AddressId": str,
@@ -1315,15 +1274,14 @@
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
         "ImpactLevel": ImpactLevelType,
         "PickupDetails": PickupDetailsOutputTypeDef,
         "SnowballId": str,
     },
-    total=False,
 )
 
 CreateJobRequestRequestTypeDef = TypedDict(
     "CreateJobRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "Resources": JobResourceTypeDef,
@@ -1348,19 +1306,19 @@
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/PKG-INFO` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.28.12
-Summary: Type annotations for boto3.Snowball 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snowball)](https://pepy.tech/project/mypy-boto3-snowball)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,90 +364,90 @@
     AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
     NotificationTypeDef,
     JobListEntryTypeDef,
     PickupDetailsTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     PickupDetailsOutputTypeDef,
     KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     ListPickupLocationsRequestRequestTypeDef,
     NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
     S3OnDeviceServiceConfigurationOutputTypeDef,
     TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
-    ListPickupLocationsResultTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
     DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
```

### Comparing `mypy-boto3-snowball-1.28.12/mypy_boto3_snowball.egg-info/SOURCES.txt` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.12/setup.py` & `mypy-boto3-snowball-1.28.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-snowball",
-    version="1.28.12",
+    version="1.28.5",
     packages=["mypy_boto3_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Snowball 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

