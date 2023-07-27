# Comparing `tmp/mypy-boto3-inspector2-1.28.0.tar.gz` & `tmp/mypy-boto3-inspector2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.28.0.tar", last modified: Thu Jul  6 20:59:44 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector2-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
```

## Comparing `mypy-boto3-inspector2-1.28.0.tar` & `mypy-boto3-inspector2-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.106322 mypy-boto3-inspector2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-06 20:59:44.102322 mypy-boto3-inspector2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21720 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.098322 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-07-06 20:43:05.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-06 20:43:05.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-07-06 20:43:05.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-06 20:43:05.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-06 20:43:05.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-06 20:43:05.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    72406 2023-07-06 20:43:09.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72325 2023-07-06 20:43:06.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.102322 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-06 20:59:43.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:43.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:43.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:43.000000 mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:44.106322 mypy-boto3-inspector2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:43:04.000000 mypy-boto3-inspector2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23597 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22098 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-27 05:23:37.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79197 2023-07-27 05:23:38.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79108 2023-07-27 05:23:38.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23597 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:46.000000 mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.068491 mypy-boto3-inspector2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:23:36.000000 mypy-boto3-inspector2-1.28.12/setup.py
```

### Comparing `mypy-boto3-inspector2-1.28.0/LICENSE` & `mypy-boto3-inspector2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/PKG-INFO` & `mypy-boto3-inspector2-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.0
-Summary: Type annotations for boto3.Inspector2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Inspector2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-inspector2"></a>
 
 # mypy-boto3-inspector2
 
 [![PyPI - mypy-boto3-inspector2](https://img.shields.io/pypi/v/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,14 +428,15 @@
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AtigDataTypeDef,
+    AutoEnableOutputTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
@@ -462,19 +463,21 @@
     DestinationTypeDef,
     CreateFindingsReportResponseTypeDef,
     CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
+    DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteFilterResponseTypeDef,
+    DestinationOutputTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
@@ -485,14 +488,18 @@
     EnableDelegatedAdminAccountRequestRequestTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
+    MapFilterOutputTypeDef,
+    NumberFilterOutputTypeDef,
+    PortRangeFilterOutputTypeDef,
+    StringFilterOutputTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
@@ -516,14 +523,16 @@
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
     PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
+    ResourceMapFilterOutputTypeDef,
+    ResourceStringFilterOutputTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
     ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
@@ -550,16 +559,16 @@
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
+    UpdateOrganizationConfigurationRequestRequestTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
@@ -568,23 +577,25 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
+    PackageFilterOutputTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
     SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
@@ -595,30 +606,31 @@
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
-    CreateSbomExportRequestRequestTypeDef,
     GetSbomExportResponseTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
-    CreateFilterRequestRequestTypeDef,
-    CreateFindingsReportRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    CreateFindingsReportRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.0/README.md` & `mypy-boto3-inspector2-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-inspector2"></a>
 
 # mypy-boto3-inspector2
 
 [![PyPI - mypy-boto3-inspector2](https://img.shields.io/pypi/v/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,14 +396,15 @@
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AtigDataTypeDef,
+    AutoEnableOutputTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
@@ -430,19 +431,21 @@
     DestinationTypeDef,
     CreateFindingsReportResponseTypeDef,
     CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
+    DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteFilterResponseTypeDef,
+    DestinationOutputTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
@@ -453,14 +456,18 @@
     EnableDelegatedAdminAccountRequestRequestTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
+    MapFilterOutputTypeDef,
+    NumberFilterOutputTypeDef,
+    PortRangeFilterOutputTypeDef,
+    StringFilterOutputTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
@@ -484,14 +491,16 @@
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
     PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
+    ResourceMapFilterOutputTypeDef,
+    ResourceStringFilterOutputTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
     ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
@@ -518,16 +527,16 @@
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
+    UpdateOrganizationConfigurationRequestRequestTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
@@ -536,23 +545,25 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
+    PackageFilterOutputTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
     SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
@@ -563,30 +574,31 @@
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
-    CreateSbomExportRequestRequestTypeDef,
     GetSbomExportResponseTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
-    CreateFilterRequestRequestTypeDef,
-    CreateFindingsReportRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    CreateFindingsReportRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/__init__.py` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/__init__.pyi` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/__main__.py` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Inspector2 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
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

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/client.py` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/client.pyi` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/literals.py` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,15 @@
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
@@ -518,26 +519,28 @@
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

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/literals.pyi` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -430,14 +430,15 @@
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
@@ -516,26 +517,28 @@
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

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/paginator.py` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/paginator.pyi` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/type_defs.py` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
     "AssociateMemberResponseTypeDef",
     "AtigDataTypeDef",
+    "AutoEnableOutputTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
@@ -125,19 +126,21 @@
     "DestinationTypeDef",
     "CreateFindingsReportResponseTypeDef",
     "CreateSbomExportResponseTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
+    "DateFilterOutputTypeDef",
     "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteFilterResponseTypeDef",
+    "DestinationOutputTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
@@ -148,14 +151,18 @@
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
     "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
+    "MapFilterOutputTypeDef",
+    "NumberFilterOutputTypeDef",
+    "PortRangeFilterOutputTypeDef",
+    "StringFilterOutputTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
     "GetEc2DeepInspectionConfigurationResponseTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
     "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
@@ -179,14 +186,16 @@
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
     "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "ResetEncryptionKeyRequestRequestTypeDef",
+    "ResourceMapFilterOutputTypeDef",
+    "ResourceStringFilterOutputTypeDef",
     "ResourceMapFilterTypeDef",
     "ResourceStringFilterTypeDef",
     "ResponseMetadataTypeDef",
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
@@ -213,16 +222,16 @@
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
-    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateOrganizationConfigurationResponseTypeDef",
+    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
@@ -231,23 +240,25 @@
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "VulnerabilityTypeDef",
+    "PackageFilterOutputTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
@@ -258,30 +269,31 @@
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
+    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "CreateSbomExportRequestRequestTypeDef",
     "GetSbomExportResponseTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "CreateFilterRequestRequestTypeDef",
-    "CreateFindingsReportRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "CreateFindingsReportRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -380,14 +392,35 @@
         "lastSeen": datetime,
         "targets": List[str],
         "ttps": List[str],
     },
     total=False,
 )
 
+_RequiredAutoEnableOutputTypeDef = TypedDict(
+    "_RequiredAutoEnableOutputTypeDef",
+    {
+        "ec2": bool,
+        "ecr": bool,
+    },
+)
+_OptionalAutoEnableOutputTypeDef = TypedDict(
+    "_OptionalAutoEnableOutputTypeDef",
+    {
+        "lambda": bool,
+        "lambdaCode": bool,
+    },
+    total=False,
+)
+
+
+class AutoEnableOutputTypeDef(_RequiredAutoEnableOutputTypeDef, _OptionalAutoEnableOutputTypeDef):
+    pass
+
+
 _RequiredAutoEnableTypeDef = TypedDict(
     "_RequiredAutoEnableTypeDef",
     {
         "ec2": bool,
         "ecr": bool,
     },
 )
@@ -760,14 +793,23 @@
         "baseScore": float,
         "scoringVector": str,
         "source": str,
         "version": str,
     },
 )
 
