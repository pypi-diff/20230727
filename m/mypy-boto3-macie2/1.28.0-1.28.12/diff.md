# Comparing `tmp/mypy-boto3-macie2-1.28.0.tar.gz` & `tmp/mypy-boto3-macie2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-macie2-1.28.0.tar", last modified: Thu Jul  6 21:00:02 2023, max compression
+gzip compressed data, was "mypy-boto3-macie2-1.28.12.tar", last modified: Thu Jul 27 05:34:58 2023, max compression
```

## Comparing `mypy-boto3-macie2-1.28.0.tar` & `mypy-boto3-macie2-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.506360 mypy-boto3-macie2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:25.000000 mypy-boto3-macie2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28611 2023-07-06 21:00:02.498360 mypy-boto3-macie2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-07-06 20:46:25.000000 mypy-boto3-macie2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.498360 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-06 20:46:26.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-06 20:46:26.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:46:26.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59831 2023-07-06 20:46:28.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59728 2023-07-06 20:46:28.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17346 2023-07-06 20:46:29.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-07-06 20:46:29.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19545 2023-07-06 20:46:28.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-06 20:46:28.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:26.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    88899 2023-07-06 20:46:31.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    88844 2023-07-06 20:46:30.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:25.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-06 20:46:28.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-06 20:46:28.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.498360 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28611 2023-07-06 21:00:02.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:02.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:02.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:02.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:02.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 21:00:02.000000 mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:02.506360 mypy-boto3-macie2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:46:25.000000 mypy-boto3-macie2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.576450 mypy-boto3-macie2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-07-27 05:34:58.572450 mypy-boto3-macie2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.564450 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59831 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59728 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19545 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    96345 2023-07-27 05:25:50.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96286 2023-07-27 05:25:47.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.572450 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:58.576450 mypy-boto3-macie2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:25:45.000000 mypy-boto3-macie2-1.28.12/setup.py
```

### Comparing `mypy-boto3-macie2-1.28.0/LICENSE` & `mypy-boto3-macie2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/PKG-INFO` & `mypy-boto3-macie2-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.28.0
-Summary: Type annotations for boto3.Macie2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Macie2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-macie2"></a>
 
 # mypy-boto3-macie2
 
 [![PyPI - mypy-boto3-macie2](https://img.shields.io/pypi/v/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie2?color=blue)](https://pypistats.org/packages/mypy-boto3-macie2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -467,14 +467,15 @@
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
     AdminAccountTypeDef,
+    S3WordsListOutputTypeDef,
     S3WordsListTypeDef,
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
@@ -490,27 +491,30 @@
     KeyValuePairTypeDef,
     ObjectCountByEncryptionTypeTypeDef,
     ObjectLevelStatisticsTypeDef,
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
+    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
     CreateAllowListResponseTypeDef,
     CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
     CreateCustomDataIdentifierResponseTypeDef,
     CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
     CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
+    SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
+    CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
@@ -532,45 +536,49 @@
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
+    SeverityLevelOutputTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
-    SecurityHubConfigurationTypeDef,
+    SecurityHubConfigurationOutputTypeDef,
     SortCriteriaTypeDef,
     GetInvitationsCountResponseTypeDef,
     GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
     GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
-    RevealConfigurationTypeDef,
+    RevealConfigurationOutputTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesOutputTypeDef,
+    SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
+    MonthlyScheduleOutputTypeDef,
+    WeeklyScheduleOutputTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
+    SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
-    S3BucketDefinitionForJobTypeDef,
+    S3BucketDefinitionForJobOutputTypeDef,
     ListAllowListsRequestListAllowListsPaginateTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
     ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
     ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
@@ -597,28 +605,35 @@
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
     PaginatorConfigTypeDef,
+    SecurityHubConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    RevealConfigurationTypeDef,
+    S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
+    TagCriterionPairForJobOutputTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagValuePairOutputTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
@@ -627,124 +642,137 @@
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    AllowListCriteriaOutputTypeDef,
     AllowListCriteriaTypeDef,
     ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
     DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
+    ClassificationExportConfigurationOutputTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
-    GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetCustomDataIdentifierResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
     GetFindingsPublicationConfigurationResponseTypeDef,
-    PutFindingsPublicationConfigurationRequestRequestTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
-    UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
-    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
+    JobScheduleFrequencyOutputTypeDef,
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
+    PutFindingsPublicationConfigurationRequestRequestTypeDef,
+    UpdateRevealConfigurationRequestRequestTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
+    TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
+    TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
-    CreateAllowListRequestRequestTypeDef,
     GetAllowListResponseTypeDef,
+    CreateAllowListRequestRequestTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
-    PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
+    PutClassificationExportConfigurationRequestRequestTypeDef,
+    GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
-    GetFindingsFilterResponseTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
     AssumedRoleTypeDef,
     FederatedUserTypeDef,
+    CriteriaForJobOutputTypeDef,
     CriteriaForJobTypeDef,
+    JobScopeTermOutputTypeDef,
     JobScopeTermTypeDef,
     BucketPublicAccessTypeDef,
     SearchResourcesResponseTypeDef,
     CustomDetectionTypeDef,
     DefaultDetectionTypeDef,
     SearchResourcesCriteriaBlockTypeDef,
     GetUsageStatisticsResponseTypeDef,
     UserIdentityTypeDef,
+    CriteriaBlockForJobOutputTypeDef,
     CriteriaBlockForJobTypeDef,
+    JobScopingBlockOutputTypeDef,
     JobScopingBlockTypeDef,
     BucketMetadataTypeDef,
     S3BucketTypeDef,
     CustomDataIdentifiersTypeDef,
     SensitiveDataItemTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     FindingActorTypeDef,
+    S3BucketCriteriaForJobOutputTypeDef,
     S3BucketCriteriaForJobTypeDef,
+    ScopingOutputTypeDef,
     ScopingTypeDef,
     DescribeBucketsResponseTypeDef,
     ResourcesAffectedTypeDef,
     ClassificationResultTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     PolicyDetailsTypeDef,
     JobSummaryTypeDef,
+    S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
-    CreateClassificationJobRequestRequestTypeDef,
     DescribeClassificationJobResponseTypeDef,
+    CreateClassificationJobRequestRequestTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-macie2-1.28.0/README.md` & `mypy-boto3-macie2-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-macie2"></a>
 
 # mypy-boto3-macie2
 
 [![PyPI - mypy-boto3-macie2](https://img.shields.io/pypi/v/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie2?color=blue)](https://pypistats.org/packages/mypy-boto3-macie2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -435,14 +435,15 @@
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
     AdminAccountTypeDef,
+    S3WordsListOutputTypeDef,
     S3WordsListTypeDef,
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
@@ -458,27 +459,30 @@
     KeyValuePairTypeDef,
     ObjectCountByEncryptionTypeTypeDef,
     ObjectLevelStatisticsTypeDef,
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
+    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
     CreateAllowListResponseTypeDef,
     CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
     CreateCustomDataIdentifierResponseTypeDef,
     CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
     CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
+    SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
+    CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
@@ -500,45 +504,49 @@
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
+    SeverityLevelOutputTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
-    SecurityHubConfigurationTypeDef,
+    SecurityHubConfigurationOutputTypeDef,
     SortCriteriaTypeDef,
     GetInvitationsCountResponseTypeDef,
     GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
     GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
-    RevealConfigurationTypeDef,
+    RevealConfigurationOutputTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesOutputTypeDef,
+    SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
+    MonthlyScheduleOutputTypeDef,
+    WeeklyScheduleOutputTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
+    SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
-    S3BucketDefinitionForJobTypeDef,
+    S3BucketDefinitionForJobOutputTypeDef,
     ListAllowListsRequestListAllowListsPaginateTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
     ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
     ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
@@ -565,28 +573,35 @@
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
     PaginatorConfigTypeDef,
+    SecurityHubConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    RevealConfigurationTypeDef,
+    S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
+    TagCriterionPairForJobOutputTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagValuePairOutputTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
@@ -595,124 +610,137 @@
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    AllowListCriteriaOutputTypeDef,
     AllowListCriteriaTypeDef,
     ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
     DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
+    ClassificationExportConfigurationOutputTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
-    GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetCustomDataIdentifierResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
     GetFindingsPublicationConfigurationResponseTypeDef,
-    PutFindingsPublicationConfigurationRequestRequestTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
-    UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
-    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
+    JobScheduleFrequencyOutputTypeDef,
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
+    PutFindingsPublicationConfigurationRequestRequestTypeDef,
+    UpdateRevealConfigurationRequestRequestTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
+    TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
+    TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
-    CreateAllowListRequestRequestTypeDef,
     GetAllowListResponseTypeDef,
+    CreateAllowListRequestRequestTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
-    PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
+    PutClassificationExportConfigurationRequestRequestTypeDef,
+    GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
-    GetFindingsFilterResponseTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
     AssumedRoleTypeDef,
     FederatedUserTypeDef,
+    CriteriaForJobOutputTypeDef,
     CriteriaForJobTypeDef,
+    JobScopeTermOutputTypeDef,
     JobScopeTermTypeDef,
     BucketPublicAccessTypeDef,
     SearchResourcesResponseTypeDef,
     CustomDetectionTypeDef,
     DefaultDetectionTypeDef,
     SearchResourcesCriteriaBlockTypeDef,
     GetUsageStatisticsResponseTypeDef,
     UserIdentityTypeDef,
+    CriteriaBlockForJobOutputTypeDef,
     CriteriaBlockForJobTypeDef,
+    JobScopingBlockOutputTypeDef,
     JobScopingBlockTypeDef,
     BucketMetadataTypeDef,
     S3BucketTypeDef,
     CustomDataIdentifiersTypeDef,
     SensitiveDataItemTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     FindingActorTypeDef,
+    S3BucketCriteriaForJobOutputTypeDef,
     S3BucketCriteriaForJobTypeDef,
+    ScopingOutputTypeDef,
     ScopingTypeDef,
     DescribeBucketsResponseTypeDef,
     ResourcesAffectedTypeDef,
     ClassificationResultTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     PolicyDetailsTypeDef,
     JobSummaryTypeDef,
+    S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
-    CreateClassificationJobRequestRequestTypeDef,
     DescribeClassificationJobResponseTypeDef,
+    CreateClassificationJobRequestRequestTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/__init__.py` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/__init__.pyi` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/__main__.py` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Macie2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Macie2 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
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

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/client.py` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/client.pyi` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/literals.py` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,14 +360,15 @@
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
@@ -446,26 +447,28 @@
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

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/literals.pyi` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -358,14 +358,15 @@
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
@@ -444,26 +445,28 @@
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

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/paginator.py` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/paginator.pyi` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/type_defs.py` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccountDetailTypeDef",
     "BlockPublicAccessTypeDef",
     "AdminAccountTypeDef",
+    "S3WordsListOutputTypeDef",
     "S3WordsListTypeDef",
     "AllowListStatusTypeDef",
     "AllowListSummaryTypeDef",
     "ApiCallDetailsTypeDef",
     "AwsAccountTypeDef",
     "AwsServiceTypeDef",
     "BatchGetCustomDataIdentifierSummaryTypeDef",
@@ -103,27 +104,30 @@
     "KeyValuePairTypeDef",
     "ObjectCountByEncryptionTypeTypeDef",
     "ObjectLevelStatisticsTypeDef",
     "ReplicationDetailsTypeDef",
     "BucketSortCriteriaTypeDef",
     "SensitivityAggregationsTypeDef",
     "CellTypeDef",
+    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
     "CreateAllowListResponseTypeDef",
     "CreateClassificationJobResponseTypeDef",
     "SeverityLevelTypeDef",
     "CreateCustomDataIdentifierResponseTypeDef",
     "CreateFindingsFilterResponseTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
     "CreateMemberResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
+    "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
+    "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
@@ -145,45 +149,49 @@
     "FindingsFilterListItemTypeDef",
     "InvitationTypeDef",
     "GetAllowListRequestRequestTypeDef",
     "GetAutomatedDiscoveryConfigurationResponseTypeDef",
     "GetBucketStatisticsRequestRequestTypeDef",
     "GetClassificationScopeRequestRequestTypeDef",
     "GetCustomDataIdentifierRequestRequestTypeDef",
+    "SeverityLevelOutputTypeDef",
     "GroupCountTypeDef",
     "GetFindingsFilterRequestRequestTypeDef",
-    "SecurityHubConfigurationTypeDef",
+    "SecurityHubConfigurationOutputTypeDef",
     "SortCriteriaTypeDef",
     "GetInvitationsCountResponseTypeDef",
     "GetMacieSessionResponseTypeDef",
     "GetMemberRequestRequestTypeDef",
     "GetMemberResponseTypeDef",
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
-    "RevealConfigurationTypeDef",
+    "RevealConfigurationOutputTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    "SensitivityInspectionTemplateIncludesTypeDef",
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
+    "MonthlyScheduleOutputTypeDef",
+    "WeeklyScheduleOutputTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
+    "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
-    "S3BucketDefinitionForJobTypeDef",
+    "S3BucketDefinitionForJobOutputTypeDef",
     "ListAllowListsRequestListAllowListsPaginateTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
     "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
     "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
@@ -210,28 +218,35 @@
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
     "PaginatorConfigTypeDef",
+    "SecurityHubConfigurationTypeDef",
     "ResponseMetadataTypeDef",
+    "RevealConfigurationTypeDef",
+    "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
+    "TagCriterionPairForJobOutputTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagValuePairOutputTypeDef",
     "TagValuePairTypeDef",
     "TestCustomDataIdentifierRequestRequestTypeDef",
     "TestCustomDataIdentifierResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAllowListResponseTypeDef",
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     "UpdateClassificationJobRequestRequestTypeDef",
@@ -240,124 +255,137 @@
     "UpdateMemberSessionRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateResourceProfileRequestRequestTypeDef",
     "UserIdentityRootTypeDef",
     "CreateMemberRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
+    "AllowListCriteriaOutputTypeDef",
     "AllowListCriteriaTypeDef",
     "ListAllowListsResponseTypeDef",
     "FindingActionTypeDef",
     "BatchGetCustomDataIdentifiersResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "MatchingBucketTypeDef",
     "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "DescribeBucketsRequestRequestTypeDef",
     "BucketStatisticsBySensitivityTypeDef",
+    "ClassificationExportConfigurationOutputTypeDef",
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
-    "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
     "GetSensitiveDataOccurrencesResponseTypeDef",
     "ListResourceProfileDetectionsResponseTypeDef",
     "ListFindingsFiltersResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
+    "GetCustomDataIdentifierResponseTypeDef",
     "GetFindingStatisticsResponseTypeDef",
     "GetFindingsPublicationConfigurationResponseTypeDef",
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
-    "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
-    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
+    "JobScheduleFrequencyOutputTypeDef",
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
+    "UpdateRevealConfigurationRequestRequestTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
+    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
+    "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
+    "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
-    "CreateAllowListRequestRequestTypeDef",
     "GetAllowListResponseTypeDef",
+    "CreateAllowListRequestRequestTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
-    "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
+    "PutClassificationExportConfigurationRequestRequestTypeDef",
+    "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
-    "GetFindingsFilterResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
     "AssumedRoleTypeDef",
     "FederatedUserTypeDef",
+    "CriteriaForJobOutputTypeDef",
     "CriteriaForJobTypeDef",
+    "JobScopeTermOutputTypeDef",
     "JobScopeTermTypeDef",
     "BucketPublicAccessTypeDef",
     "SearchResourcesResponseTypeDef",
     "CustomDetectionTypeDef",
     "DefaultDetectionTypeDef",
     "SearchResourcesCriteriaBlockTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "UserIdentityTypeDef",
+    "CriteriaBlockForJobOutputTypeDef",
     "CriteriaBlockForJobTypeDef",
+    "JobScopingBlockOutputTypeDef",
     "JobScopingBlockTypeDef",
     "BucketMetadataTypeDef",
     "S3BucketTypeDef",
     "CustomDataIdentifiersTypeDef",
     "SensitiveDataItemTypeDef",
     "SearchResourcesBucketCriteriaTypeDef",
     "FindingActorTypeDef",
+    "S3BucketCriteriaForJobOutputTypeDef",
     "S3BucketCriteriaForJobTypeDef",
+    "ScopingOutputTypeDef",
     "ScopingTypeDef",
     "DescribeBucketsResponseTypeDef",
     "ResourcesAffectedTypeDef",
     "ClassificationResultTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "PolicyDetailsTypeDef",
     "JobSummaryTypeDef",
+    "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
-    "CreateClassificationJobRequestRequestTypeDef",
     "DescribeClassificationJobResponseTypeDef",
+    "CreateClassificationJobRequestRequestTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -413,14 +441,22 @@
     {
         "accountId": str,
         "status": AdminStatusType,
     },
     total=False,
 )
 
+S3WordsListOutputTypeDef = TypedDict(
+    "S3WordsListOutputTypeDef",
+    {
+        "bucketName": str,
+        "objectKey": str,
+    },
+)
+
 S3WordsListTypeDef = TypedDict(
     "S3WordsListTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -660,14 +696,36 @@
         "column": int,
         "columnName": str,
         "row": int,
     },
     total=False,
 )
 
+_RequiredS3DestinationOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationOutputTypeDef",
+    {
+        "bucketName": str,
+        "kmsKeyArn": str,
+    },
+)
+_OptionalS3DestinationOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+
+class S3DestinationOutputTypeDef(
+    _RequiredS3DestinationOutputTypeDef, _OptionalS3DestinationOutputTypeDef
+):
+    pass
+
+
 _RequiredS3DestinationTypeDef = TypedDict(
     "_RequiredS3DestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -789,24 +847,48 @@
     "CreateSampleFindingsRequestRequestTypeDef",
     {
         "findingTypes": Sequence[FindingTypeType],
     },
     total=False,
 )
 
+SimpleCriterionForJobOutputTypeDef = TypedDict(
+    "SimpleCriterionForJobOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": SimpleCriterionKeyForJobType,
+        "values": List[str],
+    },
+    total=False,
+)
+
 SimpleCriterionForJobTypeDef = TypedDict(
     "SimpleCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "key": SimpleCriterionKeyForJobType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+CriterionAdditionalPropertiesOutputTypeDef = TypedDict(
+    "CriterionAdditionalPropertiesOutputTypeDef",
+    {
+        "eq": List[str],
+        "eqExactMatch": List[str],
+        "gt": int,
+        "gte": int,
+        "lt": int,
+        "lte": int,
+        "neq": List[str],
+    },
+    total=False,
+)
+
 CriterionAdditionalPropertiesTypeDef = TypedDict(
     "CriterionAdditionalPropertiesTypeDef",
     {
         "eq": Sequence[str],
         "eqExactMatch": Sequence[str],
         "gt": int,
         "gte": int,
@@ -1081,14 +1163,22 @@
 GetCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "GetCustomDataIdentifierRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+SeverityLevelOutputTypeDef = TypedDict(
+    "SeverityLevelOutputTypeDef",
+    {
+        "occurrencesThreshold": int,
+        "severity": DataIdentifierSeverityType,
+    },
+)
+
 GroupCountTypeDef = TypedDict(
     "GroupCountTypeDef",
     {
         "count": int,
         "groupKey": str,
     },
     total=False,
@@ -1097,16 +1187,16 @@
 GetFindingsFilterRequestRequestTypeDef = TypedDict(
     "GetFindingsFilterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SecurityHubConfigurationTypeDef = TypedDict(
-    "SecurityHubConfigurationTypeDef",
+SecurityHubConfigurationOutputTypeDef = TypedDict(
+    "SecurityHubConfigurationOutputTypeDef",
     {
         "publishClassificationFindings": bool,
         "publishPolicyFindings": bool,
     },
 )
 
 SortCriteriaTypeDef = TypedDict(
@@ -1180,31 +1270,31 @@
         "totalItemsSkippedInvalidEncryption": int,
         "totalItemsSkippedInvalidKms": int,
         "totalItemsSkippedPermissionDenied": int,
     },
     total=False,
 )
 
-_RequiredRevealConfigurationTypeDef = TypedDict(
-    "_RequiredRevealConfigurationTypeDef",
+_RequiredRevealConfigurationOutputTypeDef = TypedDict(
+    "_RequiredRevealConfigurationOutputTypeDef",
     {
         "status": RevealStatusType,
     },
 )
-_OptionalRevealConfigurationTypeDef = TypedDict(
-    "_OptionalRevealConfigurationTypeDef",
+_OptionalRevealConfigurationOutputTypeDef = TypedDict(
+    "_OptionalRevealConfigurationOutputTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
 
-class RevealConfigurationTypeDef(
-    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
+class RevealConfigurationOutputTypeDef(
+    _RequiredRevealConfigurationOutputTypeDef, _OptionalRevealConfigurationOutputTypeDef
 ):
     pass
 
 
 GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     {
@@ -1240,24 +1330,24 @@
 GetSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesTypeDef",
+SensitivityInspectionTemplateExcludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
     {
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesTypeDef",
+SensitivityInspectionTemplateIncludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     {
         "allowListIds": List[str],
         "customDataIdentifierIds": List[str],
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
@@ -1343,14 +1433,30 @@
         "asnOrg": str,
         "isp": str,
         "org": str,
     },
     total=False,
 )
 
+MonthlyScheduleOutputTypeDef = TypedDict(
+    "MonthlyScheduleOutputTypeDef",
+    {
+        "dayOfMonth": int,
+    },
+    total=False,
+)
+
+WeeklyScheduleOutputTypeDef = TypedDict(
+    "WeeklyScheduleOutputTypeDef",
+    {
+        "dayOfWeek": DayOfWeekType,
+    },
+    total=False,
+)
+
 MonthlyScheduleTypeDef = TypedDict(
     "MonthlyScheduleTypeDef",
     {
         "dayOfMonth": int,
     },
     total=False,
 )
@@ -1359,29 +1465,39 @@
     "WeeklyScheduleTypeDef",
     {
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
+SimpleScopeTermOutputTypeDef = TypedDict(
+    "SimpleScopeTermOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": ScopeFilterKeyType,
+        "values": List[str],
+    },
+    total=False,
+)
+
 SimpleScopeTermTypeDef = TypedDict(
     "SimpleScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": ScopeFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-S3BucketDefinitionForJobTypeDef = TypedDict(
-    "S3BucketDefinitionForJobTypeDef",
+S3BucketDefinitionForJobOutputTypeDef = TypedDict(
+    "S3BucketDefinitionForJobOutputTypeDef",
     {
         "accountId": str,
-        "buckets": Sequence[str],
+        "buckets": List[str],
     },
 )
 
 ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
     "ListAllowListsRequestListAllowListsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1753,25 +1869,62 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+SecurityHubConfigurationTypeDef = TypedDict(
+    "SecurityHubConfigurationTypeDef",
+    {
+        "publishClassificationFindings": bool,
+        "publishPolicyFindings": bool,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredRevealConfigurationTypeDef = TypedDict(
+    "_RequiredRevealConfigurationTypeDef",
+    {
+        "status": RevealStatusType,
+    },
+)
+_OptionalRevealConfigurationTypeDef = TypedDict(
+    "_OptionalRevealConfigurationTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class RevealConfigurationTypeDef(
+    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
+):
+    pass
+
+
+S3BucketDefinitionForJobTypeDef = TypedDict(
+    "S3BucketDefinitionForJobTypeDef",
+    {
+        "accountId": str,
+        "buckets": Sequence[str],
+    },
+)
+
 S3BucketOwnerTypeDef = TypedDict(
     "S3BucketOwnerTypeDef",
     {
         "displayName": str,
         "id": str,
     },
     total=False,
@@ -1825,14 +1978,32 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    {
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
+SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesTypeDef",
+    {
+        "allowListIds": Sequence[str],
+        "customDataIdentifierIds": Sequence[str],
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
 ServiceLimitTypeDef = TypedDict(
     "ServiceLimitTypeDef",
     {
         "isServiceLimited": bool,
         "unit": Literal["TERABYTES"],
         "value": int,
     },
@@ -1865,14 +2036,23 @@
     {
         "id": str,
         "type": DataIdentifierTypeType,
     },
     total=False,
 )
 
+TagCriterionPairForJobOutputTypeDef = TypedDict(
+    "TagCriterionPairForJobOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 TagCriterionPairForJobTypeDef = TypedDict(
     "TagCriterionPairForJobTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -1882,14 +2062,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
+TagValuePairOutputTypeDef = TypedDict(
+    "TagValuePairOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 TagValuePairTypeDef = TypedDict(
     "TagValuePairTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -2059,14 +2248,23 @@
     {
         "adminAccounts": List[AdminAccountTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AllowListCriteriaOutputTypeDef = TypedDict(
+    "AllowListCriteriaOutputTypeDef",
+    {
+        "regex": str,
+        "s3WordsList": S3WordsListOutputTypeDef,
+    },
+    total=False,
+)
+
 AllowListCriteriaTypeDef = TypedDict(
     "AllowListCriteriaTypeDef",
     {
         "regex": str,
         "s3WordsList": S3WordsListTypeDef,
     },
     total=False,
@@ -2159,14 +2357,22 @@
         "notClassified": SensitivityAggregationsTypeDef,
         "notSensitive": SensitivityAggregationsTypeDef,
         "sensitive": SensitivityAggregationsTypeDef,
     },
     total=False,
 )
 
+ClassificationExportConfigurationOutputTypeDef = TypedDict(
+    "ClassificationExportConfigurationOutputTypeDef",
+    {
+        "s3Destination": S3DestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassificationExportConfigurationTypeDef = TypedDict(
     "ClassificationExportConfigurationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -2205,33 +2411,14 @@
 class CreateCustomDataIdentifierRequestRequestTypeDef(
     _RequiredCreateCustomDataIdentifierRequestRequestTypeDef,
     _OptionalCreateCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
 
-GetCustomDataIdentifierResponseTypeDef = TypedDict(
-    "GetCustomDataIdentifierResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "deleted": bool,
-        "description": str,
-        "id": str,
-        "ignoreWords": List[str],
-        "keywords": List[str],
-        "maximumMatchDistance": int,
-        "name": str,
-        "regex": str,
-        "severityLevels": List[SeverityLevelTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateInvitationsResponseTypeDef = TypedDict(
     "CreateInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2248,14 +2435,22 @@
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
+    },
+    total=False,
+)
+
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "criterion": Mapping[str, CriterionAdditionalPropertiesTypeDef],
     },
     total=False,
 )
@@ -2318,39 +2513,49 @@
     {
         "invitations": List[InvitationTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetCustomDataIdentifierResponseTypeDef = TypedDict(
+    "GetCustomDataIdentifierResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deleted": bool,
+        "description": str,
+        "id": str,
+        "ignoreWords": List[str],
+        "keywords": List[str],
+        "maximumMatchDistance": int,
+        "name": str,
+        "regex": str,
+        "severityLevels": List[SeverityLevelOutputTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFindingStatisticsResponseTypeDef = TypedDict(
     "GetFindingStatisticsResponseTypeDef",
     {
         "countsByGroup": List[GroupCountTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFindingsPublicationConfigurationResponseTypeDef = TypedDict(
     "GetFindingsPublicationConfigurationResponseTypeDef",
     {
-        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
+        "securityHubConfiguration": SecurityHubConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "findingIds": Sequence[str],
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -2378,30 +2583,23 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRevealConfigurationResponseTypeDef = TypedDict(
     "GetRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationTypeDef,
+        "configuration": RevealConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateRevealConfigurationRequestRequestTypeDef",
-    {
-        "configuration": RevealConfigurationTypeDef,
-    },
-)
-
 UpdateRevealConfigurationResponseTypeDef = TypedDict(
     "UpdateRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationTypeDef,
+        "configuration": RevealConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef = TypedDict(
     "_RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     {
@@ -2424,46 +2622,22 @@
     pass
 
 
 GetSensitivityInspectionTemplateResponseTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+        "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
-    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-):
-    pass
-
-
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -2500,14 +2674,24 @@
         "ipCountry": IpCountryTypeDef,
         "ipGeoLocation": IpGeoLocationTypeDef,
         "ipOwner": IpOwnerTypeDef,
     },
     total=False,
 )
 
+JobScheduleFrequencyOutputTypeDef = TypedDict(
+    "JobScheduleFrequencyOutputTypeDef",
+    {
+        "dailySchedule": Dict[str, Any],
+        "monthlySchedule": MonthlyScheduleOutputTypeDef,
+        "weeklySchedule": WeeklyScheduleOutputTypeDef,
+    },
+    total=False,
+)
+
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
         "dailySchedule": Mapping[str, Any],
         "monthlySchedule": MonthlyScheduleTypeDef,
         "weeklySchedule": WeeklyScheduleTypeDef,
     },
@@ -2565,14 +2749,30 @@
         "lineRange": RangeTypeDef,
         "offsetRange": RangeTypeDef,
         "pageNumber": int,
     },
     total=False,
 )
 
+PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
+    },
+    total=False,
+)
+
+UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateRevealConfigurationRequestRequestTypeDef",
+    {
+        "configuration": RevealConfigurationTypeDef,
+    },
+)
+
 S3ObjectTypeDef = TypedDict(
     "S3ObjectTypeDef",
     {
         "bucketArn": str,
         "eTag": str,
         "extension": str,
         "key": str,
@@ -2607,14 +2807,38 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "description": str,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
+    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+):
+    pass
+
+
 UsageByAccountTypeDef = TypedDict(
     "UsageByAccountTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedCost": str,
         "serviceLimit": ServiceLimitTypeDef,
         "type": UsageTypeType,
@@ -2649,34 +2873,70 @@
 class UpdateResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredUpdateResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalUpdateResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
 
+TagCriterionForJobOutputTypeDef = TypedDict(
+    "TagCriterionForJobOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "tagValues": List[TagCriterionPairForJobOutputTypeDef],
+    },
+    total=False,
+)
+
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "tagValues": Sequence[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
+TagScopeTermOutputTypeDef = TypedDict(
+    "TagScopeTermOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": str,
+        "tagValues": List[TagValuePairOutputTypeDef],
+        "target": Literal["S3_OBJECT"],
+    },
+    total=False,
+)
+
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
     },
     total=False,
 )
 
+GetAllowListResponseTypeDef = TypedDict(
+    "GetAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": AllowListCriteriaOutputTypeDef,
+        "description": str,
+        "id": str,
+        "name": str,
+        "status": AllowListStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAllowListRequestRequestTypeDef",
     {
         "clientToken": str,
         "criteria": AllowListCriteriaTypeDef,
         "name": str,
     },
@@ -2693,30 +2953,14 @@
 
 class CreateAllowListRequestRequestTypeDef(
     _RequiredCreateAllowListRequestRequestTypeDef, _OptionalCreateAllowListRequestRequestTypeDef
 ):
     pass
 
 
-GetAllowListResponseTypeDef = TypedDict(
-    "GetAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": AllowListCriteriaTypeDef,
-        "description": str,
-        "id": str,
-        "name": str,
-        "status": AllowListStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAllowListRequestRequestTypeDef",
     {
         "criteria": AllowListCriteriaTypeDef,
         "id": str,
         "name": str,
     },
@@ -2775,30 +3019,45 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClassificationExportConfigurationResponseTypeDef = TypedDict(
     "GetClassificationExportConfigurationResponseTypeDef",
     {
-        "configuration": ClassificationExportConfigurationTypeDef,
+        "configuration": ClassificationExportConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutClassificationExportConfigurationResponseTypeDef = TypedDict(
+    "PutClassificationExportConfigurationResponseTypeDef",
+    {
+        "configuration": ClassificationExportConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
     },
 )
 
-PutClassificationExportConfigurationResponseTypeDef = TypedDict(
-    "PutClassificationExportConfigurationResponseTypeDef",
+GetFindingsFilterResponseTypeDef = TypedDict(
+    "GetFindingsFilterResponseTypeDef",
     {
-        "configuration": ClassificationExportConfigurationTypeDef,
+        "action": FindingsFilterActionType,
+        "arn": str,
+        "description": str,
+        "findingCriteria": FindingCriteriaOutputTypeDef,
+        "id": str,
+        "name": str,
+        "position": int,
+        "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
@@ -2846,29 +3105,14 @@
 class GetFindingStatisticsRequestRequestTypeDef(
     _RequiredGetFindingStatisticsRequestRequestTypeDef,
     _OptionalGetFindingStatisticsRequestRequestTypeDef,
 ):
     pass
 
 
-GetFindingsFilterResponseTypeDef = TypedDict(
-    "GetFindingsFilterResponseTypeDef",
-    {
-        "action": FindingsFilterActionType,
-        "arn": str,
-        "description": str,
-        "findingCriteria": FindingCriteriaTypeDef,
-        "id": str,
-        "name": str,
-        "position": int,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -3018,23 +3262,41 @@
         "arn": str,
         "principalId": str,
         "sessionContext": SessionContextTypeDef,
     },
     total=False,
 )
 
+CriteriaForJobOutputTypeDef = TypedDict(
+    "CriteriaForJobOutputTypeDef",
+    {
+        "simpleCriterion": SimpleCriterionForJobOutputTypeDef,
+        "tagCriterion": TagCriterionForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 CriteriaForJobTypeDef = TypedDict(
     "CriteriaForJobTypeDef",
     {
         "simpleCriterion": SimpleCriterionForJobTypeDef,
         "tagCriterion": TagCriterionForJobTypeDef,
     },
     total=False,
 )
 
+JobScopeTermOutputTypeDef = TypedDict(
+    "JobScopeTermOutputTypeDef",
+    {
+        "simpleScopeTerm": SimpleScopeTermOutputTypeDef,
+        "tagScopeTerm": TagScopeTermOutputTypeDef,
+    },
+    total=False,
+)
+
 JobScopeTermTypeDef = TypedDict(
     "JobScopeTermTypeDef",
     {
         "simpleScopeTerm": SimpleScopeTermTypeDef,
         "tagScopeTerm": TagScopeTermTypeDef,
     },
     total=False,
@@ -3107,22 +3369,38 @@
         "iamUser": IamUserTypeDef,
         "root": UserIdentityRootTypeDef,
         "type": UserIdentityTypeType,
     },
     total=False,
 )
 
+CriteriaBlockForJobOutputTypeDef = TypedDict(
+    "CriteriaBlockForJobOutputTypeDef",
+    {
+        "and": List[CriteriaForJobOutputTypeDef],
+    },
+    total=False,
+)
+
 CriteriaBlockForJobTypeDef = TypedDict(
     "CriteriaBlockForJobTypeDef",
     {
         "and": Sequence[CriteriaForJobTypeDef],
     },
     total=False,
 )
 
+JobScopingBlockOutputTypeDef = TypedDict(
+    "JobScopingBlockOutputTypeDef",
+    {
+        "and": List[JobScopeTermOutputTypeDef],
+    },
+    total=False,
+)
+
 JobScopingBlockTypeDef = TypedDict(
     "JobScopingBlockTypeDef",
     {
         "and": Sequence[JobScopeTermTypeDef],
     },
     total=False,
 )
@@ -3209,23 +3487,41 @@
         "domainDetails": DomainDetailsTypeDef,
         "ipAddressDetails": IpAddressDetailsTypeDef,
         "userIdentity": UserIdentityTypeDef,
     },
     total=False,
 )
 
+S3BucketCriteriaForJobOutputTypeDef = TypedDict(
+    "S3BucketCriteriaForJobOutputTypeDef",
+    {
+        "excludes": CriteriaBlockForJobOutputTypeDef,
+        "includes": CriteriaBlockForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 S3BucketCriteriaForJobTypeDef = TypedDict(
     "S3BucketCriteriaForJobTypeDef",
     {
         "excludes": CriteriaBlockForJobTypeDef,
         "includes": CriteriaBlockForJobTypeDef,
     },
     total=False,
 )
 
+ScopingOutputTypeDef = TypedDict(
+    "ScopingOutputTypeDef",
+    {
+        "excludes": JobScopingBlockOutputTypeDef,
+        "includes": JobScopingBlockOutputTypeDef,
+    },
+    total=False,
+)
+
 ScopingTypeDef = TypedDict(
     "ScopingTypeDef",
     {
         "excludes": JobScopingBlockTypeDef,
         "includes": JobScopingBlockTypeDef,
     },
     total=False,
@@ -3291,27 +3587,37 @@
     },
     total=False,
 )
 
 JobSummaryTypeDef = TypedDict(
     "JobSummaryTypeDef",
     {
-        "bucketCriteria": S3BucketCriteriaForJobTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobTypeDef],
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
         "createdAt": datetime,
         "jobId": str,
         "jobStatus": JobStatusType,
         "jobType": JobTypeType,
         "lastRunErrorStatus": LastRunErrorStatusTypeDef,
         "name": str,
         "userPausedDetails": UserPausedDetailsTypeDef,
     },
     total=False,
 )
 
+S3JobDefinitionOutputTypeDef = TypedDict(
+    "S3JobDefinitionOutputTypeDef",
+    {
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
+        "scoping": ScopingOutputTypeDef,
+    },
+    total=False,
+)
+
 S3JobDefinitionTypeDef = TypedDict(
     "S3JobDefinitionTypeDef",
     {
         "bucketCriteria": S3BucketCriteriaForJobTypeDef,
         "bucketDefinitions": Sequence[S3BucketDefinitionForJobTypeDef],
         "scoping": ScopingTypeDef,
     },
@@ -3335,14 +3641,42 @@
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeClassificationJobResponseTypeDef = TypedDict(
+    "DescribeClassificationJobResponseTypeDef",
+    {
+        "allowListIds": List[str],
+        "clientToken": str,
+        "createdAt": datetime,
+        "customDataIdentifierIds": List[str],
+        "description": str,
+        "initialRun": bool,
+        "jobArn": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "jobType": JobTypeType,
+        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
+        "lastRunTime": datetime,
+        "managedDataIdentifierIds": List[str],
+        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
+        "name": str,
+        "s3JobDefinition": S3JobDefinitionOutputTypeDef,
+        "samplingPercentage": int,
+        "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
+        "statistics": StatisticsTypeDef,
+        "tags": Dict[str, str],
+        "userPausedDetails": UserPausedDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
         "jobType": JobTypeType,
         "name": str,
         "s3JobDefinition": S3JobDefinitionTypeDef,
@@ -3368,42 +3702,14 @@
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeClassificationJobResponseTypeDef = TypedDict(
-    "DescribeClassificationJobResponseTypeDef",
-    {
-        "allowListIds": List[str],
-        "clientToken": str,
-        "createdAt": datetime,
-        "customDataIdentifierIds": List[str],
-        "description": str,
-        "initialRun": bool,
-        "jobArn": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "jobType": JobTypeType,
-        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
-        "lastRunTime": datetime,
-        "managedDataIdentifierIds": List[str],
-        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
-        "name": str,
-        "s3JobDefinition": S3JobDefinitionTypeDef,
-        "samplingPercentage": int,
-        "scheduleFrequency": JobScheduleFrequencyTypeDef,
-        "statistics": StatisticsTypeDef,
-        "tags": Dict[str, str],
-        "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
```

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/type_defs.pyi` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccountDetailTypeDef",
     "BlockPublicAccessTypeDef",
     "AdminAccountTypeDef",
+    "S3WordsListOutputTypeDef",
     "S3WordsListTypeDef",
     "AllowListStatusTypeDef",
     "AllowListSummaryTypeDef",
     "ApiCallDetailsTypeDef",
     "AwsAccountTypeDef",
     "AwsServiceTypeDef",
     "BatchGetCustomDataIdentifierSummaryTypeDef",
@@ -102,27 +103,30 @@
     "KeyValuePairTypeDef",
     "ObjectCountByEncryptionTypeTypeDef",
     "ObjectLevelStatisticsTypeDef",
     "ReplicationDetailsTypeDef",
     "BucketSortCriteriaTypeDef",
     "SensitivityAggregationsTypeDef",
     "CellTypeDef",
+    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
     "CreateAllowListResponseTypeDef",
     "CreateClassificationJobResponseTypeDef",
     "SeverityLevelTypeDef",
     "CreateCustomDataIdentifierResponseTypeDef",
     "CreateFindingsFilterResponseTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
     "CreateMemberResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
+    "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
+    "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
@@ -144,45 +148,49 @@
     "FindingsFilterListItemTypeDef",
     "InvitationTypeDef",
     "GetAllowListRequestRequestTypeDef",
     "GetAutomatedDiscoveryConfigurationResponseTypeDef",
     "GetBucketStatisticsRequestRequestTypeDef",
     "GetClassificationScopeRequestRequestTypeDef",
     "GetCustomDataIdentifierRequestRequestTypeDef",
+    "SeverityLevelOutputTypeDef",
     "GroupCountTypeDef",
     "GetFindingsFilterRequestRequestTypeDef",
-    "SecurityHubConfigurationTypeDef",
+    "SecurityHubConfigurationOutputTypeDef",
     "SortCriteriaTypeDef",
     "GetInvitationsCountResponseTypeDef",
     "GetMacieSessionResponseTypeDef",
     "GetMemberRequestRequestTypeDef",
     "GetMemberResponseTypeDef",
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
-    "RevealConfigurationTypeDef",
+    "RevealConfigurationOutputTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    "SensitivityInspectionTemplateIncludesTypeDef",
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
+    "MonthlyScheduleOutputTypeDef",
+    "WeeklyScheduleOutputTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
+    "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
-    "S3BucketDefinitionForJobTypeDef",
+    "S3BucketDefinitionForJobOutputTypeDef",
     "ListAllowListsRequestListAllowListsPaginateTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
     "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
     "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
@@ -209,28 +217,35 @@
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
     "PaginatorConfigTypeDef",
+    "SecurityHubConfigurationTypeDef",
     "ResponseMetadataTypeDef",
+    "RevealConfigurationTypeDef",
+    "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
+    "TagCriterionPairForJobOutputTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagValuePairOutputTypeDef",
     "TagValuePairTypeDef",
     "TestCustomDataIdentifierRequestRequestTypeDef",
     "TestCustomDataIdentifierResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAllowListResponseTypeDef",
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     "UpdateClassificationJobRequestRequestTypeDef",
@@ -239,124 +254,137 @@
     "UpdateMemberSessionRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateResourceProfileRequestRequestTypeDef",
     "UserIdentityRootTypeDef",
     "CreateMemberRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
+    "AllowListCriteriaOutputTypeDef",
     "AllowListCriteriaTypeDef",
     "ListAllowListsResponseTypeDef",
     "FindingActionTypeDef",
     "BatchGetCustomDataIdentifiersResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "MatchingBucketTypeDef",
     "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "DescribeBucketsRequestRequestTypeDef",
     "BucketStatisticsBySensitivityTypeDef",
+    "ClassificationExportConfigurationOutputTypeDef",
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
-    "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
     "GetSensitiveDataOccurrencesResponseTypeDef",
     "ListResourceProfileDetectionsResponseTypeDef",
     "ListFindingsFiltersResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
+    "GetCustomDataIdentifierResponseTypeDef",
     "GetFindingStatisticsResponseTypeDef",
     "GetFindingsPublicationConfigurationResponseTypeDef",
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
-    "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
-    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
+    "JobScheduleFrequencyOutputTypeDef",
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
+    "UpdateRevealConfigurationRequestRequestTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
+    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
+    "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
+    "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
-    "CreateAllowListRequestRequestTypeDef",
     "GetAllowListResponseTypeDef",
+    "CreateAllowListRequestRequestTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
-    "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
+    "PutClassificationExportConfigurationRequestRequestTypeDef",
+    "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
-    "GetFindingsFilterResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
     "AssumedRoleTypeDef",
     "FederatedUserTypeDef",
+    "CriteriaForJobOutputTypeDef",
     "CriteriaForJobTypeDef",
+    "JobScopeTermOutputTypeDef",
     "JobScopeTermTypeDef",
     "BucketPublicAccessTypeDef",
     "SearchResourcesResponseTypeDef",
     "CustomDetectionTypeDef",
     "DefaultDetectionTypeDef",
     "SearchResourcesCriteriaBlockTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "UserIdentityTypeDef",
+    "CriteriaBlockForJobOutputTypeDef",
     "CriteriaBlockForJobTypeDef",
+    "JobScopingBlockOutputTypeDef",
     "JobScopingBlockTypeDef",
     "BucketMetadataTypeDef",
     "S3BucketTypeDef",
     "CustomDataIdentifiersTypeDef",
     "SensitiveDataItemTypeDef",
     "SearchResourcesBucketCriteriaTypeDef",
     "FindingActorTypeDef",
+    "S3BucketCriteriaForJobOutputTypeDef",
     "S3BucketCriteriaForJobTypeDef",
+    "ScopingOutputTypeDef",
     "ScopingTypeDef",
     "DescribeBucketsResponseTypeDef",
     "ResourcesAffectedTypeDef",
     "ClassificationResultTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "PolicyDetailsTypeDef",
     "JobSummaryTypeDef",
+    "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
-    "CreateClassificationJobRequestRequestTypeDef",
     "DescribeClassificationJobResponseTypeDef",
+    "CreateClassificationJobRequestRequestTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -410,14 +438,22 @@
     {
         "accountId": str,
         "status": AdminStatusType,
     },
     total=False,
 )
 
+S3WordsListOutputTypeDef = TypedDict(
+    "S3WordsListOutputTypeDef",
+    {
+        "bucketName": str,
+        "objectKey": str,
+    },
+)
+
 S3WordsListTypeDef = TypedDict(
     "S3WordsListTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -655,14 +691,34 @@
         "column": int,
         "columnName": str,
         "row": int,
     },
     total=False,
 )
 
+_RequiredS3DestinationOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationOutputTypeDef",
+    {
+        "bucketName": str,
+        "kmsKeyArn": str,
+    },
+)
+_OptionalS3DestinationOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+class S3DestinationOutputTypeDef(
+    _RequiredS3DestinationOutputTypeDef, _OptionalS3DestinationOutputTypeDef
+):
+    pass
+
 _RequiredS3DestinationTypeDef = TypedDict(
     "_RequiredS3DestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -780,24 +836,48 @@
     "CreateSampleFindingsRequestRequestTypeDef",
     {
         "findingTypes": Sequence[FindingTypeType],
     },
     total=False,
 )
 
+SimpleCriterionForJobOutputTypeDef = TypedDict(
+    "SimpleCriterionForJobOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": SimpleCriterionKeyForJobType,
+        "values": List[str],
+    },
+    total=False,
+)
+
 SimpleCriterionForJobTypeDef = TypedDict(
     "SimpleCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "key": SimpleCriterionKeyForJobType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+CriterionAdditionalPropertiesOutputTypeDef = TypedDict(
+    "CriterionAdditionalPropertiesOutputTypeDef",
+    {
+        "eq": List[str],
+        "eqExactMatch": List[str],
+        "gt": int,
+        "gte": int,
+        "lt": int,
+        "lte": int,
+        "neq": List[str],
+    },
+    total=False,
+)
+
 CriterionAdditionalPropertiesTypeDef = TypedDict(
     "CriterionAdditionalPropertiesTypeDef",
     {
         "eq": Sequence[str],
         "eqExactMatch": Sequence[str],
         "gt": int,
         "gte": int,
@@ -1068,14 +1148,22 @@
 GetCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "GetCustomDataIdentifierRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+SeverityLevelOutputTypeDef = TypedDict(
+    "SeverityLevelOutputTypeDef",
+    {
+        "occurrencesThreshold": int,
+        "severity": DataIdentifierSeverityType,
+    },
+)
+
 GroupCountTypeDef = TypedDict(
     "GroupCountTypeDef",
     {
         "count": int,
         "groupKey": str,
     },
     total=False,
@@ -1084,16 +1172,16 @@
 GetFindingsFilterRequestRequestTypeDef = TypedDict(
     "GetFindingsFilterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SecurityHubConfigurationTypeDef = TypedDict(
-    "SecurityHubConfigurationTypeDef",
+SecurityHubConfigurationOutputTypeDef = TypedDict(
+    "SecurityHubConfigurationOutputTypeDef",
     {
         "publishClassificationFindings": bool,
         "publishPolicyFindings": bool,
     },
 )
 
 SortCriteriaTypeDef = TypedDict(
@@ -1167,30 +1255,30 @@
         "totalItemsSkippedInvalidEncryption": int,
         "totalItemsSkippedInvalidKms": int,
         "totalItemsSkippedPermissionDenied": int,
     },
     total=False,
 )
 
-_RequiredRevealConfigurationTypeDef = TypedDict(
-    "_RequiredRevealConfigurationTypeDef",
+_RequiredRevealConfigurationOutputTypeDef = TypedDict(
+    "_RequiredRevealConfigurationOutputTypeDef",
     {
         "status": RevealStatusType,
     },
 )
-_OptionalRevealConfigurationTypeDef = TypedDict(
-    "_OptionalRevealConfigurationTypeDef",
+_OptionalRevealConfigurationOutputTypeDef = TypedDict(
+    "_OptionalRevealConfigurationOutputTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
-class RevealConfigurationTypeDef(
-    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
+class RevealConfigurationOutputTypeDef(
+    _RequiredRevealConfigurationOutputTypeDef, _OptionalRevealConfigurationOutputTypeDef
 ):
     pass
 
 GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     {
         "findingId": str,
@@ -1225,24 +1313,24 @@
 GetSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesTypeDef",
+SensitivityInspectionTemplateExcludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
     {
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesTypeDef",
+SensitivityInspectionTemplateIncludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     {
         "allowListIds": List[str],
         "customDataIdentifierIds": List[str],
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
@@ -1328,14 +1416,30 @@
         "asnOrg": str,
         "isp": str,
         "org": str,
     },
     total=False,
 )
 
+MonthlyScheduleOutputTypeDef = TypedDict(
+    "MonthlyScheduleOutputTypeDef",
+    {
+        "dayOfMonth": int,
+    },
+    total=False,
+)
+
+WeeklyScheduleOutputTypeDef = TypedDict(
+    "WeeklyScheduleOutputTypeDef",
+    {
+        "dayOfWeek": DayOfWeekType,
+    },
+    total=False,
+)
+
 MonthlyScheduleTypeDef = TypedDict(
     "MonthlyScheduleTypeDef",
     {
         "dayOfMonth": int,
     },
     total=False,
 )
@@ -1344,29 +1448,39 @@
     "WeeklyScheduleTypeDef",
     {
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
+SimpleScopeTermOutputTypeDef = TypedDict(
+    "SimpleScopeTermOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": ScopeFilterKeyType,
+        "values": List[str],
+    },
+    total=False,
+)
+
 SimpleScopeTermTypeDef = TypedDict(
     "SimpleScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": ScopeFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-S3BucketDefinitionForJobTypeDef = TypedDict(
-    "S3BucketDefinitionForJobTypeDef",
+S3BucketDefinitionForJobOutputTypeDef = TypedDict(
+    "S3BucketDefinitionForJobOutputTypeDef",
     {
         "accountId": str,
-        "buckets": Sequence[str],
+        "buckets": List[str],
     },
 )
 
 ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
     "ListAllowListsRequestListAllowListsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1728,25 +1842,60 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+SecurityHubConfigurationTypeDef = TypedDict(
+    "SecurityHubConfigurationTypeDef",
+    {
+        "publishClassificationFindings": bool,
+        "publishPolicyFindings": bool,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredRevealConfigurationTypeDef = TypedDict(
+    "_RequiredRevealConfigurationTypeDef",
+    {
+        "status": RevealStatusType,
+    },
+)
+_OptionalRevealConfigurationTypeDef = TypedDict(
+    "_OptionalRevealConfigurationTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+class RevealConfigurationTypeDef(
+    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
+):
+    pass
+
+S3BucketDefinitionForJobTypeDef = TypedDict(
+    "S3BucketDefinitionForJobTypeDef",
+    {
+        "accountId": str,
+        "buckets": Sequence[str],
+    },
+)
+
 S3BucketOwnerTypeDef = TypedDict(
     "S3BucketOwnerTypeDef",
     {
         "displayName": str,
         "id": str,
     },
     total=False,
@@ -1800,14 +1949,32 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    {
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
+SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesTypeDef",
+    {
+        "allowListIds": Sequence[str],
+        "customDataIdentifierIds": Sequence[str],
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
 ServiceLimitTypeDef = TypedDict(
     "ServiceLimitTypeDef",
     {
         "isServiceLimited": bool,
         "unit": Literal["TERABYTES"],
         "value": int,
     },
@@ -1840,14 +2007,23 @@
     {
         "id": str,
         "type": DataIdentifierTypeType,
     },
     total=False,
 )
 
+TagCriterionPairForJobOutputTypeDef = TypedDict(
+    "TagCriterionPairForJobOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 TagCriterionPairForJobTypeDef = TypedDict(
     "TagCriterionPairForJobTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -1857,14 +2033,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
+TagValuePairOutputTypeDef = TypedDict(
+    "TagValuePairOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 TagValuePairTypeDef = TypedDict(
     "TagValuePairTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -2028,14 +2213,23 @@
     {
         "adminAccounts": List[AdminAccountTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AllowListCriteriaOutputTypeDef = TypedDict(
+    "AllowListCriteriaOutputTypeDef",
+    {
+        "regex": str,
+        "s3WordsList": S3WordsListOutputTypeDef,
+    },
+    total=False,
+)
+
 AllowListCriteriaTypeDef = TypedDict(
     "AllowListCriteriaTypeDef",
     {
         "regex": str,
         "s3WordsList": S3WordsListTypeDef,
     },
     total=False,
@@ -2128,14 +2322,22 @@
         "notClassified": SensitivityAggregationsTypeDef,
         "notSensitive": SensitivityAggregationsTypeDef,
         "sensitive": SensitivityAggregationsTypeDef,
     },
     total=False,
 )
 
+ClassificationExportConfigurationOutputTypeDef = TypedDict(
+    "ClassificationExportConfigurationOutputTypeDef",
+    {
+        "s3Destination": S3DestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassificationExportConfigurationTypeDef = TypedDict(
     "ClassificationExportConfigurationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -2172,33 +2374,14 @@
 
 class CreateCustomDataIdentifierRequestRequestTypeDef(
     _RequiredCreateCustomDataIdentifierRequestRequestTypeDef,
     _OptionalCreateCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
-GetCustomDataIdentifierResponseTypeDef = TypedDict(
-    "GetCustomDataIdentifierResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "deleted": bool,
-        "description": str,
-        "id": str,
-        "ignoreWords": List[str],
-        "keywords": List[str],
-        "maximumMatchDistance": int,
-        "name": str,
-        "regex": str,
-        "severityLevels": List[SeverityLevelTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateInvitationsResponseTypeDef = TypedDict(
     "CreateInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2215,14 +2398,22 @@
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
+    },
+    total=False,
+)
+
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "criterion": Mapping[str, CriterionAdditionalPropertiesTypeDef],
     },
     total=False,
 )
@@ -2285,39 +2476,49 @@
     {
         "invitations": List[InvitationTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetCustomDataIdentifierResponseTypeDef = TypedDict(
+    "GetCustomDataIdentifierResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deleted": bool,
+        "description": str,
+        "id": str,
+        "ignoreWords": List[str],
+        "keywords": List[str],
+        "maximumMatchDistance": int,
+        "name": str,
+        "regex": str,
+        "severityLevels": List[SeverityLevelOutputTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFindingStatisticsResponseTypeDef = TypedDict(
     "GetFindingStatisticsResponseTypeDef",
     {
         "countsByGroup": List[GroupCountTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFindingsPublicationConfigurationResponseTypeDef = TypedDict(
     "GetFindingsPublicationConfigurationResponseTypeDef",
     {
-        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
+        "securityHubConfiguration": SecurityHubConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "findingIds": Sequence[str],
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -2343,30 +2544,23 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRevealConfigurationResponseTypeDef = TypedDict(
     "GetRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationTypeDef,
+        "configuration": RevealConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateRevealConfigurationRequestRequestTypeDef",
-    {
-        "configuration": RevealConfigurationTypeDef,
-    },
-)
-
 UpdateRevealConfigurationResponseTypeDef = TypedDict(
     "UpdateRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationTypeDef,
+        "configuration": RevealConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef = TypedDict(
     "_RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     {
@@ -2387,44 +2581,22 @@
 ):
     pass
 
 GetSensitivityInspectionTemplateResponseTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+        "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
-    },
-    total=False,
-)
-
-class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
-    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-):
-    pass
-
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -2461,14 +2633,24 @@
         "ipCountry": IpCountryTypeDef,
         "ipGeoLocation": IpGeoLocationTypeDef,
         "ipOwner": IpOwnerTypeDef,
     },
     total=False,
 )
 
+JobScheduleFrequencyOutputTypeDef = TypedDict(
+    "JobScheduleFrequencyOutputTypeDef",
+    {
+        "dailySchedule": Dict[str, Any],
+        "monthlySchedule": MonthlyScheduleOutputTypeDef,
+        "weeklySchedule": WeeklyScheduleOutputTypeDef,
+    },
+    total=False,
+)
+
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
         "dailySchedule": Mapping[str, Any],
         "monthlySchedule": MonthlyScheduleTypeDef,
         "weeklySchedule": WeeklyScheduleTypeDef,
     },
@@ -2526,14 +2708,30 @@
         "lineRange": RangeTypeDef,
         "offsetRange": RangeTypeDef,
         "pageNumber": int,
     },
     total=False,
 )
 
+PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
+    },
+    total=False,
+)
+
+UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateRevealConfigurationRequestRequestTypeDef",
+    {
+        "configuration": RevealConfigurationTypeDef,
+    },
+)
+
 S3ObjectTypeDef = TypedDict(
     "S3ObjectTypeDef",
     {
         "bucketArn": str,
         "eTag": str,
         "extension": str,
         "key": str,
@@ -2568,14 +2766,36 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "description": str,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
+    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+):
+    pass
+
 UsageByAccountTypeDef = TypedDict(
     "UsageByAccountTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedCost": str,
         "serviceLimit": ServiceLimitTypeDef,
         "type": UsageTypeType,
@@ -2608,34 +2828,70 @@
 
 class UpdateResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredUpdateResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalUpdateResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
+TagCriterionForJobOutputTypeDef = TypedDict(
+    "TagCriterionForJobOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "tagValues": List[TagCriterionPairForJobOutputTypeDef],
+    },
+    total=False,
+)
+
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "tagValues": Sequence[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
+TagScopeTermOutputTypeDef = TypedDict(
+    "TagScopeTermOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": str,
+        "tagValues": List[TagValuePairOutputTypeDef],
+        "target": Literal["S3_OBJECT"],
+    },
+    total=False,
+)
+
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
     },
     total=False,
 )
 
+GetAllowListResponseTypeDef = TypedDict(
+    "GetAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": AllowListCriteriaOutputTypeDef,
+        "description": str,
+        "id": str,
+        "name": str,
+        "status": AllowListStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAllowListRequestRequestTypeDef",
     {
         "clientToken": str,
         "criteria": AllowListCriteriaTypeDef,
         "name": str,
     },
@@ -2650,30 +2906,14 @@
 )
 
 class CreateAllowListRequestRequestTypeDef(
     _RequiredCreateAllowListRequestRequestTypeDef, _OptionalCreateAllowListRequestRequestTypeDef
 ):
     pass
 
-GetAllowListResponseTypeDef = TypedDict(
-    "GetAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": AllowListCriteriaTypeDef,
-        "description": str,
-        "id": str,
-        "name": str,
-        "status": AllowListStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAllowListRequestRequestTypeDef",
     {
         "criteria": AllowListCriteriaTypeDef,
         "id": str,
         "name": str,
     },
@@ -2730,30 +2970,45 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClassificationExportConfigurationResponseTypeDef = TypedDict(
     "GetClassificationExportConfigurationResponseTypeDef",
     {
-        "configuration": ClassificationExportConfigurationTypeDef,
+        "configuration": ClassificationExportConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutClassificationExportConfigurationResponseTypeDef = TypedDict(
+    "PutClassificationExportConfigurationResponseTypeDef",
+    {
+        "configuration": ClassificationExportConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
     },
 )
 
-PutClassificationExportConfigurationResponseTypeDef = TypedDict(
-    "PutClassificationExportConfigurationResponseTypeDef",
+GetFindingsFilterResponseTypeDef = TypedDict(
+    "GetFindingsFilterResponseTypeDef",
     {
-        "configuration": ClassificationExportConfigurationTypeDef,
+        "action": FindingsFilterActionType,
+        "arn": str,
+        "description": str,
+        "findingCriteria": FindingCriteriaOutputTypeDef,
+        "id": str,
+        "name": str,
+        "position": int,
+        "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
@@ -2797,29 +3052,14 @@
 
 class GetFindingStatisticsRequestRequestTypeDef(
     _RequiredGetFindingStatisticsRequestRequestTypeDef,
     _OptionalGetFindingStatisticsRequestRequestTypeDef,
 ):
     pass
 
-GetFindingsFilterResponseTypeDef = TypedDict(
-    "GetFindingsFilterResponseTypeDef",
-    {
-        "action": FindingsFilterActionType,
-        "arn": str,
-        "description": str,
-        "findingCriteria": FindingCriteriaTypeDef,
-        "id": str,
-        "name": str,
-        "position": int,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -2965,23 +3205,41 @@
         "arn": str,
         "principalId": str,
         "sessionContext": SessionContextTypeDef,
     },
     total=False,
 )
 
+CriteriaForJobOutputTypeDef = TypedDict(
+    "CriteriaForJobOutputTypeDef",
+    {
+        "simpleCriterion": SimpleCriterionForJobOutputTypeDef,
+        "tagCriterion": TagCriterionForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 CriteriaForJobTypeDef = TypedDict(
     "CriteriaForJobTypeDef",
     {
         "simpleCriterion": SimpleCriterionForJobTypeDef,
         "tagCriterion": TagCriterionForJobTypeDef,
     },
     total=False,
 )
 
+JobScopeTermOutputTypeDef = TypedDict(
+    "JobScopeTermOutputTypeDef",
+    {
+        "simpleScopeTerm": SimpleScopeTermOutputTypeDef,
+        "tagScopeTerm": TagScopeTermOutputTypeDef,
+    },
+    total=False,
+)
+
 JobScopeTermTypeDef = TypedDict(
     "JobScopeTermTypeDef",
     {
         "simpleScopeTerm": SimpleScopeTermTypeDef,
         "tagScopeTerm": TagScopeTermTypeDef,
     },
     total=False,
@@ -3054,22 +3312,38 @@
         "iamUser": IamUserTypeDef,
         "root": UserIdentityRootTypeDef,
         "type": UserIdentityTypeType,
     },
     total=False,
 )
 
+CriteriaBlockForJobOutputTypeDef = TypedDict(
+    "CriteriaBlockForJobOutputTypeDef",
+    {
+        "and": List[CriteriaForJobOutputTypeDef],
+    },
+    total=False,
+)
+
 CriteriaBlockForJobTypeDef = TypedDict(
     "CriteriaBlockForJobTypeDef",
     {
         "and": Sequence[CriteriaForJobTypeDef],
     },
     total=False,
 )
 
+JobScopingBlockOutputTypeDef = TypedDict(
+    "JobScopingBlockOutputTypeDef",
+    {
+        "and": List[JobScopeTermOutputTypeDef],
+    },
+    total=False,
+)
+
 JobScopingBlockTypeDef = TypedDict(
     "JobScopingBlockTypeDef",
     {
         "and": Sequence[JobScopeTermTypeDef],
     },
     total=False,
 )
@@ -3156,23 +3430,41 @@
         "domainDetails": DomainDetailsTypeDef,
         "ipAddressDetails": IpAddressDetailsTypeDef,
         "userIdentity": UserIdentityTypeDef,
     },
     total=False,
 )
 
+S3BucketCriteriaForJobOutputTypeDef = TypedDict(
+    "S3BucketCriteriaForJobOutputTypeDef",
+    {
+        "excludes": CriteriaBlockForJobOutputTypeDef,
+        "includes": CriteriaBlockForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 S3BucketCriteriaForJobTypeDef = TypedDict(
     "S3BucketCriteriaForJobTypeDef",
     {
         "excludes": CriteriaBlockForJobTypeDef,
         "includes": CriteriaBlockForJobTypeDef,
     },
     total=False,
 )
 
+ScopingOutputTypeDef = TypedDict(
+    "ScopingOutputTypeDef",
+    {
+        "excludes": JobScopingBlockOutputTypeDef,
+        "includes": JobScopingBlockOutputTypeDef,
+    },
+    total=False,
+)
+
 ScopingTypeDef = TypedDict(
     "ScopingTypeDef",
     {
         "excludes": JobScopingBlockTypeDef,
         "includes": JobScopingBlockTypeDef,
     },
     total=False,
@@ -3238,27 +3530,37 @@
     },
     total=False,
 )
 
 JobSummaryTypeDef = TypedDict(
     "JobSummaryTypeDef",
     {
-        "bucketCriteria": S3BucketCriteriaForJobTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobTypeDef],
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
         "createdAt": datetime,
         "jobId": str,
         "jobStatus": JobStatusType,
         "jobType": JobTypeType,
         "lastRunErrorStatus": LastRunErrorStatusTypeDef,
         "name": str,
         "userPausedDetails": UserPausedDetailsTypeDef,
     },
     total=False,
 )
 
+S3JobDefinitionOutputTypeDef = TypedDict(
+    "S3JobDefinitionOutputTypeDef",
+    {
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
+        "scoping": ScopingOutputTypeDef,
+    },
+    total=False,
+)
+
 S3JobDefinitionTypeDef = TypedDict(
     "S3JobDefinitionTypeDef",
     {
         "bucketCriteria": S3BucketCriteriaForJobTypeDef,
         "bucketDefinitions": Sequence[S3BucketDefinitionForJobTypeDef],
         "scoping": ScopingTypeDef,
     },
@@ -3282,14 +3584,42 @@
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeClassificationJobResponseTypeDef = TypedDict(
+    "DescribeClassificationJobResponseTypeDef",
+    {
+        "allowListIds": List[str],
+        "clientToken": str,
+        "createdAt": datetime,
+        "customDataIdentifierIds": List[str],
+        "description": str,
+        "initialRun": bool,
+        "jobArn": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "jobType": JobTypeType,
+        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
+        "lastRunTime": datetime,
+        "managedDataIdentifierIds": List[str],
+        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
+        "name": str,
+        "s3JobDefinition": S3JobDefinitionOutputTypeDef,
+        "samplingPercentage": int,
+        "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
+        "statistics": StatisticsTypeDef,
+        "tags": Dict[str, str],
+        "userPausedDetails": UserPausedDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
         "jobType": JobTypeType,
         "name": str,
         "s3JobDefinition": S3JobDefinitionTypeDef,
@@ -3313,42 +3643,14 @@
 
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
-DescribeClassificationJobResponseTypeDef = TypedDict(
-    "DescribeClassificationJobResponseTypeDef",
-    {
-        "allowListIds": List[str],
-        "clientToken": str,
-        "createdAt": datetime,
-        "customDataIdentifierIds": List[str],
-        "description": str,
-        "initialRun": bool,
-        "jobArn": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "jobType": JobTypeType,
-        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
-        "lastRunTime": datetime,
-        "managedDataIdentifierIds": List[str],
-        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
-        "name": str,
-        "s3JobDefinition": S3JobDefinitionTypeDef,
-        "samplingPercentage": int,
-        "scheduleFrequency": JobScheduleFrequencyTypeDef,
-        "statistics": StatisticsTypeDef,
-        "tags": Dict[str, str],
-        "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
```

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/waiter.py` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2/waiter.pyi` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/PKG-INFO` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.28.0
-Summary: Type annotations for boto3.Macie2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Macie2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-macie2"></a>
 
 # mypy-boto3-macie2
 
 [![PyPI - mypy-boto3-macie2](https://img.shields.io/pypi/v/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie2?color=blue)](https://pypistats.org/packages/mypy-boto3-macie2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -467,14 +467,15 @@
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
     AdminAccountTypeDef,
+    S3WordsListOutputTypeDef,
     S3WordsListTypeDef,
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
@@ -490,27 +491,30 @@
     KeyValuePairTypeDef,
     ObjectCountByEncryptionTypeTypeDef,
     ObjectLevelStatisticsTypeDef,
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
+    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
     CreateAllowListResponseTypeDef,
     CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
     CreateCustomDataIdentifierResponseTypeDef,
     CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
     CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
+    SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
+    CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
@@ -532,45 +536,49 @@
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
+    SeverityLevelOutputTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
-    SecurityHubConfigurationTypeDef,
+    SecurityHubConfigurationOutputTypeDef,
     SortCriteriaTypeDef,
     GetInvitationsCountResponseTypeDef,
     GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
     GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
-    RevealConfigurationTypeDef,
+    RevealConfigurationOutputTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesOutputTypeDef,
+    SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
+    MonthlyScheduleOutputTypeDef,
+    WeeklyScheduleOutputTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
+    SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
-    S3BucketDefinitionForJobTypeDef,
+    S3BucketDefinitionForJobOutputTypeDef,
     ListAllowListsRequestListAllowListsPaginateTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
     ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
     ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
@@ -597,28 +605,35 @@
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
     PaginatorConfigTypeDef,
+    SecurityHubConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    RevealConfigurationTypeDef,
+    S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
+    TagCriterionPairForJobOutputTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagValuePairOutputTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
@@ -627,124 +642,137 @@
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    AllowListCriteriaOutputTypeDef,
     AllowListCriteriaTypeDef,
     ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
     DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
+    ClassificationExportConfigurationOutputTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
-    GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetCustomDataIdentifierResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
     GetFindingsPublicationConfigurationResponseTypeDef,
-    PutFindingsPublicationConfigurationRequestRequestTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
-    UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
-    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
+    JobScheduleFrequencyOutputTypeDef,
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
+    PutFindingsPublicationConfigurationRequestRequestTypeDef,
+    UpdateRevealConfigurationRequestRequestTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
+    TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
+    TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
-    CreateAllowListRequestRequestTypeDef,
     GetAllowListResponseTypeDef,
+    CreateAllowListRequestRequestTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
-    PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
+    PutClassificationExportConfigurationRequestRequestTypeDef,
+    GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
-    GetFindingsFilterResponseTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
     AssumedRoleTypeDef,
     FederatedUserTypeDef,
+    CriteriaForJobOutputTypeDef,
     CriteriaForJobTypeDef,
+    JobScopeTermOutputTypeDef,
     JobScopeTermTypeDef,
     BucketPublicAccessTypeDef,
     SearchResourcesResponseTypeDef,
     CustomDetectionTypeDef,
     DefaultDetectionTypeDef,
     SearchResourcesCriteriaBlockTypeDef,
     GetUsageStatisticsResponseTypeDef,
     UserIdentityTypeDef,
+    CriteriaBlockForJobOutputTypeDef,
     CriteriaBlockForJobTypeDef,
+    JobScopingBlockOutputTypeDef,
     JobScopingBlockTypeDef,
     BucketMetadataTypeDef,
     S3BucketTypeDef,
     CustomDataIdentifiersTypeDef,
     SensitiveDataItemTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     FindingActorTypeDef,
+    S3BucketCriteriaForJobOutputTypeDef,
     S3BucketCriteriaForJobTypeDef,
+    ScopingOutputTypeDef,
     ScopingTypeDef,
     DescribeBucketsResponseTypeDef,
     ResourcesAffectedTypeDef,
     ClassificationResultTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     PolicyDetailsTypeDef,
     JobSummaryTypeDef,
+    S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
-    CreateClassificationJobRequestRequestTypeDef,
     DescribeClassificationJobResponseTypeDef,
+    CreateClassificationJobRequestRequestTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-macie2-1.28.0/mypy_boto3_macie2.egg-info/SOURCES.txt` & `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.0/setup.py` & `mypy-boto3-macie2-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-macie2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Macie2 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Macie2 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

