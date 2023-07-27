# Comparing `tmp/mypy-boto3-opensearch-1.28.0.tar.gz` & `tmp/mypy-boto3-opensearch-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearch-1.28.0.tar", last modified: Thu Jul  6 21:00:14 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearch-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-opensearch-1.28.0.tar` & `mypy-boto3-opensearch-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.914385 mypy-boto3-opensearch-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-06 21:00:14.910385 mypy-boto3-opensearch-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.910385 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41084 2023-07-06 20:48:38.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41023 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-07-06 20:48:38.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-07-06 20:48:38.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68125 2023-07-06 20:48:40.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68068 2023-07-06 20:48:39.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.910385 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-06 21:00:14.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-06 21:00:14.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:14.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:14.000000 mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:14.914385 mypy-boto3-opensearch-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:48:37.000000 mypy-boto3-opensearch-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.829133 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41084 2023-07-27 11:40:56.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41023 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-27 11:40:56.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-27 11:40:56.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74311 2023-07-27 11:40:58.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-07-27 11:40:57.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/setup.py
```

### Comparing `mypy-boto3-opensearch-1.28.0/LICENSE` & `mypy-boto3-opensearch-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.0/PKG-INFO` & `mypy-boto3-opensearch-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.0
-Summary: Type annotations for boto3.OpenSearchService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpenSearchService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opensearch"></a>
 
 # mypy-boto3-opensearch
 
 [![PyPI - mypy-boto3-opensearch](https://img.shields.io/pypi/v/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,36 +338,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
+    AWSDomainInformationOutputTypeDef,
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
+    DurationOutputTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
+    ColdStorageOptionsOutputTypeDef,
+    ZoneAwarenessConfigOutputTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
+    CognitoOptionsOutputTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
+    CrossClusterSearchConnectionPropertiesOutputTypeDef,
     CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
@@ -395,163 +402,179 @@
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
     DescribeReservedInstanceOfferingsRequestRequestTypeDef,
     DescribeReservedInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
+    DomainEndpointOptionsOutputTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
+    EBSOptionsOutputTypeDef,
+    EncryptionAtRestOptionsOutputTypeDef,
+    LogPublishingOptionOutputTypeDef,
+    NodeToNodeEncryptionOptionsOutputTypeDef,
+    SnapshotOptionsOutputTypeDef,
+    SoftwareUpdateOptionsOutputTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    WindowStartTimeOutputTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
+    SAMLIdpOutputTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
+    DomainInformationContainerOutputTypeDef,
     DomainInformationContainerTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListVersionsResponseTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
+    ClusterConfigOutputTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
+    ConnectionPropertiesOutputTypeDef,
     ConnectionPropertiesTypeDef,
-    DomainEndpointOptionsStatusTypeDef,
-    EBSOptionsStatusTypeDef,
-    EncryptionAtRestOptionsStatusTypeDef,
-    LogPublishingOptionsStatusTypeDef,
-    NodeToNodeEncryptionOptionsStatusTypeDef,
-    SnapshotOptionsStatusTypeDef,
-    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
+    DomainEndpointOptionsStatusTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
+    EBSOptionsStatusTypeDef,
+    EncryptionAtRestOptionsStatusTypeDef,
+    LogPublishingOptionsStatusTypeDef,
+    NodeToNodeEncryptionOptionsStatusTypeDef,
+    SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListScheduledActionsResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
+    ListTagsResponseTypeDef,
+    OffPeakWindowOutputTypeDef,
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
-    SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
+    SAMLOptionsInputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     OutboundConnectionTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
+    OffPeakWindowOptionsOutputTypeDef,
     OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
-    AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
+    AdvancedSecurityOptionsInputTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainConfigRequestRequestTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_structure() -> AWSDomainInformationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.0/README.md` & `mypy-boto3-opensearch-1.28.12/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opensearch"></a>
 
 # mypy-boto3-opensearch
 
 [![PyPI - mypy-boto3-opensearch](https://img.shields.io/pypi/v/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,36 +306,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
+    AWSDomainInformationOutputTypeDef,
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
+    DurationOutputTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
+    ColdStorageOptionsOutputTypeDef,
+    ZoneAwarenessConfigOutputTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
+    CognitoOptionsOutputTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
+    CrossClusterSearchConnectionPropertiesOutputTypeDef,
     CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
@@ -363,163 +370,179 @@
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
     DescribeReservedInstanceOfferingsRequestRequestTypeDef,
     DescribeReservedInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
+    DomainEndpointOptionsOutputTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
+    EBSOptionsOutputTypeDef,
+    EncryptionAtRestOptionsOutputTypeDef,
+    LogPublishingOptionOutputTypeDef,
+    NodeToNodeEncryptionOptionsOutputTypeDef,
+    SnapshotOptionsOutputTypeDef,
+    SoftwareUpdateOptionsOutputTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    WindowStartTimeOutputTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
+    SAMLIdpOutputTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
+    DomainInformationContainerOutputTypeDef,
     DomainInformationContainerTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListVersionsResponseTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
+    ClusterConfigOutputTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
+    ConnectionPropertiesOutputTypeDef,
     ConnectionPropertiesTypeDef,
-    DomainEndpointOptionsStatusTypeDef,
-    EBSOptionsStatusTypeDef,
-    EncryptionAtRestOptionsStatusTypeDef,
-    LogPublishingOptionsStatusTypeDef,
-    NodeToNodeEncryptionOptionsStatusTypeDef,
-    SnapshotOptionsStatusTypeDef,
-    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
+    DomainEndpointOptionsStatusTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
+    EBSOptionsStatusTypeDef,
+    EncryptionAtRestOptionsStatusTypeDef,
+    LogPublishingOptionsStatusTypeDef,
+    NodeToNodeEncryptionOptionsStatusTypeDef,
+    SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListScheduledActionsResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
+    ListTagsResponseTypeDef,
+    OffPeakWindowOutputTypeDef,
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
-    SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
+    SAMLOptionsInputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     OutboundConnectionTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
+    OffPeakWindowOptionsOutputTypeDef,
     OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
-    AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
+    AdvancedSecurityOptionsInputTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainConfigRequestRequestTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_structure() -> AWSDomainInformationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/__main__.py` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.OpenSearchService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
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

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/client.py` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/client.pyi` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/literals.py` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,14 +372,15 @@
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
@@ -458,26 +459,28 @@
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

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/literals.pyi` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -370,14 +370,15 @@
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
@@ -456,26 +457,28 @@
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

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/type_defs.py` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opensearch service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opensearch.type_defs import AWSDomainInformationTypeDef
+    from mypy_boto3_opensearch.type_defs import AWSDomainInformationOutputTypeDef
 
-    data: AWSDomainInformationTypeDef = {...}
+    data: AWSDomainInformationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,36 +64,43 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AWSDomainInformationOutputTypeDef",
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
+    "DurationOutputTypeDef",
     "DurationTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
+    "ColdStorageOptionsOutputTypeDef",
+    "ZoneAwarenessConfigOutputTypeDef",
     "ColdStorageOptionsTypeDef",
     "ZoneAwarenessConfigTypeDef",
+    "CognitoOptionsOutputTypeDef",
     "CognitoOptionsTypeDef",
     "CompatibleVersionsMapTypeDef",
+    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
     "CrossClusterSearchConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
@@ -121,161 +128,199 @@
     "DescribeInstanceTypeLimitsRequestRequestTypeDef",
     "DescribePackagesFilterTypeDef",
     "DescribeReservedInstanceOfferingsRequestRequestTypeDef",
     "DescribeReservedInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
+    "DomainEndpointOptionsOutputTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
+    "EBSOptionsOutputTypeDef",
+    "EncryptionAtRestOptionsOutputTypeDef",
+    "LogPublishingOptionOutputTypeDef",
+    "NodeToNodeEncryptionOptionsOutputTypeDef",
+    "SnapshotOptionsOutputTypeDef",
+    "SoftwareUpdateOptionsOutputTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListVersionsResponseTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
+    "WindowStartTimeOutputTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
+    "SAMLIdpOutputTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
+    "DomainInformationContainerOutputTypeDef",
     "DomainInformationContainerTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
+    "ListVersionsResponseTypeDef",
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
+    "ClusterConfigOutputTypeDef",
     "ClusterConfigTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleVersionsResponseTypeDef",
+    "ConnectionPropertiesOutputTypeDef",
     "ConnectionPropertiesTypeDef",
-    "DomainEndpointOptionsStatusTypeDef",
-    "EBSOptionsStatusTypeDef",
-    "EncryptionAtRestOptionsStatusTypeDef",
-    "LogPublishingOptionsStatusTypeDef",
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    "SnapshotOptionsStatusTypeDef",
-    "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeDomainNodesResponseTypeDef",
     "DescribeInboundConnectionsRequestRequestTypeDef",
     "DescribeOutboundConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
+    "DomainEndpointOptionsStatusTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
+    "EBSOptionsStatusTypeDef",
+    "EncryptionAtRestOptionsStatusTypeDef",
+    "LogPublishingOptionsStatusTypeDef",
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    "SnapshotOptionsStatusTypeDef",
+    "SoftwareUpdateOptionsStatusTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "DryRunProgressStatusTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
     "InstanceLimitsTypeDef",
     "ListInstanceTypeDetailsResponseTypeDef",
     "ListScheduledActionsResponseTypeDef",
     "UpdateScheduledActionResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "OffPeakWindowOutputTypeDef",
     "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
-    "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
+    "SAMLOptionsInputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
-    "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
     "OutboundConnectionTypeDef",
+    "CreateOutboundConnectionRequestRequestTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
     "ListDomainsForPackageResponseTypeDef",
     "ListPackagesForDomainResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
     "UpdatePackageResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DescribeVpcEndpointsResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
+    "OffPeakWindowOptionsOutputTypeDef",
     "OffPeakWindowOptionsTypeDef",
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     "DescribeReservedInstancesResponseTypeDef",
-    "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
+    "AdvancedSecurityOptionsInputTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "UpdateDomainConfigRequestRequestTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
     "DescribeDryRunProgressResponseTypeDef",
     "DescribeDomainConfigResponseTypeDef",
     "UpdateDomainConfigResponseTypeDef",
 )
 
+_RequiredAWSDomainInformationOutputTypeDef = TypedDict(
+    "_RequiredAWSDomainInformationOutputTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalAWSDomainInformationOutputTypeDef = TypedDict(
+    "_OptionalAWSDomainInformationOutputTypeDef",
+    {
+        "OwnerId": str,
+        "Region": str,
+    },
+    total=False,
+)
+
+
+class AWSDomainInformationOutputTypeDef(
+    _RequiredAWSDomainInformationOutputTypeDef, _OptionalAWSDomainInformationOutputTypeDef
+):
+    pass
+
+
 _RequiredAWSDomainInformationTypeDef = TypedDict(
     "_RequiredAWSDomainInformationTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalAWSDomainInformationTypeDef = TypedDict(
@@ -297,14 +342,25 @@
 AcceptInboundConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
 )
 
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -382,14 +438,23 @@
         "ActionType": ScheduledAutoTuneActionTypeType,
         "Action": str,
         "Severity": ScheduledAutoTuneSeverityTypeType,
     },
     total=False,
 )
 
+DurationOutputTypeDef = TypedDict(
+    "DurationOutputTypeDef",
+    {
+        "Value": int,
+        "Unit": Literal["HOURS"],
+    },
+    total=False,
+)
+
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
@@ -479,14 +544,29 @@
         "Status": str,
         "Description": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
+ColdStorageOptionsOutputTypeDef = TypedDict(
+    "ColdStorageOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+
+ZoneAwarenessConfigOutputTypeDef = TypedDict(
+    "ZoneAwarenessConfigOutputTypeDef",
+    {
+        "AvailabilityZoneCount": int,
+    },
+    total=False,
+)
+
 ColdStorageOptionsTypeDef = TypedDict(
     "ColdStorageOptionsTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -494,14 +574,25 @@
     "ZoneAwarenessConfigTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
+CognitoOptionsOutputTypeDef = TypedDict(
+    "CognitoOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "UserPoolId": str,
+        "IdentityPoolId": str,
+        "RoleArn": str,
+    },
+    total=False,
+)
+
 CognitoOptionsTypeDef = TypedDict(
     "CognitoOptionsTypeDef",
     {
         "Enabled": bool,
         "UserPoolId": str,
         "IdentityPoolId": str,
         "RoleArn": str,
@@ -514,14 +605,22 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
+CrossClusterSearchConnectionPropertiesOutputTypeDef = TypedDict(
+    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
+    {
+        "SkipUnavailable": SkipUnavailableStatusType,
+    },
+    total=False,
+)
+
 CrossClusterSearchConnectionPropertiesTypeDef = TypedDict(
     "CrossClusterSearchConnectionPropertiesTypeDef",
     {
         "SkipUnavailable": SkipUnavailableStatusType,
     },
     total=False,
 )
@@ -874,14 +973,26 @@
     "DissociatePackageRequestRequestTypeDef",
     {
         "PackageID": str,
         "DomainName": str,
     },
 )
 
+DomainEndpointOptionsOutputTypeDef = TypedDict(
+    "DomainEndpointOptionsOutputTypeDef",
+    {
+        "EnforceHTTPS": bool,
+        "TLSSecurityPolicy": TLSSecurityPolicyType,
+        "CustomEndpointEnabled": bool,
+        "CustomEndpoint": str,
+        "CustomEndpointCertificateArn": str,
+    },
+    total=False,
+)
+
 DomainInfoTypeDef = TypedDict(
     "DomainInfoTypeDef",
     {
         "DomainName": str,
         "EngineType": EngineTypeType,
     },
     total=False,
@@ -892,14 +1003,68 @@
     {
         "ErrorType": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+EBSOptionsOutputTypeDef = TypedDict(
+    "EBSOptionsOutputTypeDef",
+    {
+        "EBSEnabled": bool,
+        "VolumeType": VolumeTypeType,
+        "VolumeSize": int,
+        "Iops": int,
+        "Throughput": int,
+    },
+    total=False,
+)
+
+EncryptionAtRestOptionsOutputTypeDef = TypedDict(
+    "EncryptionAtRestOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+LogPublishingOptionOutputTypeDef = TypedDict(
+    "LogPublishingOptionOutputTypeDef",
+    {
+        "CloudWatchLogsLogGroupArn": str,
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+NodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
+    "NodeToNodeEncryptionOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+SnapshotOptionsOutputTypeDef = TypedDict(
+    "SnapshotOptionsOutputTypeDef",
+    {
+        "AutomatedSnapshotStartHour": int,
+    },
+    total=False,
+)
+
+SoftwareUpdateOptionsOutputTypeDef = TypedDict(
+    "SoftwareUpdateOptionsOutputTypeDef",
+    {
+        "AutoSoftwareUpdateEnabled": bool,
+    },
+    total=False,
+)
+
 VPCDerivedInfoTypeDef = TypedDict(
     "VPCDerivedInfoTypeDef",
     {
         "VPCId": str,
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
@@ -912,21 +1077,14 @@
     {
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCompatibleVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -989,24 +1147,14 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InboundConnectionStatusTypeDef = TypedDict(
     "InboundConnectionStatusTypeDef",
     {
         "StatusCode": InboundConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -1168,30 +1316,29 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ARN": str,
     },
 )
 
-ListVersionsRequestRequestTypeDef = TypedDict(
-    "ListVersionsRequestRequestTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
+ListVersionsRequestRequestTypeDef = TypedDict(
+    "ListVersionsRequestRequestTypeDef",
     {
-        "Versions": List[str],
+        "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
 _RequiredListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
     },
@@ -1238,14 +1385,22 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+WindowStartTimeOutputTypeDef = TypedDict(
+    "WindowStartTimeOutputTypeDef",
+    {
+        "Hours": int,
+        "Minutes": int,
+    },
+)
+
 WindowStartTimeTypeDef = TypedDict(
     "WindowStartTimeTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
@@ -1269,23 +1424,14 @@
 class PurchaseReservedInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
 
-PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
-    {
-        "ReservedInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1302,33 +1448,30 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
     },
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
 
+SAMLIdpOutputTypeDef = TypedDict(
+    "SAMLIdpOutputTypeDef",
+    {
+        "MetadataContent": str,
+        "EntityId": str,
+    },
+)
+
 SAMLIdpTypeDef = TypedDict(
     "SAMLIdpTypeDef",
     {
         "MetadataContent": str,
         "EntityId": str,
     },
 )
@@ -1420,22 +1563,65 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
+DomainInformationContainerOutputTypeDef = TypedDict(
+    "DomainInformationContainerOutputTypeDef",
+    {
+        "AWSDomainInformation": AWSDomainInformationOutputTypeDef,
+    },
+    total=False,
+)
+
 DomainInformationContainerTypeDef = TypedDict(
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "Versions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
+    {
+        "ReservedInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1460,47 +1646,49 @@
     "AddTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
+    {
+        "StartAt": datetime,
+        "Duration": DurationOutputTypeDef,
+        "CronExpressionForRecurrence": str,
+    },
+    total=False,
+)
+
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": Union[datetime, str],
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
@@ -1515,36 +1703,36 @@
     total=False,
 )
 
 CancelServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpgradeDomainResponseTypeDef = TypedDict(
     "UpgradeDomainResponseTypeDef",
     {
         "UpgradeId": str,
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "AdvancedOptions": Dict[str, str],
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1554,14 +1742,33 @@
         "CompletedProperties": List[str],
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
+ClusterConfigOutputTypeDef = TypedDict(
+    "ClusterConfigOutputTypeDef",
+    {
+        "InstanceType": OpenSearchPartitionInstanceTypeType,
+        "InstanceCount": int,
+        "DedicatedMasterEnabled": bool,
+        "ZoneAwarenessEnabled": bool,
+        "ZoneAwarenessConfig": ZoneAwarenessConfigOutputTypeDef,
+        "DedicatedMasterType": OpenSearchPartitionInstanceTypeType,
+        "DedicatedMasterCount": int,
+        "WarmEnabled": bool,
+        "WarmType": OpenSearchWarmPartitionInstanceTypeType,
+        "WarmCount": int,
+        "ColdStorageOptions": ColdStorageOptionsOutputTypeDef,
+        "MultiAZWithStandbyEnabled": bool,
+    },
+    total=False,
+)
+
 ClusterConfigTypeDef = TypedDict(
     "ClusterConfigTypeDef",
     {
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "InstanceCount": int,
         "DedicatedMasterEnabled": bool,
         "ZoneAwarenessEnabled": bool,
@@ -1576,90 +1783,41 @@
     },
     total=False,
 )
 
 CognitoOptionsStatusTypeDef = TypedDict(
     "CognitoOptionsStatusTypeDef",
     {
-        "Options": CognitoOptionsTypeDef,
+        "Options": CognitoOptionsOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConnectionPropertiesTypeDef = TypedDict(
-    "ConnectionPropertiesTypeDef",
+ConnectionPropertiesOutputTypeDef = TypedDict(
+    "ConnectionPropertiesOutputTypeDef",
     {
         "Endpoint": str,
-        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-DomainEndpointOptionsStatusTypeDef = TypedDict(
-    "DomainEndpointOptionsStatusTypeDef",
-    {
-        "Options": DomainEndpointOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-EBSOptionsStatusTypeDef = TypedDict(
-    "EBSOptionsStatusTypeDef",
-    {
-        "Options": EBSOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-EncryptionAtRestOptionsStatusTypeDef = TypedDict(
-    "EncryptionAtRestOptionsStatusTypeDef",
-    {
-        "Options": EncryptionAtRestOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-LogPublishingOptionsStatusTypeDef = TypedDict(
-    "LogPublishingOptionsStatusTypeDef",
-    {
-        "Options": Dict[LogTypeType, LogPublishingOptionTypeDef],
-        "Status": OptionStatusTypeDef,
-    },
-    total=False,
-)
-
-NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    {
-        "Options": NodeToNodeEncryptionOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SnapshotOptionsStatusTypeDef = TypedDict(
-    "SnapshotOptionsStatusTypeDef",
-    {
-        "Options": SnapshotOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SoftwareUpdateOptionsStatusTypeDef = TypedDict(
-    "SoftwareUpdateOptionsStatusTypeDef",
+ConnectionPropertiesTypeDef = TypedDict(
+    "ConnectionPropertiesTypeDef",
     {
-        "Options": SoftwareUpdateOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
+        "Endpoint": str,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointRequestRequestTypeDef",
     {
@@ -1736,41 +1894,41 @@
     pass
 
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainNodesResponseTypeDef = TypedDict(
     "DescribeDomainNodesResponseTypeDef",
     {
         "DomainNodesStatusList": List[DomainNodesStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1796,19 +1954,27 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DomainEndpointOptionsStatusTypeDef = TypedDict(
+    "DomainEndpointOptionsStatusTypeDef",
+    {
+        "Options": DomainEndpointOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1836,14 +2002,64 @@
         "LastUpdatedAt": datetime,
         "AvailablePackageVersion": str,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
+EBSOptionsStatusTypeDef = TypedDict(
+    "EBSOptionsStatusTypeDef",
+    {
+        "Options": EBSOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+EncryptionAtRestOptionsStatusTypeDef = TypedDict(
+    "EncryptionAtRestOptionsStatusTypeDef",
+    {
+        "Options": EncryptionAtRestOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+LogPublishingOptionsStatusTypeDef = TypedDict(
+    "LogPublishingOptionsStatusTypeDef",
+    {
+        "Options": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
+NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    {
+        "Options": NodeToNodeEncryptionOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SnapshotOptionsStatusTypeDef = TypedDict(
+    "SnapshotOptionsStatusTypeDef",
+    {
+        "Options": SnapshotOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SoftwareUpdateOptionsStatusTypeDef = TypedDict(
+    "SoftwareUpdateOptionsStatusTypeDef",
+    {
+        "Options": SoftwareUpdateOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
 VPCDerivedInfoStatusTypeDef = TypedDict(
     "VPCDerivedInfoStatusTypeDef",
     {
         "Options": VPCDerivedInfoTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1887,15 +2103,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceLimitsTypeDef = TypedDict(
     "InstanceLimitsTypeDef",
     {
         "InstanceCountLimits": InstanceCountLimitsTypeDef,
@@ -1904,35 +2120,51 @@
 )
 
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OffPeakWindowOutputTypeDef = TypedDict(
+    "OffPeakWindowOutputTypeDef",
+    {
+        "WindowStartTime": WindowStartTimeOutputTypeDef,
+    },
+    total=False,
+)
+
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
     },
     total=False,
 )
@@ -1969,33 +2201,33 @@
         "State": str,
         "PaymentOption": ReservedInstancePaymentOptionType,
         "RecurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
-SAMLOptionsInputTypeDef = TypedDict(
-    "SAMLOptionsInputTypeDef",
+SAMLOptionsOutputTypeDef = TypedDict(
+    "SAMLOptionsOutputTypeDef",
     {
         "Enabled": bool,
-        "Idp": SAMLIdpTypeDef,
-        "MasterUserName": str,
-        "MasterBackendRole": str,
+        "Idp": SAMLIdpOutputTypeDef,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
-SAMLOptionsOutputTypeDef = TypedDict(
-    "SAMLOptionsOutputTypeDef",
+SAMLOptionsInputTypeDef = TypedDict(
+    "SAMLOptionsInputTypeDef",
     {
         "Enabled": bool,
         "Idp": SAMLIdpTypeDef,
+        "MasterUserName": str,
+        "MasterBackendRole": str,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
@@ -2019,16 +2251,16 @@
     },
     total=False,
 )
 
 InboundConnectionTypeDef = TypedDict(
     "InboundConnectionTypeDef",
     {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
         "ConnectionId": str,
         "ConnectionStatus": InboundConnectionStatusTypeDef,
         "ConnectionMode": ConnectionModeType,
     },
     total=False,
 )
 
@@ -2037,14 +2269,25 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsExtraOutputTypeDef = TypedDict(
+    "AutoTuneOptionsExtraOutputTypeDef",
+    {
+        "DesiredState": AutoTuneDesiredStateType,
+        "RollbackOnDisable": RollbackOnDisableType,
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
+        "UseOffPeakWindow": bool,
+    },
+    total=False,
+)
+
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
@@ -2052,15 +2295,15 @@
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
@@ -2074,34 +2317,62 @@
         "MasterEligibleNodeCount": str,
         "WarmNodeCount": str,
         "MasterNode": MasterNodeStatusType,
         "ClusterHealth": DomainHealthType,
         "TotalShards": str,
         "TotalUnAssignedShards": str,
         "EnvironmentInformation": List[EnvironmentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
-        "Options": ClusterConfigTypeDef,
+        "Options": ClusterConfigOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
+CreateOutboundConnectionResponseTypeDef = TypedDict(
+    "CreateOutboundConnectionResponseTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionId": str,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OutboundConnectionTypeDef = TypedDict(
+    "OutboundConnectionTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
+        "ConnectionId": str,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionAlias": str,
     },
@@ -2119,180 +2390,161 @@
 class CreateOutboundConnectionRequestRequestTypeDef(
     _RequiredCreateOutboundConnectionRequestRequestTypeDef,
     _OptionalCreateOutboundConnectionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateOutboundConnectionResponseTypeDef = TypedDict(
-    "CreateOutboundConnectionResponseTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionId": str,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OutboundConnectionTypeDef = TypedDict(
-    "OutboundConnectionTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionId": str,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
-    },
-    total=False,
-)
-
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OffPeakWindowOptionsOutputTypeDef = TypedDict(
+    "OffPeakWindowOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "OffPeakWindow": OffPeakWindowOutputTypeDef,
+    },
+    total=False,
+)
+
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
         "OffPeakWindow": OffPeakWindowTypeDef,
     },
     total=False,
 )
 
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdvancedSecurityOptionsInputTypeDef = TypedDict(
-    "AdvancedSecurityOptionsInputTypeDef",
+AdvancedSecurityOptionsTypeDef = TypedDict(
+    "AdvancedSecurityOptionsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "MasterUserOptions": MasterUserOptionsTypeDef,
-        "SAMLOptions": SAMLOptionsInputTypeDef,
+        "SAMLOptions": SAMLOptionsOutputTypeDef,
+        "AnonymousAuthDisableDate": datetime,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
-AdvancedSecurityOptionsTypeDef = TypedDict(
-    "AdvancedSecurityOptionsTypeDef",
+AdvancedSecurityOptionsInputTypeDef = TypedDict(
+    "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "SAMLOptions": SAMLOptionsOutputTypeDef,
-        "AnonymousAuthDisableDate": datetime,
+        "MasterUserOptions": MasterUserOptionsTypeDef,
+        "SAMLOptions": SAMLOptionsInputTypeDef,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
 LimitsTypeDef = TypedDict(
     "LimitsTypeDef",
@@ -2305,95 +2557,147 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInboundConnectionResponseTypeDef = TypedDict(
     "DeleteInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsTypeDef,
+        "Options": AutoTuneOptionsExtraOutputTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOutboundConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundConnectionsResponseTypeDef",
     {
         "Connections": List[OutboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
-        "Options": OffPeakWindowOptionsTypeDef,
+        "Options": OffPeakWindowOptionsOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
     total=False,
 )
 
+AdvancedSecurityOptionsStatusTypeDef = TypedDict(
+    "AdvancedSecurityOptionsStatusTypeDef",
+    {
+        "Options": AdvancedSecurityOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+_RequiredDomainStatusTypeDef = TypedDict(
+    "_RequiredDomainStatusTypeDef",
+    {
+        "DomainId": str,
+        "DomainName": str,
+        "ARN": str,
+        "ClusterConfig": ClusterConfigOutputTypeDef,
+    },
+)
+_OptionalDomainStatusTypeDef = TypedDict(
+    "_OptionalDomainStatusTypeDef",
+    {
+        "Created": bool,
+        "Deleted": bool,
+        "Endpoint": str,
+        "Endpoints": Dict[str, str],
+        "Processing": bool,
+        "UpgradeProcessing": bool,
+        "EngineVersion": str,
+        "EBSOptions": EBSOptionsOutputTypeDef,
+        "AccessPolicies": str,
+        "SnapshotOptions": SnapshotOptionsOutputTypeDef,
+        "VPCOptions": VPCDerivedInfoTypeDef,
+        "CognitoOptions": CognitoOptionsOutputTypeDef,
+        "EncryptionAtRestOptions": EncryptionAtRestOptionsOutputTypeDef,
+        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsOutputTypeDef,
+        "AdvancedOptions": Dict[str, str],
+        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
+        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
+        "DomainEndpointOptions": DomainEndpointOptionsOutputTypeDef,
+        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
+        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
+        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsOutputTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
+    pass
+
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
@@ -2461,71 +2765,19 @@
 class UpdateDomainConfigRequestRequestTypeDef(
     _RequiredUpdateDomainConfigRequestRequestTypeDef,
     _OptionalUpdateDomainConfigRequestRequestTypeDef,
 ):
     pass
 
 
-AdvancedSecurityOptionsStatusTypeDef = TypedDict(
-    "AdvancedSecurityOptionsStatusTypeDef",
-    {
-        "Options": AdvancedSecurityOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-_RequiredDomainStatusTypeDef = TypedDict(
-    "_RequiredDomainStatusTypeDef",
-    {
-        "DomainId": str,
-        "DomainName": str,
-        "ARN": str,
-        "ClusterConfig": ClusterConfigTypeDef,
-    },
-)
-_OptionalDomainStatusTypeDef = TypedDict(
-    "_OptionalDomainStatusTypeDef",
-    {
-        "Created": bool,
-        "Deleted": bool,
-        "Endpoint": str,
-        "Endpoints": Dict[str, str],
-        "Processing": bool,
-        "UpgradeProcessing": bool,
-        "EngineVersion": str,
-        "EBSOptions": EBSOptionsTypeDef,
-        "AccessPolicies": str,
-        "SnapshotOptions": SnapshotOptionsTypeDef,
-        "VPCOptions": VPCDerivedInfoTypeDef,
-        "CognitoOptions": CognitoOptionsTypeDef,
-        "EncryptionAtRestOptions": EncryptionAtRestOptionsTypeDef,
-        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
-        "AdvancedOptions": Dict[str, str],
-        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionTypeDef],
-        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
-        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
-        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
-        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
-        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
-    pass
-
-
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainConfigTypeDef = TypedDict(
     "DomainConfigTypeDef",
     {
         "EngineVersion": VersionStatusTypeDef,
@@ -2549,62 +2801,62 @@
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDryRunProgressResponseTypeDef = TypedDict(
     "DescribeDryRunProgressResponseTypeDef",
     {
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
         "DryRunConfig": DomainStatusTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainConfigResponseTypeDef = TypedDict(
     "DescribeDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainConfigResponseTypeDef = TypedDict(
     "UpdateDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch/type_defs.pyi` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opensearch service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opensearch.type_defs import AWSDomainInformationTypeDef
+    from mypy_boto3_opensearch.type_defs import AWSDomainInformationOutputTypeDef
 
-    data: AWSDomainInformationTypeDef = {...}
+    data: AWSDomainInformationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -63,36 +63,43 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AWSDomainInformationOutputTypeDef",
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
+    "DurationOutputTypeDef",
     "DurationTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
+    "ColdStorageOptionsOutputTypeDef",
+    "ZoneAwarenessConfigOutputTypeDef",
     "ColdStorageOptionsTypeDef",
     "ZoneAwarenessConfigTypeDef",
+    "CognitoOptionsOutputTypeDef",
     "CognitoOptionsTypeDef",
     "CompatibleVersionsMapTypeDef",
+    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
     "CrossClusterSearchConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
@@ -120,161 +127,197 @@
     "DescribeInstanceTypeLimitsRequestRequestTypeDef",
     "DescribePackagesFilterTypeDef",
     "DescribeReservedInstanceOfferingsRequestRequestTypeDef",
     "DescribeReservedInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
+    "DomainEndpointOptionsOutputTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
+    "EBSOptionsOutputTypeDef",
+    "EncryptionAtRestOptionsOutputTypeDef",
+    "LogPublishingOptionOutputTypeDef",
+    "NodeToNodeEncryptionOptionsOutputTypeDef",
+    "SnapshotOptionsOutputTypeDef",
+    "SoftwareUpdateOptionsOutputTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListVersionsResponseTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
+    "WindowStartTimeOutputTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
+    "SAMLIdpOutputTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
+    "DomainInformationContainerOutputTypeDef",
     "DomainInformationContainerTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
+    "ListVersionsResponseTypeDef",
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
+    "ClusterConfigOutputTypeDef",
     "ClusterConfigTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleVersionsResponseTypeDef",
+    "ConnectionPropertiesOutputTypeDef",
     "ConnectionPropertiesTypeDef",
-    "DomainEndpointOptionsStatusTypeDef",
-    "EBSOptionsStatusTypeDef",
-    "EncryptionAtRestOptionsStatusTypeDef",
-    "LogPublishingOptionsStatusTypeDef",
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    "SnapshotOptionsStatusTypeDef",
-    "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeDomainNodesResponseTypeDef",
     "DescribeInboundConnectionsRequestRequestTypeDef",
     "DescribeOutboundConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
+    "DomainEndpointOptionsStatusTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
+    "EBSOptionsStatusTypeDef",
+    "EncryptionAtRestOptionsStatusTypeDef",
+    "LogPublishingOptionsStatusTypeDef",
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    "SnapshotOptionsStatusTypeDef",
+    "SoftwareUpdateOptionsStatusTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "DryRunProgressStatusTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
     "InstanceLimitsTypeDef",
     "ListInstanceTypeDetailsResponseTypeDef",
     "ListScheduledActionsResponseTypeDef",
     "UpdateScheduledActionResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "OffPeakWindowOutputTypeDef",
     "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
-    "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
+    "SAMLOptionsInputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
-    "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
     "OutboundConnectionTypeDef",
+    "CreateOutboundConnectionRequestRequestTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
     "ListDomainsForPackageResponseTypeDef",
     "ListPackagesForDomainResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
     "UpdatePackageResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DescribeVpcEndpointsResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
+    "OffPeakWindowOptionsOutputTypeDef",
     "OffPeakWindowOptionsTypeDef",
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     "DescribeReservedInstancesResponseTypeDef",
-    "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
+    "AdvancedSecurityOptionsInputTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "UpdateDomainConfigRequestRequestTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
     "DescribeDryRunProgressResponseTypeDef",
     "DescribeDomainConfigResponseTypeDef",
     "UpdateDomainConfigResponseTypeDef",
 )
 
+_RequiredAWSDomainInformationOutputTypeDef = TypedDict(
+    "_RequiredAWSDomainInformationOutputTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalAWSDomainInformationOutputTypeDef = TypedDict(
+    "_OptionalAWSDomainInformationOutputTypeDef",
+    {
+        "OwnerId": str,
+        "Region": str,
+    },
+    total=False,
+)
+
+class AWSDomainInformationOutputTypeDef(
+    _RequiredAWSDomainInformationOutputTypeDef, _OptionalAWSDomainInformationOutputTypeDef
+):
+    pass
+
 _RequiredAWSDomainInformationTypeDef = TypedDict(
     "_RequiredAWSDomainInformationTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalAWSDomainInformationTypeDef = TypedDict(
@@ -294,14 +337,25 @@
 AcceptInboundConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
 )
 
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -377,14 +431,23 @@
         "ActionType": ScheduledAutoTuneActionTypeType,
         "Action": str,
         "Severity": ScheduledAutoTuneSeverityTypeType,
     },
     total=False,
 )
 
+DurationOutputTypeDef = TypedDict(
+    "DurationOutputTypeDef",
+    {
+        "Value": int,
+        "Unit": Literal["HOURS"],
+    },
+    total=False,
+)
+
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
@@ -472,14 +535,29 @@
         "Status": str,
         "Description": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
+ColdStorageOptionsOutputTypeDef = TypedDict(
+    "ColdStorageOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+
+ZoneAwarenessConfigOutputTypeDef = TypedDict(
+    "ZoneAwarenessConfigOutputTypeDef",
+    {
+        "AvailabilityZoneCount": int,
+    },
+    total=False,
+)
+
 ColdStorageOptionsTypeDef = TypedDict(
     "ColdStorageOptionsTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -487,14 +565,25 @@
     "ZoneAwarenessConfigTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
+CognitoOptionsOutputTypeDef = TypedDict(
+    "CognitoOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "UserPoolId": str,
+        "IdentityPoolId": str,
+        "RoleArn": str,
+    },
+    total=False,
+)
+
 CognitoOptionsTypeDef = TypedDict(
     "CognitoOptionsTypeDef",
     {
         "Enabled": bool,
         "UserPoolId": str,
         "IdentityPoolId": str,
         "RoleArn": str,
@@ -507,14 +596,22 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
+CrossClusterSearchConnectionPropertiesOutputTypeDef = TypedDict(
+    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
+    {
+        "SkipUnavailable": SkipUnavailableStatusType,
+    },
+    total=False,
+)
+
 CrossClusterSearchConnectionPropertiesTypeDef = TypedDict(
     "CrossClusterSearchConnectionPropertiesTypeDef",
     {
         "SkipUnavailable": SkipUnavailableStatusType,
     },
     total=False,
 )
@@ -859,14 +956,26 @@
     "DissociatePackageRequestRequestTypeDef",
     {
         "PackageID": str,
         "DomainName": str,
     },
 )
 
+DomainEndpointOptionsOutputTypeDef = TypedDict(
+    "DomainEndpointOptionsOutputTypeDef",
+    {
+        "EnforceHTTPS": bool,
+        "TLSSecurityPolicy": TLSSecurityPolicyType,
+        "CustomEndpointEnabled": bool,
+        "CustomEndpoint": str,
+        "CustomEndpointCertificateArn": str,
+    },
+    total=False,
+)
+
 DomainInfoTypeDef = TypedDict(
     "DomainInfoTypeDef",
     {
         "DomainName": str,
         "EngineType": EngineTypeType,
     },
     total=False,
@@ -877,14 +986,68 @@
     {
         "ErrorType": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+EBSOptionsOutputTypeDef = TypedDict(
+    "EBSOptionsOutputTypeDef",
+    {
+        "EBSEnabled": bool,
+        "VolumeType": VolumeTypeType,
+        "VolumeSize": int,
+        "Iops": int,
+        "Throughput": int,
+    },
+    total=False,
+)
+
+EncryptionAtRestOptionsOutputTypeDef = TypedDict(
+    "EncryptionAtRestOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+LogPublishingOptionOutputTypeDef = TypedDict(
+    "LogPublishingOptionOutputTypeDef",
+    {
+        "CloudWatchLogsLogGroupArn": str,
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+NodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
+    "NodeToNodeEncryptionOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+SnapshotOptionsOutputTypeDef = TypedDict(
+    "SnapshotOptionsOutputTypeDef",
+    {
+        "AutomatedSnapshotStartHour": int,
+    },
+    total=False,
+)
+
+SoftwareUpdateOptionsOutputTypeDef = TypedDict(
+    "SoftwareUpdateOptionsOutputTypeDef",
+    {
+        "AutoSoftwareUpdateEnabled": bool,
+    },
+    total=False,
+)
+
 VPCDerivedInfoTypeDef = TypedDict(
     "VPCDerivedInfoTypeDef",
     {
         "VPCId": str,
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
@@ -897,21 +1060,14 @@
     {
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCompatibleVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -970,24 +1126,14 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InboundConnectionStatusTypeDef = TypedDict(
     "InboundConnectionStatusTypeDef",
     {
         "StatusCode": InboundConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -1139,30 +1285,29 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ARN": str,
     },
 )
 
-ListVersionsRequestRequestTypeDef = TypedDict(
-    "ListVersionsRequestRequestTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
+ListVersionsRequestRequestTypeDef = TypedDict(
+    "ListVersionsRequestRequestTypeDef",
     {
-        "Versions": List[str],
+        "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
 _RequiredListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
     },
@@ -1205,14 +1350,22 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+WindowStartTimeOutputTypeDef = TypedDict(
+    "WindowStartTimeOutputTypeDef",
+    {
+        "Hours": int,
+        "Minutes": int,
+    },
+)
+
 WindowStartTimeTypeDef = TypedDict(
     "WindowStartTimeTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
@@ -1234,23 +1387,14 @@
 
 class PurchaseReservedInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
-PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
-    {
-        "ReservedInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1267,33 +1411,30 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
     },
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
 
+SAMLIdpOutputTypeDef = TypedDict(
+    "SAMLIdpOutputTypeDef",
+    {
+        "MetadataContent": str,
+        "EntityId": str,
+    },
+)
+
 SAMLIdpTypeDef = TypedDict(
     "SAMLIdpTypeDef",
     {
         "MetadataContent": str,
         "EntityId": str,
     },
 )
@@ -1379,22 +1520,65 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
+DomainInformationContainerOutputTypeDef = TypedDict(
+    "DomainInformationContainerOutputTypeDef",
+    {
+        "AWSDomainInformation": AWSDomainInformationOutputTypeDef,
+    },
+    total=False,
+)
+
 DomainInformationContainerTypeDef = TypedDict(
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "Versions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
+    {
+        "ReservedInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1419,47 +1603,49 @@
     "AddTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
+    {
+        "StartAt": datetime,
+        "Duration": DurationOutputTypeDef,
+        "CronExpressionForRecurrence": str,
+    },
+    total=False,
+)
+
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": Union[datetime, str],
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
@@ -1474,36 +1660,36 @@
     total=False,
 )
 
 CancelServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpgradeDomainResponseTypeDef = TypedDict(
     "UpgradeDomainResponseTypeDef",
     {
         "UpgradeId": str,
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "AdvancedOptions": Dict[str, str],
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1513,14 +1699,33 @@
         "CompletedProperties": List[str],
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
+ClusterConfigOutputTypeDef = TypedDict(
+    "ClusterConfigOutputTypeDef",
+    {
+        "InstanceType": OpenSearchPartitionInstanceTypeType,
+        "InstanceCount": int,
+        "DedicatedMasterEnabled": bool,
+        "ZoneAwarenessEnabled": bool,
+        "ZoneAwarenessConfig": ZoneAwarenessConfigOutputTypeDef,
+        "DedicatedMasterType": OpenSearchPartitionInstanceTypeType,
+        "DedicatedMasterCount": int,
+        "WarmEnabled": bool,
+        "WarmType": OpenSearchWarmPartitionInstanceTypeType,
+        "WarmCount": int,
+        "ColdStorageOptions": ColdStorageOptionsOutputTypeDef,
+        "MultiAZWithStandbyEnabled": bool,
+    },
+    total=False,
+)
+
 ClusterConfigTypeDef = TypedDict(
     "ClusterConfigTypeDef",
     {
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "InstanceCount": int,
         "DedicatedMasterEnabled": bool,
         "ZoneAwarenessEnabled": bool,
@@ -1535,90 +1740,41 @@
     },
     total=False,
 )
 
 CognitoOptionsStatusTypeDef = TypedDict(
     "CognitoOptionsStatusTypeDef",
     {
-        "Options": CognitoOptionsTypeDef,
+        "Options": CognitoOptionsOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConnectionPropertiesTypeDef = TypedDict(
-    "ConnectionPropertiesTypeDef",
+ConnectionPropertiesOutputTypeDef = TypedDict(
+    "ConnectionPropertiesOutputTypeDef",
     {
         "Endpoint": str,
-        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-DomainEndpointOptionsStatusTypeDef = TypedDict(
-    "DomainEndpointOptionsStatusTypeDef",
-    {
-        "Options": DomainEndpointOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-EBSOptionsStatusTypeDef = TypedDict(
-    "EBSOptionsStatusTypeDef",
-    {
-        "Options": EBSOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-EncryptionAtRestOptionsStatusTypeDef = TypedDict(
-    "EncryptionAtRestOptionsStatusTypeDef",
-    {
-        "Options": EncryptionAtRestOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-LogPublishingOptionsStatusTypeDef = TypedDict(
-    "LogPublishingOptionsStatusTypeDef",
-    {
-        "Options": Dict[LogTypeType, LogPublishingOptionTypeDef],
-        "Status": OptionStatusTypeDef,
-    },
-    total=False,
-)
-
-NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    {
-        "Options": NodeToNodeEncryptionOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SnapshotOptionsStatusTypeDef = TypedDict(
-    "SnapshotOptionsStatusTypeDef",
-    {
-        "Options": SnapshotOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SoftwareUpdateOptionsStatusTypeDef = TypedDict(
-    "SoftwareUpdateOptionsStatusTypeDef",
+ConnectionPropertiesTypeDef = TypedDict(
+    "ConnectionPropertiesTypeDef",
     {
-        "Options": SoftwareUpdateOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
+        "Endpoint": str,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointRequestRequestTypeDef",
     {
@@ -1689,41 +1845,41 @@
 ):
     pass
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainNodesResponseTypeDef = TypedDict(
     "DescribeDomainNodesResponseTypeDef",
     {
         "DomainNodesStatusList": List[DomainNodesStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1749,19 +1905,27 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DomainEndpointOptionsStatusTypeDef = TypedDict(
+    "DomainEndpointOptionsStatusTypeDef",
+    {
+        "Options": DomainEndpointOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1789,14 +1953,64 @@
         "LastUpdatedAt": datetime,
         "AvailablePackageVersion": str,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
+EBSOptionsStatusTypeDef = TypedDict(
+    "EBSOptionsStatusTypeDef",
+    {
+        "Options": EBSOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+EncryptionAtRestOptionsStatusTypeDef = TypedDict(
+    "EncryptionAtRestOptionsStatusTypeDef",
+    {
+        "Options": EncryptionAtRestOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+LogPublishingOptionsStatusTypeDef = TypedDict(
+    "LogPublishingOptionsStatusTypeDef",
+    {
+        "Options": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
+NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    {
+        "Options": NodeToNodeEncryptionOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SnapshotOptionsStatusTypeDef = TypedDict(
+    "SnapshotOptionsStatusTypeDef",
+    {
+        "Options": SnapshotOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SoftwareUpdateOptionsStatusTypeDef = TypedDict(
+    "SoftwareUpdateOptionsStatusTypeDef",
+    {
+        "Options": SoftwareUpdateOptionsOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
 VPCDerivedInfoStatusTypeDef = TypedDict(
     "VPCDerivedInfoStatusTypeDef",
     {
         "Options": VPCDerivedInfoTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1838,15 +2052,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceLimitsTypeDef = TypedDict(
     "InstanceLimitsTypeDef",
     {
         "InstanceCountLimits": InstanceCountLimitsTypeDef,
@@ -1855,35 +2069,51 @@
 )
 
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OffPeakWindowOutputTypeDef = TypedDict(
+    "OffPeakWindowOutputTypeDef",
+    {
+        "WindowStartTime": WindowStartTimeOutputTypeDef,
+    },
+    total=False,
+)
+
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
     },
     total=False,
 )
@@ -1920,33 +2150,33 @@
         "State": str,
         "PaymentOption": ReservedInstancePaymentOptionType,
         "RecurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
-SAMLOptionsInputTypeDef = TypedDict(
-    "SAMLOptionsInputTypeDef",
+SAMLOptionsOutputTypeDef = TypedDict(
+    "SAMLOptionsOutputTypeDef",
     {
         "Enabled": bool,
-        "Idp": SAMLIdpTypeDef,
-        "MasterUserName": str,
-        "MasterBackendRole": str,
+        "Idp": SAMLIdpOutputTypeDef,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
-SAMLOptionsOutputTypeDef = TypedDict(
-    "SAMLOptionsOutputTypeDef",
+SAMLOptionsInputTypeDef = TypedDict(
+    "SAMLOptionsInputTypeDef",
     {
         "Enabled": bool,
         "Idp": SAMLIdpTypeDef,
+        "MasterUserName": str,
+        "MasterBackendRole": str,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
@@ -1970,16 +2200,16 @@
     },
     total=False,
 )
 
 InboundConnectionTypeDef = TypedDict(
     "InboundConnectionTypeDef",
     {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
         "ConnectionId": str,
         "ConnectionStatus": InboundConnectionStatusTypeDef,
         "ConnectionMode": ConnectionModeType,
     },
     total=False,
 )
 
@@ -1988,14 +2218,25 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsExtraOutputTypeDef = TypedDict(
+    "AutoTuneOptionsExtraOutputTypeDef",
+    {
+        "DesiredState": AutoTuneDesiredStateType,
+        "RollbackOnDisable": RollbackOnDisableType,
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
+        "UseOffPeakWindow": bool,
+    },
+    total=False,
+)
+
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
@@ -2003,15 +2244,15 @@
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
@@ -2025,223 +2266,232 @@
         "MasterEligibleNodeCount": str,
         "WarmNodeCount": str,
         "MasterNode": MasterNodeStatusType,
         "ClusterHealth": DomainHealthType,
         "TotalShards": str,
         "TotalUnAssignedShards": str,
         "EnvironmentInformation": List[EnvironmentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
-        "Options": ClusterConfigTypeDef,
+        "Options": ClusterConfigOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
-_RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
+CreateOutboundConnectionResponseTypeDef = TypedDict(
+    "CreateOutboundConnectionResponseTypeDef",
     {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
         "ConnectionAlias": str,
-    },
-)
-_OptionalCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOutboundConnectionRequestRequestTypeDef",
-    {
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionId": str,
         "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
+        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateOutboundConnectionRequestRequestTypeDef(
-    _RequiredCreateOutboundConnectionRequestRequestTypeDef,
-    _OptionalCreateOutboundConnectionRequestRequestTypeDef,
-):
-    pass
-
-CreateOutboundConnectionResponseTypeDef = TypedDict(
-    "CreateOutboundConnectionResponseTypeDef",
+OutboundConnectionTypeDef = TypedDict(
+    "OutboundConnectionTypeDef",
     {
-        "LocalDomainInfo": DomainInformationContainerTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
+        "ConnectionId": str,
         "ConnectionAlias": str,
         "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionId": str,
         "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
     },
+    total=False,
 )
 
-OutboundConnectionTypeDef = TypedDict(
-    "OutboundConnectionTypeDef",
+_RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
-        "ConnectionId": str,
         "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+    },
+)
+_OptionalCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOutboundConnectionRequestRequestTypeDef",
+    {
         "ConnectionMode": ConnectionModeType,
         "ConnectionProperties": ConnectionPropertiesTypeDef,
     },
     total=False,
 )
 
+class CreateOutboundConnectionRequestRequestTypeDef(
+    _RequiredCreateOutboundConnectionRequestRequestTypeDef,
+    _OptionalCreateOutboundConnectionRequestRequestTypeDef,
+):
+    pass
+
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OffPeakWindowOptionsOutputTypeDef = TypedDict(
+    "OffPeakWindowOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "OffPeakWindow": OffPeakWindowOutputTypeDef,
+    },
+    total=False,
+)
+
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
         "OffPeakWindow": OffPeakWindowTypeDef,
     },
     total=False,
 )
 
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdvancedSecurityOptionsInputTypeDef = TypedDict(
-    "AdvancedSecurityOptionsInputTypeDef",
+AdvancedSecurityOptionsTypeDef = TypedDict(
+    "AdvancedSecurityOptionsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "MasterUserOptions": MasterUserOptionsTypeDef,
-        "SAMLOptions": SAMLOptionsInputTypeDef,
+        "SAMLOptions": SAMLOptionsOutputTypeDef,
+        "AnonymousAuthDisableDate": datetime,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
-AdvancedSecurityOptionsTypeDef = TypedDict(
-    "AdvancedSecurityOptionsTypeDef",
+AdvancedSecurityOptionsInputTypeDef = TypedDict(
+    "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "SAMLOptions": SAMLOptionsOutputTypeDef,
-        "AnonymousAuthDisableDate": datetime,
+        "MasterUserOptions": MasterUserOptionsTypeDef,
+        "SAMLOptions": SAMLOptionsInputTypeDef,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
 LimitsTypeDef = TypedDict(
     "LimitsTypeDef",
@@ -2254,95 +2504,145 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInboundConnectionResponseTypeDef = TypedDict(
     "DeleteInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsTypeDef,
+        "Options": AutoTuneOptionsExtraOutputTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOutboundConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundConnectionsResponseTypeDef",
     {
         "Connections": List[OutboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
-        "Options": OffPeakWindowOptionsTypeDef,
+        "Options": OffPeakWindowOptionsOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
     total=False,
 )
 
+AdvancedSecurityOptionsStatusTypeDef = TypedDict(
+    "AdvancedSecurityOptionsStatusTypeDef",
+    {
+        "Options": AdvancedSecurityOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+_RequiredDomainStatusTypeDef = TypedDict(
+    "_RequiredDomainStatusTypeDef",
+    {
+        "DomainId": str,
+        "DomainName": str,
+        "ARN": str,
+        "ClusterConfig": ClusterConfigOutputTypeDef,
+    },
+)
+_OptionalDomainStatusTypeDef = TypedDict(
+    "_OptionalDomainStatusTypeDef",
+    {
+        "Created": bool,
+        "Deleted": bool,
+        "Endpoint": str,
+        "Endpoints": Dict[str, str],
+        "Processing": bool,
+        "UpgradeProcessing": bool,
+        "EngineVersion": str,
+        "EBSOptions": EBSOptionsOutputTypeDef,
+        "AccessPolicies": str,
+        "SnapshotOptions": SnapshotOptionsOutputTypeDef,
+        "VPCOptions": VPCDerivedInfoTypeDef,
+        "CognitoOptions": CognitoOptionsOutputTypeDef,
+        "EncryptionAtRestOptions": EncryptionAtRestOptionsOutputTypeDef,
+        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsOutputTypeDef,
+        "AdvancedOptions": Dict[str, str],
+        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
+        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
+        "DomainEndpointOptions": DomainEndpointOptionsOutputTypeDef,
+        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
+        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
+        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsOutputTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
+    pass
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
@@ -2406,69 +2706,19 @@
 
 class UpdateDomainConfigRequestRequestTypeDef(
     _RequiredUpdateDomainConfigRequestRequestTypeDef,
     _OptionalUpdateDomainConfigRequestRequestTypeDef,
 ):
     pass
 
-AdvancedSecurityOptionsStatusTypeDef = TypedDict(
-    "AdvancedSecurityOptionsStatusTypeDef",
-    {
-        "Options": AdvancedSecurityOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-_RequiredDomainStatusTypeDef = TypedDict(
-    "_RequiredDomainStatusTypeDef",
-    {
-        "DomainId": str,
-        "DomainName": str,
-        "ARN": str,
-        "ClusterConfig": ClusterConfigTypeDef,
-    },
-)
-_OptionalDomainStatusTypeDef = TypedDict(
-    "_OptionalDomainStatusTypeDef",
-    {
-        "Created": bool,
-        "Deleted": bool,
-        "Endpoint": str,
-        "Endpoints": Dict[str, str],
-        "Processing": bool,
-        "UpgradeProcessing": bool,
-        "EngineVersion": str,
-        "EBSOptions": EBSOptionsTypeDef,
-        "AccessPolicies": str,
-        "SnapshotOptions": SnapshotOptionsTypeDef,
-        "VPCOptions": VPCDerivedInfoTypeDef,
-        "CognitoOptions": CognitoOptionsTypeDef,
-        "EncryptionAtRestOptions": EncryptionAtRestOptionsTypeDef,
-        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
-        "AdvancedOptions": Dict[str, str],
-        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionTypeDef],
-        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
-        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
-        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
-        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
-        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
-    },
-    total=False,
-)
-
-class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
-    pass
-
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainConfigTypeDef = TypedDict(
     "DomainConfigTypeDef",
     {
         "EngineVersion": VersionStatusTypeDef,
@@ -2492,62 +2742,62 @@
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDryRunProgressResponseTypeDef = TypedDict(
     "DescribeDryRunProgressResponseTypeDef",
     {
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
         "DryRunConfig": DomainStatusTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainConfigResponseTypeDef = TypedDict(
     "DescribeDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainConfigResponseTypeDef = TypedDict(
     "UpdateDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/PKG-INFO` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.0
-Summary: Type annotations for boto3.OpenSearchService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpenSearchService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opensearch"></a>
 
 # mypy-boto3-opensearch
 
 [![PyPI - mypy-boto3-opensearch](https://img.shields.io/pypi/v/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,36 +338,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
+    AWSDomainInformationOutputTypeDef,
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
+    DurationOutputTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
+    ColdStorageOptionsOutputTypeDef,
+    ZoneAwarenessConfigOutputTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
+    CognitoOptionsOutputTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
+    CrossClusterSearchConnectionPropertiesOutputTypeDef,
     CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
@@ -395,163 +402,179 @@
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
     DescribeReservedInstanceOfferingsRequestRequestTypeDef,
     DescribeReservedInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
+    DomainEndpointOptionsOutputTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
+    EBSOptionsOutputTypeDef,
+    EncryptionAtRestOptionsOutputTypeDef,
+    LogPublishingOptionOutputTypeDef,
+    NodeToNodeEncryptionOptionsOutputTypeDef,
+    SnapshotOptionsOutputTypeDef,
+    SoftwareUpdateOptionsOutputTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    WindowStartTimeOutputTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
+    SAMLIdpOutputTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
+    DomainInformationContainerOutputTypeDef,
     DomainInformationContainerTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListVersionsResponseTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
+    ClusterConfigOutputTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
+    ConnectionPropertiesOutputTypeDef,
     ConnectionPropertiesTypeDef,
-    DomainEndpointOptionsStatusTypeDef,
-    EBSOptionsStatusTypeDef,
-    EncryptionAtRestOptionsStatusTypeDef,
-    LogPublishingOptionsStatusTypeDef,
-    NodeToNodeEncryptionOptionsStatusTypeDef,
-    SnapshotOptionsStatusTypeDef,
-    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
+    DomainEndpointOptionsStatusTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
+    EBSOptionsStatusTypeDef,
+    EncryptionAtRestOptionsStatusTypeDef,
+    LogPublishingOptionsStatusTypeDef,
+    NodeToNodeEncryptionOptionsStatusTypeDef,
+    SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListScheduledActionsResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
+    ListTagsResponseTypeDef,
+    OffPeakWindowOutputTypeDef,
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
-    SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
+    SAMLOptionsInputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     OutboundConnectionTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
+    OffPeakWindowOptionsOutputTypeDef,
     OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
-    AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
+    AdvancedSecurityOptionsInputTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainConfigRequestRequestTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_structure() -> AWSDomainInformationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.0/mypy_boto3_opensearch.egg-info/SOURCES.txt` & `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.0/setup.py` & `mypy-boto3-opensearch-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearch",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.OpenSearchService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