+DateFilterOutputTypeDef = TypedDict(
+    "DateFilterOutputTypeDef",
+    {
+        "endInclusive": datetime,
+        "startInclusive": datetime,
+    },
+    total=False,
+)
+
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "endInclusive": Union[datetime, str],
         "startInclusive": Union[datetime, str],
     },
     total=False,
@@ -802,14 +844,36 @@
     "DeleteFilterResponseTypeDef",
     {
         "arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDestinationOutputTypeDef = TypedDict(
+    "_RequiredDestinationOutputTypeDef",
+    {
+        "bucketName": str,
+        "kmsKeyArn": str,
+    },
+)
+_OptionalDestinationOutputTypeDef = TypedDict(
+    "_OptionalDestinationOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+
+class DestinationOutputTypeDef(
+    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
+):
+    pass
+
+
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
@@ -990,14 +1054,60 @@
     "ExploitabilityDetailsTypeDef",
     {
         "lastKnownExploitAt": datetime,
     },
     total=False,
 )
 
+_RequiredMapFilterOutputTypeDef = TypedDict(
+    "_RequiredMapFilterOutputTypeDef",
+    {
+        "comparison": Literal["EQUALS"],
+        "key": str,
+    },
+)
+_OptionalMapFilterOutputTypeDef = TypedDict(
+    "_OptionalMapFilterOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class MapFilterOutputTypeDef(_RequiredMapFilterOutputTypeDef, _OptionalMapFilterOutputTypeDef):
+    pass
+
+
+NumberFilterOutputTypeDef = TypedDict(
+    "NumberFilterOutputTypeDef",
+    {
+        "lowerInclusive": float,
+        "upperInclusive": float,
+    },
+    total=False,
+)
+
+PortRangeFilterOutputTypeDef = TypedDict(
+    "PortRangeFilterOutputTypeDef",
+    {
+        "beginInclusive": int,
+        "endInclusive": int,
+    },
+    total=False,
+)
+
+StringFilterOutputTypeDef = TypedDict(
+    "StringFilterOutputTypeDef",
+    {
+        "comparison": StringComparisonType,
+        "value": str,
+    },
+)
+
 NumberFilterTypeDef = TypedDict(
     "NumberFilterTypeDef",
     {
         "lowerInclusive": float,
         "upperInclusive": float,
     },
     total=False,
@@ -1288,14 +1398,44 @@
     "ResetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
+_RequiredResourceMapFilterOutputTypeDef = TypedDict(
+    "_RequiredResourceMapFilterOutputTypeDef",
+    {
+        "comparison": Literal["EQUALS"],
+        "key": str,
+    },
+)
+_OptionalResourceMapFilterOutputTypeDef = TypedDict(
+    "_OptionalResourceMapFilterOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class ResourceMapFilterOutputTypeDef(
+    _RequiredResourceMapFilterOutputTypeDef, _OptionalResourceMapFilterOutputTypeDef
+):
+    pass
+
+
+ResourceStringFilterOutputTypeDef = TypedDict(
+    "ResourceStringFilterOutputTypeDef",
+    {
+        "comparison": ResourceStringComparisonType,
+        "value": str,
+    },
+)
+
 _RequiredResourceMapFilterTypeDef = TypedDict(
     "_RequiredResourceMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -1780,32 +1920,32 @@
     },
     total=False,
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnable": AutoEnableTypeDef,
+        "autoEnable": AutoEnableOutputTypeDef,
         "maxAccountLimitReached": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationRequestRequestTypeDef",
+UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnable": AutoEnableTypeDef,
+        "autoEnable": AutoEnableOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationResponseTypeDef",
+UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -2039,14 +2179,28 @@
 )
 
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
 
+PackageFilterOutputTypeDef = TypedDict(
+    "PackageFilterOutputTypeDef",
+    {
+        "architecture": StringFilterOutputTypeDef,
+        "epoch": NumberFilterOutputTypeDef,
+        "name": StringFilterOutputTypeDef,
+        "release": StringFilterOutputTypeDef,
+        "sourceLambdaLayerArn": StringFilterOutputTypeDef,
+        "sourceLayerHash": StringFilterOutputTypeDef,
+        "version": StringFilterOutputTypeDef,
+    },
+    total=False,
+)
+
 PackageFilterTypeDef = TypedDict(
     "PackageFilterTypeDef",
     {
         "architecture": StringFilterTypeDef,
         "epoch": NumberFilterTypeDef,
         "name": StringFilterTypeDef,
         "release": StringFilterTypeDef,
@@ -2143,14 +2297,29 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+ResourceFilterCriteriaOutputTypeDef = TypedDict(
+    "ResourceFilterCriteriaOutputTypeDef",
+    {
+        "accountId": List[ResourceStringFilterOutputTypeDef],
+        "ec2InstanceTags": List[ResourceMapFilterOutputTypeDef],
+        "ecrImageTags": List[ResourceStringFilterOutputTypeDef],
+        "ecrRepositoryName": List[ResourceStringFilterOutputTypeDef],
+        "lambdaFunctionName": List[ResourceStringFilterOutputTypeDef],
+        "lambdaFunctionTags": List[ResourceMapFilterOutputTypeDef],
+        "resourceId": List[ResourceStringFilterOutputTypeDef],
+        "resourceType": List[ResourceStringFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": Sequence[ResourceStringFilterTypeDef],
         "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
         "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
         "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
@@ -2357,14 +2526,63 @@
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FilterCriteriaOutputTypeDef = TypedDict(
+    "FilterCriteriaOutputTypeDef",
+    {
+        "awsAccountId": List[StringFilterOutputTypeDef],
+        "codeVulnerabilityDetectorName": List[StringFilterOutputTypeDef],
+        "codeVulnerabilityDetectorTags": List[StringFilterOutputTypeDef],
+        "codeVulnerabilityFilePath": List[StringFilterOutputTypeDef],
+        "componentId": List[StringFilterOutputTypeDef],
+        "componentType": List[StringFilterOutputTypeDef],
+        "ec2InstanceImageId": List[StringFilterOutputTypeDef],
+        "ec2InstanceSubnetId": List[StringFilterOutputTypeDef],
+        "ec2InstanceVpcId": List[StringFilterOutputTypeDef],
+        "ecrImageArchitecture": List[StringFilterOutputTypeDef],
+        "ecrImageHash": List[StringFilterOutputTypeDef],
+        "ecrImagePushedAt": List[DateFilterOutputTypeDef],
+        "ecrImageRegistry": List[StringFilterOutputTypeDef],
+        "ecrImageRepositoryName": List[StringFilterOutputTypeDef],
+        "ecrImageTags": List[StringFilterOutputTypeDef],
+        "epssScore": List[NumberFilterOutputTypeDef],
+        "exploitAvailable": List[StringFilterOutputTypeDef],
+        "findingArn": List[StringFilterOutputTypeDef],
+        "findingStatus": List[StringFilterOutputTypeDef],
+        "findingType": List[StringFilterOutputTypeDef],
+        "firstObservedAt": List[DateFilterOutputTypeDef],
+        "fixAvailable": List[StringFilterOutputTypeDef],
+        "inspectorScore": List[NumberFilterOutputTypeDef],
+        "lambdaFunctionExecutionRoleArn": List[StringFilterOutputTypeDef],
+        "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
+        "lambdaFunctionLayers": List[StringFilterOutputTypeDef],
+        "lambdaFunctionName": List[StringFilterOutputTypeDef],
+        "lambdaFunctionRuntime": List[StringFilterOutputTypeDef],
+        "lastObservedAt": List[DateFilterOutputTypeDef],
+        "networkProtocol": List[StringFilterOutputTypeDef],
+        "portRange": List[PortRangeFilterOutputTypeDef],
+        "relatedVulnerabilities": List[StringFilterOutputTypeDef],
+        "resourceId": List[StringFilterOutputTypeDef],
+        "resourceTags": List[MapFilterOutputTypeDef],
+        "resourceType": List[StringFilterOutputTypeDef],
+        "severity": List[StringFilterOutputTypeDef],
+        "title": List[StringFilterOutputTypeDef],
+        "updatedAt": List[DateFilterOutputTypeDef],
+        "vendorSeverity": List[StringFilterOutputTypeDef],
+        "vulnerabilityId": List[StringFilterOutputTypeDef],
+        "vulnerabilitySource": List[StringFilterOutputTypeDef],
+        "vulnerablePackages": List[PackageFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorTags": Sequence[StringFilterTypeDef],
         "codeVulnerabilityFilePath": Sequence[StringFilterTypeDef],
@@ -2448,14 +2666,28 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationOutputTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
         "s3Destination": DestinationTypeDef,
     },
 )
@@ -2470,28 +2702,14 @@
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
 
-GetSbomExportResponseTypeDef = TypedDict(
-    "GetSbomExportResponseTypeDef",
-    {
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaTypeDef,
-        "format": SbomReportFormatType,
-        "reportId": str,
-        "s3Destination": DestinationTypeDef,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2584,14 +2802,54 @@
 class ListFindingAggregationsRequestRequestTypeDef(
     _RequiredListFindingAggregationsRequestRequestTypeDef,
     _OptionalListFindingAggregationsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredFilterTypeDef = TypedDict(
+    "_RequiredFilterTypeDef",
+    {
+        "action": FilterActionType,
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": FilterCriteriaOutputTypeDef,
+        "name": str,
+        "ownerId": str,
+        "updatedAt": datetime,
+    },
+)
+_OptionalFilterTypeDef = TypedDict(
+    "_OptionalFilterTypeDef",
+    {
+        "description": str,
+        "reason": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
+    pass
+
+
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
+    {
+        "destination": DestinationOutputTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaOutputTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
         "name": str,
     },
@@ -2632,54 +2890,14 @@
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredFilterTypeDef = TypedDict(
-    "_RequiredFilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-    },
-)
-_OptionalFilterTypeDef = TypedDict(
-    "_OptionalFilterTypeDef",
-    {
-        "description": str,
-        "reason": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
-    pass
-
-
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
-    {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
```

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2/type_defs.pyi` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
     "AssociateMemberResponseTypeDef",
     "AtigDataTypeDef",
+    "AutoEnableOutputTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
@@ -124,19 +125,21 @@
     "DestinationTypeDef",
     "CreateFindingsReportResponseTypeDef",
     "CreateSbomExportResponseTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
+    "DateFilterOutputTypeDef",
     "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteFilterResponseTypeDef",
+    "DestinationOutputTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
@@ -147,14 +150,18 @@
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
     "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
+    "MapFilterOutputTypeDef",
+    "NumberFilterOutputTypeDef",
+    "PortRangeFilterOutputTypeDef",
+    "StringFilterOutputTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
     "GetEc2DeepInspectionConfigurationResponseTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
     "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
@@ -178,14 +185,16 @@
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
     "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "ResetEncryptionKeyRequestRequestTypeDef",
+    "ResourceMapFilterOutputTypeDef",
+    "ResourceStringFilterOutputTypeDef",
     "ResourceMapFilterTypeDef",
     "ResourceStringFilterTypeDef",
     "ResponseMetadataTypeDef",
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
@@ -212,16 +221,16 @@
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
-    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateOrganizationConfigurationResponseTypeDef",
+    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
@@ -230,23 +239,25 @@
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "VulnerabilityTypeDef",
+    "PackageFilterOutputTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
@@ -257,30 +268,31 @@
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
+    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "CreateSbomExportRequestRequestTypeDef",
     "GetSbomExportResponseTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "CreateFilterRequestRequestTypeDef",
-    "CreateFindingsReportRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "CreateFindingsReportRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -377,14 +389,33 @@
         "lastSeen": datetime,
         "targets": List[str],
         "ttps": List[str],
     },
     total=False,
 )
 
+_RequiredAutoEnableOutputTypeDef = TypedDict(
+    "_RequiredAutoEnableOutputTypeDef",
+    {
+        "ec2": bool,
+        "ecr": bool,
+    },
+)
+_OptionalAutoEnableOutputTypeDef = TypedDict(
+    "_OptionalAutoEnableOutputTypeDef",
+    {
+        "lambda": bool,
+        "lambdaCode": bool,
+    },
+    total=False,
+)
+
+class AutoEnableOutputTypeDef(_RequiredAutoEnableOutputTypeDef, _OptionalAutoEnableOutputTypeDef):
+    pass
+
 _RequiredAutoEnableTypeDef = TypedDict(
     "_RequiredAutoEnableTypeDef",
     {
         "ec2": bool,
         "ecr": bool,
     },
 )
@@ -745,14 +776,23 @@
         "baseScore": float,
         "scoringVector": str,
         "source": str,
         "version": str,
     },
 )
 
+DateFilterOutputTypeDef = TypedDict(
+    "DateFilterOutputTypeDef",
+    {
+        "endInclusive": datetime,
+        "startInclusive": datetime,
+    },
+    total=False,
+)
+
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "endInclusive": Union[datetime, str],
         "startInclusive": Union[datetime, str],
     },
     total=False,
@@ -787,14 +827,34 @@
     "DeleteFilterResponseTypeDef",
     {
         "arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDestinationOutputTypeDef = TypedDict(
+    "_RequiredDestinationOutputTypeDef",
+    {
+        "bucketName": str,
+        "kmsKeyArn": str,
+    },
+)
+_OptionalDestinationOutputTypeDef = TypedDict(
+    "_OptionalDestinationOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+class DestinationOutputTypeDef(
+    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
+):
+    pass
+
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
@@ -969,14 +1029,58 @@
     "ExploitabilityDetailsTypeDef",
     {
         "lastKnownExploitAt": datetime,
     },
     total=False,
 )
 
+_RequiredMapFilterOutputTypeDef = TypedDict(
+    "_RequiredMapFilterOutputTypeDef",
+    {
+        "comparison": Literal["EQUALS"],
+        "key": str,
+    },
+)
+_OptionalMapFilterOutputTypeDef = TypedDict(
+    "_OptionalMapFilterOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class MapFilterOutputTypeDef(_RequiredMapFilterOutputTypeDef, _OptionalMapFilterOutputTypeDef):
+    pass
+
+NumberFilterOutputTypeDef = TypedDict(
+    "NumberFilterOutputTypeDef",
+    {
+        "lowerInclusive": float,
+        "upperInclusive": float,
+    },
+    total=False,
+)
+
+PortRangeFilterOutputTypeDef = TypedDict(
+    "PortRangeFilterOutputTypeDef",
+    {
+        "beginInclusive": int,
+        "endInclusive": int,
+    },
+    total=False,
+)
+
+StringFilterOutputTypeDef = TypedDict(
+    "StringFilterOutputTypeDef",
+    {
+        "comparison": StringComparisonType,
+        "value": str,
+    },
+)
+
 NumberFilterTypeDef = TypedDict(
     "NumberFilterTypeDef",
     {
         "lowerInclusive": float,
         "upperInclusive": float,
     },
     total=False,
@@ -1265,14 +1369,42 @@
     "ResetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
+_RequiredResourceMapFilterOutputTypeDef = TypedDict(
+    "_RequiredResourceMapFilterOutputTypeDef",
+    {
+        "comparison": Literal["EQUALS"],
+        "key": str,
+    },
+)
+_OptionalResourceMapFilterOutputTypeDef = TypedDict(
+    "_OptionalResourceMapFilterOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class ResourceMapFilterOutputTypeDef(
+    _RequiredResourceMapFilterOutputTypeDef, _OptionalResourceMapFilterOutputTypeDef
+):
+    pass
+
+ResourceStringFilterOutputTypeDef = TypedDict(
+    "ResourceStringFilterOutputTypeDef",
+    {
+        "comparison": ResourceStringComparisonType,
+        "value": str,
+    },
+)
+
 _RequiredResourceMapFilterTypeDef = TypedDict(
     "_RequiredResourceMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -1733,32 +1865,32 @@
     },
     total=False,
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnable": AutoEnableTypeDef,
+        "autoEnable": AutoEnableOutputTypeDef,
         "maxAccountLimitReached": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationRequestRequestTypeDef",
+UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnable": AutoEnableTypeDef,
+        "autoEnable": AutoEnableOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
-    "UpdateOrganizationConfigurationResponseTypeDef",
+UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -1984,14 +2116,28 @@
     },
     total=False,
 )
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
+PackageFilterOutputTypeDef = TypedDict(
+    "PackageFilterOutputTypeDef",
+    {
+        "architecture": StringFilterOutputTypeDef,
+        "epoch": NumberFilterOutputTypeDef,
+        "name": StringFilterOutputTypeDef,
+        "release": StringFilterOutputTypeDef,
+        "sourceLambdaLayerArn": StringFilterOutputTypeDef,
+        "sourceLayerHash": StringFilterOutputTypeDef,
+        "version": StringFilterOutputTypeDef,
+    },
+    total=False,
+)
+
 PackageFilterTypeDef = TypedDict(
     "PackageFilterTypeDef",
     {
         "architecture": StringFilterTypeDef,
         "epoch": NumberFilterTypeDef,
         "name": StringFilterTypeDef,
         "release": StringFilterTypeDef,
@@ -2086,14 +2232,29 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+ResourceFilterCriteriaOutputTypeDef = TypedDict(
+    "ResourceFilterCriteriaOutputTypeDef",
+    {
+        "accountId": List[ResourceStringFilterOutputTypeDef],
+        "ec2InstanceTags": List[ResourceMapFilterOutputTypeDef],
+        "ecrImageTags": List[ResourceStringFilterOutputTypeDef],
+        "ecrRepositoryName": List[ResourceStringFilterOutputTypeDef],
+        "lambdaFunctionName": List[ResourceStringFilterOutputTypeDef],
+        "lambdaFunctionTags": List[ResourceMapFilterOutputTypeDef],
+        "resourceId": List[ResourceStringFilterOutputTypeDef],
+        "resourceType": List[ResourceStringFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": Sequence[ResourceStringFilterTypeDef],
         "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
         "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
         "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
@@ -2296,14 +2457,63 @@
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FilterCriteriaOutputTypeDef = TypedDict(
+    "FilterCriteriaOutputTypeDef",
+    {
+        "awsAccountId": List[StringFilterOutputTypeDef],
+        "codeVulnerabilityDetectorName": List[StringFilterOutputTypeDef],
+        "codeVulnerabilityDetectorTags": List[StringFilterOutputTypeDef],
+        "codeVulnerabilityFilePath": List[StringFilterOutputTypeDef],
+        "componentId": List[StringFilterOutputTypeDef],
+        "componentType": List[StringFilterOutputTypeDef],
+        "ec2InstanceImageId": List[StringFilterOutputTypeDef],
+        "ec2InstanceSubnetId": List[StringFilterOutputTypeDef],
+        "ec2InstanceVpcId": List[StringFilterOutputTypeDef],
+        "ecrImageArchitecture": List[StringFilterOutputTypeDef],
+        "ecrImageHash": List[StringFilterOutputTypeDef],
+        "ecrImagePushedAt": List[DateFilterOutputTypeDef],
+        "ecrImageRegistry": List[StringFilterOutputTypeDef],
+        "ecrImageRepositoryName": List[StringFilterOutputTypeDef],
+        "ecrImageTags": List[StringFilterOutputTypeDef],
+        "epssScore": List[NumberFilterOutputTypeDef],
+        "exploitAvailable": List[StringFilterOutputTypeDef],
+        "findingArn": List[StringFilterOutputTypeDef],
+        "findingStatus": List[StringFilterOutputTypeDef],
+        "findingType": List[StringFilterOutputTypeDef],
+        "firstObservedAt": List[DateFilterOutputTypeDef],
+        "fixAvailable": List[StringFilterOutputTypeDef],
+        "inspectorScore": List[NumberFilterOutputTypeDef],
+        "lambdaFunctionExecutionRoleArn": List[StringFilterOutputTypeDef],
+        "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
+        "lambdaFunctionLayers": List[StringFilterOutputTypeDef],
+        "lambdaFunctionName": List[StringFilterOutputTypeDef],
+        "lambdaFunctionRuntime": List[StringFilterOutputTypeDef],
+        "lastObservedAt": List[DateFilterOutputTypeDef],
+        "networkProtocol": List[StringFilterOutputTypeDef],
+        "portRange": List[PortRangeFilterOutputTypeDef],
+        "relatedVulnerabilities": List[StringFilterOutputTypeDef],
+        "resourceId": List[StringFilterOutputTypeDef],
+        "resourceTags": List[MapFilterOutputTypeDef],
+        "resourceType": List[StringFilterOutputTypeDef],
+        "severity": List[StringFilterOutputTypeDef],
+        "title": List[StringFilterOutputTypeDef],
+        "updatedAt": List[DateFilterOutputTypeDef],
+        "vendorSeverity": List[StringFilterOutputTypeDef],
+        "vulnerabilityId": List[StringFilterOutputTypeDef],
+        "vulnerabilitySource": List[StringFilterOutputTypeDef],
+        "vulnerablePackages": List[PackageFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorTags": Sequence[StringFilterTypeDef],
         "codeVulnerabilityFilePath": Sequence[StringFilterTypeDef],
@@ -2385,14 +2595,28 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationOutputTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
         "s3Destination": DestinationTypeDef,
     },
 )
@@ -2405,28 +2629,14 @@
 )
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
-GetSbomExportResponseTypeDef = TypedDict(
-    "GetSbomExportResponseTypeDef",
-    {
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaTypeDef,
-        "format": SbomReportFormatType,
-        "reportId": str,
-        "s3Destination": DestinationTypeDef,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2513,14 +2723,52 @@
 
 class ListFindingAggregationsRequestRequestTypeDef(
     _RequiredListFindingAggregationsRequestRequestTypeDef,
     _OptionalListFindingAggregationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredFilterTypeDef = TypedDict(
+    "_RequiredFilterTypeDef",
+    {
+        "action": FilterActionType,
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": FilterCriteriaOutputTypeDef,
+        "name": str,
+        "ownerId": str,
+        "updatedAt": datetime,
+    },
+)
+_OptionalFilterTypeDef = TypedDict(
+    "_OptionalFilterTypeDef",
+    {
+        "description": str,
+        "reason": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
+    pass
+
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
+    {
+        "destination": DestinationOutputTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaOutputTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
         "name": str,
     },
@@ -2557,52 +2805,14 @@
 
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
-_RequiredFilterTypeDef = TypedDict(
-    "_RequiredFilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-    },
-)
-_OptionalFilterTypeDef = TypedDict(
-    "_OptionalFilterTypeDef",
-    {
-        "description": str,
-        "reason": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
-    pass
-
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
-    {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
```

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.0
-Summary: Type annotations for boto3.Inspector2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Inspector2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-inspector2"></a>
 
 # mypy-boto3-inspector2
 
 [![PyPI - mypy-boto3-inspector2](https://img.shields.io/pypi/v/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,14 +428,15 @@
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AtigDataTypeDef,
+    AutoEnableOutputTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
     CodeSnippetErrorTypeDef,
@@ -462,19 +463,21 @@
     DestinationTypeDef,
     CreateFindingsReportResponseTypeDef,
     CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
+    DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteFilterResponseTypeDef,
+    DestinationOutputTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
@@ -485,14 +488,18 @@
     EnableDelegatedAdminAccountRequestRequestTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
+    MapFilterOutputTypeDef,
+    NumberFilterOutputTypeDef,
+    PortRangeFilterOutputTypeDef,
+    StringFilterOutputTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
@@ -516,14 +523,16 @@
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
     PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
+    ResourceMapFilterOutputTypeDef,
+    ResourceStringFilterOutputTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
     ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
@@ -550,16 +559,16 @@
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
+    UpdateOrganizationConfigurationRequestRequestTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
@@ -568,23 +577,25 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
+    PackageFilterOutputTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
     SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
@@ -595,30 +606,31 @@
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
-    CreateSbomExportRequestRequestTypeDef,
     GetSbomExportResponseTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
-    CreateFilterRequestRequestTypeDef,
-    CreateFindingsReportRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    CreateFindingsReportRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
```

### Comparing `mypy-boto3-inspector2-1.28.0/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy-boto3-inspector2-1.28.12/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.0/setup.py` & `mypy-boto3-inspector2-1.28.12/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector2 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Inspector2 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

