# Comparing `tmp/mypy-boto3-lightsail-1.28.0.tar.gz` & `tmp/mypy-boto3-lightsail-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lightsail-1.28.0.tar", last modified: Thu Jul  6 21:00:00 2023, max compression
+gzip compressed data, was "mypy-boto3-lightsail-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
```

## Comparing `mypy-boto3-lightsail-1.28.0.tar` & `mypy-boto3-lightsail-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:00.698356 mypy-boto3-lightsail-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36513 2023-07-06 21:00:00.686356 mypy-boto3-lightsail-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35020 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:00.678356 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113940 2023-07-06 20:45:53.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   113754 2023-07-06 20:45:51.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-07-06 20:45:54.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-07-06 20:45:54.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-07-06 20:45:53.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-07-06 20:45:53.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   146638 2023-07-06 20:46:00.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146539 2023-07-06 20:45:56.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:00.686356 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36513 2023-07-06 21:00:00.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:00.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:00.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:00.000000 mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:00.698356 mypy-boto3-lightsail-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:45:50.000000 mypy-boto3-lightsail-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.292455 mypy-boto3-lightsail-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36949 2023-07-27 05:34:57.284455 mypy-boto3-lightsail-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.284455 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113940 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113754 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-07-27 05:25:26.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   150553 2023-07-27 05:25:28.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150452 2023-07-27 05:25:27.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.284455 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36949 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.292455 mypy-boto3-lightsail-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/setup.py
```

### Comparing `mypy-boto3-lightsail-1.28.0/LICENSE` & `mypy-boto3-lightsail-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/PKG-INFO` & `mypy-boto3-lightsail-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.0
-Summary: Type annotations for boto3.Lightsail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Lightsail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lightsail"></a>
 
 # mypy-boto3-lightsail
 
 [![PyPI - mypy-boto3-lightsail](https://img.shields.io/pypi/v/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -474,14 +474,15 @@
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
+    AccessRulesOutputTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
@@ -490,39 +491,48 @@
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
     BlueprintTypeDef,
+    BucketAccessLogConfigOutputTypeDef,
     BucketAccessLogConfigTypeDef,
     BucketBundleTypeDef,
     BucketStateTypeDef,
     ResourceReceivingAccessTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     BundleTypeDef,
+    CacheBehaviorOutputTypeDef,
+    CacheBehaviorPerPathOutputTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
+    CookieObjectOutputTypeDef,
+    HeaderObjectOutputTypeDef,
+    QueryStringObjectOutputTypeDef,
     CookieObjectTypeDef,
     HeaderObjectTypeDef,
     QueryStringObjectTypeDef,
     PortInfoTypeDef,
     CloudFormationStackRecordSourceInfoTypeDef,
     DestinationInfoTypeDef,
     ContainerImageTypeDef,
+    ContainerOutputTypeDef,
     ContainerTypeDef,
     ContainerServiceECRImagePullerRoleRequestTypeDef,
     ContainerServiceECRImagePullerRoleTypeDef,
+    ContainerServiceHealthCheckConfigOutputTypeDef,
     ContainerServiceHealthCheckConfigTypeDef,
     ContainerServiceLogEventTypeDef,
     ContainerServicePowerTypeDef,
     ContainerServiceRegistryLoginTypeDef,
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
+    TagTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
@@ -551,14 +561,15 @@
     DetachInstancesFromLoadBalancerRequestRequestTypeDef,
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
+    DomainEntryOutputTypeDef,
     ResourceRecordTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetActiveNamesResultTypeDef,
@@ -640,15 +651,15 @@
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
     GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
-    RelationalDatabaseParameterTypeDef,
+    RelationalDatabaseParameterOutputTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
     GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
@@ -673,14 +684,15 @@
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
+    RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
@@ -704,45 +716,46 @@
     StaticIpTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
-    CreateBucketRequestRequestTypeDef,
-    CreateCertificateRequestRequestTypeDef,
-    CreateDiskSnapshotRequestRequestTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateInstanceSnapshotRequestRequestTypeDef,
-    CreateKeyPairRequestRequestTypeDef,
-    CreateLoadBalancerRequestRequestTypeDef,
-    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    CreateRelationalDatabaseRequestRequestTypeDef,
-    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
-    TagResourceRequestRequestTypeDef,
     GetBundlesResultTypeDef,
+    CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
     GetContainerImagesResultTypeDef,
     RegisterContainerImageResultTypeDef,
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
+    CreateBucketRequestRequestTypeDef,
+    CreateCertificateRequestRequestTypeDef,
+    CreateDiskSnapshotRequestRequestTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    CreateInstanceSnapshotRequestRequestTypeDef,
+    CreateKeyPairRequestRequestTypeDef,
+    CreateLoadBalancerRequestRequestTypeDef,
+    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    CreateRelationalDatabaseRequestRequestTypeDef,
+    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
@@ -758,22 +771,22 @@
     GetInstanceStateResultTypeDef,
     GetLoadBalancerTlsPoliciesResultTypeDef,
     GetRelationalDatabaseBlueprintsResultTypeDef,
     GetRelationalDatabaseBundlesResultTypeDef,
     GetRelationalDatabaseEventsResultTypeDef,
     GetRelationalDatabaseLogEventsResultTypeDef,
     GetRelationalDatabaseParametersResultTypeDef,
-    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     InstanceAccessDetailsTypeDef,
     InstanceNetworkingTypeDef,
     LoadBalancerTlsCertificateDomainValidationRecordTypeDef,
     LoadBalancerTlsCertificateRenewalSummaryTypeDef,
     LoadBalancerTypeDef,
     RegisteredDomainDelegationInfoTypeDef,
     RelationalDatabaseTypeDef,
+    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     GetBucketAccessKeysResultTypeDef,
     CreateDiskFromSnapshotRequestRequestTypeDef,
     CreateDiskRequestRequestTypeDef,
     CreateInstancesFromSnapshotRequestRequestTypeDef,
     CreateInstancesRequestRequestTypeDef,
     EnableAddOnRequestRequestTypeDef,
     GetAlarmsResultTypeDef,
@@ -875,16 +888,16 @@
     InstanceHardwareTypeDef,
     InstanceSnapshotTypeDef,
     CreateKeyPairResultTypeDef,
     GetKeyPairResultTypeDef,
     GetKeyPairsResultTypeDef,
     GetRelationalDatabaseSnapshotResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
-    CreateDistributionRequestRequestTypeDef,
     LightsailDistributionTypeDef,
+    CreateDistributionRequestRequestTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
     ExportSnapshotRecordSourceInfoTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.0/README.md` & `mypy-boto3-lightsail-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lightsail"></a>
 
 # mypy-boto3-lightsail
 
 [![PyPI - mypy-boto3-lightsail](https://img.shields.io/pypi/v/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -442,14 +442,15 @@
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
+    AccessRulesOutputTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
@@ -458,39 +459,48 @@
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
     BlueprintTypeDef,
+    BucketAccessLogConfigOutputTypeDef,
     BucketAccessLogConfigTypeDef,
     BucketBundleTypeDef,
     BucketStateTypeDef,
     ResourceReceivingAccessTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     BundleTypeDef,
+    CacheBehaviorOutputTypeDef,
+    CacheBehaviorPerPathOutputTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
+    CookieObjectOutputTypeDef,
+    HeaderObjectOutputTypeDef,
+    QueryStringObjectOutputTypeDef,
     CookieObjectTypeDef,
     HeaderObjectTypeDef,
     QueryStringObjectTypeDef,
     PortInfoTypeDef,
     CloudFormationStackRecordSourceInfoTypeDef,
     DestinationInfoTypeDef,
     ContainerImageTypeDef,
+    ContainerOutputTypeDef,
     ContainerTypeDef,
     ContainerServiceECRImagePullerRoleRequestTypeDef,
     ContainerServiceECRImagePullerRoleTypeDef,
+    ContainerServiceHealthCheckConfigOutputTypeDef,
     ContainerServiceHealthCheckConfigTypeDef,
     ContainerServiceLogEventTypeDef,
     ContainerServicePowerTypeDef,
     ContainerServiceRegistryLoginTypeDef,
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
+    TagTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
@@ -519,14 +529,15 @@
     DetachInstancesFromLoadBalancerRequestRequestTypeDef,
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
+    DomainEntryOutputTypeDef,
     ResourceRecordTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetActiveNamesResultTypeDef,
@@ -608,15 +619,15 @@
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
     GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
-    RelationalDatabaseParameterTypeDef,
+    RelationalDatabaseParameterOutputTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
     GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
@@ -641,14 +652,15 @@
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
+    RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
@@ -672,45 +684,46 @@
     StaticIpTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
-    CreateBucketRequestRequestTypeDef,
-    CreateCertificateRequestRequestTypeDef,
-    CreateDiskSnapshotRequestRequestTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateInstanceSnapshotRequestRequestTypeDef,
-    CreateKeyPairRequestRequestTypeDef,
-    CreateLoadBalancerRequestRequestTypeDef,
-    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    CreateRelationalDatabaseRequestRequestTypeDef,
-    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
-    TagResourceRequestRequestTypeDef,
     GetBundlesResultTypeDef,
+    CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
     GetContainerImagesResultTypeDef,
     RegisterContainerImageResultTypeDef,
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
+    CreateBucketRequestRequestTypeDef,
+    CreateCertificateRequestRequestTypeDef,
+    CreateDiskSnapshotRequestRequestTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    CreateInstanceSnapshotRequestRequestTypeDef,
+    CreateKeyPairRequestRequestTypeDef,
+    CreateLoadBalancerRequestRequestTypeDef,
+    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    CreateRelationalDatabaseRequestRequestTypeDef,
+    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
@@ -726,22 +739,22 @@
     GetInstanceStateResultTypeDef,
     GetLoadBalancerTlsPoliciesResultTypeDef,
     GetRelationalDatabaseBlueprintsResultTypeDef,
     GetRelationalDatabaseBundlesResultTypeDef,
     GetRelationalDatabaseEventsResultTypeDef,
     GetRelationalDatabaseLogEventsResultTypeDef,
     GetRelationalDatabaseParametersResultTypeDef,
-    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     InstanceAccessDetailsTypeDef,
     InstanceNetworkingTypeDef,
     LoadBalancerTlsCertificateDomainValidationRecordTypeDef,
     LoadBalancerTlsCertificateRenewalSummaryTypeDef,
     LoadBalancerTypeDef,
     RegisteredDomainDelegationInfoTypeDef,
     RelationalDatabaseTypeDef,
+    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     GetBucketAccessKeysResultTypeDef,
     CreateDiskFromSnapshotRequestRequestTypeDef,
     CreateDiskRequestRequestTypeDef,
     CreateInstancesFromSnapshotRequestRequestTypeDef,
     CreateInstancesRequestRequestTypeDef,
     EnableAddOnRequestRequestTypeDef,
     GetAlarmsResultTypeDef,
@@ -843,16 +856,16 @@
     InstanceHardwareTypeDef,
     InstanceSnapshotTypeDef,
     CreateKeyPairResultTypeDef,
     GetKeyPairResultTypeDef,
     GetKeyPairsResultTypeDef,
     GetRelationalDatabaseSnapshotResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
-    CreateDistributionRequestRequestTypeDef,
     LightsailDistributionTypeDef,
+    CreateDistributionRequestRequestTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
     ExportSnapshotRecordSourceInfoTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/__init__.py` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/__init__.pyi` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/__main__.py` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lightsail 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Lightsail 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
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

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/client.py` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/client.pyi` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/literals.py` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,14 +653,15 @@
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
@@ -739,26 +740,28 @@
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

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/literals.pyi` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -651,14 +651,15 @@
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
@@ -737,26 +738,28 @@
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

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/paginator.py` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/paginator.pyi` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/type_defs.py` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessKeyLastUsedTypeDef",
+    "AccessRulesOutputTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
     "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
@@ -115,39 +116,48 @@
     "AttachDiskRequestRequestTypeDef",
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     "AttachLoadBalancerTlsCertificateRequestRequestTypeDef",
     "AttachStaticIpRequestRequestTypeDef",
     "AttachedDiskTypeDef",
     "AvailabilityZoneTypeDef",
     "BlueprintTypeDef",
+    "BucketAccessLogConfigOutputTypeDef",
     "BucketAccessLogConfigTypeDef",
     "BucketBundleTypeDef",
     "BucketStateTypeDef",
     "ResourceReceivingAccessTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "BundleTypeDef",
+    "CacheBehaviorOutputTypeDef",
+    "CacheBehaviorPerPathOutputTypeDef",
     "CacheBehaviorPerPathTypeDef",
     "CacheBehaviorTypeDef",
+    "CookieObjectOutputTypeDef",
+    "HeaderObjectOutputTypeDef",
+    "QueryStringObjectOutputTypeDef",
     "CookieObjectTypeDef",
     "HeaderObjectTypeDef",
     "QueryStringObjectTypeDef",
     "PortInfoTypeDef",
     "CloudFormationStackRecordSourceInfoTypeDef",
     "DestinationInfoTypeDef",
     "ContainerImageTypeDef",
+    "ContainerOutputTypeDef",
     "ContainerTypeDef",
     "ContainerServiceECRImagePullerRoleRequestTypeDef",
     "ContainerServiceECRImagePullerRoleTypeDef",
+    "ContainerServiceHealthCheckConfigOutputTypeDef",
     "ContainerServiceHealthCheckConfigTypeDef",
     "ContainerServiceLogEventTypeDef",
     "ContainerServicePowerTypeDef",
     "ContainerServiceRegistryLoginTypeDef",
     "ContainerServiceStateDetailTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateBucketAccessKeyRequestRequestTypeDef",
+    "TagTypeDef",
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
     "CreateGUISessionAccessDetailsRequestRequestTypeDef",
     "SessionTypeDef",
     "DiskMapTypeDef",
@@ -176,14 +186,15 @@
     "DetachInstancesFromLoadBalancerRequestRequestTypeDef",
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
+    "DomainEntryOutputTypeDef",
     "ResourceRecordTypeDef",
     "DownloadDefaultKeyPairResultTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetActiveNamesResultTypeDef",
@@ -265,15 +276,15 @@
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     "GetRelationalDatabaseLogStreamsResultTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
-    "RelationalDatabaseParameterTypeDef",
+    "RelationalDatabaseParameterOutputTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
@@ -298,14 +309,15 @@
     "PutAlarmRequestRequestTypeDef",
     "R53HostedZoneDeletionStateTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RebootRelationalDatabaseRequestRequestTypeDef",
     "RegisterContainerImageRequestRequestTypeDef",
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
+    "RelationalDatabaseParameterTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
     "StartGUISessionRequestRequestTypeDef",
@@ -329,45 +341,46 @@
     "StaticIpTypeDef",
     "AutoSnapshotDetailsTypeDef",
     "RegionTypeDef",
     "GetBlueprintsResultTypeDef",
     "UpdateBucketRequestRequestTypeDef",
     "GetBucketBundlesResultTypeDef",
     "BucketTypeDef",
-    "CreateBucketRequestRequestTypeDef",
-    "CreateCertificateRequestRequestTypeDef",
-    "CreateDiskSnapshotRequestRequestTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "CreateInstanceSnapshotRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateLoadBalancerRequestRequestTypeDef",
-    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
-    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    "CreateRelationalDatabaseRequestRequestTypeDef",
-    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "GetBundlesResultTypeDef",
+    "CacheSettingsOutputTypeDef",
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
     "GetContainerImagesResultTypeDef",
     "RegisterContainerImageResultTypeDef",
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
+    "CreateBucketRequestRequestTypeDef",
+    "CreateCertificateRequestRequestTypeDef",
+    "CreateDiskSnapshotRequestRequestTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "CreateInstanceSnapshotRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateLoadBalancerRequestRequestTypeDef",
+    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    "CreateRelationalDatabaseRequestRequestTypeDef",
+    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
@@ -383,22 +396,22 @@
     "GetInstanceStateResultTypeDef",
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     "GetRelationalDatabaseBundlesResultTypeDef",
     "GetRelationalDatabaseEventsResultTypeDef",
     "GetRelationalDatabaseLogEventsResultTypeDef",
     "GetRelationalDatabaseParametersResultTypeDef",
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "InstanceAccessDetailsTypeDef",
     "InstanceNetworkingTypeDef",
     "LoadBalancerTlsCertificateDomainValidationRecordTypeDef",
     "LoadBalancerTlsCertificateRenewalSummaryTypeDef",
     "LoadBalancerTypeDef",
     "RegisteredDomainDelegationInfoTypeDef",
     "RelationalDatabaseTypeDef",
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "GetBucketAccessKeysResultTypeDef",
     "CreateDiskFromSnapshotRequestRequestTypeDef",
     "CreateDiskRequestRequestTypeDef",
     "CreateInstancesFromSnapshotRequestRequestTypeDef",
     "CreateInstancesRequestRequestTypeDef",
     "EnableAddOnRequestRequestTypeDef",
     "GetAlarmsResultTypeDef",
@@ -500,16 +513,16 @@
     "InstanceHardwareTypeDef",
     "InstanceSnapshotTypeDef",
     "CreateKeyPairResultTypeDef",
     "GetKeyPairResultTypeDef",
     "GetKeyPairsResultTypeDef",
     "GetRelationalDatabaseSnapshotResultTypeDef",
     "GetRelationalDatabaseSnapshotsResultTypeDef",
-    "CreateDistributionRequestRequestTypeDef",
     "LightsailDistributionTypeDef",
+    "CreateDistributionRequestRequestTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
     "ExportSnapshotRecordSourceInfoTypeDef",
@@ -555,14 +568,23 @@
         "lastUsedDate": datetime,
         "region": str,
         "serviceName": str,
     },
     total=False,
 )
 
+AccessRulesOutputTypeDef = TypedDict(
+    "AccessRulesOutputTypeDef",
+    {
+        "getObject": AccessTypeType,
+        "allowPublicOverrides": bool,
+    },
+    total=False,
+)
+
 AccessRulesTypeDef = TypedDict(
     "AccessRulesTypeDef",
     {
         "getObject": AccessTypeType,
         "allowPublicOverrides": bool,
     },
     total=False,
@@ -724,14 +746,36 @@
         "licenseUrl": str,
         "platform": InstancePlatformType,
         "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
+_RequiredBucketAccessLogConfigOutputTypeDef = TypedDict(
+    "_RequiredBucketAccessLogConfigOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalBucketAccessLogConfigOutputTypeDef = TypedDict(
+    "_OptionalBucketAccessLogConfigOutputTypeDef",
+    {
+        "destination": str,
+        "prefix": str,
+    },
+    total=False,
+)
+
+
+class BucketAccessLogConfigOutputTypeDef(
+    _RequiredBucketAccessLogConfigOutputTypeDef, _OptionalBucketAccessLogConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredBucketAccessLogConfigTypeDef = TypedDict(
     "_RequiredBucketAccessLogConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalBucketAccessLogConfigTypeDef = TypedDict(
@@ -777,16 +821,16 @@
     {
         "name": str,
         "resourceType": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
@@ -805,14 +849,31 @@
         "transferPerMonthInGb": int,
         "supportedPlatforms": List[InstancePlatformType],
         "supportedAppCategories": List[Literal["LfR"]],
     },
     total=False,
 )
 
+CacheBehaviorOutputTypeDef = TypedDict(
+    "CacheBehaviorOutputTypeDef",
+    {
+        "behavior": BehaviorEnumType,
+    },
+    total=False,
+)
+
+CacheBehaviorPerPathOutputTypeDef = TypedDict(
+    "CacheBehaviorPerPathOutputTypeDef",
+    {
+        "path": str,
+        "behavior": BehaviorEnumType,
+    },
+    total=False,
+)
+
 CacheBehaviorPerPathTypeDef = TypedDict(
     "CacheBehaviorPerPathTypeDef",
     {
         "path": str,
         "behavior": BehaviorEnumType,
     },
     total=False,
@@ -822,14 +883,41 @@
     "CacheBehaviorTypeDef",
     {
         "behavior": BehaviorEnumType,
     },
     total=False,
 )
 
+CookieObjectOutputTypeDef = TypedDict(
+    "CookieObjectOutputTypeDef",
+    {
+        "option": ForwardValuesType,
+        "cookiesAllowList": List[str],
+    },
+    total=False,
+)
+
+HeaderObjectOutputTypeDef = TypedDict(
+    "HeaderObjectOutputTypeDef",
+    {
+        "option": ForwardValuesType,
+        "headersAllowList": List[HeaderEnumType],
+    },
+    total=False,
+)
+
+QueryStringObjectOutputTypeDef = TypedDict(
+    "QueryStringObjectOutputTypeDef",
+    {
+        "option": bool,
+        "queryStringsAllowList": List[str],
+    },
+    total=False,
+)
+
 CookieObjectTypeDef = TypedDict(
     "CookieObjectTypeDef",
     {
         "option": ForwardValuesType,
         "cookiesAllowList": Sequence[str],
     },
     total=False,
@@ -891,14 +979,25 @@
         "image": str,
         "digest": str,
         "createdAt": datetime,
     },
     total=False,
 )
 
+ContainerOutputTypeDef = TypedDict(
+    "ContainerOutputTypeDef",
+    {
+        "image": str,
+        "command": List[str],
+        "environment": Dict[str, str],
+        "ports": Dict[str, ContainerServiceProtocolType],
+    },
+    total=False,
+)
+
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "image": str,
         "command": Sequence[str],
         "environment": Mapping[str, str],
         "ports": Mapping[str, ContainerServiceProtocolType],
@@ -919,14 +1018,27 @@
     {
         "isActive": bool,
         "principalArn": str,
     },
     total=False,
 )
 
+ContainerServiceHealthCheckConfigOutputTypeDef = TypedDict(
+    "ContainerServiceHealthCheckConfigOutputTypeDef",
+    {
+        "healthyThreshold": int,
+        "unhealthyThreshold": int,
+        "timeoutSeconds": int,
+        "intervalSeconds": int,
+        "path": str,
+        "successCodes": str,
+    },
+    total=False,
+)
+
 ContainerServiceHealthCheckConfigTypeDef = TypedDict(
     "ContainerServiceHealthCheckConfigTypeDef",
     {
         "healthyThreshold": int,
         "unhealthyThreshold": int,
         "timeoutSeconds": int,
         "intervalSeconds": int,
@@ -1006,14 +1118,23 @@
 CreateBucketAccessKeyRequestRequestTypeDef = TypedDict(
     "CreateBucketAccessKeyRequestRequestTypeDef",
     {
         "bucketName": str,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 _RequiredInstanceEntryTypeDef = TypedDict(
     "_RequiredInstanceEntryTypeDef",
     {
         "sourceName": str,
         "instanceType": str,
         "portInfoSource": PortInfoSourceTypeType,
         "availabilityZone": str,
@@ -1394,14 +1515,27 @@
     {
         "code": DnsRecordCreationStateCodeType,
         "message": str,
     },
     total=False,
 )
 
+DomainEntryOutputTypeDef = TypedDict(
+    "DomainEntryOutputTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "target": str,
+        "isAlias": bool,
+        "type": str,
+        "options": Dict[str, str],
+    },
+    total=False,
+)
+
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "name": str,
         "type": str,
         "value": str,
     },
@@ -2317,16 +2451,16 @@
 class GetRelationalDatabaseParametersRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef,
 ):
     pass
 
 
-RelationalDatabaseParameterTypeDef = TypedDict(
-    "RelationalDatabaseParameterTypeDef",
+RelationalDatabaseParameterOutputTypeDef = TypedDict(
+    "RelationalDatabaseParameterOutputTypeDef",
     {
         "allowedValues": str,
         "applyMethod": str,
         "applyType": str,
         "dataType": str,
         "description": str,
         "isModifiable": bool,
@@ -2645,14 +2779,29 @@
         "cpuCount": int,
         "diskSizeInGb": int,
         "ramSizeInGb": float,
     },
     total=False,
 )
 
+RelationalDatabaseParameterTypeDef = TypedDict(
+    "RelationalDatabaseParameterTypeDef",
+    {
+        "allowedValues": str,
+        "applyMethod": str,
+        "applyType": str,
+        "dataType": str,
+        "description": str,
+        "isModifiable": bool,
+        "parameterName": str,
+        "parameterValue": str,
+    },
+    total=False,
+)
+
 ReleaseStaticIpRequestRequestTypeDef = TypedDict(
     "ReleaseStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
@@ -3057,33 +3206,282 @@
     },
 )
 
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "resourceType": str,
-        "accessRules": AccessRulesTypeDef,
+        "accessRules": AccessRulesOutputTypeDef,
         "arn": str,
         "bundleId": str,
         "createdAt": datetime,
         "url": str,
         "location": ResourceLocationTypeDef,
         "name": str,
         "supportCode": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "objectVersioning": str,
         "ableToUpdateBundle": bool,
         "readonlyAccessAccounts": List[str],
         "resourcesReceivingAccess": List[ResourceReceivingAccessTypeDef],
         "state": BucketStateTypeDef,
-        "accessLogConfig": BucketAccessLogConfigTypeDef,
+        "accessLogConfig": BucketAccessLogConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+DiskSnapshotTypeDef = TypedDict(
+    "DiskSnapshotTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "sizeInGb": int,
+        "state": DiskSnapshotStateType,
+        "progress": str,
+        "fromDiskName": str,
+        "fromDiskArn": str,
+        "fromInstanceName": str,
+        "fromInstanceArn": str,
+        "isFromAutoSnapshot": bool,
+    },
+    total=False,
+)
+
+DiskTypeDef = TypedDict(
+    "DiskTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "addOns": List[AddOnTypeDef],
+        "sizeInGb": int,
+        "isSystemDisk": bool,
+        "iops": int,
+        "path": str,
+        "state": DiskStateType,
+        "attachedTo": str,
+        "isAttached": bool,
+        "attachmentState": str,
+        "gbInUse": int,
+        "autoMountStatus": AutoMountStatusType,
+    },
+    total=False,
+)
+
+KeyPairTypeDef = TypedDict(
+    "KeyPairTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "fingerprint": str,
+    },
+    total=False,
+)
+
+RelationalDatabaseSnapshotTypeDef = TypedDict(
+    "RelationalDatabaseSnapshotTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "engine": str,
+        "engineVersion": str,
+        "sizeInGb": int,
+        "state": str,
+        "fromRelationalDatabaseName": str,
+        "fromRelationalDatabaseArn": str,
+        "fromRelationalDatabaseBundleId": str,
+        "fromRelationalDatabaseBlueprintId": str,
+    },
+    total=False,
+)
+
+GetBundlesResultTypeDef = TypedDict(
+    "GetBundlesResultTypeDef",
+    {
+        "bundles": List[BundleTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CacheSettingsOutputTypeDef = TypedDict(
+    "CacheSettingsOutputTypeDef",
+    {
+        "defaultTTL": int,
+        "minimumTTL": int,
+        "maximumTTL": int,
+        "allowedHTTPMethods": str,
+        "cachedHTTPMethods": str,
+        "forwardedCookies": CookieObjectOutputTypeDef,
+        "forwardedHeaders": HeaderObjectOutputTypeDef,
+        "forwardedQueryStrings": QueryStringObjectOutputTypeDef,
+    },
+    total=False,
+)
+
+CacheSettingsTypeDef = TypedDict(
+    "CacheSettingsTypeDef",
+    {
+        "defaultTTL": int,
+        "minimumTTL": int,
+        "maximumTTL": int,
+        "allowedHTTPMethods": str,
+        "cachedHTTPMethods": str,
+        "forwardedCookies": CookieObjectTypeDef,
+        "forwardedHeaders": HeaderObjectTypeDef,
+        "forwardedQueryStrings": QueryStringObjectTypeDef,
+    },
+    total=False,
+)
+
+CloseInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "CloseInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfo": PortInfoTypeDef,
+        "instanceName": str,
+    },
+)
+
+OpenInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "OpenInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfo": PortInfoTypeDef,
+        "instanceName": str,
+    },
+)
+
+PutInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "PutInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfos": Sequence[PortInfoTypeDef],
+        "instanceName": str,
+    },
+)
+
+CloudFormationStackRecordTypeDef = TypedDict(
+    "CloudFormationStackRecordTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "state": RecordStateType,
+        "sourceInfo": List[CloudFormationStackRecordSourceInfoTypeDef],
+        "destinationInfo": DestinationInfoTypeDef,
+    },
+    total=False,
+)
+
+GetContainerImagesResultTypeDef = TypedDict(
+    "GetContainerImagesResultTypeDef",
+    {
+        "containerImages": List[ContainerImageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterContainerImageResultTypeDef = TypedDict(
+    "RegisterContainerImageResultTypeDef",
+    {
+        "containerImage": ContainerImageTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PrivateRegistryAccessRequestTypeDef = TypedDict(
+    "PrivateRegistryAccessRequestTypeDef",
+    {
+        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
+    },
+    total=False,
+)
+
+PrivateRegistryAccessTypeDef = TypedDict(
+    "PrivateRegistryAccessTypeDef",
+    {
+        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleTypeDef,
+    },
+    total=False,
+)
+
+ContainerServiceEndpointTypeDef = TypedDict(
+    "ContainerServiceEndpointTypeDef",
+    {
+        "containerName": str,
+        "containerPort": int,
+        "healthCheck": ContainerServiceHealthCheckConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredEndpointRequestTypeDef = TypedDict(
+    "_RequiredEndpointRequestTypeDef",
+    {
+        "containerName": str,
+        "containerPort": int,
+    },
+)
+_OptionalEndpointRequestTypeDef = TypedDict(
+    "_OptionalEndpointRequestTypeDef",
+    {
+        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
     },
     total=False,
 )
 
+
+class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
+    pass
+
+
+GetContainerLogResultTypeDef = TypedDict(
+    "GetContainerLogResultTypeDef",
+    {
+        "logEvents": List[ContainerServiceLogEventTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetContainerServicePowersResultTypeDef = TypedDict(
+    "GetContainerServicePowersResultTypeDef",
+    {
+        "powers": List[ContainerServicePowerTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
+    "CreateContainerServiceRegistryLoginResultTypeDef",
+    {
+        "registryLogin": ContainerServiceRegistryLoginTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBucketRequestRequestTypeDef",
     {
         "bucketName": str,
         "bundleId": str,
     },
 )
@@ -3348,98 +3746,14 @@
 class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
 ):
     pass
 
 
-DiskSnapshotTypeDef = TypedDict(
-    "DiskSnapshotTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "sizeInGb": int,
-        "state": DiskSnapshotStateType,
-        "progress": str,
-        "fromDiskName": str,
-        "fromDiskArn": str,
-        "fromInstanceName": str,
-        "fromInstanceArn": str,
-        "isFromAutoSnapshot": bool,
-    },
-    total=False,
-)
-
-DiskTypeDef = TypedDict(
-    "DiskTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "addOns": List[AddOnTypeDef],
-        "sizeInGb": int,
-        "isSystemDisk": bool,
-        "iops": int,
-        "path": str,
-        "state": DiskStateType,
-        "attachedTo": str,
-        "isAttached": bool,
-        "attachmentState": str,
-        "gbInUse": int,
-        "autoMountStatus": AutoMountStatusType,
-    },
-    total=False,
-)
-
-KeyPairTypeDef = TypedDict(
-    "KeyPairTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "fingerprint": str,
-    },
-    total=False,
-)
-
-RelationalDatabaseSnapshotTypeDef = TypedDict(
-    "RelationalDatabaseSnapshotTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "engine": str,
-        "engineVersion": str,
-        "sizeInGb": int,
-        "state": str,
-        "fromRelationalDatabaseName": str,
-        "fromRelationalDatabaseArn": str,
-        "fromRelationalDatabaseBundleId": str,
-        "fromRelationalDatabaseBlueprintId": str,
-    },
-    total=False,
-)
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceName": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -3454,164 +3768,14 @@
 
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
 
-GetBundlesResultTypeDef = TypedDict(
-    "GetBundlesResultTypeDef",
-    {
-        "bundles": List[BundleTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CacheSettingsTypeDef = TypedDict(
-    "CacheSettingsTypeDef",
-    {
-        "defaultTTL": int,
-        "minimumTTL": int,
-        "maximumTTL": int,
-        "allowedHTTPMethods": str,
-        "cachedHTTPMethods": str,
-        "forwardedCookies": CookieObjectTypeDef,
-        "forwardedHeaders": HeaderObjectTypeDef,
-        "forwardedQueryStrings": QueryStringObjectTypeDef,
-    },
-    total=False,
-)
-
-CloseInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "CloseInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfo": PortInfoTypeDef,
-        "instanceName": str,
-    },
-)
-
-OpenInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "OpenInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfo": PortInfoTypeDef,
-        "instanceName": str,
-    },
-)
-
-PutInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "PutInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfos": Sequence[PortInfoTypeDef],
-        "instanceName": str,
-    },
-)
-
-CloudFormationStackRecordTypeDef = TypedDict(
-    "CloudFormationStackRecordTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "state": RecordStateType,
-        "sourceInfo": List[CloudFormationStackRecordSourceInfoTypeDef],
-        "destinationInfo": DestinationInfoTypeDef,
-    },
-    total=False,
-)
-
-GetContainerImagesResultTypeDef = TypedDict(
-    "GetContainerImagesResultTypeDef",
-    {
-        "containerImages": List[ContainerImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterContainerImageResultTypeDef = TypedDict(
-    "RegisterContainerImageResultTypeDef",
-    {
-        "containerImage": ContainerImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PrivateRegistryAccessRequestTypeDef = TypedDict(
-    "PrivateRegistryAccessRequestTypeDef",
-    {
-        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
-    },
-    total=False,
-)
-
-PrivateRegistryAccessTypeDef = TypedDict(
-    "PrivateRegistryAccessTypeDef",
-    {
-        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleTypeDef,
-    },
-    total=False,
-)
-
-ContainerServiceEndpointTypeDef = TypedDict(
-    "ContainerServiceEndpointTypeDef",
-    {
-        "containerName": str,
-        "containerPort": int,
-        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredEndpointRequestTypeDef = TypedDict(
-    "_RequiredEndpointRequestTypeDef",
-    {
-        "containerName": str,
-        "containerPort": int,
-    },
-)
-_OptionalEndpointRequestTypeDef = TypedDict(
-    "_OptionalEndpointRequestTypeDef",
-    {
-        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
-    pass
-
-
-GetContainerLogResultTypeDef = TypedDict(
-    "GetContainerLogResultTypeDef",
-    {
-        "logEvents": List[ContainerServiceLogEventTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetContainerServicePowersResultTypeDef = TypedDict(
-    "GetContainerServicePowersResultTypeDef",
-    {
-        "powers": List[ContainerServicePowerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
-    "CreateContainerServiceRegistryLoginResultTypeDef",
-    {
-        "registryLogin": ContainerServiceRegistryLoginTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateCloudFormationStackRequestRequestTypeDef = TypedDict(
     "CreateCloudFormationStackRequestRequestTypeDef",
     {
         "instances": Sequence[InstanceEntryTypeDef],
     },
 )
 
@@ -3807,28 +3971,20 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseParametersResultTypeDef = TypedDict(
     "GetRelationalDatabaseParametersResultTypeDef",
     {
-        "parameters": List[RelationalDatabaseParameterTypeDef],
+        "parameters": List[RelationalDatabaseParameterOutputTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
-    },
-)
-
 InstanceAccessDetailsTypeDef = TypedDict(
     "InstanceAccessDetailsTypeDef",
     {
         "certKey": str,
         "expiresAt": datetime,
         "ipAddress": str,
         "password": str,
@@ -3878,15 +4034,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "dnsName": str,
         "state": LoadBalancerStateType,
         "protocol": LoadBalancerProtocolType,
         "publicPorts": List[int],
         "healthCheckPath": str,
         "instancePort": int,
         "instanceHealthSummary": List[InstanceHealthSummaryTypeDef],
@@ -3913,15 +4069,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
         "hardware": RelationalDatabaseHardwareTypeDef,
         "state": str,
         "secondaryAvailabilityZone": str,
         "backupRetentionEnabled": bool,
@@ -3937,14 +4093,22 @@
         "masterEndpoint": RelationalDatabaseEndpointTypeDef,
         "pendingMaintenanceActions": List[PendingMaintenanceActionTypeDef],
         "caCertificateIdentifier": str,
     },
     total=False,
 )
 
+UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
+    },
+)
+
 GetBucketAccessKeysResultTypeDef = TypedDict(
     "GetBucketAccessKeysResultTypeDef",
     {
         "accessKeys": List[AccessKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4871,15 +5035,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "state": InstanceSnapshotStateType,
         "progress": str,
         "fromAttachedDisks": List[DiskTypeDef],
         "fromInstanceName": str,
         "fromInstanceArn": str,
         "fromBlueprintId": str,
         "fromBundleId": str,
@@ -4930,14 +5094,41 @@
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LightsailDistributionTypeDef = TypedDict(
+    "LightsailDistributionTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "alternativeDomainNames": List[str],
+        "status": str,
+        "isEnabled": bool,
+        "domainName": str,
+        "bundleId": str,
+        "certificateName": str,
+        "origin": OriginTypeDef,
+        "originPublicDNS": str,
+        "defaultCacheBehavior": CacheBehaviorOutputTypeDef,
+        "cacheBehaviorSettings": CacheSettingsOutputTypeDef,
+        "cacheBehaviors": List[CacheBehaviorPerPathOutputTypeDef],
+        "ableToUpdateBundle": bool,
+        "ipAddressType": IpAddressTypeType,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
@@ -4958,41 +5149,14 @@
 class CreateDistributionRequestRequestTypeDef(
     _RequiredCreateDistributionRequestRequestTypeDef,
     _OptionalCreateDistributionRequestRequestTypeDef,
 ):
     pass
 
 
-LightsailDistributionTypeDef = TypedDict(
-    "LightsailDistributionTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "alternativeDomainNames": List[str],
-        "status": str,
-        "isEnabled": bool,
-        "domainName": str,
-        "bundleId": str,
-        "certificateName": str,
-        "origin": OriginTypeDef,
-        "originPublicDNS": str,
-        "defaultCacheBehavior": CacheBehaviorTypeDef,
-        "cacheBehaviorSettings": CacheSettingsTypeDef,
-        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
-        "ableToUpdateBundle": bool,
-        "ipAddressType": IpAddressTypeType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
     },
 )
 _OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
@@ -5051,15 +5215,15 @@
 
 
 ContainerServiceDeploymentTypeDef = TypedDict(
     "ContainerServiceDeploymentTypeDef",
     {
         "version": int,
         "state": ContainerServiceDeploymentStateType,
-        "containers": Dict[str, ContainerTypeDef],
+        "containers": Dict[str, ContainerOutputTypeDef],
         "publicEndpoint": ContainerServiceEndpointTypeDef,
         "createdAt": datetime,
     },
     total=False,
 )
 
 ContainerServiceDeploymentRequestTypeDef = TypedDict(
@@ -5142,15 +5306,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "loadBalancerName": str,
         "isAttached": bool,
         "status": LoadBalancerTlsCertificateStatusType,
         "domainName": str,
         "domainValidationRecords": List[LoadBalancerTlsCertificateDomainValidationRecordTypeDef],
         "failureReason": LoadBalancerTlsCertificateFailureReasonType,
         "issuedAt": datetime,
@@ -5191,16 +5355,16 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "domainEntries": List[DomainEntryTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "domainEntries": List[DomainEntryOutputTypeDef],
         "registeredDomainDelegationInfo": RegisteredDomainDelegationInfoTypeDef,
     },
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
@@ -5224,15 +5388,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "blueprintId": str,
         "blueprintName": str,
         "bundleId": str,
         "addOns": List[AddOnTypeDef],
         "isStaticIp": bool,
         "privateIpAddress": str,
         "publicIpAddress": str,
@@ -5287,15 +5451,15 @@
     "ContainerServiceTypeDef",
     {
         "containerServiceName": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "power": ContainerServicePowerNameType,
         "powerId": str,
         "state": ContainerServiceStateType,
         "stateDetail": ContainerServiceStateDetailTypeDef,
         "scale": int,
         "currentDeployment": ContainerServiceDeploymentTypeDef,
         "nextDeployment": ContainerServiceDeploymentTypeDef,
@@ -5377,15 +5541,15 @@
         "issuerCA": str,
         "notBefore": datetime,
         "notAfter": datetime,
         "eligibleToRenew": str,
         "renewalSummary": RenewalSummaryTypeDef,
         "revokedAt": datetime,
         "revocationReason": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "supportCode": str,
     },
     total=False,
 )
 
 ResourceBudgetEstimateTypeDef = TypedDict(
     "ResourceBudgetEstimateTypeDef",
@@ -5485,15 +5649,15 @@
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "certificateArn": str,
         "certificateName": str,
         "domainName": str,
         "certificateDetail": CertificateTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 GetCostEstimateResultTypeDef = TypedDict(
     "GetCostEstimateResultTypeDef",
     {
```

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail/type_defs.pyi` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessKeyLastUsedTypeDef",
+    "AccessRulesOutputTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
     "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
@@ -114,39 +115,48 @@
     "AttachDiskRequestRequestTypeDef",
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     "AttachLoadBalancerTlsCertificateRequestRequestTypeDef",
     "AttachStaticIpRequestRequestTypeDef",
     "AttachedDiskTypeDef",
     "AvailabilityZoneTypeDef",
     "BlueprintTypeDef",
+    "BucketAccessLogConfigOutputTypeDef",
     "BucketAccessLogConfigTypeDef",
     "BucketBundleTypeDef",
     "BucketStateTypeDef",
     "ResourceReceivingAccessTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "BundleTypeDef",
+    "CacheBehaviorOutputTypeDef",
+    "CacheBehaviorPerPathOutputTypeDef",
     "CacheBehaviorPerPathTypeDef",
     "CacheBehaviorTypeDef",
+    "CookieObjectOutputTypeDef",
+    "HeaderObjectOutputTypeDef",
+    "QueryStringObjectOutputTypeDef",
     "CookieObjectTypeDef",
     "HeaderObjectTypeDef",
     "QueryStringObjectTypeDef",
     "PortInfoTypeDef",
     "CloudFormationStackRecordSourceInfoTypeDef",
     "DestinationInfoTypeDef",
     "ContainerImageTypeDef",
+    "ContainerOutputTypeDef",
     "ContainerTypeDef",
     "ContainerServiceECRImagePullerRoleRequestTypeDef",
     "ContainerServiceECRImagePullerRoleTypeDef",
+    "ContainerServiceHealthCheckConfigOutputTypeDef",
     "ContainerServiceHealthCheckConfigTypeDef",
     "ContainerServiceLogEventTypeDef",
     "ContainerServicePowerTypeDef",
     "ContainerServiceRegistryLoginTypeDef",
     "ContainerServiceStateDetailTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateBucketAccessKeyRequestRequestTypeDef",
+    "TagTypeDef",
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
     "CreateGUISessionAccessDetailsRequestRequestTypeDef",
     "SessionTypeDef",
     "DiskMapTypeDef",
@@ -175,14 +185,15 @@
     "DetachInstancesFromLoadBalancerRequestRequestTypeDef",
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
+    "DomainEntryOutputTypeDef",
     "ResourceRecordTypeDef",
     "DownloadDefaultKeyPairResultTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetActiveNamesResultTypeDef",
@@ -264,15 +275,15 @@
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     "GetRelationalDatabaseLogStreamsResultTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
-    "RelationalDatabaseParameterTypeDef",
+    "RelationalDatabaseParameterOutputTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
@@ -297,14 +308,15 @@
     "PutAlarmRequestRequestTypeDef",
     "R53HostedZoneDeletionStateTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RebootRelationalDatabaseRequestRequestTypeDef",
     "RegisterContainerImageRequestRequestTypeDef",
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
+    "RelationalDatabaseParameterTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
     "StartGUISessionRequestRequestTypeDef",
@@ -328,45 +340,46 @@
     "StaticIpTypeDef",
     "AutoSnapshotDetailsTypeDef",
     "RegionTypeDef",
     "GetBlueprintsResultTypeDef",
     "UpdateBucketRequestRequestTypeDef",
     "GetBucketBundlesResultTypeDef",
     "BucketTypeDef",
-    "CreateBucketRequestRequestTypeDef",
-    "CreateCertificateRequestRequestTypeDef",
-    "CreateDiskSnapshotRequestRequestTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "CreateInstanceSnapshotRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateLoadBalancerRequestRequestTypeDef",
-    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
-    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    "CreateRelationalDatabaseRequestRequestTypeDef",
-    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "GetBundlesResultTypeDef",
+    "CacheSettingsOutputTypeDef",
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
     "GetContainerImagesResultTypeDef",
     "RegisterContainerImageResultTypeDef",
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
+    "CreateBucketRequestRequestTypeDef",
+    "CreateCertificateRequestRequestTypeDef",
+    "CreateDiskSnapshotRequestRequestTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "CreateInstanceSnapshotRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateLoadBalancerRequestRequestTypeDef",
+    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    "CreateRelationalDatabaseRequestRequestTypeDef",
+    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
@@ -382,22 +395,22 @@
     "GetInstanceStateResultTypeDef",
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     "GetRelationalDatabaseBundlesResultTypeDef",
     "GetRelationalDatabaseEventsResultTypeDef",
     "GetRelationalDatabaseLogEventsResultTypeDef",
     "GetRelationalDatabaseParametersResultTypeDef",
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "InstanceAccessDetailsTypeDef",
     "InstanceNetworkingTypeDef",
     "LoadBalancerTlsCertificateDomainValidationRecordTypeDef",
     "LoadBalancerTlsCertificateRenewalSummaryTypeDef",
     "LoadBalancerTypeDef",
     "RegisteredDomainDelegationInfoTypeDef",
     "RelationalDatabaseTypeDef",
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "GetBucketAccessKeysResultTypeDef",
     "CreateDiskFromSnapshotRequestRequestTypeDef",
     "CreateDiskRequestRequestTypeDef",
     "CreateInstancesFromSnapshotRequestRequestTypeDef",
     "CreateInstancesRequestRequestTypeDef",
     "EnableAddOnRequestRequestTypeDef",
     "GetAlarmsResultTypeDef",
@@ -499,16 +512,16 @@
     "InstanceHardwareTypeDef",
     "InstanceSnapshotTypeDef",
     "CreateKeyPairResultTypeDef",
     "GetKeyPairResultTypeDef",
     "GetKeyPairsResultTypeDef",
     "GetRelationalDatabaseSnapshotResultTypeDef",
     "GetRelationalDatabaseSnapshotsResultTypeDef",
-    "CreateDistributionRequestRequestTypeDef",
     "LightsailDistributionTypeDef",
+    "CreateDistributionRequestRequestTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
     "ExportSnapshotRecordSourceInfoTypeDef",
@@ -554,14 +567,23 @@
         "lastUsedDate": datetime,
         "region": str,
         "serviceName": str,
     },
     total=False,
 )
 
+AccessRulesOutputTypeDef = TypedDict(
+    "AccessRulesOutputTypeDef",
+    {
+        "getObject": AccessTypeType,
+        "allowPublicOverrides": bool,
+    },
+    total=False,
+)
+
 AccessRulesTypeDef = TypedDict(
     "AccessRulesTypeDef",
     {
         "getObject": AccessTypeType,
         "allowPublicOverrides": bool,
     },
     total=False,
@@ -721,14 +743,34 @@
         "licenseUrl": str,
         "platform": InstancePlatformType,
         "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
+_RequiredBucketAccessLogConfigOutputTypeDef = TypedDict(
+    "_RequiredBucketAccessLogConfigOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalBucketAccessLogConfigOutputTypeDef = TypedDict(
+    "_OptionalBucketAccessLogConfigOutputTypeDef",
+    {
+        "destination": str,
+        "prefix": str,
+    },
+    total=False,
+)
+
+class BucketAccessLogConfigOutputTypeDef(
+    _RequiredBucketAccessLogConfigOutputTypeDef, _OptionalBucketAccessLogConfigOutputTypeDef
+):
+    pass
+
 _RequiredBucketAccessLogConfigTypeDef = TypedDict(
     "_RequiredBucketAccessLogConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalBucketAccessLogConfigTypeDef = TypedDict(
@@ -772,16 +814,16 @@
     {
         "name": str,
         "resourceType": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
@@ -800,14 +842,31 @@
         "transferPerMonthInGb": int,
         "supportedPlatforms": List[InstancePlatformType],
         "supportedAppCategories": List[Literal["LfR"]],
     },
     total=False,
 )
 
+CacheBehaviorOutputTypeDef = TypedDict(
+    "CacheBehaviorOutputTypeDef",
+    {
+        "behavior": BehaviorEnumType,
+    },
+    total=False,
+)
+
+CacheBehaviorPerPathOutputTypeDef = TypedDict(
+    "CacheBehaviorPerPathOutputTypeDef",
+    {
+        "path": str,
+        "behavior": BehaviorEnumType,
+    },
+    total=False,
+)
+
 CacheBehaviorPerPathTypeDef = TypedDict(
     "CacheBehaviorPerPathTypeDef",
     {
         "path": str,
         "behavior": BehaviorEnumType,
     },
     total=False,
@@ -817,14 +876,41 @@
     "CacheBehaviorTypeDef",
     {
         "behavior": BehaviorEnumType,
     },
     total=False,
 )
 
+CookieObjectOutputTypeDef = TypedDict(
+    "CookieObjectOutputTypeDef",
+    {
+        "option": ForwardValuesType,
+        "cookiesAllowList": List[str],
+    },
+    total=False,
+)
+
+HeaderObjectOutputTypeDef = TypedDict(
+    "HeaderObjectOutputTypeDef",
+    {
+        "option": ForwardValuesType,
+        "headersAllowList": List[HeaderEnumType],
+    },
+    total=False,
+)
+
+QueryStringObjectOutputTypeDef = TypedDict(
+    "QueryStringObjectOutputTypeDef",
+    {
+        "option": bool,
+        "queryStringsAllowList": List[str],
+    },
+    total=False,
+)
+
 CookieObjectTypeDef = TypedDict(
     "CookieObjectTypeDef",
     {
         "option": ForwardValuesType,
         "cookiesAllowList": Sequence[str],
     },
     total=False,
@@ -886,14 +972,25 @@
         "image": str,
         "digest": str,
         "createdAt": datetime,
     },
     total=False,
 )
 
+ContainerOutputTypeDef = TypedDict(
+    "ContainerOutputTypeDef",
+    {
+        "image": str,
+        "command": List[str],
+        "environment": Dict[str, str],
+        "ports": Dict[str, ContainerServiceProtocolType],
+    },
+    total=False,
+)
+
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "image": str,
         "command": Sequence[str],
         "environment": Mapping[str, str],
         "ports": Mapping[str, ContainerServiceProtocolType],
@@ -914,14 +1011,27 @@
     {
         "isActive": bool,
         "principalArn": str,
     },
     total=False,
 )
 
+ContainerServiceHealthCheckConfigOutputTypeDef = TypedDict(
+    "ContainerServiceHealthCheckConfigOutputTypeDef",
+    {
+        "healthyThreshold": int,
+        "unhealthyThreshold": int,
+        "timeoutSeconds": int,
+        "intervalSeconds": int,
+        "path": str,
+        "successCodes": str,
+    },
+    total=False,
+)
+
 ContainerServiceHealthCheckConfigTypeDef = TypedDict(
     "ContainerServiceHealthCheckConfigTypeDef",
     {
         "healthyThreshold": int,
         "unhealthyThreshold": int,
         "timeoutSeconds": int,
         "intervalSeconds": int,
@@ -999,14 +1109,23 @@
 CreateBucketAccessKeyRequestRequestTypeDef = TypedDict(
     "CreateBucketAccessKeyRequestRequestTypeDef",
     {
         "bucketName": str,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 _RequiredInstanceEntryTypeDef = TypedDict(
     "_RequiredInstanceEntryTypeDef",
     {
         "sourceName": str,
         "instanceType": str,
         "portInfoSource": PortInfoSourceTypeType,
         "availabilityZone": str,
@@ -1373,14 +1492,27 @@
     {
         "code": DnsRecordCreationStateCodeType,
         "message": str,
     },
     total=False,
 )
 
+DomainEntryOutputTypeDef = TypedDict(
+    "DomainEntryOutputTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "target": str,
+        "isAlias": bool,
+        "type": str,
+        "options": Dict[str, str],
+    },
+    total=False,
+)
+
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "name": str,
         "type": str,
         "value": str,
     },
@@ -2278,16 +2410,16 @@
 
 class GetRelationalDatabaseParametersRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef,
 ):
     pass
 
-RelationalDatabaseParameterTypeDef = TypedDict(
-    "RelationalDatabaseParameterTypeDef",
+RelationalDatabaseParameterOutputTypeDef = TypedDict(
+    "RelationalDatabaseParameterOutputTypeDef",
     {
         "allowedValues": str,
         "applyMethod": str,
         "applyType": str,
         "dataType": str,
         "description": str,
         "isModifiable": bool,
@@ -2604,14 +2736,29 @@
         "cpuCount": int,
         "diskSizeInGb": int,
         "ramSizeInGb": float,
     },
     total=False,
 )
 
+RelationalDatabaseParameterTypeDef = TypedDict(
+    "RelationalDatabaseParameterTypeDef",
+    {
+        "allowedValues": str,
+        "applyMethod": str,
+        "applyType": str,
+        "dataType": str,
+        "description": str,
+        "isModifiable": bool,
+        "parameterName": str,
+        "parameterValue": str,
+    },
+    total=False,
+)
+
 ReleaseStaticIpRequestRequestTypeDef = TypedDict(
     "ReleaseStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
@@ -3002,33 +3149,280 @@
     },
 )
 
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "resourceType": str,
-        "accessRules": AccessRulesTypeDef,
+        "accessRules": AccessRulesOutputTypeDef,
         "arn": str,
         "bundleId": str,
         "createdAt": datetime,
         "url": str,
         "location": ResourceLocationTypeDef,
         "name": str,
         "supportCode": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "objectVersioning": str,
         "ableToUpdateBundle": bool,
         "readonlyAccessAccounts": List[str],
         "resourcesReceivingAccess": List[ResourceReceivingAccessTypeDef],
         "state": BucketStateTypeDef,
-        "accessLogConfig": BucketAccessLogConfigTypeDef,
+        "accessLogConfig": BucketAccessLogConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+DiskSnapshotTypeDef = TypedDict(
+    "DiskSnapshotTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "sizeInGb": int,
+        "state": DiskSnapshotStateType,
+        "progress": str,
+        "fromDiskName": str,
+        "fromDiskArn": str,
+        "fromInstanceName": str,
+        "fromInstanceArn": str,
+        "isFromAutoSnapshot": bool,
+    },
+    total=False,
+)
+
+DiskTypeDef = TypedDict(
+    "DiskTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "addOns": List[AddOnTypeDef],
+        "sizeInGb": int,
+        "isSystemDisk": bool,
+        "iops": int,
+        "path": str,
+        "state": DiskStateType,
+        "attachedTo": str,
+        "isAttached": bool,
+        "attachmentState": str,
+        "gbInUse": int,
+        "autoMountStatus": AutoMountStatusType,
+    },
+    total=False,
+)
+
+KeyPairTypeDef = TypedDict(
+    "KeyPairTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "fingerprint": str,
+    },
+    total=False,
+)
+
+RelationalDatabaseSnapshotTypeDef = TypedDict(
+    "RelationalDatabaseSnapshotTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagOutputTypeDef],
+        "engine": str,
+        "engineVersion": str,
+        "sizeInGb": int,
+        "state": str,
+        "fromRelationalDatabaseName": str,
+        "fromRelationalDatabaseArn": str,
+        "fromRelationalDatabaseBundleId": str,
+        "fromRelationalDatabaseBlueprintId": str,
+    },
+    total=False,
+)
+
+GetBundlesResultTypeDef = TypedDict(
+    "GetBundlesResultTypeDef",
+    {
+        "bundles": List[BundleTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CacheSettingsOutputTypeDef = TypedDict(
+    "CacheSettingsOutputTypeDef",
+    {
+        "defaultTTL": int,
+        "minimumTTL": int,
+        "maximumTTL": int,
+        "allowedHTTPMethods": str,
+        "cachedHTTPMethods": str,
+        "forwardedCookies": CookieObjectOutputTypeDef,
+        "forwardedHeaders": HeaderObjectOutputTypeDef,
+        "forwardedQueryStrings": QueryStringObjectOutputTypeDef,
+    },
+    total=False,
+)
+
+CacheSettingsTypeDef = TypedDict(
+    "CacheSettingsTypeDef",
+    {
+        "defaultTTL": int,
+        "minimumTTL": int,
+        "maximumTTL": int,
+        "allowedHTTPMethods": str,
+        "cachedHTTPMethods": str,
+        "forwardedCookies": CookieObjectTypeDef,
+        "forwardedHeaders": HeaderObjectTypeDef,
+        "forwardedQueryStrings": QueryStringObjectTypeDef,
+    },
+    total=False,
+)
+
+CloseInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "CloseInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfo": PortInfoTypeDef,
+        "instanceName": str,
+    },
+)
+
+OpenInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "OpenInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfo": PortInfoTypeDef,
+        "instanceName": str,
+    },
+)
+
+PutInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "PutInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfos": Sequence[PortInfoTypeDef],
+        "instanceName": str,
+    },
+)
+
+CloudFormationStackRecordTypeDef = TypedDict(
+    "CloudFormationStackRecordTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "state": RecordStateType,
+        "sourceInfo": List[CloudFormationStackRecordSourceInfoTypeDef],
+        "destinationInfo": DestinationInfoTypeDef,
+    },
+    total=False,
+)
+
+GetContainerImagesResultTypeDef = TypedDict(
+    "GetContainerImagesResultTypeDef",
+    {
+        "containerImages": List[ContainerImageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterContainerImageResultTypeDef = TypedDict(
+    "RegisterContainerImageResultTypeDef",
+    {
+        "containerImage": ContainerImageTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PrivateRegistryAccessRequestTypeDef = TypedDict(
+    "PrivateRegistryAccessRequestTypeDef",
+    {
+        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
+    },
+    total=False,
+)
+
+PrivateRegistryAccessTypeDef = TypedDict(
+    "PrivateRegistryAccessTypeDef",
+    {
+        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleTypeDef,
+    },
+    total=False,
+)
+
+ContainerServiceEndpointTypeDef = TypedDict(
+    "ContainerServiceEndpointTypeDef",
+    {
+        "containerName": str,
+        "containerPort": int,
+        "healthCheck": ContainerServiceHealthCheckConfigOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredEndpointRequestTypeDef = TypedDict(
+    "_RequiredEndpointRequestTypeDef",
+    {
+        "containerName": str,
+        "containerPort": int,
+    },
+)
+_OptionalEndpointRequestTypeDef = TypedDict(
+    "_OptionalEndpointRequestTypeDef",
+    {
+        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
+    },
+    total=False,
+)
+
+class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
+    pass
+
+GetContainerLogResultTypeDef = TypedDict(
+    "GetContainerLogResultTypeDef",
+    {
+        "logEvents": List[ContainerServiceLogEventTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetContainerServicePowersResultTypeDef = TypedDict(
+    "GetContainerServicePowersResultTypeDef",
+    {
+        "powers": List[ContainerServicePowerTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
+    "CreateContainerServiceRegistryLoginResultTypeDef",
+    {
+        "registryLogin": ContainerServiceRegistryLoginTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBucketRequestRequestTypeDef",
     {
         "bucketName": str,
         "bundleId": str,
     },
 )
@@ -3271,98 +3665,14 @@
 
 class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
 ):
     pass
 
-DiskSnapshotTypeDef = TypedDict(
-    "DiskSnapshotTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "sizeInGb": int,
-        "state": DiskSnapshotStateType,
-        "progress": str,
-        "fromDiskName": str,
-        "fromDiskArn": str,
-        "fromInstanceName": str,
-        "fromInstanceArn": str,
-        "isFromAutoSnapshot": bool,
-    },
-    total=False,
-)
-
-DiskTypeDef = TypedDict(
-    "DiskTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "addOns": List[AddOnTypeDef],
-        "sizeInGb": int,
-        "isSystemDisk": bool,
-        "iops": int,
-        "path": str,
-        "state": DiskStateType,
-        "attachedTo": str,
-        "isAttached": bool,
-        "attachmentState": str,
-        "gbInUse": int,
-        "autoMountStatus": AutoMountStatusType,
-    },
-    total=False,
-)
-
-KeyPairTypeDef = TypedDict(
-    "KeyPairTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "fingerprint": str,
-    },
-    total=False,
-)
-
-RelationalDatabaseSnapshotTypeDef = TypedDict(
-    "RelationalDatabaseSnapshotTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "engine": str,
-        "engineVersion": str,
-        "sizeInGb": int,
-        "state": str,
-        "fromRelationalDatabaseName": str,
-        "fromRelationalDatabaseArn": str,
-        "fromRelationalDatabaseBundleId": str,
-        "fromRelationalDatabaseBlueprintId": str,
-    },
-    total=False,
-)
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceName": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -3375,162 +3685,14 @@
 )
 
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-GetBundlesResultTypeDef = TypedDict(
-    "GetBundlesResultTypeDef",
-    {
-        "bundles": List[BundleTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CacheSettingsTypeDef = TypedDict(
-    "CacheSettingsTypeDef",
-    {
-        "defaultTTL": int,
-        "minimumTTL": int,
-        "maximumTTL": int,
-        "allowedHTTPMethods": str,
-        "cachedHTTPMethods": str,
-        "forwardedCookies": CookieObjectTypeDef,
-        "forwardedHeaders": HeaderObjectTypeDef,
-        "forwardedQueryStrings": QueryStringObjectTypeDef,
-    },
-    total=False,
-)
-
-CloseInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "CloseInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfo": PortInfoTypeDef,
-        "instanceName": str,
-    },
-)
-
-OpenInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "OpenInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfo": PortInfoTypeDef,
-        "instanceName": str,
-    },
-)
-
-PutInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "PutInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfos": Sequence[PortInfoTypeDef],
-        "instanceName": str,
-    },
-)
-
-CloudFormationStackRecordTypeDef = TypedDict(
-    "CloudFormationStackRecordTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "state": RecordStateType,
-        "sourceInfo": List[CloudFormationStackRecordSourceInfoTypeDef],
-        "destinationInfo": DestinationInfoTypeDef,
-    },
-    total=False,
-)
-
-GetContainerImagesResultTypeDef = TypedDict(
-    "GetContainerImagesResultTypeDef",
-    {
-        "containerImages": List[ContainerImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterContainerImageResultTypeDef = TypedDict(
-    "RegisterContainerImageResultTypeDef",
-    {
-        "containerImage": ContainerImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PrivateRegistryAccessRequestTypeDef = TypedDict(
-    "PrivateRegistryAccessRequestTypeDef",
-    {
-        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
-    },
-    total=False,
-)
-
-PrivateRegistryAccessTypeDef = TypedDict(
-    "PrivateRegistryAccessTypeDef",
-    {
-        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleTypeDef,
-    },
-    total=False,
-)
-
-ContainerServiceEndpointTypeDef = TypedDict(
-    "ContainerServiceEndpointTypeDef",
-    {
-        "containerName": str,
-        "containerPort": int,
-        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredEndpointRequestTypeDef = TypedDict(
-    "_RequiredEndpointRequestTypeDef",
-    {
-        "containerName": str,
-        "containerPort": int,
-    },
-)
-_OptionalEndpointRequestTypeDef = TypedDict(
-    "_OptionalEndpointRequestTypeDef",
-    {
-        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
-    },
-    total=False,
-)
-
-class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
-    pass
-
-GetContainerLogResultTypeDef = TypedDict(
-    "GetContainerLogResultTypeDef",
-    {
-        "logEvents": List[ContainerServiceLogEventTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetContainerServicePowersResultTypeDef = TypedDict(
-    "GetContainerServicePowersResultTypeDef",
-    {
-        "powers": List[ContainerServicePowerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
-    "CreateContainerServiceRegistryLoginResultTypeDef",
-    {
-        "registryLogin": ContainerServiceRegistryLoginTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateCloudFormationStackRequestRequestTypeDef = TypedDict(
     "CreateCloudFormationStackRequestRequestTypeDef",
     {
         "instances": Sequence[InstanceEntryTypeDef],
     },
 )
 
@@ -3726,28 +3888,20 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRelationalDatabaseParametersResultTypeDef = TypedDict(
     "GetRelationalDatabaseParametersResultTypeDef",
     {
-        "parameters": List[RelationalDatabaseParameterTypeDef],
+        "parameters": List[RelationalDatabaseParameterOutputTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
-    },
-)
-
 InstanceAccessDetailsTypeDef = TypedDict(
     "InstanceAccessDetailsTypeDef",
     {
         "certKey": str,
         "expiresAt": datetime,
         "ipAddress": str,
         "password": str,
@@ -3797,15 +3951,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "dnsName": str,
         "state": LoadBalancerStateType,
         "protocol": LoadBalancerProtocolType,
         "publicPorts": List[int],
         "healthCheckPath": str,
         "instancePort": int,
         "instanceHealthSummary": List[InstanceHealthSummaryTypeDef],
@@ -3832,15 +3986,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
         "hardware": RelationalDatabaseHardwareTypeDef,
         "state": str,
         "secondaryAvailabilityZone": str,
         "backupRetentionEnabled": bool,
@@ -3856,14 +4010,22 @@
         "masterEndpoint": RelationalDatabaseEndpointTypeDef,
         "pendingMaintenanceActions": List[PendingMaintenanceActionTypeDef],
         "caCertificateIdentifier": str,
     },
     total=False,
 )
 
+UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
+    },
+)
+
 GetBucketAccessKeysResultTypeDef = TypedDict(
     "GetBucketAccessKeysResultTypeDef",
     {
         "accessKeys": List[AccessKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4782,15 +4944,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "state": InstanceSnapshotStateType,
         "progress": str,
         "fromAttachedDisks": List[DiskTypeDef],
         "fromInstanceName": str,
         "fromInstanceArn": str,
         "fromBlueprintId": str,
         "fromBundleId": str,
@@ -4841,14 +5003,41 @@
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LightsailDistributionTypeDef = TypedDict(
+    "LightsailDistributionTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "alternativeDomainNames": List[str],
+        "status": str,
+        "isEnabled": bool,
+        "domainName": str,
+        "bundleId": str,
+        "certificateName": str,
+        "origin": OriginTypeDef,
+        "originPublicDNS": str,
+        "defaultCacheBehavior": CacheBehaviorOutputTypeDef,
+        "cacheBehaviorSettings": CacheSettingsOutputTypeDef,
+        "cacheBehaviors": List[CacheBehaviorPerPathOutputTypeDef],
+        "ableToUpdateBundle": bool,
+        "ipAddressType": IpAddressTypeType,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
@@ -4867,41 +5056,14 @@
 
 class CreateDistributionRequestRequestTypeDef(
     _RequiredCreateDistributionRequestRequestTypeDef,
     _OptionalCreateDistributionRequestRequestTypeDef,
 ):
     pass
 
-LightsailDistributionTypeDef = TypedDict(
-    "LightsailDistributionTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "alternativeDomainNames": List[str],
-        "status": str,
-        "isEnabled": bool,
-        "domainName": str,
-        "bundleId": str,
-        "certificateName": str,
-        "origin": OriginTypeDef,
-        "originPublicDNS": str,
-        "defaultCacheBehavior": CacheBehaviorTypeDef,
-        "cacheBehaviorSettings": CacheSettingsTypeDef,
-        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
-        "ableToUpdateBundle": bool,
-        "ipAddressType": IpAddressTypeType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
     },
 )
 _OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
@@ -4956,15 +5118,15 @@
     pass
 
 ContainerServiceDeploymentTypeDef = TypedDict(
     "ContainerServiceDeploymentTypeDef",
     {
         "version": int,
         "state": ContainerServiceDeploymentStateType,
-        "containers": Dict[str, ContainerTypeDef],
+        "containers": Dict[str, ContainerOutputTypeDef],
         "publicEndpoint": ContainerServiceEndpointTypeDef,
         "createdAt": datetime,
     },
     total=False,
 )
 
 ContainerServiceDeploymentRequestTypeDef = TypedDict(
@@ -5045,15 +5207,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "loadBalancerName": str,
         "isAttached": bool,
         "status": LoadBalancerTlsCertificateStatusType,
         "domainName": str,
         "domainValidationRecords": List[LoadBalancerTlsCertificateDomainValidationRecordTypeDef],
         "failureReason": LoadBalancerTlsCertificateFailureReasonType,
         "issuedAt": datetime,
@@ -5094,16 +5256,16 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
-        "domainEntries": List[DomainEntryTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "domainEntries": List[DomainEntryOutputTypeDef],
         "registeredDomainDelegationInfo": RegisteredDomainDelegationInfoTypeDef,
     },
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
@@ -5127,15 +5289,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "blueprintId": str,
         "blueprintName": str,
         "bundleId": str,
         "addOns": List[AddOnTypeDef],
         "isStaticIp": bool,
         "privateIpAddress": str,
         "publicIpAddress": str,
@@ -5190,15 +5352,15 @@
     "ContainerServiceTypeDef",
     {
         "containerServiceName": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "power": ContainerServicePowerNameType,
         "powerId": str,
         "state": ContainerServiceStateType,
         "stateDetail": ContainerServiceStateDetailTypeDef,
         "scale": int,
         "currentDeployment": ContainerServiceDeploymentTypeDef,
         "nextDeployment": ContainerServiceDeploymentTypeDef,
@@ -5278,15 +5440,15 @@
         "issuerCA": str,
         "notBefore": datetime,
         "notAfter": datetime,
         "eligibleToRenew": str,
         "renewalSummary": RenewalSummaryTypeDef,
         "revokedAt": datetime,
         "revocationReason": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "supportCode": str,
     },
     total=False,
 )
 
 ResourceBudgetEstimateTypeDef = TypedDict(
     "ResourceBudgetEstimateTypeDef",
@@ -5386,15 +5548,15 @@
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "certificateArn": str,
         "certificateName": str,
         "domainName": str,
         "certificateDetail": CertificateTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 GetCostEstimateResultTypeDef = TypedDict(
     "GetCostEstimateResultTypeDef",
     {
```

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/PKG-INFO` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.0
-Summary: Type annotations for boto3.Lightsail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Lightsail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lightsail"></a>
 
 # mypy-boto3-lightsail
 
 [![PyPI - mypy-boto3-lightsail](https://img.shields.io/pypi/v/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -474,14 +474,15 @@
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
+    AccessRulesOutputTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
@@ -490,39 +491,48 @@
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
     BlueprintTypeDef,
+    BucketAccessLogConfigOutputTypeDef,
     BucketAccessLogConfigTypeDef,
     BucketBundleTypeDef,
     BucketStateTypeDef,
     ResourceReceivingAccessTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     BundleTypeDef,
+    CacheBehaviorOutputTypeDef,
+    CacheBehaviorPerPathOutputTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
+    CookieObjectOutputTypeDef,
+    HeaderObjectOutputTypeDef,
+    QueryStringObjectOutputTypeDef,
     CookieObjectTypeDef,
     HeaderObjectTypeDef,
     QueryStringObjectTypeDef,
     PortInfoTypeDef,
     CloudFormationStackRecordSourceInfoTypeDef,
     DestinationInfoTypeDef,
     ContainerImageTypeDef,
+    ContainerOutputTypeDef,
     ContainerTypeDef,
     ContainerServiceECRImagePullerRoleRequestTypeDef,
     ContainerServiceECRImagePullerRoleTypeDef,
+    ContainerServiceHealthCheckConfigOutputTypeDef,
     ContainerServiceHealthCheckConfigTypeDef,
     ContainerServiceLogEventTypeDef,
     ContainerServicePowerTypeDef,
     ContainerServiceRegistryLoginTypeDef,
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
+    TagTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
@@ -551,14 +561,15 @@
     DetachInstancesFromLoadBalancerRequestRequestTypeDef,
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
+    DomainEntryOutputTypeDef,
     ResourceRecordTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetActiveNamesResultTypeDef,
@@ -640,15 +651,15 @@
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
     GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
     GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
-    RelationalDatabaseParameterTypeDef,
+    RelationalDatabaseParameterOutputTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
     GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
@@ -673,14 +684,15 @@
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
+    RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
@@ -704,45 +716,46 @@
     StaticIpTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
-    CreateBucketRequestRequestTypeDef,
-    CreateCertificateRequestRequestTypeDef,
-    CreateDiskSnapshotRequestRequestTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateInstanceSnapshotRequestRequestTypeDef,
-    CreateKeyPairRequestRequestTypeDef,
-    CreateLoadBalancerRequestRequestTypeDef,
-    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    CreateRelationalDatabaseRequestRequestTypeDef,
-    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
-    TagResourceRequestRequestTypeDef,
     GetBundlesResultTypeDef,
+    CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
     GetContainerImagesResultTypeDef,
     RegisterContainerImageResultTypeDef,
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
+    CreateBucketRequestRequestTypeDef,
+    CreateCertificateRequestRequestTypeDef,
+    CreateDiskSnapshotRequestRequestTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    CreateInstanceSnapshotRequestRequestTypeDef,
+    CreateKeyPairRequestRequestTypeDef,
+    CreateLoadBalancerRequestRequestTypeDef,
+    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    CreateRelationalDatabaseRequestRequestTypeDef,
+    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
@@ -758,22 +771,22 @@
     GetInstanceStateResultTypeDef,
     GetLoadBalancerTlsPoliciesResultTypeDef,
     GetRelationalDatabaseBlueprintsResultTypeDef,
     GetRelationalDatabaseBundlesResultTypeDef,
     GetRelationalDatabaseEventsResultTypeDef,
     GetRelationalDatabaseLogEventsResultTypeDef,
     GetRelationalDatabaseParametersResultTypeDef,
-    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     InstanceAccessDetailsTypeDef,
     InstanceNetworkingTypeDef,
     LoadBalancerTlsCertificateDomainValidationRecordTypeDef,
     LoadBalancerTlsCertificateRenewalSummaryTypeDef,
     LoadBalancerTypeDef,
     RegisteredDomainDelegationInfoTypeDef,
     RelationalDatabaseTypeDef,
+    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     GetBucketAccessKeysResultTypeDef,
     CreateDiskFromSnapshotRequestRequestTypeDef,
     CreateDiskRequestRequestTypeDef,
     CreateInstancesFromSnapshotRequestRequestTypeDef,
     CreateInstancesRequestRequestTypeDef,
     EnableAddOnRequestRequestTypeDef,
     GetAlarmsResultTypeDef,
@@ -875,16 +888,16 @@
     InstanceHardwareTypeDef,
     InstanceSnapshotTypeDef,
     CreateKeyPairResultTypeDef,
     GetKeyPairResultTypeDef,
     GetKeyPairsResultTypeDef,
     GetRelationalDatabaseSnapshotResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
-    CreateDistributionRequestRequestTypeDef,
     LightsailDistributionTypeDef,
+    CreateDistributionRequestRequestTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
     ExportSnapshotRecordSourceInfoTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.0/mypy_boto3_lightsail.egg-info/SOURCES.txt` & `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.0/setup.py` & `mypy-boto3-lightsail-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lightsail",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lightsail 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Lightsail 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

