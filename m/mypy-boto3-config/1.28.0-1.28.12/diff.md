# Comparing `tmp/mypy-boto3-config-1.28.0.tar.gz` & `tmp/mypy-boto3-config-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-config-1.28.0.tar", last modified: Thu Jul  6 20:59:19 2023, max compression
+gzip compressed data, was "mypy-boto3-config-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
```

## Comparing `mypy-boto3-config-1.28.0.tar` & `mypy-boto3-config-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.106266 mypy-boto3-config-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:43.000000 mypy-boto3-config-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36585 2023-07-06 20:59:19.106266 mypy-boto3-config-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-07-06 20:36:43.000000 mypy-boto3-config-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.098266 mypy-boto3-config-1.28.0/mypy_boto3_config/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-06 20:36:43.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-06 20:36:43.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 20:36:44.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88855 2023-07-06 20:36:46.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88725 2023-07-06 20:36:45.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30072 2023-07-06 20:36:46.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-07-06 20:36:46.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42993 2023-07-06 20:36:46.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    42960 2023-07-06 20:36:46.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:44.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   128172 2023-07-06 20:36:51.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   128021 2023-07-06 20:36:48.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:43.000000 mypy-boto3-config-1.28.0/mypy_boto3_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.106266 mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36585 2023-07-06 20:59:18.000000 mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:59:18.000000 mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:18.000000 mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:18.000000 mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:18.000000 mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:18.000000 mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:19.106266 mypy-boto3-config-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-06 20:36:43.000000 mypy-boto3-config-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.368543 mypy-boto3-config-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37783 2023-07-27 05:34:31.360543 mypy-boto3-config-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36293 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.356543 mypy-boto3-config-1.28.12/mypy_boto3_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88855 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88725 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42993 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42960 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   141473 2023-07-27 05:19:36.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141296 2023-07-27 05:19:35.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.360543 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37783 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.368543 mypy-boto3-config-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/setup.py
```

### Comparing `mypy-boto3-config-1.28.0/LICENSE` & `mypy-boto3-config-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/PKG-INFO` & `mypy-boto3-config-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.28.0
-Summary: Type annotations for boto3.ConfigService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ConfigService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-config"></a>
 
 # mypy-boto3-config
 
 [![PyPI - mypy-boto3-config](https://img.shields.io/pypi/v/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-config?color=blue)](https://pypistats.org/packages/mypy-boto3-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -506,45 +506,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_config.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_config.type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
+    AggregateResourceIdentifierOutputTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
     ResourceKeyTypeDef,
+    ResourceKeyOutputTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
+    EvaluationModeConfigurationOutputTypeDef,
+    ScopeOutputTypeDef,
     EvaluationModeConfigurationTypeDef,
     ScopeTypeDef,
+    ConfigSnapshotDeliveryPropertiesOutputTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
-    ConformancePackInputParameterTypeDef,
-    TemplateSSMDocumentDetailsTypeDef,
+    ConformancePackInputParameterOutputTypeDef,
+    TemplateSSMDocumentDetailsOutputTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
+    ConformancePackInputParameterTypeDef,
     ConformancePackRuleComplianceTypeDef,
     ConformancePackStatusDetailTypeDef,
+    CustomPolicyDetailsOutputTypeDef,
     CustomPolicyDetailsTypeDef,
     DeleteAggregationAuthorizationRequestRequestTypeDef,
     DeleteConfigRuleRequestRequestTypeDef,
     DeleteConfigurationAggregatorRequestRequestTypeDef,
     DeleteConfigurationRecorderRequestRequestTypeDef,
     DeleteConformancePackRequestRequestTypeDef,
     DeleteDeliveryChannelRequestRequestTypeDef,
@@ -595,21 +603,26 @@
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
     DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
+    EvaluationContextOutputTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
     EvaluationTypeDef,
+    ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
+    SsmControlsOutputTypeDef,
     SsmControlsTypeDef,
     ExternalEvaluationTypeDef,
+    RemediationExceptionResourceKeyOutputTypeDef,
     FieldInfoTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
     GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
@@ -627,141 +640,157 @@
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
     GetOrganizationCustomRulePolicyResponseTypeDef,
     GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
-    ResourceDetailsTypeDef,
+    ResourceDetailsOutputTypeDef,
     GetStoredQueryRequestRequestTypeDef,
-    StoredQueryTypeDef,
+    StoredQueryOutputTypeDef,
     ResourceFiltersTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
+    OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    OrganizationCustomPolicyRuleMetadataTypeDef,
     PaginatorConfigTypeDef,
+    TagTypeDef,
+    TemplateSSMDocumentDetailsTypeDef,
     PutConformancePackResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
+    StoredQueryTypeDef,
     PutStoredQueryResponseTypeDef,
+    RecordingStrategyOutputTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
+    ResourceValueOutputTypeDef,
+    StaticValueOutputTypeDef,
     ResourceValueTypeDef,
     StaticValueTypeDef,
+    ResourceDetailsTypeDef,
     TimeWindowTypeDef,
     ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
     SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
     SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+    SourceDetailOutputTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
     StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
     DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
-    BatchGetResourceConfigResponseTypeDef,
     DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
+    BatchGetResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
+    DeliveryChannelOutputTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
     DescribeConfigurationRecorderStatusResponseTypeDef,
     DescribeConformancePackComplianceRequestRequestTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListConformancePackComplianceScoresRequestRequestTypeDef,
     GetConformancePackComplianceSummaryResponseTypeDef,
     OrganizationConformancePackTypeDef,
-    PutOrganizationConformancePackRequestRequestTypeDef,
     ConformancePackDetailTypeDef,
-    PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
+    PutOrganizationConformancePackRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
-    FailedDeleteRemediationExceptionsBatchTypeDef,
     PutRemediationExceptionsRequestRequestTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
+    PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
     PutEvaluationsRequestRequestTypeDef,
-    PutEvaluationsResponseTypeDef,
+    ExecutionControlsOutputTypeDef,
     ExecutionControlsTypeDef,
     PutExternalEvaluationRequestRequestTypeDef,
+    FailedDeleteRemediationExceptionsBatchTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     GetOrganizationConformancePackDetailedStatusResponseTypeDef,
     GetResourceEvaluationSummaryResponseTypeDef,
-    StartResourceEvaluationRequestRequestTypeDef,
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    OrganizationConfigRuleTypeDef,
+    PutOrganizationConfigRuleRequestRequestTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
     PutConfigurationAggregatorRequestRequestTypeDef,
-    PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    OrganizationConfigRuleTypeDef,
-    PutOrganizationConfigRuleRequestRequestTypeDef,
+    PutConformancePackRequestRequestTypeDef,
+    PutStoredQueryRequestRequestTypeDef,
+    RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
+    RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
+    StartResourceEvaluationRequestRequestTypeDef,
     ResourceEvaluationFiltersTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
@@ -772,27 +801,30 @@
     DescribeDeliveryChannelStatusResponseTypeDef,
     DescribeConfigurationAggregatorsResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetResourceConfigHistoryResponseTypeDef,
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
-    DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    DeleteRemediationExceptionsResponseTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
     ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
     ListResourceEvaluationsRequestRequestTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
@@ -806,15 +838,15 @@
     PutRemediationConfigurationsRequestRequestTypeDef,
     DescribeConfigRulesResponseTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceTypeDef:
+def get_structure() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-config-1.28.0/README.md` & `mypy-boto3-config-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-config"></a>
 
 # mypy-boto3-config
 
 [![PyPI - mypy-boto3-config](https://img.shields.io/pypi/v/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-config?color=blue)](https://pypistats.org/packages/mypy-boto3-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -474,45 +474,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_config.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_config.type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
+    AggregateResourceIdentifierOutputTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
     ResourceKeyTypeDef,
+    ResourceKeyOutputTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
+    EvaluationModeConfigurationOutputTypeDef,
+    ScopeOutputTypeDef,
     EvaluationModeConfigurationTypeDef,
     ScopeTypeDef,
+    ConfigSnapshotDeliveryPropertiesOutputTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
-    ConformancePackInputParameterTypeDef,
-    TemplateSSMDocumentDetailsTypeDef,
+    ConformancePackInputParameterOutputTypeDef,
+    TemplateSSMDocumentDetailsOutputTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
+    ConformancePackInputParameterTypeDef,
     ConformancePackRuleComplianceTypeDef,
     ConformancePackStatusDetailTypeDef,
+    CustomPolicyDetailsOutputTypeDef,
     CustomPolicyDetailsTypeDef,
     DeleteAggregationAuthorizationRequestRequestTypeDef,
     DeleteConfigRuleRequestRequestTypeDef,
     DeleteConfigurationAggregatorRequestRequestTypeDef,
     DeleteConfigurationRecorderRequestRequestTypeDef,
     DeleteConformancePackRequestRequestTypeDef,
     DeleteDeliveryChannelRequestRequestTypeDef,
@@ -563,21 +571,26 @@
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
     DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
+    EvaluationContextOutputTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
     EvaluationTypeDef,
+    ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
+    SsmControlsOutputTypeDef,
     SsmControlsTypeDef,
     ExternalEvaluationTypeDef,
+    RemediationExceptionResourceKeyOutputTypeDef,
     FieldInfoTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
     GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
@@ -595,141 +608,157 @@
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
     GetOrganizationCustomRulePolicyResponseTypeDef,
     GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
-    ResourceDetailsTypeDef,
+    ResourceDetailsOutputTypeDef,
     GetStoredQueryRequestRequestTypeDef,
-    StoredQueryTypeDef,
+    StoredQueryOutputTypeDef,
     ResourceFiltersTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
+    OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    OrganizationCustomPolicyRuleMetadataTypeDef,
     PaginatorConfigTypeDef,
+    TagTypeDef,
+    TemplateSSMDocumentDetailsTypeDef,
     PutConformancePackResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
+    StoredQueryTypeDef,
     PutStoredQueryResponseTypeDef,
+    RecordingStrategyOutputTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
+    ResourceValueOutputTypeDef,
+    StaticValueOutputTypeDef,
     ResourceValueTypeDef,
     StaticValueTypeDef,
+    ResourceDetailsTypeDef,
     TimeWindowTypeDef,
     ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
     SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
     SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+    SourceDetailOutputTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
     StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
     DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
-    BatchGetResourceConfigResponseTypeDef,
     DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
+    BatchGetResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
+    DeliveryChannelOutputTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
     DescribeConfigurationRecorderStatusResponseTypeDef,
     DescribeConformancePackComplianceRequestRequestTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListConformancePackComplianceScoresRequestRequestTypeDef,
     GetConformancePackComplianceSummaryResponseTypeDef,
     OrganizationConformancePackTypeDef,
-    PutOrganizationConformancePackRequestRequestTypeDef,
     ConformancePackDetailTypeDef,
-    PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
+    PutOrganizationConformancePackRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
-    FailedDeleteRemediationExceptionsBatchTypeDef,
     PutRemediationExceptionsRequestRequestTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
+    PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
     PutEvaluationsRequestRequestTypeDef,
-    PutEvaluationsResponseTypeDef,
+    ExecutionControlsOutputTypeDef,
     ExecutionControlsTypeDef,
     PutExternalEvaluationRequestRequestTypeDef,
+    FailedDeleteRemediationExceptionsBatchTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     GetOrganizationConformancePackDetailedStatusResponseTypeDef,
     GetResourceEvaluationSummaryResponseTypeDef,
-    StartResourceEvaluationRequestRequestTypeDef,
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    OrganizationConfigRuleTypeDef,
+    PutOrganizationConfigRuleRequestRequestTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
     PutConfigurationAggregatorRequestRequestTypeDef,
-    PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    OrganizationConfigRuleTypeDef,
-    PutOrganizationConfigRuleRequestRequestTypeDef,
+    PutConformancePackRequestRequestTypeDef,
+    PutStoredQueryRequestRequestTypeDef,
+    RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
+    RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
+    StartResourceEvaluationRequestRequestTypeDef,
     ResourceEvaluationFiltersTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
@@ -740,27 +769,30 @@
     DescribeDeliveryChannelStatusResponseTypeDef,
     DescribeConfigurationAggregatorsResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetResourceConfigHistoryResponseTypeDef,
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
-    DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    DeleteRemediationExceptionsResponseTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
     ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
     ListResourceEvaluationsRequestRequestTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
@@ -774,15 +806,15 @@
     PutRemediationConfigurationsRequestRequestTypeDef,
     DescribeConfigRulesResponseTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceTypeDef:
+def get_structure() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/__init__.py` & `mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/__init__.pyi` & `mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/__main__.py` & `mypy-boto3-config-1.28.12/mypy_boto3_config/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConfigService 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ConfigService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/client.py` & `mypy-boto3-config-1.28.12/mypy_boto3_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/client.pyi` & `mypy-boto3-config-1.28.12/mypy_boto3_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/literals.py` & `mypy-boto3-config-1.28.12/mypy_boto3_config/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,14 +676,15 @@
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
@@ -762,26 +763,28 @@
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

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/literals.pyi` & `mypy-boto3-config-1.28.12/mypy_boto3_config/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -674,14 +674,15 @@
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
@@ -760,26 +761,28 @@
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

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/paginator.py` & `mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/paginator.pyi` & `mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/type_defs.py` & `mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for config service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_config.type_defs import AccountAggregationSourceTypeDef
+    from mypy_boto3_config.type_defs import AccountAggregationSourceOutputTypeDef
 
-    data: AccountAggregationSourceTypeDef = {...}
+    data: AccountAggregationSourceOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,47 +52,54 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
+    "AggregateResourceIdentifierOutputTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
     "AggregationAuthorizationTypeDef",
     "BaseConfigurationItemTypeDef",
     "ResourceKeyTypeDef",
+    "ResourceKeyOutputTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
+    "EvaluationModeConfigurationOutputTypeDef",
+    "ScopeOutputTypeDef",
     "EvaluationModeConfigurationTypeDef",
     "ScopeTypeDef",
+    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
-    "OrganizationAggregationSourceTypeDef",
+    "OrganizationAggregationSourceOutputTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
-    "ConformancePackInputParameterTypeDef",
-    "TemplateSSMDocumentDetailsTypeDef",
+    "ConformancePackInputParameterOutputTypeDef",
+    "TemplateSSMDocumentDetailsOutputTypeDef",
     "ConformancePackEvaluationFiltersTypeDef",
+    "ConformancePackInputParameterTypeDef",
     "ConformancePackRuleComplianceTypeDef",
     "ConformancePackStatusDetailTypeDef",
+    "CustomPolicyDetailsOutputTypeDef",
     "CustomPolicyDetailsTypeDef",
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     "DeleteConfigRuleRequestRequestTypeDef",
     "DeleteConfigurationAggregatorRequestRequestTypeDef",
     "DeleteConfigurationRecorderRequestRequestTypeDef",
     "DeleteConformancePackRequestRequestTypeDef",
     "DeleteDeliveryChannelRequestRequestTypeDef",
@@ -143,21 +150,26 @@
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EvaluationContextOutputTypeDef",
     "EvaluationContextTypeDef",
+    "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
     "EvaluationTypeDef",
+    "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
+    "SsmControlsOutputTypeDef",
     "SsmControlsTypeDef",
     "ExternalEvaluationTypeDef",
+    "RemediationExceptionResourceKeyOutputTypeDef",
     "FieldInfoTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
     "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
@@ -175,141 +187,157 @@
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     "GetOrganizationCustomRulePolicyResponseTypeDef",
     "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
-    "ResourceDetailsTypeDef",
+    "ResourceDetailsOutputTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
-    "StoredQueryTypeDef",
+    "StoredQueryOutputTypeDef",
     "ResourceFiltersTypeDef",
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
+    "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
+    "OrganizationCustomRuleMetadataOutputTypeDef",
+    "OrganizationManagedRuleMetadataOutputTypeDef",
+    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
-    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "PaginatorConfigTypeDef",
+    "TagTypeDef",
+    "TemplateSSMDocumentDetailsTypeDef",
     "PutConformancePackResponseTypeDef",
     "PutOrganizationConfigRuleResponseTypeDef",
     "PutOrganizationConformancePackResponseTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
+    "StoredQueryTypeDef",
     "PutStoredQueryResponseTypeDef",
+    "RecordingStrategyOutputTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
+    "ResourceValueOutputTypeDef",
+    "StaticValueOutputTypeDef",
     "ResourceValueTypeDef",
     "StaticValueTypeDef",
+    "ResourceDetailsTypeDef",
     "TimeWindowTypeDef",
     "ResponseMetadataTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
     "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
     "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    "SourceDetailOutputTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
     "StartResourceEvaluationResponseTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     "DescribeAggregationAuthorizationsResponseTypeDef",
     "PutAggregationAuthorizationResponseTypeDef",
     "BatchGetAggregateResourceConfigResponseTypeDef",
     "BatchGetResourceConfigRequestRequestTypeDef",
-    "BatchGetResourceConfigResponseTypeDef",
     "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     "DescribeRemediationExecutionStatusRequestRequestTypeDef",
     "StartRemediationExecutionRequestRequestTypeDef",
+    "BatchGetResourceConfigResponseTypeDef",
     "StartRemediationExecutionResponseTypeDef",
     "ComplianceSummaryTypeDef",
     "ComplianceTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     "GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
+    "DeliveryChannelOutputTypeDef",
     "DeliveryChannelTypeDef",
     "DeliveryChannelStatusTypeDef",
     "ConfigurationAggregatorTypeDef",
     "ConfigurationItemTypeDef",
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     "DescribeConformancePackComplianceRequestRequestTypeDef",
     "ListConformancePackComplianceScoresResponseTypeDef",
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     "GetConformancePackComplianceSummaryResponseTypeDef",
     "OrganizationConformancePackTypeDef",
-    "PutOrganizationConformancePackRequestRequestTypeDef",
     "ConformancePackDetailTypeDef",
-    "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
+    "PutOrganizationConformancePackRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "PutRemediationExceptionsRequestRequestTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
+    "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
     "PutEvaluationsRequestRequestTypeDef",
-    "PutEvaluationsResponseTypeDef",
+    "ExecutionControlsOutputTypeDef",
     "ExecutionControlsTypeDef",
     "PutExternalEvaluationRequestRequestTypeDef",
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     "GetResourceEvaluationSummaryResponseTypeDef",
-    "StartResourceEvaluationRequestRequestTypeDef",
     "GetStoredQueryResponseTypeDef",
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "OrganizationConfigRuleTypeDef",
+    "PutOrganizationConfigRuleRequestRequestTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
     "PutConfigurationAggregatorRequestRequestTypeDef",
-    "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "OrganizationConfigRuleTypeDef",
-    "PutOrganizationConfigRuleRequestRequestTypeDef",
+    "PutConformancePackRequestRequestTypeDef",
+    "PutStoredQueryRequestRequestTypeDef",
+    "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
+    "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
+    "StartResourceEvaluationRequestRequestTypeDef",
     "ResourceEvaluationFiltersTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
@@ -320,27 +348,30 @@
     "DescribeDeliveryChannelStatusResponseTypeDef",
     "DescribeConfigurationAggregatorsResponseTypeDef",
     "PutConfigurationAggregatorResponseTypeDef",
     "GetAggregateResourceConfigResponseTypeDef",
     "GetResourceConfigHistoryResponseTypeDef",
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
-    "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
+    "DeleteRemediationExceptionsResponseTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
+    "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
+    "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     "ListResourceEvaluationsRequestRequestTypeDef",
+    "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
@@ -353,36 +384,54 @@
     "FailedRemediationBatchTypeDef",
     "PutRemediationConfigurationsRequestRequestTypeDef",
     "DescribeConfigRulesResponseTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
 )
 
+_RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredAccountAggregationSourceOutputTypeDef",
+    {
+        "AccountIds": List[str],
+    },
+)
+_OptionalAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalAccountAggregationSourceOutputTypeDef",
+    {
+        "AllAwsRegions": bool,
+        "AwsRegions": List[str],
+    },
+    total=False,
+)
+
+class AccountAggregationSourceOutputTypeDef(
+    _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
+):
+    pass
+
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
-        "AccountIds": List[str],
+        "AccountIds": Sequence[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
     "_OptionalAccountAggregationSourceTypeDef",
     {
         "AllAwsRegions": bool,
-        "AwsRegions": List[str],
+        "AwsRegions": Sequence[str],
     },
     total=False,
 )
 
-
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
 ):
     pass
 
