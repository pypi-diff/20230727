# Comparing `tmp/mypy-boto3-guardduty-1.28.0.tar.gz` & `tmp/mypy-boto3-guardduty-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-guardduty-1.28.0.tar", last modified: Thu Jul  6 20:59:41 2023, max compression
+gzip compressed data, was "mypy-boto3-guardduty-1.28.12.tar", last modified: Thu Jul 27 05:34:45 2023, max compression
```

## Comparing `mypy-boto3-guardduty-1.28.0.tar` & `mypy-boto3-guardduty-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:41.306316 mypy-boto3-guardduty-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-07-06 20:59:41.302316 mypy-boto3-guardduty-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24354 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:41.302316 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49732 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49647 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-06 20:42:29.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-07-06 20:42:29.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93093 2023-07-06 20:42:31.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93006 2023-07-06 20:42:30.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:41.302316 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-07-06 20:59:41.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 20:59:41.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:41.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:41.000000 mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:41.306316 mypy-boto3-guardduty-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:42:28.000000 mypy-boto3-guardduty-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.324497 mypy-boto3-guardduty-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-07-27 05:34:45.320497 mypy-boto3-guardduty-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.316497 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49732 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49647 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94960 2023-07-27 05:23:16.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94871 2023-07-27 05:23:14.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.320497 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:45.324497 mypy-boto3-guardduty-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/setup.py
```

### Comparing `mypy-boto3-guardduty-1.28.0/LICENSE` & `mypy-boto3-guardduty-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/PKG-INFO` & `mypy-boto3-guardduty-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.0
-Summary: Type annotations for boto3.GuardDuty 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GuardDuty 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-guardduty"></a>
 
 # mypy-boto3-guardduty
 
 [![PyPI - mypy-boto3-guardduty](https://img.shields.io/pypi/v/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,14 +407,15 @@
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
@@ -440,14 +441,15 @@
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
+    DestinationPropertiesOutputTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
@@ -526,14 +528,15 @@
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
     PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
     ResponseMetadataTypeDef,
+    ScanConditionPairOutputTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
@@ -551,33 +554,34 @@
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
-    DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
     GetFindingsRequestRequestTypeDef,
+    DescribePublishingDestinationResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
@@ -601,25 +605,26 @@
     OrganizationFeatureConfigurationResultTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
+    ScanConditionOutputTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
-    CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -633,14 +638,15 @@
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
     CoverageResourceTypeDef,
     PublicAccessTypeDef,
     GetCoverageStatisticsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.28.0/README.md` & `mypy-boto3-guardduty-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-guardduty"></a>
 
 # mypy-boto3-guardduty
 
 [![PyPI - mypy-boto3-guardduty](https://img.shields.io/pypi/v/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,14 +375,15 @@
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
@@ -408,14 +409,15 @@
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
+    DestinationPropertiesOutputTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
@@ -494,14 +496,15 @@
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
     PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
     ResponseMetadataTypeDef,
+    ScanConditionPairOutputTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
@@ -519,33 +522,34 @@
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
-    DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
     GetFindingsRequestRequestTypeDef,
+    DescribePublishingDestinationResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
@@ -569,25 +573,26 @@
     OrganizationFeatureConfigurationResultTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
+    ScanConditionOutputTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
-    CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -601,14 +606,15 @@
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
     CoverageResourceTypeDef,
     PublicAccessTypeDef,
     GetCoverageStatisticsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/__init__.py` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/__init__.pyi` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/__main__.py` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GuardDuty 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.GuardDuty 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
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

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/client.py` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/client.pyi` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/literals.py` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,15 @@
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
@@ -392,26 +393,28 @@
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

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/literals.pyi` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.pyi`

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

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/paginator.py` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/paginator.pyi` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/type_defs.py` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
@@ -106,14 +107,15 @@
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
+    "DestinationPropertiesOutputTypeDef",
     "DestinationTypeDef",
     "DetectorAdditionalConfigurationResultTypeDef",
     "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateFromAdministratorAccountRequestRequestTypeDef",
     "DisassociateFromMasterAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
@@ -192,14 +194,15 @@
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
     "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
     "ResponseMetadataTypeDef",
+    "ScanConditionPairOutputTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
@@ -217,33 +220,34 @@
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
     "GetCoverageStatisticsResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
-    "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     "GetFindingsRequestRequestTypeDef",
+    "DescribePublishingDestinationResponseTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
     "DetectorFeatureConfigurationResultTypeDef",
     "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
     "RdsDbInstanceDetailsTypeDef",
@@ -267,25 +271,26 @@
     "OrganizationFeatureConfigurationResultTypeDef",
     "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
+    "ScanConditionOutputTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
-    "CreateFilterRequestRequestTypeDef",
     "GetFilterResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -299,14 +304,15 @@
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
+    "ScanResourceCriteriaOutputTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
     "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
     "GetCoverageStatisticsRequestRequestTypeDef",
@@ -497,14 +503,33 @@
 CloudTrailConfigurationResultTypeDef = TypedDict(
     "CloudTrailConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "Eq": List[str],
+        "Neq": List[str],
+        "Gt": int,
+        "Gte": int,
+        "Lt": int,
+        "Lte": int,
+        "Equals": List[str],
+        "NotEquals": List[str],
+        "GreaterThan": int,
+        "GreaterThanOrEqual": int,
+        "LessThan": int,
+        "LessThanOrEqual": int,
+    },
+    total=False,
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "Eq": Sequence[str],
         "Neq": Sequence[str],
         "Gt": int,
         "Gte": int,
@@ -839,14 +864,23 @@
     "DescribePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
 
+DestinationPropertiesOutputTypeDef = TypedDict(
+    "DestinationPropertiesOutputTypeDef",
+    {
+        "DestinationArn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
     },
@@ -1768,14 +1802,35 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredScanConditionPairOutputTypeDef = TypedDict(
+    "_RequiredScanConditionPairOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalScanConditionPairOutputTypeDef = TypedDict(
+    "_OptionalScanConditionPairOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class ScanConditionPairOutputTypeDef(
+    _RequiredScanConditionPairOutputTypeDef, _OptionalScanConditionPairOutputTypeDef
+):
+    pass
+
+
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
@@ -2043,14 +2098,22 @@
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "Criterion": Dict[str, ConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "Criterion": Mapping[str, ConditionTypeDef],
     },
     total=False,
 )
@@ -2178,26 +2241,14 @@
 class CreatePublishingDestinationRequestRequestTypeDef(
     _RequiredCreatePublishingDestinationRequestRequestTypeDef,
     _OptionalCreatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
 
-DescribePublishingDestinationResponseTypeDef = TypedDict(
-    "DescribePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "DestinationType": Literal["S3"],
-        "Status": PublishingStatusType,
-        "PublishingFailureStartTimestamp": int,
-        "DestinationProperties": DestinationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
@@ -2251,14 +2302,26 @@
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
 
+DescribePublishingDestinationResponseTypeDef = TypedDict(
+    "DescribePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "DestinationType": Literal["S3"],
+        "Status": PublishingStatusType,
+        "PublishingFailureStartTimestamp": int,
+        "DestinationProperties": DestinationPropertiesOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2571,18 +2634,25 @@
         "GeoLocation": GeoLocationTypeDef,
         "IpAddressV4": str,
         "Organization": OrganizationTypeDef,
     },
     total=False,
 )
 
+ScanConditionOutputTypeDef = TypedDict(
+    "ScanConditionOutputTypeDef",
+    {
+        "MapEquals": List[ScanConditionPairOutputTypeDef],
+    },
+)
+
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
-        "MapEquals": List[ScanConditionPairTypeDef],
+        "MapEquals": Sequence[ScanConditionPairTypeDef],
     },
 )
 
 ScanThreatNameTypeDef = TypedDict(
     "ScanThreatNameTypeDef",
     {
         "Name": str,
@@ -2665,14 +2735,27 @@
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
 )
 
+GetFilterResponseTypeDef = TypedDict(
+    "GetFilterResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Action": FilterActionType,
+        "Rank": int,
+        "FindingCriteria": FindingCriteriaOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
@@ -2692,27 +2775,14 @@
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
 
-GetFilterResponseTypeDef = TypedDict(
-    "GetFilterResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Action": FilterActionType,
-        "Rank": int,
-        "FindingCriteria": FindingCriteriaTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -3022,19 +3092,28 @@
     {
         "RemoteIpDetails": RemoteIpDetailsTypeDef,
         "LoginAttributes": List[LoginAttributeTypeDef],
     },
     total=False,
 )
 
+ScanResourceCriteriaOutputTypeDef = TypedDict(
+    "ScanResourceCriteriaOutputTypeDef",
+    {
+        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 ScanResourceCriteriaTypeDef = TypedDict(
     "ScanResourceCriteriaTypeDef",
     {
-        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
-        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Include": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Exclude": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
     },
     total=False,
 )
 
 ThreatDetectedByNameTypeDef = TypedDict(
     "ThreatDetectedByNameTypeDef",
     {
@@ -3400,15 +3479,15 @@
     },
     total=False,
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
-        "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
+        "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
```

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty/type_defs.pyi` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
@@ -105,14 +106,15 @@
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
+    "DestinationPropertiesOutputTypeDef",
     "DestinationTypeDef",
     "DetectorAdditionalConfigurationResultTypeDef",
     "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateFromAdministratorAccountRequestRequestTypeDef",
     "DisassociateFromMasterAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
@@ -191,14 +193,15 @@
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
     "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
     "ResponseMetadataTypeDef",
+    "ScanConditionPairOutputTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
@@ -216,33 +219,34 @@
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
     "GetCoverageStatisticsResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
-    "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     "GetFindingsRequestRequestTypeDef",
+    "DescribePublishingDestinationResponseTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
     "DetectorFeatureConfigurationResultTypeDef",
     "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
     "RdsDbInstanceDetailsTypeDef",
@@ -266,25 +270,26 @@
     "OrganizationFeatureConfigurationResultTypeDef",
     "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
+    "ScanConditionOutputTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
-    "CreateFilterRequestRequestTypeDef",
     "GetFilterResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -298,14 +303,15 @@
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
+    "ScanResourceCriteriaOutputTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
     "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
     "GetCoverageStatisticsRequestRequestTypeDef",
@@ -496,14 +502,33 @@
 CloudTrailConfigurationResultTypeDef = TypedDict(
     "CloudTrailConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "Eq": List[str],
+        "Neq": List[str],
+        "Gt": int,
+        "Gte": int,
+        "Lt": int,
+        "Lte": int,
+        "Equals": List[str],
+        "NotEquals": List[str],
+        "GreaterThan": int,
+        "GreaterThanOrEqual": int,
+        "LessThan": int,
+        "LessThanOrEqual": int,
+    },
+    total=False,
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "Eq": Sequence[str],
         "Neq": Sequence[str],
         "Gt": int,
         "Gte": int,
@@ -830,14 +855,23 @@
     "DescribePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
 
+DestinationPropertiesOutputTypeDef = TypedDict(
+    "DestinationPropertiesOutputTypeDef",
+    {
+        "DestinationArn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
     },
@@ -1735,14 +1769,33 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredScanConditionPairOutputTypeDef = TypedDict(
+    "_RequiredScanConditionPairOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalScanConditionPairOutputTypeDef = TypedDict(
+    "_OptionalScanConditionPairOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class ScanConditionPairOutputTypeDef(
+    _RequiredScanConditionPairOutputTypeDef, _OptionalScanConditionPairOutputTypeDef
+):
+    pass
+
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
@@ -2002,14 +2055,22 @@
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "Criterion": Dict[str, ConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "Criterion": Mapping[str, ConditionTypeDef],
     },
     total=False,
 )
@@ -2135,26 +2196,14 @@
 
 class CreatePublishingDestinationRequestRequestTypeDef(
     _RequiredCreatePublishingDestinationRequestRequestTypeDef,
     _OptionalCreatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
-DescribePublishingDestinationResponseTypeDef = TypedDict(
-    "DescribePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "DestinationType": Literal["S3"],
-        "Status": PublishingStatusType,
-        "PublishingFailureStartTimestamp": int,
-        "DestinationProperties": DestinationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
@@ -2204,14 +2253,26 @@
 )
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
+DescribePublishingDestinationResponseTypeDef = TypedDict(
+    "DescribePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "DestinationType": Literal["S3"],
+        "Status": PublishingStatusType,
+        "PublishingFailureStartTimestamp": int,
+        "DestinationProperties": DestinationPropertiesOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2522,18 +2583,25 @@
         "GeoLocation": GeoLocationTypeDef,
         "IpAddressV4": str,
         "Organization": OrganizationTypeDef,
     },
     total=False,
 )
 
+ScanConditionOutputTypeDef = TypedDict(
+    "ScanConditionOutputTypeDef",
+    {
+        "MapEquals": List[ScanConditionPairOutputTypeDef],
+    },
+)
+
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
-        "MapEquals": List[ScanConditionPairTypeDef],
+        "MapEquals": Sequence[ScanConditionPairTypeDef],
     },
 )
 
 ScanThreatNameTypeDef = TypedDict(
     "ScanThreatNameTypeDef",
     {
         "Name": str,
@@ -2616,14 +2684,27 @@
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
 )
 
+GetFilterResponseTypeDef = TypedDict(
+    "GetFilterResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Action": FilterActionType,
+        "Rank": int,
+        "FindingCriteria": FindingCriteriaOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
@@ -2641,27 +2722,14 @@
 )
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
-GetFilterResponseTypeDef = TypedDict(
-    "GetFilterResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Action": FilterActionType,
-        "Rank": int,
-        "FindingCriteria": FindingCriteriaTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -2963,19 +3031,28 @@
     {
         "RemoteIpDetails": RemoteIpDetailsTypeDef,
         "LoginAttributes": List[LoginAttributeTypeDef],
     },
     total=False,
 )
 
+ScanResourceCriteriaOutputTypeDef = TypedDict(
+    "ScanResourceCriteriaOutputTypeDef",
+    {
+        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 ScanResourceCriteriaTypeDef = TypedDict(
     "ScanResourceCriteriaTypeDef",
     {
-        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
-        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Include": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Exclude": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
     },
     total=False,
 )
 
 ThreatDetectedByNameTypeDef = TypedDict(
     "ThreatDetectedByNameTypeDef",
     {
@@ -3321,15 +3398,15 @@
     },
     total=False,
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
-        "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
+        "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
```

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/PKG-INFO` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.0
-Summary: Type annotations for boto3.GuardDuty 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GuardDuty 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-guardduty"></a>
 
 # mypy-boto3-guardduty
 
 [![PyPI - mypy-boto3-guardduty](https://img.shields.io/pypi/v/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-guardduty?color=blue)](https://pypistats.org/packages/mypy-boto3-guardduty)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,14 +407,15 @@
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
@@ -440,14 +441,15 @@
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
+    DestinationPropertiesOutputTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
@@ -526,14 +528,15 @@
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
     PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
     ResponseMetadataTypeDef,
+    ScanConditionPairOutputTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
@@ -551,33 +554,34 @@
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
-    DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
     GetFindingsRequestRequestTypeDef,
+    DescribePublishingDestinationResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
@@ -601,25 +605,26 @@
     OrganizationFeatureConfigurationResultTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
+    ScanConditionOutputTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
-    CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -633,14 +638,15 @@
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
     CoverageResourceTypeDef,
     PublicAccessTypeDef,
     GetCoverageStatisticsRequestRequestTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.28.0/mypy_boto3_guardduty.egg-info/SOURCES.txt` & `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.0/setup.py` & `mypy-boto3-guardduty-1.28.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-guardduty",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GuardDuty 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.GuardDuty 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