-
 AggregateConformancePackComplianceTypeDef = TypedDict(
     "AggregateConformancePackComplianceTypeDef",
     {
         "ComplianceType": ConformancePackComplianceTypeType,
         "CompliantRuleCount": int,
         "NonCompliantRuleCount": int,
         "TotalRuleCount": int,
@@ -415,14 +464,37 @@
     {
         "AccountId": str,
         "AwsRegion": str,
     },
     total=False,
 )
 
+_RequiredAggregateResourceIdentifierOutputTypeDef = TypedDict(
+    "_RequiredAggregateResourceIdentifierOutputTypeDef",
+    {
+        "SourceAccountId": str,
+        "SourceRegion": str,
+        "ResourceId": str,
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalAggregateResourceIdentifierOutputTypeDef = TypedDict(
+    "_OptionalAggregateResourceIdentifierOutputTypeDef",
+    {
+        "ResourceName": str,
+    },
+    total=False,
+)
+
+class AggregateResourceIdentifierOutputTypeDef(
+    _RequiredAggregateResourceIdentifierOutputTypeDef,
+    _OptionalAggregateResourceIdentifierOutputTypeDef,
+):
+    pass
+
 _RequiredAggregateResourceIdentifierTypeDef = TypedDict(
     "_RequiredAggregateResourceIdentifierTypeDef",
     {
         "SourceAccountId": str,
         "SourceRegion": str,
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
@@ -432,21 +504,19 @@
     "_OptionalAggregateResourceIdentifierTypeDef",
     {
         "ResourceName": str,
     },
     total=False,
 )
 
-
 class AggregateResourceIdentifierTypeDef(
     _RequiredAggregateResourceIdentifierTypeDef, _OptionalAggregateResourceIdentifierTypeDef
 ):
     pass
 
-
 AggregatedSourceStatusTypeDef = TypedDict(
     "AggregatedSourceStatusTypeDef",
     {
         "SourceId": str,
         "SourceType": AggregatedSourceTypeType,
         "AwsRegion": str,
         "LastUpdateStatus": AggregatedSourceStatusTypeType,
@@ -493,14 +563,22 @@
     "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
 
+ResourceKeyOutputTypeDef = TypedDict(
+    "ResourceKeyOutputTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+
 ComplianceContributorCountTypeDef = TypedDict(
     "ComplianceContributorCountTypeDef",
     {
         "CappedCount": int,
         "CapExceeded": bool,
     },
     total=False,
@@ -557,33 +635,60 @@
         "LastDebugLogDeliveryStatus": str,
         "LastDebugLogDeliveryStatusReason": str,
         "LastDebugLogDeliveryTime": datetime,
     },
     total=False,
 )
 
+EvaluationModeConfigurationOutputTypeDef = TypedDict(
+    "EvaluationModeConfigurationOutputTypeDef",
+    {
+        "Mode": EvaluationModeType,
+    },
+    total=False,
+)
+
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "ComplianceResourceTypes": List[str],
+        "TagKey": str,
+        "TagValue": str,
+        "ComplianceResourceId": str,
+    },
+    total=False,
+)
+
 EvaluationModeConfigurationTypeDef = TypedDict(
     "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
-        "ComplianceResourceTypes": List[str],
+        "ComplianceResourceTypes": Sequence[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
+ConfigSnapshotDeliveryPropertiesOutputTypeDef = TypedDict(
+    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
+    {
+        "deliveryFrequency": MaximumExecutionFrequencyType,
+    },
+    total=False,
+)
+
 ConfigSnapshotDeliveryPropertiesTypeDef = TypedDict(
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     {
         "deliveryFrequency": MaximumExecutionFrequencyType,
     },
     total=False,
 )
@@ -595,36 +700,35 @@
         "lastErrorCode": str,
         "lastErrorMessage": str,
         "lastStatusChangeTime": datetime,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceTypeDef",
+_RequiredOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceOutputTypeDef",
     {
         "RoleArn": str,
     },
 )
-_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceTypeDef",
+_OptionalOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceOutputTypeDef",
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
-
-class OrganizationAggregationSourceTypeDef(
-    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+class OrganizationAggregationSourceOutputTypeDef(
+    _RequiredOrganizationAggregationSourceOutputTypeDef,
+    _OptionalOrganizationAggregationSourceOutputTypeDef,
 ):
     pass
 
-
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "relationshipName": str,
@@ -677,54 +781,61 @@
     "ConformancePackComplianceSummaryTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackComplianceStatus": ConformancePackComplianceTypeType,
     },
 )
 
-ConformancePackInputParameterTypeDef = TypedDict(
-    "ConformancePackInputParameterTypeDef",
+ConformancePackInputParameterOutputTypeDef = TypedDict(
+    "ConformancePackInputParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
 )
 
-_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_RequiredTemplateSSMDocumentDetailsTypeDef",
+_RequiredTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
+    "_RequiredTemplateSSMDocumentDetailsOutputTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_OptionalTemplateSSMDocumentDetailsTypeDef",
+_OptionalTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
+    "_OptionalTemplateSSMDocumentDetailsOutputTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-
-class TemplateSSMDocumentDetailsTypeDef(
-    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
+class TemplateSSMDocumentDetailsOutputTypeDef(
+    _RequiredTemplateSSMDocumentDetailsOutputTypeDef,
+    _OptionalTemplateSSMDocumentDetailsOutputTypeDef,
 ):
     pass
 
-
 ConformancePackEvaluationFiltersTypeDef = TypedDict(
     "ConformancePackEvaluationFiltersTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceType": ConformancePackComplianceTypeType,
         "ResourceType": str,
         "ResourceIds": Sequence[str],
     },
     total=False,
 )
 
+ConformancePackInputParameterTypeDef = TypedDict(
+    "ConformancePackInputParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+    },
+)
+
 ConformancePackRuleComplianceTypeDef = TypedDict(
     "ConformancePackRuleComplianceTypeDef",
     {
         "ConfigRuleName": str,
         "ComplianceType": ConformancePackComplianceTypeType,
         "Controls": List[str],
     },
@@ -747,20 +858,38 @@
     {
         "ConformancePackStatusReason": str,
         "LastUpdateCompletedTime": datetime,
     },
     total=False,
 )
 
-
 class ConformancePackStatusDetailTypeDef(
     _RequiredConformancePackStatusDetailTypeDef, _OptionalConformancePackStatusDetailTypeDef
 ):
     pass
 
+_RequiredCustomPolicyDetailsOutputTypeDef = TypedDict(
+    "_RequiredCustomPolicyDetailsOutputTypeDef",
+    {
+        "PolicyRuntime": str,
+        "PolicyText": str,
+    },
+)
+_OptionalCustomPolicyDetailsOutputTypeDef = TypedDict(
+    "_OptionalCustomPolicyDetailsOutputTypeDef",
+    {
+        "EnableDebugLogDelivery": bool,
+    },
+    total=False,
+)
+
+class CustomPolicyDetailsOutputTypeDef(
+    _RequiredCustomPolicyDetailsOutputTypeDef, _OptionalCustomPolicyDetailsOutputTypeDef
+):
+    pass
 
 _RequiredCustomPolicyDetailsTypeDef = TypedDict(
     "_RequiredCustomPolicyDetailsTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
@@ -769,21 +898,19 @@
     "_OptionalCustomPolicyDetailsTypeDef",
     {
         "EnableDebugLogDelivery": bool,
     },
     total=False,
 )
 
-
 class CustomPolicyDetailsTypeDef(
     _RequiredCustomPolicyDetailsTypeDef, _OptionalCustomPolicyDetailsTypeDef
 ):
     pass
 
-
 DeleteAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
         "AuthorizedAwsRegion": str,
     },
 )
@@ -862,22 +989,20 @@
     "_OptionalDeleteRemediationConfigurationRequestRequestTypeDef",
     {
         "ResourceType": str,
     },
     total=False,
 )
 
-
 class DeleteRemediationConfigurationRequestRequestTypeDef(
     _RequiredDeleteRemediationConfigurationRequestRequestTypeDef,
     _OptionalDeleteRemediationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 RemediationExceptionResourceKeyTypeDef = TypedDict(
     "RemediationExceptionResourceKeyTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
     },
     total=False,
@@ -1020,22 +1145,20 @@
     {
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
@@ -1044,22 +1167,20 @@
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1177,21 +1298,19 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
-
 DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1239,22 +1358,20 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
-
 DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1316,21 +1433,19 @@
     {
         "Message": str,
         "ExpirationTime": datetime,
     },
     total=False,
 )
 
-
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
-
 DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1356,22 +1471,50 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EvaluationContextOutputTypeDef = TypedDict(
+    "EvaluationContextOutputTypeDef",
+    {
+        "EvaluationContextIdentifier": str,
+    },
+    total=False,
+)
+
 EvaluationContextTypeDef = TypedDict(
     "EvaluationContextTypeDef",
     {
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
 
+_RequiredEvaluationOutputTypeDef = TypedDict(
+    "_RequiredEvaluationOutputTypeDef",
+    {
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": datetime,
+    },
+)
+_OptionalEvaluationOutputTypeDef = TypedDict(
+    "_OptionalEvaluationOutputTypeDef",
+    {
+        "Annotation": str,
+    },
+    total=False,
+)
+
+class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
+    pass
+
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1389,19 +1532,17 @@
     "_OptionalEvaluationStatusTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
-
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
-
 _RequiredEvaluationTypeDef = TypedDict(
     "_RequiredEvaluationTypeDef",
     {
         "ComplianceResourceType": str,
         "ComplianceResourceId": str,
         "ComplianceType": ComplianceTypeType,
         "OrderingTimestamp": Union[datetime, str],
@@ -1411,23 +1552,38 @@
     "_OptionalEvaluationTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
-
 class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
     pass
 
+ExclusionByResourceTypesOutputTypeDef = TypedDict(
+    "ExclusionByResourceTypesOutputTypeDef",
+    {
+        "resourceTypes": List[ResourceTypeType],
+    },
+    total=False,
+)
 
 ExclusionByResourceTypesTypeDef = TypedDict(
     "ExclusionByResourceTypesTypeDef",
     {
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
+    },
+    total=False,
+)
+
+SsmControlsOutputTypeDef = TypedDict(
+    "SsmControlsOutputTypeDef",
+    {
+        "ConcurrentExecutionRatePercentage": int,
+        "ErrorPercentage": int,
     },
     total=False,
 )
 
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
@@ -1450,20 +1606,27 @@
     "_OptionalExternalEvaluationTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
-
 class ExternalEvaluationTypeDef(
     _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
+RemediationExceptionResourceKeyOutputTypeDef = TypedDict(
+    "RemediationExceptionResourceKeyOutputTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+    },
+    total=False,
+)
 
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
@@ -1483,22 +1646,20 @@
     {
         "ComplianceType": ComplianceTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigRuleName": str,
         "AccountId": str,
         "AwsRegion": str,
@@ -1510,22 +1671,20 @@
         "ComplianceType": ComplianceTypeType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceCountFiltersTypeDef = TypedDict(
     "ResourceCountFiltersTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "AccountId": str,
         "Region": str,
     },
@@ -1551,22 +1710,20 @@
     {
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
@@ -1575,22 +1732,20 @@
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-
 GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "ResourceEvaluationId": str,
@@ -1629,22 +1784,20 @@
     "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
     },
 )
 _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -1652,22 +1805,20 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
-
 GetCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
@@ -1722,21 +1873,19 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class MemberAccountStatusTypeDef(
     _RequiredMemberAccountStatusTypeDef, _OptionalMemberAccountStatusTypeDef
 ):
     pass
 
-
 OrganizationResourceDetailedStatusFiltersTypeDef = TypedDict(
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     {
         "AccountId": str,
         "Status": OrganizationResourceDetailedStatusType,
     },
     total=False,
@@ -1756,22 +1905,20 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class OrganizationConformancePackDetailedStatusTypeDef(
     _RequiredOrganizationConformancePackDetailedStatusTypeDef,
     _OptionalOrganizationConformancePackDetailedStatusTypeDef,
 ):
     pass
 
-
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
@@ -1797,22 +1944,20 @@
         "earlierTime": Union[datetime, str],
         "chronologicalOrder": ChronologicalOrderType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
     _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
@@ -1824,79 +1969,77 @@
         "chronologicalOrder": ChronologicalOrderType,
         "limit": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class GetResourceConfigHistoryRequestRequestTypeDef(
     _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
     _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
-_RequiredResourceDetailsTypeDef = TypedDict(
-    "_RequiredResourceDetailsTypeDef",
+_RequiredResourceDetailsOutputTypeDef = TypedDict(
+    "_RequiredResourceDetailsOutputTypeDef",
     {
         "ResourceId": str,
         "ResourceType": str,
         "ResourceConfiguration": str,
     },
 )
-_OptionalResourceDetailsTypeDef = TypedDict(
-    "_OptionalResourceDetailsTypeDef",
+_OptionalResourceDetailsOutputTypeDef = TypedDict(
+    "_OptionalResourceDetailsOutputTypeDef",
     {
         "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
     },
     total=False,
 )
 
-
-class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
+class ResourceDetailsOutputTypeDef(
+    _RequiredResourceDetailsOutputTypeDef, _OptionalResourceDetailsOutputTypeDef
+):
     pass
 
-
 GetStoredQueryRequestRequestTypeDef = TypedDict(
     "GetStoredQueryRequestRequestTypeDef",
     {
         "QueryName": str,
     },
 )
 
-_RequiredStoredQueryTypeDef = TypedDict(
-    "_RequiredStoredQueryTypeDef",
+_RequiredStoredQueryOutputTypeDef = TypedDict(
+    "_RequiredStoredQueryOutputTypeDef",
     {
         "QueryName": str,
     },
 )
-_OptionalStoredQueryTypeDef = TypedDict(
-    "_OptionalStoredQueryTypeDef",
+_OptionalStoredQueryOutputTypeDef = TypedDict(
+    "_OptionalStoredQueryOutputTypeDef",
     {
         "QueryId": str,
         "QueryArn": str,
         "Description": str,
         "Expression": str,
     },
     total=False,
 )
 
-
-class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
+class StoredQueryOutputTypeDef(
+    _RequiredStoredQueryOutputTypeDef, _OptionalStoredQueryOutputTypeDef
+):
     pass
 
-
 ResourceFiltersTypeDef = TypedDict(
     "ResourceFiltersTypeDef",
     {
         "AccountId": str,
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
@@ -1917,22 +2060,20 @@
         "resourceName": str,
         "includeDeletedResources": bool,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
     _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
@@ -1943,22 +2084,20 @@
         "limit": int,
         "includeDeletedResources": bool,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "resourceDeletionTime": datetime,
@@ -1997,43 +2136,39 @@
     "_OptionalStoredQueryMetadataTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -2041,31 +2176,49 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceTypeDef",
+    {
+        "RoleArn": str,
+    },
+)
+_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceTypeDef",
+    {
+        "AwsRegions": Sequence[str],
+        "AllAwsRegions": bool,
+    },
+    total=False,
+)
+
+class OrganizationAggregationSourceTypeDef(
+    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+):
+    pass
+
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -2075,69 +2228,67 @@
         "TagValueScope": str,
         "PolicyRuntime": str,
         "DebugLogDeliveryAccounts": List[str],
     },
     total=False,
 )
 
-_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataTypeDef",
+_RequiredOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeType],
     },
 )
-_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataTypeDef",
+_OptionalOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-
-class OrganizationCustomRuleMetadataTypeDef(
-    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+class OrganizationCustomRuleMetadataOutputTypeDef(
+    _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
+    _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
 ):
     pass
 
-
-_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataTypeDef",
+_RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
-_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataTypeDef",
+_OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-
-class OrganizationManagedRuleMetadataTypeDef(
-    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+class OrganizationManagedRuleMetadataOutputTypeDef(
+    _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
+    _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
 ):
     pass
 
-
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -2153,32 +2304,109 @@
         "TagKeyScope": str,
         "TagValueScope": str,
         "DebugLogDeliveryAccounts": Sequence[str],
     },
     total=False,
 )
 
-
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
+_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataTypeDef",
+    {
+        "LambdaFunctionArn": str,
+        "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
+    },
+)
+_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataTypeDef",
+    {
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
+    },
+    total=False,
+)
+
+class OrganizationCustomRuleMetadataTypeDef(
+    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+):
+    pass
+
+_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataTypeDef",
+    {
+        "RuleIdentifier": str,
+    },
+)
+_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataTypeDef",
+    {
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
+    },
+    total=False,
+)
+
+class OrganizationManagedRuleMetadataTypeDef(
+    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+):
+    pass
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_RequiredTemplateSSMDocumentDetailsTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_OptionalTemplateSSMDocumentDetailsTypeDef",
+    {
+        "DocumentVersion": str,
+    },
+    total=False,
+)
+
+class TemplateSSMDocumentDetailsTypeDef(
+    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
+):
+    pass
+
 PutConformancePackResponseTypeDef = TypedDict(
     "PutConformancePackResponseTypeDef",
     {
         "ConformancePackArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2213,36 +2441,62 @@
     {
         "ResourceName": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class PutResourceConfigRequestRequestTypeDef(
     _RequiredPutResourceConfigRequestRequestTypeDef, _OptionalPutResourceConfigRequestRequestTypeDef
 ):
     pass
 
-
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
+_RequiredStoredQueryTypeDef = TypedDict(
+    "_RequiredStoredQueryTypeDef",
+    {
+        "QueryName": str,
+    },
+)
+_OptionalStoredQueryTypeDef = TypedDict(
+    "_OptionalStoredQueryTypeDef",
+    {
+        "QueryId": str,
+        "QueryArn": str,
+        "Description": str,
+        "Expression": str,
+    },
+    total=False,
+)
+
+class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
+    pass
+
 PutStoredQueryResponseTypeDef = TypedDict(
     "PutStoredQueryResponseTypeDef",
     {
         "QueryArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RecordingStrategyOutputTypeDef = TypedDict(
+    "RecordingStrategyOutputTypeDef",
+    {
+        "useOnly": RecordingStrategyTypeType,
+    },
+    total=False,
+)
+
 RecordingStrategyTypeDef = TypedDict(
     "RecordingStrategyTypeDef",
     {
         "useOnly": RecordingStrategyTypeType,
     },
     total=False,
 )
@@ -2255,28 +2509,61 @@
         "ErrorMessage": str,
         "StartTime": datetime,
         "StopTime": datetime,
     },
     total=False,
 )
 
+ResourceValueOutputTypeDef = TypedDict(
+    "ResourceValueOutputTypeDef",
+    {
+        "Value": Literal["RESOURCE_ID"],
+    },
+)
+
+StaticValueOutputTypeDef = TypedDict(
+    "StaticValueOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
+
 ResourceValueTypeDef = TypedDict(
     "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
-        "Values": List[str],
+        "Values": Sequence[str],
+    },
+)
+
+_RequiredResourceDetailsTypeDef = TypedDict(
+    "_RequiredResourceDetailsTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ResourceConfiguration": str,
+    },
+)
+_OptionalResourceDetailsTypeDef = TypedDict(
+    "_OptionalResourceDetailsTypeDef",
+    {
+        "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
     },
+    total=False,
 )
 
+class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
+    pass
+
 TimeWindowTypeDef = TypedDict(
     "TimeWindowTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
@@ -2306,22 +2593,20 @@
         "Limit": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
     TypedDict(
         "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
         {
             "Expression": str,
             "ConfigurationAggregatorName": str,
         },
@@ -2334,22 +2619,20 @@
             "MaxResults": int,
             "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
-
 class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
     _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2357,43 +2640,49 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
     _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
 ):
     pass
 
+SourceDetailOutputTypeDef = TypedDict(
+    "SourceDetailOutputTypeDef",
+    {
+        "EventSource": Literal["aws.config"],
+        "MessageType": MessageTypeType,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+    },
+    total=False,
+)
 
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -2470,22 +2759,20 @@
     {
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
@@ -2494,22 +2781,20 @@
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2519,21 +2804,28 @@
         "GroupByKey": AggregateConformancePackComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
+ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
+    {
+        "ResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 BatchGetAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifiers": Sequence[AggregateResourceIdentifierTypeDef],
     },
@@ -2543,23 +2835,14 @@
     "GetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifier": AggregateResourceIdentifierTypeDef,
     },
 )
 
-ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
-    {
-        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeConfigurationAggregatorSourcesStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     {
         "AggregatedSourceStatusList": List[AggregatedSourceStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2582,35 +2865,26 @@
     },
 )
 
 BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigResponseTypeDef",
     {
         "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetResourceConfigRequestRequestTypeDef",
     {
         "resourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
 
-BatchGetResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetResourceConfigResponseTypeDef",
-    {
-        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
@@ -2618,22 +2892,20 @@
     {
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
@@ -2642,35 +2914,42 @@
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeRemediationExecutionStatusRequestRequestTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestRequestTypeDef,
 ):
     pass
 
-
 StartRemediationExecutionRequestRequestTypeDef = TypedDict(
     "StartRemediationExecutionRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
 
+BatchGetResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetResourceConfigResponseTypeDef",
+    {
+        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "unprocessedResourceKeys": List[ResourceKeyOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartRemediationExecutionResponseTypeDef = TypedDict(
     "StartRemediationExecutionResponseTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[ResourceKeyTypeDef],
+        "FailedItems": List[ResourceKeyOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComplianceSummaryTypeDef = TypedDict(
     "ComplianceSummaryTypeDef",
     {
@@ -2701,22 +2980,20 @@
     {
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
@@ -2725,22 +3002,20 @@
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2750,31 +3025,42 @@
         "GroupByKey": ConfigRuleComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeliveryChannelOutputTypeDef = TypedDict(
+    "DeliveryChannelOutputTypeDef",
+    {
+        "name": str,
+        "s3BucketName": str,
+        "s3KeyPrefix": str,
+        "s3KmsKeyArn": str,
+        "snsTopicARN": str,
+        "configSnapshotDeliveryProperties": ConfigSnapshotDeliveryPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 DeliveryChannelTypeDef = TypedDict(
     "DeliveryChannelTypeDef",
     {
         "name": str,
         "s3BucketName": str,
         "s3KeyPrefix": str,
         "s3KmsKeyArn": str,
@@ -2796,16 +3082,16 @@
 )
 
 ConfigurationAggregatorTypeDef = TypedDict(
     "ConfigurationAggregatorTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigurationAggregatorArn": str,
-        "AccountAggregationSources": List[AccountAggregationSourceTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "AccountAggregationSources": List[AccountAggregationSourceOutputTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
@@ -2854,22 +3140,20 @@
         "Filters": ConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeConformancePackComplianceRequestRequestTypeDef(
     _RequiredDescribeConformancePackComplianceRequestRequestTypeDef,
     _OptionalDescribeConformancePackComplianceRequestRequestTypeDef,
 ):
     pass
 
-
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2905,109 +3189,51 @@
     },
 )
 _OptionalOrganizationConformancePackTypeDef = TypedDict(
     "_OptionalOrganizationConformancePackTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
         "ExcludedAccounts": List[str],
     },
     total=False,
 )
 
-
 class OrganizationConformancePackTypeDef(
     _RequiredOrganizationConformancePackTypeDef, _OptionalOrganizationConformancePackTypeDef
 ):
     pass
 
-
-_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
-    {
-        "OrganizationConformancePackName": str,
-    },
-)
-_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
-    {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "ExcludedAccounts": Sequence[str],
-    },
-    total=False,
-)
-
-
-class PutOrganizationConformancePackRequestRequestTypeDef(
-    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
-    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredConformancePackDetailTypeDef = TypedDict(
     "_RequiredConformancePackDetailTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackArn": str,
         "ConformancePackId": str,
     },
 )
 _OptionalConformancePackDetailTypeDef = TypedDict(
     "_OptionalConformancePackDetailTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
         "LastUpdateRequestedTime": datetime,
         "CreatedBy": str,
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsOutputTypeDef,
     },
     total=False,
 )
 
-
 class ConformancePackDetailTypeDef(
     _RequiredConformancePackDetailTypeDef, _OptionalConformancePackDetailTypeDef
 ):
     pass
 
-
-_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConformancePackRequestRequestTypeDef",
-    {
-        "ConformancePackName": str,
-    },
-)
-_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConformancePackRequestRequestTypeDef",
-    {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
-    },
-    total=False,
-)
-
-
-class PutConformancePackRequestRequestTypeDef(
-    _RequiredPutConformancePackRequestRequestTypeDef,
-    _OptionalPutConformancePackRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
 _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
@@ -3016,21 +3242,44 @@
         "Filters": ConformancePackEvaluationFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConformancePackComplianceDetailsRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "OrganizationConformancePackName": str,
+    },
+)
+_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "ExcludedAccounts": Sequence[str],
+    },
+    total=False,
+)
+
+class PutOrganizationConformancePackRequestRequestTypeDef(
+    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
+    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
+):
+    pass
 
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
@@ -3067,31 +3316,20 @@
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeRemediationExceptionsRequestRequestTypeDef(
     _RequiredDescribeRemediationExceptionsRequestRequestTypeDef,
     _OptionalDescribeRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
-
-FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
-    {
-        "FailureMessage": str,
-        "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
-    },
-    total=False,
-)
-
 _RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
 )
@@ -3100,22 +3338,20 @@
     {
         "Message": str,
         "ExpirationTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class PutRemediationExceptionsRequestRequestTypeDef(
     _RequiredPutRemediationExceptionsRequestRequestTypeDef,
     _OptionalPutRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -3190,14 +3426,22 @@
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutEvaluationsResponseTypeDef = TypedDict(
+    "PutEvaluationsResponseTypeDef",
+    {
+        "FailedEvaluations": List[EvaluationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
@@ -3215,27 +3459,25 @@
     {
         "Evaluations": Sequence[EvaluationTypeDef],
         "TestMode": bool,
     },
     total=False,
 )
 
-
 class PutEvaluationsRequestRequestTypeDef(
     _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
 ):
     pass
 
-
-PutEvaluationsResponseTypeDef = TypedDict(
-    "PutEvaluationsResponseTypeDef",
+ExecutionControlsOutputTypeDef = TypedDict(
+    "ExecutionControlsOutputTypeDef",
     {
-        "FailedEvaluations": List[EvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SsmControls": SsmControlsOutputTypeDef,
     },
+    total=False,
 )
 
 ExecutionControlsTypeDef = TypedDict(
     "ExecutionControlsTypeDef",
     {
         "SsmControls": SsmControlsTypeDef,
     },
@@ -3246,14 +3488,23 @@
     "PutExternalEvaluationRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ExternalEvaluation": ExternalEvaluationTypeDef,
     },
 )
 
+FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
+    {
+        "FailureMessage": str,
+        "FailedItems": List[RemediationExceptionResourceKeyOutputTypeDef],
+    },
+    total=False,
+)
+
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
     total=False,
 )
@@ -3271,22 +3522,20 @@
         "GroupByKey": ResourceCountGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAggregateDiscoveredResourceCountsRequestRequestTypeDef(
     _RequiredGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     _OptionalGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
 ):
     pass
 
-
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
@@ -3315,22 +3564,20 @@
     {
         "Filters": StatusDetailFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3339,22 +3586,20 @@
         "Filters": StatusDetailFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
-
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3371,22 +3616,20 @@
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3395,22 +3638,20 @@
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
-
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
@@ -3422,49 +3663,24 @@
     "GetResourceEvaluationSummaryResponseTypeDef",
     {
         "ResourceEvaluationId": str,
         "EvaluationMode": EvaluationModeType,
         "EvaluationStatus": EvaluationStatusTypeDef,
         "EvaluationStartTimestamp": datetime,
         "Compliance": ComplianceTypeType,
-        "EvaluationContext": EvaluationContextTypeDef,
-        "ResourceDetails": ResourceDetailsTypeDef,
+        "EvaluationContext": EvaluationContextOutputTypeDef,
+        "ResourceDetails": ResourceDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "ResourceDetails": ResourceDetailsTypeDef,
-        "EvaluationMode": EvaluationModeType,
-    },
-)
-_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "EvaluationContext": EvaluationContextTypeDef,
-        "EvaluationTimeout": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class StartResourceEvaluationRequestRequestTypeDef(
-    _RequiredStartResourceEvaluationRequestRequestTypeDef,
-    _OptionalStartResourceEvaluationRequestRequestTypeDef,
-):
-    pass
-
-
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
-        "StoredQuery": StoredQueryTypeDef,
+        "StoredQuery": StoredQueryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
@@ -3477,22 +3693,20 @@
     {
         "Filters": ResourceFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
@@ -3502,22 +3716,20 @@
         "Filters": ResourceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAggregateDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3540,20 +3752,67 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredOrganizationConfigRuleTypeDef = TypedDict(
+    "_RequiredOrganizationConfigRuleTypeDef",
+    {
+        "OrganizationConfigRuleName": str,
+        "OrganizationConfigRuleArn": str,
+    },
+)
+_OptionalOrganizationConfigRuleTypeDef = TypedDict(
+    "_OptionalOrganizationConfigRuleTypeDef",
+    {
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
+        "ExcludedAccounts": List[str],
+        "LastUpdateTime": datetime,
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    },
+    total=False,
+)
+
+class OrganizationConfigRuleTypeDef(
+    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
+):
+    pass
+
+_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
+    {
+        "OrganizationConfigRuleName": str,
+    },
+)
+_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
+    {
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
+        "ExcludedAccounts": Sequence[str],
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
+    },
+    total=False,
+)
+
+class PutOrganizationConfigRuleRequestRequestTypeDef(
+    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
+    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
+):
+    pass
+
 _RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
         "AuthorizedAwsRegion": str,
     },
 )
@@ -3561,22 +3820,20 @@
     "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
@@ -3585,166 +3842,197 @@
         "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
         "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutConfigurationAggregatorRequestRequestTypeDef(
     _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
     _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredPutStoredQueryRequestRequestTypeDef",
-    {
-        "StoredQuery": StoredQueryTypeDef,
-    },
-)
-_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalPutStoredQueryRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutStoredQueryRequestRequestTypeDef(
-    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
-):
-    pass
-
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredOrganizationConfigRuleTypeDef = TypedDict(
-    "_RequiredOrganizationConfigRuleTypeDef",
+_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConformancePackRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
-        "OrganizationConfigRuleArn": str,
+        "ConformancePackName": str,
     },
 )
-_OptionalOrganizationConfigRuleTypeDef = TypedDict(
-    "_OptionalOrganizationConfigRuleTypeDef",
+_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConformancePackRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
-        "ExcludedAccounts": List[str],
-        "LastUpdateTime": datetime,
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
-
-class OrganizationConfigRuleTypeDef(
-    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
+class PutConformancePackRequestRequestTypeDef(
+    _RequiredPutConformancePackRequestRequestTypeDef,
+    _OptionalPutConformancePackRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
+_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
+        "StoredQuery": StoredQueryTypeDef,
     },
 )
-_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
+_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
-        "ExcludedAccounts": Sequence[str],
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
-class PutOrganizationConfigRuleRequestRequestTypeDef(
-    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
-    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
+class PutStoredQueryRequestRequestTypeDef(
+    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
 ):
     pass
 
+RecordingGroupOutputTypeDef = TypedDict(
+    "RecordingGroupOutputTypeDef",
+    {
+        "allSupported": bool,
+        "includeGlobalResourceTypes": bool,
+        "resourceTypes": List[ResourceTypeType],
+        "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
+        "recordingStrategy": RecordingStrategyOutputTypeDef,
+    },
+    total=False,
+)
 
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesTypeDef,
         "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
     "RemediationExecutionStatusTypeDef",
     {
-        "ResourceKey": ResourceKeyTypeDef,
+        "ResourceKey": ResourceKeyOutputTypeDef,
         "State": RemediationExecutionStateType,
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
+RemediationParameterValueOutputTypeDef = TypedDict(
+    "RemediationParameterValueOutputTypeDef",
+    {
+        "ResourceValue": ResourceValueOutputTypeDef,
+        "StaticValue": StaticValueOutputTypeDef,
+    },
+    total=False,
+)
+
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
+_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "ResourceDetails": ResourceDetailsTypeDef,
+        "EvaluationMode": EvaluationModeType,
+    },
+)
+_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "EvaluationContext": EvaluationContextTypeDef,
+        "EvaluationTimeout": int,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class StartResourceEvaluationRequestRequestTypeDef(
+    _RequiredStartResourceEvaluationRequestRequestTypeDef,
+    _OptionalStartResourceEvaluationRequestRequestTypeDef,
+):
+    pass
+
 ResourceEvaluationFiltersTypeDef = TypedDict(
     "ResourceEvaluationFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
         "TimeWindow": TimeWindowTypeDef,
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
 
+_RequiredSourceOutputTypeDef = TypedDict(
+    "_RequiredSourceOutputTypeDef",
+    {
+        "Owner": OwnerType,
+    },
+)
+_OptionalSourceOutputTypeDef = TypedDict(
+    "_OptionalSourceOutputTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceDetails": List[SourceDetailOutputTypeDef],
+        "CustomPolicyDetails": CustomPolicyDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
+    pass
+
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailTypeDef],
+        "SourceDetails": Sequence[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
-
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
-
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3817,15 +4105,15 @@
     },
     total=False,
 )
 
 DescribeDeliveryChannelsResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelsResponseTypeDef",
     {
-        "DeliveryChannels": List[DeliveryChannelTypeDef],
+        "DeliveryChannels": List[DeliveryChannelOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDeliveryChannelRequestRequestTypeDef = TypedDict(
     "PutDeliveryChannelRequestRequestTypeDef",
     {
@@ -3889,22 +4177,14 @@
     {
         "ConformancePackDetails": List[ConformancePackDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRemediationExceptionsResponseTypeDef = TypedDict(
-    "DeleteRemediationExceptionsResponseTypeDef",
-    {
-        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutRemediationExceptionsResponseTypeDef = TypedDict(
     "PutRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationExceptionBatchTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3936,34 +4216,40 @@
     "_OptionalConformancePackEvaluationResultTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
-
 class ConformancePackEvaluationResultTypeDef(
     _RequiredConformancePackEvaluationResultTypeDef, _OptionalConformancePackEvaluationResultTypeDef
 ):
     pass
 
-
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
         "ComplianceType": ComplianceTypeType,
         "ResultRecordedTime": datetime,
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
+DeleteRemediationExceptionsResponseTypeDef = TypedDict(
+    "DeleteRemediationExceptionsResponseTypeDef",
+    {
+        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -3985,14 +4271,24 @@
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConfigurationRecorderOutputTypeDef = TypedDict(
+    "ConfigurationRecorderOutputTypeDef",
+    {
+        "name": str,
+        "roleARN": str,
+        "recordingGroup": RecordingGroupOutputTypeDef,
+    },
+    total=False,
+)
+
 ConfigurationRecorderTypeDef = TypedDict(
     "ConfigurationRecorderTypeDef",
     {
         "name": str,
         "roleARN": str,
         "recordingGroup": RecordingGroupTypeDef,
     },
@@ -4004,45 +4300,72 @@
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRemediationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredRemediationConfigurationOutputTypeDef",
+    {
+        "ConfigRuleName": str,
+        "TargetType": Literal["SSM_DOCUMENT"],
+        "TargetId": str,
+    },
+)
+_OptionalRemediationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalRemediationConfigurationOutputTypeDef",
+    {
+        "TargetVersion": str,
+        "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
+        "ResourceType": str,
+        "Automatic": bool,
+        "ExecutionControls": ExecutionControlsOutputTypeDef,
+        "MaximumAutomaticAttempts": int,
+        "RetryAttemptSeconds": int,
+        "Arn": str,
+        "CreatedByService": str,
+    },
+    total=False,
+)
+
+class RemediationConfigurationOutputTypeDef(
+    _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
 )
 _OptionalRemediationConfigurationTypeDef = TypedDict(
     "_OptionalRemediationConfigurationTypeDef",
     {
         "TargetVersion": str,
-        "Parameters": Dict[str, RemediationParameterValueTypeDef],
+        "Parameters": Mapping[str, RemediationParameterValueTypeDef],
         "ResourceType": str,
         "Automatic": bool,
         "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
 
-
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
-
 ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     {
         "Filters": ResourceEvaluationFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -4054,14 +4377,40 @@
         "Filters": ResourceEvaluationFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredConfigRuleOutputTypeDef = TypedDict(
+    "_RequiredConfigRuleOutputTypeDef",
+    {
+        "Source": SourceOutputTypeDef,
+    },
+)
+_OptionalConfigRuleOutputTypeDef = TypedDict(
+    "_OptionalConfigRuleOutputTypeDef",
+    {
+        "ConfigRuleName": str,
+        "ConfigRuleArn": str,
+        "ConfigRuleId": str,
+        "Description": str,
+        "Scope": ScopeOutputTypeDef,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ConfigRuleState": ConfigRuleStateType,
+        "CreatedBy": str,
+        "EvaluationModes": List[EvaluationModeConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
+    pass
+
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -4072,24 +4421,22 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
+        "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
 
-
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4167,54 +4514,54 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
-        "ConfigurationRecorders": List[ConfigurationRecorderTypeDef],
+        "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
-        "RemediationConfigurations": List[RemediationConfigurationTypeDef],
+        "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[RemediationConfigurationTypeDef],
+        "FailedItems": List[RemediationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
     "PutRemediationConfigurationsRequestRequestTypeDef",
     {
         "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
     },
 )
 
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
-        "ConfigRules": List[ConfigRuleTypeDef],
+        "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
@@ -4226,21 +4573,19 @@
     "_OptionalPutConfigRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutConfigRuleRequestRequestTypeDef(
     _RequiredPutConfigRuleRequestRequestTypeDef, _OptionalPutConfigRuleRequestRequestTypeDef
 ):
     pass
 
-
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config/type_defs.pyi` & `mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for config service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_config.type_defs import AccountAggregationSourceTypeDef
+    from mypy_boto3_config.type_defs import AccountAggregationSourceOutputTypeDef
 
-    data: AccountAggregationSourceTypeDef = {...}
+    data: AccountAggregationSourceOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,46 +52,55 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
+    "AggregateResourceIdentifierOutputTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
     "AggregationAuthorizationTypeDef",
     "BaseConfigurationItemTypeDef",
     "ResourceKeyTypeDef",
+    "ResourceKeyOutputTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
+    "EvaluationModeConfigurationOutputTypeDef",
+    "ScopeOutputTypeDef",
     "EvaluationModeConfigurationTypeDef",
     "ScopeTypeDef",
+    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
-    "OrganizationAggregationSourceTypeDef",
+    "OrganizationAggregationSourceOutputTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
-    "ConformancePackInputParameterTypeDef",
-    "TemplateSSMDocumentDetailsTypeDef",
+    "ConformancePackInputParameterOutputTypeDef",
+    "TemplateSSMDocumentDetailsOutputTypeDef",
     "ConformancePackEvaluationFiltersTypeDef",
+    "ConformancePackInputParameterTypeDef",
     "ConformancePackRuleComplianceTypeDef",
     "ConformancePackStatusDetailTypeDef",
+    "CustomPolicyDetailsOutputTypeDef",
     "CustomPolicyDetailsTypeDef",
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     "DeleteConfigRuleRequestRequestTypeDef",
     "DeleteConfigurationAggregatorRequestRequestTypeDef",
     "DeleteConfigurationRecorderRequestRequestTypeDef",
     "DeleteConformancePackRequestRequestTypeDef",
     "DeleteDeliveryChannelRequestRequestTypeDef",
@@ -142,21 +151,26 @@
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EvaluationContextOutputTypeDef",
     "EvaluationContextTypeDef",
+    "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
     "EvaluationTypeDef",
+    "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
+    "SsmControlsOutputTypeDef",
     "SsmControlsTypeDef",
     "ExternalEvaluationTypeDef",
+    "RemediationExceptionResourceKeyOutputTypeDef",
     "FieldInfoTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
     "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
@@ -174,141 +188,157 @@
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     "GetOrganizationCustomRulePolicyResponseTypeDef",
     "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
-    "ResourceDetailsTypeDef",
+    "ResourceDetailsOutputTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
-    "StoredQueryTypeDef",
+    "StoredQueryOutputTypeDef",
     "ResourceFiltersTypeDef",
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
+    "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
+    "OrganizationCustomRuleMetadataOutputTypeDef",
+    "OrganizationManagedRuleMetadataOutputTypeDef",
+    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
-    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "PaginatorConfigTypeDef",
+    "TagTypeDef",
+    "TemplateSSMDocumentDetailsTypeDef",
     "PutConformancePackResponseTypeDef",
     "PutOrganizationConfigRuleResponseTypeDef",
     "PutOrganizationConformancePackResponseTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
+    "StoredQueryTypeDef",
     "PutStoredQueryResponseTypeDef",
+    "RecordingStrategyOutputTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
+    "ResourceValueOutputTypeDef",
+    "StaticValueOutputTypeDef",
     "ResourceValueTypeDef",
     "StaticValueTypeDef",
+    "ResourceDetailsTypeDef",
     "TimeWindowTypeDef",
     "ResponseMetadataTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
     "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
     "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    "SourceDetailOutputTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
     "StartResourceEvaluationResponseTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     "DescribeAggregationAuthorizationsResponseTypeDef",
     "PutAggregationAuthorizationResponseTypeDef",
     "BatchGetAggregateResourceConfigResponseTypeDef",
     "BatchGetResourceConfigRequestRequestTypeDef",
-    "BatchGetResourceConfigResponseTypeDef",
     "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     "DescribeRemediationExecutionStatusRequestRequestTypeDef",
     "StartRemediationExecutionRequestRequestTypeDef",
+    "BatchGetResourceConfigResponseTypeDef",
     "StartRemediationExecutionResponseTypeDef",
     "ComplianceSummaryTypeDef",
     "ComplianceTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     "GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
+    "DeliveryChannelOutputTypeDef",
     "DeliveryChannelTypeDef",
     "DeliveryChannelStatusTypeDef",
     "ConfigurationAggregatorTypeDef",
     "ConfigurationItemTypeDef",
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     "DescribeConformancePackComplianceRequestRequestTypeDef",
     "ListConformancePackComplianceScoresResponseTypeDef",
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     "GetConformancePackComplianceSummaryResponseTypeDef",
     "OrganizationConformancePackTypeDef",
-    "PutOrganizationConformancePackRequestRequestTypeDef",
     "ConformancePackDetailTypeDef",
-    "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
+    "PutOrganizationConformancePackRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "PutRemediationExceptionsRequestRequestTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
+    "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
     "PutEvaluationsRequestRequestTypeDef",
-    "PutEvaluationsResponseTypeDef",
+    "ExecutionControlsOutputTypeDef",
     "ExecutionControlsTypeDef",
     "PutExternalEvaluationRequestRequestTypeDef",
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     "GetResourceEvaluationSummaryResponseTypeDef",
-    "StartResourceEvaluationRequestRequestTypeDef",
     "GetStoredQueryResponseTypeDef",
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "OrganizationConfigRuleTypeDef",
+    "PutOrganizationConfigRuleRequestRequestTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
     "PutConfigurationAggregatorRequestRequestTypeDef",
-    "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "OrganizationConfigRuleTypeDef",
-    "PutOrganizationConfigRuleRequestRequestTypeDef",
+    "PutConformancePackRequestRequestTypeDef",
+    "PutStoredQueryRequestRequestTypeDef",
+    "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
+    "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
+    "StartResourceEvaluationRequestRequestTypeDef",
     "ResourceEvaluationFiltersTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
@@ -319,27 +349,30 @@
     "DescribeDeliveryChannelStatusResponseTypeDef",
     "DescribeConfigurationAggregatorsResponseTypeDef",
     "PutConfigurationAggregatorResponseTypeDef",
     "GetAggregateResourceConfigResponseTypeDef",
     "GetResourceConfigHistoryResponseTypeDef",
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
-    "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
+    "DeleteRemediationExceptionsResponseTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
+    "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
+    "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     "ListResourceEvaluationsRequestRequestTypeDef",
+    "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
@@ -352,34 +385,58 @@
     "FailedRemediationBatchTypeDef",
     "PutRemediationConfigurationsRequestRequestTypeDef",
     "DescribeConfigRulesResponseTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
 )
 
+_RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredAccountAggregationSourceOutputTypeDef",
+    {
+        "AccountIds": List[str],
+    },
+)
+_OptionalAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalAccountAggregationSourceOutputTypeDef",
+    {
+        "AllAwsRegions": bool,
+        "AwsRegions": List[str],
+    },
+    total=False,
+)
+
+
+class AccountAggregationSourceOutputTypeDef(
+    _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
+):
+    pass
+
+
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
-        "AccountIds": List[str],
+        "AccountIds": Sequence[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
     "_OptionalAccountAggregationSourceTypeDef",
     {
         "AllAwsRegions": bool,
-        "AwsRegions": List[str],
+        "AwsRegions": Sequence[str],
     },
     total=False,
 )
 
+
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
 ):
     pass
 
+
 AggregateConformancePackComplianceTypeDef = TypedDict(
     "AggregateConformancePackComplianceTypeDef",
     {
         "ComplianceType": ConformancePackComplianceTypeType,
         "CompliantRuleCount": int,
         "NonCompliantRuleCount": int,
         "TotalRuleCount": int,
@@ -412,14 +469,39 @@
     {
         "AccountId": str,
         "AwsRegion": str,
     },
     total=False,
 )
 
+_RequiredAggregateResourceIdentifierOutputTypeDef = TypedDict(
+    "_RequiredAggregateResourceIdentifierOutputTypeDef",
+    {
+        "SourceAccountId": str,
+        "SourceRegion": str,
+        "ResourceId": str,
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalAggregateResourceIdentifierOutputTypeDef = TypedDict(
+    "_OptionalAggregateResourceIdentifierOutputTypeDef",
+    {
+        "ResourceName": str,
+    },
+    total=False,
+)
+
+
+class AggregateResourceIdentifierOutputTypeDef(
+    _RequiredAggregateResourceIdentifierOutputTypeDef,
+    _OptionalAggregateResourceIdentifierOutputTypeDef,
+):
+    pass
+
+
 _RequiredAggregateResourceIdentifierTypeDef = TypedDict(
     "_RequiredAggregateResourceIdentifierTypeDef",
     {
         "SourceAccountId": str,
         "SourceRegion": str,
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
@@ -429,19 +511,21 @@
     "_OptionalAggregateResourceIdentifierTypeDef",
     {
         "ResourceName": str,
     },
     total=False,
 )
 
+
 class AggregateResourceIdentifierTypeDef(
     _RequiredAggregateResourceIdentifierTypeDef, _OptionalAggregateResourceIdentifierTypeDef
 ):
     pass
 
+
 AggregatedSourceStatusTypeDef = TypedDict(
     "AggregatedSourceStatusTypeDef",
     {
         "SourceId": str,
         "SourceType": AggregatedSourceTypeType,
         "AwsRegion": str,
         "LastUpdateStatus": AggregatedSourceStatusTypeType,
@@ -488,14 +572,22 @@
     "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
 
+ResourceKeyOutputTypeDef = TypedDict(
+    "ResourceKeyOutputTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+
 ComplianceContributorCountTypeDef = TypedDict(
     "ComplianceContributorCountTypeDef",
     {
         "CappedCount": int,
         "CapExceeded": bool,
     },
     total=False,
@@ -552,33 +644,60 @@
         "LastDebugLogDeliveryStatus": str,
         "LastDebugLogDeliveryStatusReason": str,
         "LastDebugLogDeliveryTime": datetime,
     },
     total=False,
 )
 
+EvaluationModeConfigurationOutputTypeDef = TypedDict(
+    "EvaluationModeConfigurationOutputTypeDef",
+    {
+        "Mode": EvaluationModeType,
+    },
+    total=False,
+)
+
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "ComplianceResourceTypes": List[str],
+        "TagKey": str,
+        "TagValue": str,
+        "ComplianceResourceId": str,
+    },
+    total=False,
+)
+
 EvaluationModeConfigurationTypeDef = TypedDict(
     "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
-        "ComplianceResourceTypes": List[str],
+        "ComplianceResourceTypes": Sequence[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
+ConfigSnapshotDeliveryPropertiesOutputTypeDef = TypedDict(
+    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
+    {
+        "deliveryFrequency": MaximumExecutionFrequencyType,
+    },
+    total=False,
+)
+
 ConfigSnapshotDeliveryPropertiesTypeDef = TypedDict(
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     {
         "deliveryFrequency": MaximumExecutionFrequencyType,
     },
     total=False,
 )
@@ -590,34 +709,37 @@
         "lastErrorCode": str,
         "lastErrorMessage": str,
         "lastStatusChangeTime": datetime,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceTypeDef",
+_RequiredOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceOutputTypeDef",
     {
         "RoleArn": str,
     },
 )
-_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceTypeDef",
+_OptionalOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceOutputTypeDef",
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
-class OrganizationAggregationSourceTypeDef(
-    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+
+class OrganizationAggregationSourceOutputTypeDef(
+    _RequiredOrganizationAggregationSourceOutputTypeDef,
+    _OptionalOrganizationAggregationSourceOutputTypeDef,
 ):
     pass
 
+
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "relationshipName": str,
@@ -670,52 +792,63 @@
     "ConformancePackComplianceSummaryTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackComplianceStatus": ConformancePackComplianceTypeType,
     },
 )
 
-ConformancePackInputParameterTypeDef = TypedDict(
-    "ConformancePackInputParameterTypeDef",
+ConformancePackInputParameterOutputTypeDef = TypedDict(
+    "ConformancePackInputParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
 )
 
-_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_RequiredTemplateSSMDocumentDetailsTypeDef",
+_RequiredTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
+    "_RequiredTemplateSSMDocumentDetailsOutputTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_OptionalTemplateSSMDocumentDetailsTypeDef",
+_OptionalTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
+    "_OptionalTemplateSSMDocumentDetailsOutputTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-class TemplateSSMDocumentDetailsTypeDef(
-    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
+
+class TemplateSSMDocumentDetailsOutputTypeDef(
+    _RequiredTemplateSSMDocumentDetailsOutputTypeDef,
+    _OptionalTemplateSSMDocumentDetailsOutputTypeDef,
 ):
     pass
 
+
 ConformancePackEvaluationFiltersTypeDef = TypedDict(
     "ConformancePackEvaluationFiltersTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceType": ConformancePackComplianceTypeType,
         "ResourceType": str,
         "ResourceIds": Sequence[str],
     },
     total=False,
 )
 
+ConformancePackInputParameterTypeDef = TypedDict(
+    "ConformancePackInputParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+    },
+)
+
 ConformancePackRuleComplianceTypeDef = TypedDict(
     "ConformancePackRuleComplianceTypeDef",
     {
         "ConfigRuleName": str,
         "ComplianceType": ConformancePackComplianceTypeType,
         "Controls": List[str],
     },
@@ -738,19 +871,43 @@
     {
         "ConformancePackStatusReason": str,
         "LastUpdateCompletedTime": datetime,
     },
     total=False,
 )
 
+
 class ConformancePackStatusDetailTypeDef(
     _RequiredConformancePackStatusDetailTypeDef, _OptionalConformancePackStatusDetailTypeDef
 ):
     pass
 
+
+_RequiredCustomPolicyDetailsOutputTypeDef = TypedDict(
+    "_RequiredCustomPolicyDetailsOutputTypeDef",
+    {
+        "PolicyRuntime": str,
+        "PolicyText": str,
+    },
+)
+_OptionalCustomPolicyDetailsOutputTypeDef = TypedDict(
+    "_OptionalCustomPolicyDetailsOutputTypeDef",
+    {
+        "EnableDebugLogDelivery": bool,
+    },
+    total=False,
+)
+
+
+class CustomPolicyDetailsOutputTypeDef(
+    _RequiredCustomPolicyDetailsOutputTypeDef, _OptionalCustomPolicyDetailsOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomPolicyDetailsTypeDef = TypedDict(
     "_RequiredCustomPolicyDetailsTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -758,19 +915,21 @@
     "_OptionalCustomPolicyDetailsTypeDef",
     {
         "EnableDebugLogDelivery": bool,
     },
     total=False,
 )
 
+
 class CustomPolicyDetailsTypeDef(
     _RequiredCustomPolicyDetailsTypeDef, _OptionalCustomPolicyDetailsTypeDef
 ):
     pass
 
+
 DeleteAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
         "AuthorizedAwsRegion": str,
     },
 )
@@ -849,20 +1008,22 @@
     "_OptionalDeleteRemediationConfigurationRequestRequestTypeDef",
     {
         "ResourceType": str,
     },
     total=False,
 )
 
+
 class DeleteRemediationConfigurationRequestRequestTypeDef(
     _RequiredDeleteRemediationConfigurationRequestRequestTypeDef,
     _OptionalDeleteRemediationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 RemediationExceptionResourceKeyTypeDef = TypedDict(
     "RemediationExceptionResourceKeyTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
     },
     total=False,
@@ -1005,20 +1166,22 @@
     {
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
@@ -1027,20 +1190,22 @@
         "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1158,19 +1323,21 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
+
 DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1218,20 +1385,22 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
+
 DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1293,19 +1462,21 @@
     {
         "Message": str,
         "ExpirationTime": datetime,
     },
     total=False,
 )
 
+
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
+
 DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1331,22 +1502,52 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EvaluationContextOutputTypeDef = TypedDict(
+    "EvaluationContextOutputTypeDef",
+    {
+        "EvaluationContextIdentifier": str,
+    },
+    total=False,
+)
+
 EvaluationContextTypeDef = TypedDict(
     "EvaluationContextTypeDef",
     {
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
 
+_RequiredEvaluationOutputTypeDef = TypedDict(
+    "_RequiredEvaluationOutputTypeDef",
+    {
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": datetime,
+    },
+)
+_OptionalEvaluationOutputTypeDef = TypedDict(
+    "_OptionalEvaluationOutputTypeDef",
+    {
+        "Annotation": str,
+    },
+    total=False,
+)
+
+
+class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
+    pass
+
+
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1364,17 +1565,19 @@
     "_OptionalEvaluationStatusTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
+
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
+
 _RequiredEvaluationTypeDef = TypedDict(
     "_RequiredEvaluationTypeDef",
     {
         "ComplianceResourceType": str,
         "ComplianceResourceId": str,
         "ComplianceType": ComplianceTypeType,
         "OrderingTimestamp": Union[datetime, str],
@@ -1384,21 +1587,40 @@
     "_OptionalEvaluationTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
+
 class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
     pass
 
+
+ExclusionByResourceTypesOutputTypeDef = TypedDict(
+    "ExclusionByResourceTypesOutputTypeDef",
+    {
+        "resourceTypes": List[ResourceTypeType],
+    },
+    total=False,
+)
+
 ExclusionByResourceTypesTypeDef = TypedDict(
     "ExclusionByResourceTypesTypeDef",
     {
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
+    },
+    total=False,
+)
+
+SsmControlsOutputTypeDef = TypedDict(
+    "SsmControlsOutputTypeDef",
+    {
+        "ConcurrentExecutionRatePercentage": int,
+        "ErrorPercentage": int,
     },
     total=False,
 )
 
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
@@ -1421,19 +1643,30 @@
     "_OptionalExternalEvaluationTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
+
 class ExternalEvaluationTypeDef(
     _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
+
+RemediationExceptionResourceKeyOutputTypeDef = TypedDict(
+    "RemediationExceptionResourceKeyOutputTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+    },
+    total=False,
+)
+
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -1452,20 +1685,22 @@
     {
         "ComplianceType": ComplianceTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigRuleName": str,
         "AccountId": str,
         "AwsRegion": str,
@@ -1477,20 +1712,22 @@
         "ComplianceType": ComplianceTypeType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceCountFiltersTypeDef = TypedDict(
     "ResourceCountFiltersTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "AccountId": str,
         "Region": str,
     },
@@ -1516,20 +1753,22 @@
     {
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
@@ -1538,20 +1777,22 @@
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
+
 GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "ResourceEvaluationId": str,
@@ -1590,20 +1831,22 @@
     "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
     },
 )
 _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -1611,20 +1854,22 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
+
 GetCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
@@ -1679,19 +1924,21 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class MemberAccountStatusTypeDef(
     _RequiredMemberAccountStatusTypeDef, _OptionalMemberAccountStatusTypeDef
 ):
     pass
 
+
 OrganizationResourceDetailedStatusFiltersTypeDef = TypedDict(
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     {
         "AccountId": str,
         "Status": OrganizationResourceDetailedStatusType,
     },
     total=False,
@@ -1711,20 +1958,22 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class OrganizationConformancePackDetailedStatusTypeDef(
     _RequiredOrganizationConformancePackDetailedStatusTypeDef,
     _OptionalOrganizationConformancePackDetailedStatusTypeDef,
 ):
     pass
 
+
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
@@ -1750,20 +1999,22 @@
         "earlierTime": Union[datetime, str],
         "chronologicalOrder": ChronologicalOrderType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
     _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
@@ -1775,73 +2026,83 @@
         "chronologicalOrder": ChronologicalOrderType,
         "limit": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class GetResourceConfigHistoryRequestRequestTypeDef(
     _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
     _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
-_RequiredResourceDetailsTypeDef = TypedDict(
-    "_RequiredResourceDetailsTypeDef",
+_RequiredResourceDetailsOutputTypeDef = TypedDict(
+    "_RequiredResourceDetailsOutputTypeDef",
     {
         "ResourceId": str,
         "ResourceType": str,
         "ResourceConfiguration": str,
     },
 )
-_OptionalResourceDetailsTypeDef = TypedDict(
-    "_OptionalResourceDetailsTypeDef",
+_OptionalResourceDetailsOutputTypeDef = TypedDict(
+    "_OptionalResourceDetailsOutputTypeDef",
     {
         "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
     },
     total=False,
 )
 
-class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
+
+class ResourceDetailsOutputTypeDef(
+    _RequiredResourceDetailsOutputTypeDef, _OptionalResourceDetailsOutputTypeDef
+):
     pass
 
+
 GetStoredQueryRequestRequestTypeDef = TypedDict(
     "GetStoredQueryRequestRequestTypeDef",
     {
         "QueryName": str,
     },
 )
 
-_RequiredStoredQueryTypeDef = TypedDict(
-    "_RequiredStoredQueryTypeDef",
+_RequiredStoredQueryOutputTypeDef = TypedDict(
+    "_RequiredStoredQueryOutputTypeDef",
     {
         "QueryName": str,
     },
 )
-_OptionalStoredQueryTypeDef = TypedDict(
-    "_OptionalStoredQueryTypeDef",
+_OptionalStoredQueryOutputTypeDef = TypedDict(
+    "_OptionalStoredQueryOutputTypeDef",
     {
         "QueryId": str,
         "QueryArn": str,
         "Description": str,
         "Expression": str,
     },
     total=False,
 )
 
-class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
+
+class StoredQueryOutputTypeDef(
+    _RequiredStoredQueryOutputTypeDef, _OptionalStoredQueryOutputTypeDef
+):
     pass
 
+
 ResourceFiltersTypeDef = TypedDict(
     "ResourceFiltersTypeDef",
     {
         "AccountId": str,
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
@@ -1862,20 +2123,22 @@
         "resourceName": str,
         "includeDeletedResources": bool,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
     _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
@@ -1886,20 +2149,22 @@
         "limit": int,
         "includeDeletedResources": bool,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
         "resourceName": str,
         "resourceDeletionTime": datetime,
@@ -1938,39 +2203,43 @@
     "_OptionalStoredQueryMetadataTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1978,29 +2247,53 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceTypeDef",
+    {
+        "RoleArn": str,
+    },
+)
+_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceTypeDef",
+    {
+        "AwsRegions": Sequence[str],
+        "AllAwsRegions": bool,
+    },
+    total=False,
+)
+
+
+class OrganizationAggregationSourceTypeDef(
+    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+):
+    pass
+
+
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -2010,65 +2303,71 @@
         "TagValueScope": str,
         "PolicyRuntime": str,
         "DebugLogDeliveryAccounts": List[str],
     },
     total=False,
 )
 
-_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataTypeDef",
+_RequiredOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeType],
     },
 )
-_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataTypeDef",
+_OptionalOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-class OrganizationCustomRuleMetadataTypeDef(
-    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+
+class OrganizationCustomRuleMetadataOutputTypeDef(
+    _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
+    _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
 ):
     pass
 
-_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataTypeDef",
+
+_RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
-_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataTypeDef",
+_OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-class OrganizationManagedRuleMetadataTypeDef(
-    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+
+class OrganizationManagedRuleMetadataOutputTypeDef(
+    _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
+    _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
 ):
     pass
 
+
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -2084,30 +2383,117 @@
         "TagKeyScope": str,
         "TagValueScope": str,
         "DebugLogDeliveryAccounts": Sequence[str],
     },
     total=False,
 )
 
+
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
+
+_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataTypeDef",
+    {
+        "LambdaFunctionArn": str,
+        "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
+    },
+)
+_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataTypeDef",
+    {
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
+    },
+    total=False,
+)
+
+
+class OrganizationCustomRuleMetadataTypeDef(
+    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+):
+    pass
+
+
+_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataTypeDef",
+    {
+        "RuleIdentifier": str,
+    },
+)
+_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataTypeDef",
+    {
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
+    },
+    total=False,
+)
+
+
+class OrganizationManagedRuleMetadataTypeDef(
+    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+):
+    pass
+
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_RequiredTemplateSSMDocumentDetailsTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_OptionalTemplateSSMDocumentDetailsTypeDef",
+    {
+        "DocumentVersion": str,
+    },
+    total=False,
+)
+
+
+class TemplateSSMDocumentDetailsTypeDef(
+    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
+):
+    pass
+
+
 PutConformancePackResponseTypeDef = TypedDict(
     "PutConformancePackResponseTypeDef",
     {
         "ConformancePackArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2142,34 +2528,66 @@
     {
         "ResourceName": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class PutResourceConfigRequestRequestTypeDef(
     _RequiredPutResourceConfigRequestRequestTypeDef, _OptionalPutResourceConfigRequestRequestTypeDef
 ):
     pass
 
+
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
+_RequiredStoredQueryTypeDef = TypedDict(
+    "_RequiredStoredQueryTypeDef",
+    {
+        "QueryName": str,
+    },
+)
+_OptionalStoredQueryTypeDef = TypedDict(
+    "_OptionalStoredQueryTypeDef",
+    {
+        "QueryId": str,
+        "QueryArn": str,
+        "Description": str,
+        "Expression": str,
+    },
+    total=False,
+)
+
+
+class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
+    pass
+
+
 PutStoredQueryResponseTypeDef = TypedDict(
     "PutStoredQueryResponseTypeDef",
     {
         "QueryArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RecordingStrategyOutputTypeDef = TypedDict(
+    "RecordingStrategyOutputTypeDef",
+    {
+        "useOnly": RecordingStrategyTypeType,
+    },
+    total=False,
+)
+
 RecordingStrategyTypeDef = TypedDict(
     "RecordingStrategyTypeDef",
     {
         "useOnly": RecordingStrategyTypeType,
     },
     total=False,
 )
@@ -2182,28 +2600,63 @@
         "ErrorMessage": str,
         "StartTime": datetime,
         "StopTime": datetime,
     },
     total=False,
 )
 
+ResourceValueOutputTypeDef = TypedDict(
+    "ResourceValueOutputTypeDef",
+    {
+        "Value": Literal["RESOURCE_ID"],
+    },
+)
+
+StaticValueOutputTypeDef = TypedDict(
+    "StaticValueOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
+
 ResourceValueTypeDef = TypedDict(
     "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
-        "Values": List[str],
+        "Values": Sequence[str],
     },
 )
 
+_RequiredResourceDetailsTypeDef = TypedDict(
+    "_RequiredResourceDetailsTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ResourceConfiguration": str,
+    },
+)
+_OptionalResourceDetailsTypeDef = TypedDict(
+    "_OptionalResourceDetailsTypeDef",
+    {
+        "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
+    },
+    total=False,
+)
+
+
+class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
+    pass
+
+
 TimeWindowTypeDef = TypedDict(
     "TimeWindowTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
@@ -2233,20 +2686,22 @@
         "Limit": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
     TypedDict(
         "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
         {
             "Expression": str,
             "ConfigurationAggregatorName": str,
         },
@@ -2259,20 +2714,22 @@
             "MaxResults": int,
             "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
+
 class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
     _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2280,40 +2737,54 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
     "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
     _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
 ):
     pass
 
+
+SourceDetailOutputTypeDef = TypedDict(
+    "SourceDetailOutputTypeDef",
+    {
+        "EventSource": Literal["aws.config"],
+        "MessageType": MessageTypeType,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+    },
+    total=False,
+)
+
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
     },
@@ -2389,20 +2860,22 @@
     {
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
@@ -2411,20 +2884,22 @@
         "Filters": AggregateConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2434,20 +2909,31 @@
         "GroupByKey": AggregateConformancePackComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
+
+ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
+    {
+        "ResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchGetAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifiers": Sequence[AggregateResourceIdentifierTypeDef],
     },
 )
@@ -2456,23 +2942,14 @@
     "GetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifier": AggregateResourceIdentifierTypeDef,
     },
 )
 
-ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
-    {
-        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeConfigurationAggregatorSourcesStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     {
         "AggregatedSourceStatusList": List[AggregatedSourceStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2495,35 +2972,26 @@
     },
 )
 
 BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigResponseTypeDef",
     {
         "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetResourceConfigRequestRequestTypeDef",
     {
         "resourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
 
-BatchGetResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetResourceConfigResponseTypeDef",
-    {
-        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
@@ -2531,20 +2999,22 @@
     {
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
@@ -2553,33 +3023,44 @@
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeRemediationExecutionStatusRequestRequestTypeDef(
     _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef,
     _OptionalDescribeRemediationExecutionStatusRequestRequestTypeDef,
 ):
     pass
 
+
 StartRemediationExecutionRequestRequestTypeDef = TypedDict(
     "StartRemediationExecutionRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
 
+BatchGetResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetResourceConfigResponseTypeDef",
+    {
+        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "unprocessedResourceKeys": List[ResourceKeyOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartRemediationExecutionResponseTypeDef = TypedDict(
     "StartRemediationExecutionResponseTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[ResourceKeyTypeDef],
+        "FailedItems": List[ResourceKeyOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComplianceSummaryTypeDef = TypedDict(
     "ComplianceSummaryTypeDef",
     {
@@ -2610,20 +3091,22 @@
     {
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
@@ -2632,20 +3115,22 @@
         "Filters": ConfigRuleComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef(
     _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -2655,29 +3140,44 @@
         "GroupByKey": ConfigRuleComplianceSummaryGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeliveryChannelOutputTypeDef = TypedDict(
+    "DeliveryChannelOutputTypeDef",
+    {
+        "name": str,
+        "s3BucketName": str,
+        "s3KeyPrefix": str,
+        "s3KmsKeyArn": str,
+        "snsTopicARN": str,
+        "configSnapshotDeliveryProperties": ConfigSnapshotDeliveryPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 DeliveryChannelTypeDef = TypedDict(
     "DeliveryChannelTypeDef",
     {
         "name": str,
         "s3BucketName": str,
         "s3KeyPrefix": str,
         "s3KmsKeyArn": str,
@@ -2699,16 +3199,16 @@
 )
 
 ConfigurationAggregatorTypeDef = TypedDict(
     "ConfigurationAggregatorTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigurationAggregatorArn": str,
-        "AccountAggregationSources": List[AccountAggregationSourceTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "AccountAggregationSources": List[AccountAggregationSourceOutputTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
@@ -2757,20 +3257,22 @@
         "Filters": ConformancePackComplianceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeConformancePackComplianceRequestRequestTypeDef(
     _RequiredDescribeConformancePackComplianceRequestRequestTypeDef,
     _OptionalDescribeConformancePackComplianceRequestRequestTypeDef,
 ):
     pass
 
+
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2806,100 +3308,54 @@
     },
 )
 _OptionalOrganizationConformancePackTypeDef = TypedDict(
     "_OptionalOrganizationConformancePackTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
         "ExcludedAccounts": List[str],
     },
     total=False,
 )
 
+
 class OrganizationConformancePackTypeDef(
     _RequiredOrganizationConformancePackTypeDef, _OptionalOrganizationConformancePackTypeDef
 ):
     pass
 
-_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
-    {
-        "OrganizationConformancePackName": str,
-    },
-)
-_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
-    {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "ExcludedAccounts": Sequence[str],
-    },
-    total=False,
-)
-
-class PutOrganizationConformancePackRequestRequestTypeDef(
-    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
-    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
-):
-    pass
 
 _RequiredConformancePackDetailTypeDef = TypedDict(
     "_RequiredConformancePackDetailTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackArn": str,
         "ConformancePackId": str,
     },
 )
 _OptionalConformancePackDetailTypeDef = TypedDict(
     "_OptionalConformancePackDetailTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
         "LastUpdateRequestedTime": datetime,
         "CreatedBy": str,
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsOutputTypeDef,
     },
     total=False,
 )
 
+
 class ConformancePackDetailTypeDef(
     _RequiredConformancePackDetailTypeDef, _OptionalConformancePackDetailTypeDef
 ):
     pass
 
-_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConformancePackRequestRequestTypeDef",
-    {
-        "ConformancePackName": str,
-    },
-)
-_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConformancePackRequestRequestTypeDef",
-    {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
-    },
-    total=False,
-)
-
-class PutConformancePackRequestRequestTypeDef(
-    _RequiredPutConformancePackRequestRequestTypeDef,
-    _OptionalPutConformancePackRequestRequestTypeDef,
-):
-    pass
 
 _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
@@ -2909,20 +3365,49 @@
         "Filters": ConformancePackEvaluationFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConformancePackComplianceDetailsRequestRequestTypeDef(
     _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
     _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "OrganizationConformancePackName": str,
+    },
+)
+_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "ExcludedAccounts": Sequence[str],
+    },
+    total=False,
+)
+
+
+class PutOrganizationConformancePackRequestRequestTypeDef(
+    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
+    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2958,28 +3443,21 @@
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeRemediationExceptionsRequestRequestTypeDef(
     _RequiredDescribeRemediationExceptionsRequestRequestTypeDef,
     _OptionalDescribeRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
-FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
-    {
-        "FailureMessage": str,
-        "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
-    },
-    total=False,
-)
 
 _RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
@@ -2989,20 +3467,22 @@
     {
         "Message": str,
         "ExpirationTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class PutRemediationExceptionsRequestRequestTypeDef(
     _RequiredPutRemediationExceptionsRequestRequestTypeDef,
     _OptionalPutRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -3077,14 +3557,22 @@
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutEvaluationsResponseTypeDef = TypedDict(
+    "PutEvaluationsResponseTypeDef",
+    {
+        "FailedEvaluations": List[EvaluationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
@@ -3102,25 +3590,27 @@
     {
         "Evaluations": Sequence[EvaluationTypeDef],
         "TestMode": bool,
     },
     total=False,
 )
 
+
 class PutEvaluationsRequestRequestTypeDef(
     _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
 ):
     pass
 
-PutEvaluationsResponseTypeDef = TypedDict(
-    "PutEvaluationsResponseTypeDef",
+
+ExecutionControlsOutputTypeDef = TypedDict(
+    "ExecutionControlsOutputTypeDef",
     {
-        "FailedEvaluations": List[EvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SsmControls": SsmControlsOutputTypeDef,
     },
+    total=False,
 )
 
 ExecutionControlsTypeDef = TypedDict(
     "ExecutionControlsTypeDef",
     {
         "SsmControls": SsmControlsTypeDef,
     },
@@ -3131,14 +3621,23 @@
     "PutExternalEvaluationRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ExternalEvaluation": ExternalEvaluationTypeDef,
     },
 )
 
+FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
+    {
+        "FailureMessage": str,
+        "FailedItems": List[RemediationExceptionResourceKeyOutputTypeDef],
+    },
+    total=False,
+)
+
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
     total=False,
 )
@@ -3156,20 +3655,22 @@
         "GroupByKey": ResourceCountGroupKeyType,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAggregateDiscoveredResourceCountsRequestRequestTypeDef(
     _RequiredGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     _OptionalGetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
 ):
     pass
 
+
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
@@ -3198,20 +3699,22 @@
     {
         "Filters": StatusDetailFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3220,20 +3723,22 @@
         "Filters": StatusDetailFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
+
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3250,20 +3755,22 @@
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = TypedDict(
@@ -3272,20 +3779,22 @@
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
 ):
     pass
 
+
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
@@ -3297,47 +3806,24 @@
     "GetResourceEvaluationSummaryResponseTypeDef",
     {
         "ResourceEvaluationId": str,
         "EvaluationMode": EvaluationModeType,
         "EvaluationStatus": EvaluationStatusTypeDef,
         "EvaluationStartTimestamp": datetime,
         "Compliance": ComplianceTypeType,
-        "EvaluationContext": EvaluationContextTypeDef,
-        "ResourceDetails": ResourceDetailsTypeDef,
+        "EvaluationContext": EvaluationContextOutputTypeDef,
+        "ResourceDetails": ResourceDetailsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "ResourceDetails": ResourceDetailsTypeDef,
-        "EvaluationMode": EvaluationModeType,
-    },
-)
-_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "EvaluationContext": EvaluationContextTypeDef,
-        "EvaluationTimeout": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class StartResourceEvaluationRequestRequestTypeDef(
-    _RequiredStartResourceEvaluationRequestRequestTypeDef,
-    _OptionalStartResourceEvaluationRequestRequestTypeDef,
-):
-    pass
-
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
-        "StoredQuery": StoredQueryTypeDef,
+        "StoredQuery": StoredQueryOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
@@ -3350,20 +3836,22 @@
     {
         "Filters": ResourceFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
@@ -3373,20 +3861,22 @@
         "Filters": ResourceFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAggregateDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3409,20 +3899,71 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredOrganizationConfigRuleTypeDef = TypedDict(
+    "_RequiredOrganizationConfigRuleTypeDef",
+    {
+        "OrganizationConfigRuleName": str,
+        "OrganizationConfigRuleArn": str,
+    },
+)
+_OptionalOrganizationConfigRuleTypeDef = TypedDict(
+    "_OptionalOrganizationConfigRuleTypeDef",
+    {
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
+        "ExcludedAccounts": List[str],
+        "LastUpdateTime": datetime,
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    },
+    total=False,
+)
+
+
+class OrganizationConfigRuleTypeDef(
+    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
+):
+    pass
+
+
+_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
+    {
+        "OrganizationConfigRuleName": str,
+    },
+)
+_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
+    {
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
+        "ExcludedAccounts": Sequence[str],
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
+    },
+    total=False,
+)
+
+
+class PutOrganizationConfigRuleRequestRequestTypeDef(
+    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
+    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
         "AuthorizedAwsRegion": str,
     },
 )
@@ -3430,20 +3971,22 @@
     "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
@@ -3452,156 +3995,209 @@
         "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
         "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutConfigurationAggregatorRequestRequestTypeDef(
     _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
     _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
 ):
     pass
 
-_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredPutStoredQueryRequestRequestTypeDef",
-    {
-        "StoredQuery": StoredQueryTypeDef,
-    },
-)
-_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalPutStoredQueryRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutStoredQueryRequestRequestTypeDef(
-    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
-):
-    pass
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredOrganizationConfigRuleTypeDef = TypedDict(
-    "_RequiredOrganizationConfigRuleTypeDef",
+_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConformancePackRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
-        "OrganizationConfigRuleArn": str,
+        "ConformancePackName": str,
     },
 )
-_OptionalOrganizationConfigRuleTypeDef = TypedDict(
-    "_OptionalOrganizationConfigRuleTypeDef",
+_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConformancePackRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
-        "ExcludedAccounts": List[str],
-        "LastUpdateTime": datetime,
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
-class OrganizationConfigRuleTypeDef(
-    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
+
+class PutConformancePackRequestRequestTypeDef(
+    _RequiredPutConformancePackRequestRequestTypeDef,
+    _OptionalPutConformancePackRequestRequestTypeDef,
 ):
     pass
 
-_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
+
+_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
+        "StoredQuery": StoredQueryTypeDef,
     },
 )
-_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
+_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
-        "ExcludedAccounts": Sequence[str],
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class PutOrganizationConfigRuleRequestRequestTypeDef(
-    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
-    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
+
+class PutStoredQueryRequestRequestTypeDef(
+    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
 ):
     pass
 
+
+RecordingGroupOutputTypeDef = TypedDict(
+    "RecordingGroupOutputTypeDef",
+    {
+        "allSupported": bool,
+        "includeGlobalResourceTypes": bool,
+        "resourceTypes": List[ResourceTypeType],
+        "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
+        "recordingStrategy": RecordingStrategyOutputTypeDef,
+    },
+    total=False,
+)
+
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesTypeDef,
         "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
     "RemediationExecutionStatusTypeDef",
     {
-        "ResourceKey": ResourceKeyTypeDef,
+        "ResourceKey": ResourceKeyOutputTypeDef,
         "State": RemediationExecutionStateType,
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
+RemediationParameterValueOutputTypeDef = TypedDict(
+    "RemediationParameterValueOutputTypeDef",
+    {
+        "ResourceValue": ResourceValueOutputTypeDef,
+        "StaticValue": StaticValueOutputTypeDef,
+    },
+    total=False,
+)
+
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
+_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "ResourceDetails": ResourceDetailsTypeDef,
+        "EvaluationMode": EvaluationModeType,
+    },
+)
+_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "EvaluationContext": EvaluationContextTypeDef,
+        "EvaluationTimeout": int,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class StartResourceEvaluationRequestRequestTypeDef(
+    _RequiredStartResourceEvaluationRequestRequestTypeDef,
+    _OptionalStartResourceEvaluationRequestRequestTypeDef,
+):
+    pass
+
+
 ResourceEvaluationFiltersTypeDef = TypedDict(
     "ResourceEvaluationFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
         "TimeWindow": TimeWindowTypeDef,
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
 
+_RequiredSourceOutputTypeDef = TypedDict(
+    "_RequiredSourceOutputTypeDef",
+    {
+        "Owner": OwnerType,
+    },
+)
+_OptionalSourceOutputTypeDef = TypedDict(
+    "_OptionalSourceOutputTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceDetails": List[SourceDetailOutputTypeDef],
+        "CustomPolicyDetails": CustomPolicyDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
+    pass
+
+
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailTypeDef],
+        "SourceDetails": Sequence[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
+
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
+
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3674,15 +4270,15 @@
     },
     total=False,
 )
 
 DescribeDeliveryChannelsResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelsResponseTypeDef",
     {
-        "DeliveryChannels": List[DeliveryChannelTypeDef],
+        "DeliveryChannels": List[DeliveryChannelOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDeliveryChannelRequestRequestTypeDef = TypedDict(
     "PutDeliveryChannelRequestRequestTypeDef",
     {
@@ -3746,22 +4342,14 @@
     {
         "ConformancePackDetails": List[ConformancePackDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRemediationExceptionsResponseTypeDef = TypedDict(
-    "DeleteRemediationExceptionsResponseTypeDef",
-    {
-        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutRemediationExceptionsResponseTypeDef = TypedDict(
     "PutRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationExceptionBatchTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3793,32 +4381,42 @@
     "_OptionalConformancePackEvaluationResultTypeDef",
     {
         "Annotation": str,
     },
     total=False,
 )
 
+
 class ConformancePackEvaluationResultTypeDef(
     _RequiredConformancePackEvaluationResultTypeDef, _OptionalConformancePackEvaluationResultTypeDef
 ):
     pass
 
+
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
         "ComplianceType": ComplianceTypeType,
         "ResultRecordedTime": datetime,
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
+DeleteRemediationExceptionsResponseTypeDef = TypedDict(
+    "DeleteRemediationExceptionsResponseTypeDef",
+    {
+        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -3840,14 +4438,24 @@
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConfigurationRecorderOutputTypeDef = TypedDict(
+    "ConfigurationRecorderOutputTypeDef",
+    {
+        "name": str,
+        "roleARN": str,
+        "recordingGroup": RecordingGroupOutputTypeDef,
+    },
+    total=False,
+)
+
 ConfigurationRecorderTypeDef = TypedDict(
     "ConfigurationRecorderTypeDef",
     {
         "name": str,
         "roleARN": str,
         "recordingGroup": RecordingGroupTypeDef,
     },
@@ -3859,43 +4467,76 @@
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRemediationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredRemediationConfigurationOutputTypeDef",
+    {
+        "ConfigRuleName": str,
+        "TargetType": Literal["SSM_DOCUMENT"],
+        "TargetId": str,
+    },
+)
+_OptionalRemediationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalRemediationConfigurationOutputTypeDef",
+    {
+        "TargetVersion": str,
+        "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
+        "ResourceType": str,
+        "Automatic": bool,
+        "ExecutionControls": ExecutionControlsOutputTypeDef,
+        "MaximumAutomaticAttempts": int,
+        "RetryAttemptSeconds": int,
+        "Arn": str,
+        "CreatedByService": str,
+    },
+    total=False,
+)
+
+
+class RemediationConfigurationOutputTypeDef(
+    _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
 )
 _OptionalRemediationConfigurationTypeDef = TypedDict(
     "_OptionalRemediationConfigurationTypeDef",
     {
         "TargetVersion": str,
-        "Parameters": Dict[str, RemediationParameterValueTypeDef],
+        "Parameters": Mapping[str, RemediationParameterValueTypeDef],
         "ResourceType": str,
         "Automatic": bool,
         "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
 
+
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
+
 ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     {
         "Filters": ResourceEvaluationFiltersTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -3907,14 +4548,42 @@
         "Filters": ResourceEvaluationFiltersTypeDef,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredConfigRuleOutputTypeDef = TypedDict(
+    "_RequiredConfigRuleOutputTypeDef",
+    {
+        "Source": SourceOutputTypeDef,
+    },
+)
+_OptionalConfigRuleOutputTypeDef = TypedDict(
+    "_OptionalConfigRuleOutputTypeDef",
+    {
+        "ConfigRuleName": str,
+        "ConfigRuleArn": str,
+        "ConfigRuleId": str,
+        "Description": str,
+        "Scope": ScopeOutputTypeDef,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ConfigRuleState": ConfigRuleStateType,
+        "CreatedBy": str,
+        "EvaluationModes": List[EvaluationModeConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
+    pass
+
+
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -3925,22 +4594,24 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
+        "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
 
+
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4018,54 +4689,54 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
-        "ConfigurationRecorders": List[ConfigurationRecorderTypeDef],
+        "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
-        "RemediationConfigurations": List[RemediationConfigurationTypeDef],
+        "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[RemediationConfigurationTypeDef],
+        "FailedItems": List[RemediationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
     "PutRemediationConfigurationsRequestRequestTypeDef",
     {
         "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
     },
 )
 
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
-        "ConfigRules": List[ConfigRuleTypeDef],
+        "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
@@ -4077,19 +4748,21 @@
     "_OptionalPutConfigRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutConfigRuleRequestRequestTypeDef(
     _RequiredPutConfigRuleRequestRequestTypeDef, _OptionalPutConfigRuleRequestRequestTypeDef
 ):
     pass
 
+
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/PKG-INFO` & `mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.28.0
-Summary: Type annotations for boto3.ConfigService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ConfigService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-config"></a>
 
 # mypy-boto3-config
 
 [![PyPI - mypy-boto3-config](https://img.shields.io/pypi/v/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-config?color=blue)](https://pypistats.org/packages/mypy-boto3-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -506,45 +506,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_config.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_config.type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
+    AggregateResourceIdentifierOutputTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
     ResourceKeyTypeDef,
+    ResourceKeyOutputTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
+    EvaluationModeConfigurationOutputTypeDef,
+    ScopeOutputTypeDef,
     EvaluationModeConfigurationTypeDef,
     ScopeTypeDef,
+    ConfigSnapshotDeliveryPropertiesOutputTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
-    ConformancePackInputParameterTypeDef,
-    TemplateSSMDocumentDetailsTypeDef,
+    ConformancePackInputParameterOutputTypeDef,
+    TemplateSSMDocumentDetailsOutputTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
+    ConformancePackInputParameterTypeDef,
     ConformancePackRuleComplianceTypeDef,
     ConformancePackStatusDetailTypeDef,
+    CustomPolicyDetailsOutputTypeDef,
     CustomPolicyDetailsTypeDef,
     DeleteAggregationAuthorizationRequestRequestTypeDef,
     DeleteConfigRuleRequestRequestTypeDef,
     DeleteConfigurationAggregatorRequestRequestTypeDef,
     DeleteConfigurationRecorderRequestRequestTypeDef,
     DeleteConformancePackRequestRequestTypeDef,
     DeleteDeliveryChannelRequestRequestTypeDef,
@@ -595,21 +603,26 @@
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
     DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
+    EvaluationContextOutputTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
     EvaluationTypeDef,
+    ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
+    SsmControlsOutputTypeDef,
     SsmControlsTypeDef,
     ExternalEvaluationTypeDef,
+    RemediationExceptionResourceKeyOutputTypeDef,
     FieldInfoTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
     GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
@@ -627,141 +640,157 @@
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
     GetOrganizationCustomRulePolicyResponseTypeDef,
     GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
-    ResourceDetailsTypeDef,
+    ResourceDetailsOutputTypeDef,
     GetStoredQueryRequestRequestTypeDef,
-    StoredQueryTypeDef,
+    StoredQueryOutputTypeDef,
     ResourceFiltersTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
+    OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    OrganizationCustomPolicyRuleMetadataTypeDef,
     PaginatorConfigTypeDef,
+    TagTypeDef,
+    TemplateSSMDocumentDetailsTypeDef,
     PutConformancePackResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
+    StoredQueryTypeDef,
     PutStoredQueryResponseTypeDef,
+    RecordingStrategyOutputTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
+    ResourceValueOutputTypeDef,
+    StaticValueOutputTypeDef,
     ResourceValueTypeDef,
     StaticValueTypeDef,
+    ResourceDetailsTypeDef,
     TimeWindowTypeDef,
     ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
     SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
     SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+    SourceDetailOutputTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
     StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
     DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
-    BatchGetResourceConfigResponseTypeDef,
     DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
+    BatchGetResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
+    DeliveryChannelOutputTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
     DescribeConfigurationRecorderStatusResponseTypeDef,
     DescribeConformancePackComplianceRequestRequestTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListConformancePackComplianceScoresRequestRequestTypeDef,
     GetConformancePackComplianceSummaryResponseTypeDef,
     OrganizationConformancePackTypeDef,
-    PutOrganizationConformancePackRequestRequestTypeDef,
     ConformancePackDetailTypeDef,
-    PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
+    PutOrganizationConformancePackRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
-    FailedDeleteRemediationExceptionsBatchTypeDef,
     PutRemediationExceptionsRequestRequestTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
+    PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
     PutEvaluationsRequestRequestTypeDef,
-    PutEvaluationsResponseTypeDef,
+    ExecutionControlsOutputTypeDef,
     ExecutionControlsTypeDef,
     PutExternalEvaluationRequestRequestTypeDef,
+    FailedDeleteRemediationExceptionsBatchTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     GetOrganizationConformancePackDetailedStatusResponseTypeDef,
     GetResourceEvaluationSummaryResponseTypeDef,
-    StartResourceEvaluationRequestRequestTypeDef,
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    OrganizationConfigRuleTypeDef,
+    PutOrganizationConfigRuleRequestRequestTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
     PutConfigurationAggregatorRequestRequestTypeDef,
-    PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    OrganizationConfigRuleTypeDef,
-    PutOrganizationConfigRuleRequestRequestTypeDef,
+    PutConformancePackRequestRequestTypeDef,
+    PutStoredQueryRequestRequestTypeDef,
+    RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
+    RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
+    StartResourceEvaluationRequestRequestTypeDef,
     ResourceEvaluationFiltersTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
@@ -772,27 +801,30 @@
     DescribeDeliveryChannelStatusResponseTypeDef,
     DescribeConfigurationAggregatorsResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetResourceConfigHistoryResponseTypeDef,
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
-    DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    DeleteRemediationExceptionsResponseTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
     ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
     ListResourceEvaluationsRequestRequestTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
@@ -806,15 +838,15 @@
     PutRemediationConfigurationsRequestRequestTypeDef,
     DescribeConfigRulesResponseTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceTypeDef:
+def get_structure() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-config-1.28.0/mypy_boto3_config.egg-info/SOURCES.txt` & `mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.0/setup.py` & `mypy-boto3-config-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-config",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConfigService 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ConfigService 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

