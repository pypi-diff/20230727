# Comparing `tmp/mypy-boto3-kendra-1.28.0.tar.gz` & `tmp/mypy-boto3-kendra-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-1.28.0.tar", last modified: Thu Jul  6 20:59:52 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-1.28.12.tar", last modified: Thu Jul 27 05:34:52 2023, max compression
```

## Comparing `mypy-boto3-kendra-1.28.0.tar` & `mypy-boto3-kendra-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.298339 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-06 20:44:34.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-07-06 20:44:34.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   110862 2023-07-06 20:44:37.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   110709 2023-07-06 20:44:35.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27095 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25612 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   153110 2023-07-27 05:24:36.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152891 2023-07-27 05:24:35.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27095 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/setup.py
```

### Comparing `mypy-boto3-kendra-1.28.0/LICENSE` & `mypy-boto3-kendra-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__main__.py` & `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.kendra 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.kendra 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.py` & `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.pyi` & `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.py` & `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,15 @@
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
@@ -472,26 +473,28 @@
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

### Comparing `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.pyi` & `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,15 @@
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
@@ -470,26 +471,28 @@
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

### Comparing `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/type_defs.py` & `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/type_defs.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -82,139 +82,193 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessControlConfigurationSummaryTypeDef",
+    "AccessControlListConfigurationOutputTypeDef",
     "AccessControlListConfigurationTypeDef",
+    "AclConfigurationOutputTypeDef",
     "AclConfigurationTypeDef",
+    "DataSourceToIndexFieldMappingOutputTypeDef",
+    "DataSourceVpcConfigurationOutputTypeDef",
+    "S3PathOutputTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "S3PathTypeDef",
     "EntityConfigurationTypeDef",
     "FailedEntityTypeDef",
     "EntityPersonaConfigurationTypeDef",
+    "SuggestableConfigOutputTypeDef",
     "SuggestableConfigTypeDef",
+    "BasicAuthenticationConfigurationOutputTypeDef",
     "BasicAuthenticationConfigurationTypeDef",
     "DataSourceSyncJobMetricTargetTypeDef",
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     "BatchDeleteFeaturedResultsSetErrorTypeDef",
     "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
     "BatchGetDocumentStatusResponseErrorTypeDef",
     "StatusTypeDef",
     "BatchPutDocumentResponseFailedDocumentTypeDef",
+    "CapacityUnitsConfigurationOutputTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "ClearQuerySuggestionsRequestRequestTypeDef",
     "ClickFeedbackTypeDef",
+    "ConfluenceAttachmentToIndexFieldMappingOutputTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
+    "ConfluenceBlogToIndexFieldMappingOutputTypeDef",
     "ConfluenceBlogToIndexFieldMappingTypeDef",
+    "ProxyConfigurationOutputTypeDef",
     "ProxyConfigurationTypeDef",
+    "ConfluencePageToIndexFieldMappingOutputTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
+    "ConfluenceSpaceToIndexFieldMappingOutputTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
+    "ConnectionConfigurationOutputTypeDef",
     "ConnectionConfigurationTypeDef",
+    "ContentSourceConfigurationOutputTypeDef",
     "ContentSourceConfigurationTypeDef",
     "CorrectionTypeDef",
     "PrincipalTypeDef",
     "CreateAccessControlConfigurationResponseTypeDef",
     "TagTypeDef",
     "CreateDataSourceResponseTypeDef",
     "CreateExperienceResponseTypeDef",
     "CreateFaqResponseTypeDef",
     "FeaturedDocumentTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "UserGroupResolutionConfigurationTypeDef",
     "CreateIndexResponseTypeDef",
     "CreateQuerySuggestionsBlockListResponseTypeDef",
     "CreateThesaurusResponseTypeDef",
+    "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "DataSourceGroupTypeDef",
     "DataSourceSummaryTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
+    "SqlConfigurationOutputTypeDef",
     "SqlConfigurationTypeDef",
     "DeleteAccessControlConfigurationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
     "DeleteExperienceRequestRequestTypeDef",
     "DeleteFaqRequestRequestTypeDef",
     "DeleteIndexRequestRequestTypeDef",
     "DeletePrincipalMappingRequestRequestTypeDef",
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     "DeleteThesaurusRequestRequestTypeDef",
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
+    "PrincipalOutputTypeDef",
     "DescribeDataSourceRequestRequestTypeDef",
     "DescribeExperienceRequestRequestTypeDef",
     "ExperienceEndpointTypeDef",
     "DescribeFaqRequestRequestTypeDef",
     "DescribeFeaturedResultsSetRequestRequestTypeDef",
     "FeaturedDocumentMissingTypeDef",
     "FeaturedDocumentWithMetadataTypeDef",
     "DescribeIndexRequestRequestTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    "UserGroupResolutionConfigurationOutputTypeDef",
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
+    "DocumentAttributeValueOutputTypeDef",
     "DocumentAttributeValueTypeDef",
+    "RelevanceOutputTypeDef",
+    "SearchOutputTypeDef",
     "RelevanceTypeDef",
     "SearchTypeDef",
+    "DocumentsMetadataConfigurationOutputTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EntityDisplayDataTypeDef",
+    "UserIdentityConfigurationOutputTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
     "FacetTypeDef",
     "FaqStatisticsTypeDef",
     "FaqSummaryTypeDef",
+    "FeaturedDocumentOutputTypeDef",
     "FeaturedResultsSetSummaryTypeDef",
     "GetSnapshotsRequestRequestTypeDef",
-    "TimeRangeTypeDef",
+    "TimeRangeOutputTypeDef",
+    "GitHubDocumentCrawlPropertiesOutputTypeDef",
+    "SaaSConfigurationOutputTypeDef",
     "GitHubDocumentCrawlPropertiesTypeDef",
     "SaaSConfigurationTypeDef",
     "MemberGroupTypeDef",
     "MemberUserTypeDef",
     "GroupSummaryTypeDef",
     "HighlightTypeDef",
     "IndexConfigurationSummaryTypeDef",
     "TextDocumentStatisticsTypeDef",
+    "JsonTokenTypeConfigurationOutputTypeDef",
     "JsonTokenTypeConfigurationTypeDef",
+    "JwtTokenTypeConfigurationOutputTypeDef",
     "JwtTokenTypeConfigurationTypeDef",
     "ListAccessControlConfigurationsRequestRequestTypeDef",
+    "TimeRangeTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListEntityPersonasRequestRequestTypeDef",
     "PersonasSummaryTypeDef",
     "ListExperienceEntitiesRequestRequestTypeDef",
     "ListExperiencesRequestRequestTypeDef",
     "ListFaqsRequestRequestTypeDef",
     "ListFeaturedResultsSetsRequestRequestTypeDef",
     "ListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     "ListIndicesRequestRequestTypeDef",
     "ListQuerySuggestionsBlockListsRequestRequestTypeDef",
     "QuerySuggestionsBlockListSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListThesauriRequestRequestTypeDef",
     "ThesaurusSummaryTypeDef",
     "SortingConfigurationTypeDef",
     "SpellCorrectionConfigurationTypeDef",
     "ScoreAttributesTypeDef",
     "WarningTypeDef",
     "RelevanceFeedbackTypeDef",
     "ResponseMetadataTypeDef",
+    "SeedUrlConfigurationOutputTypeDef",
     "SeedUrlConfigurationTypeDef",
+    "SiteMapsConfigurationOutputTypeDef",
     "SiteMapsConfigurationTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
     "StartDataSourceSyncJobResponseTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "SuggestionHighlightTypeDef",
     "TableCellTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListAccessControlConfigurationsResponseTypeDef",
+    "ColumnConfigurationOutputTypeDef",
+    "GoogleDriveConfigurationOutputTypeDef",
+    "SalesforceChatterFeedConfigurationOutputTypeDef",
+    "SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
+    "SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
+    "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
+    "SalesforceStandardObjectConfigurationOutputTypeDef",
+    "ServiceNowKnowledgeArticleConfigurationOutputTypeDef",
+    "ServiceNowServiceCatalogConfigurationOutputTypeDef",
+    "WorkDocsConfigurationOutputTypeDef",
+    "BoxConfigurationOutputTypeDef",
+    "FsxConfigurationOutputTypeDef",
+    "JiraConfigurationOutputTypeDef",
+    "QuipConfigurationOutputTypeDef",
+    "SlackConfigurationOutputTypeDef",
+    "AlfrescoConfigurationOutputTypeDef",
+    "DescribeFaqResponseTypeDef",
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    "DescribeThesaurusResponseTypeDef",
+    "OnPremiseConfigurationOutputTypeDef",
+    "OneDriveUsersOutputTypeDef",
     "ColumnConfigurationTypeDef",
     "GoogleDriveConfigurationTypeDef",
     "SalesforceChatterFeedConfigurationTypeDef",
     "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     "SalesforceStandardObjectConfigurationTypeDef",
@@ -223,160 +277,236 @@
     "WorkDocsConfigurationTypeDef",
     "BoxConfigurationTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
     "AlfrescoConfigurationTypeDef",
-    "DescribeFaqResponseTypeDef",
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    "DescribeThesaurusResponseTypeDef",
     "OnPremiseConfigurationTypeDef",
     "OneDriveUsersTypeDef",
     "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     "UpdateThesaurusRequestRequestTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
     "AssociatePersonasToEntitiesResponseTypeDef",
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     "DisassociatePersonasFromEntitiesResponseTypeDef",
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
     "AttributeSuggestionsDescribeConfigTypeDef",
     "AttributeSuggestionsUpdateConfigTypeDef",
+    "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchDeleteFeaturedResultsSetResponseTypeDef",
     "BatchGetDocumentStatusResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
+    "ConfluenceAttachmentConfigurationOutputTypeDef",
     "ConfluenceAttachmentConfigurationTypeDef",
+    "ConfluenceBlogConfigurationOutputTypeDef",
     "ConfluenceBlogConfigurationTypeDef",
+    "SharePointConfigurationOutputTypeDef",
     "SharePointConfigurationTypeDef",
+    "ConfluencePageConfigurationOutputTypeDef",
     "ConfluencePageConfigurationTypeDef",
+    "ConfluenceSpaceConfigurationOutputTypeDef",
     "ConfluenceSpaceConfigurationTypeDef",
     "SpellCorrectedQueryTypeDef",
     "HierarchicalPrincipalTypeDef",
     "CreateFaqRequestRequestTypeDef",
     "CreateQuerySuggestionsBlockListRequestRequestTypeDef",
     "CreateThesaurusRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateFeaturedResultsSetRequestRequestTypeDef",
-    "FeaturedResultsSetTypeDef",
     "UpdateFeaturedResultsSetRequestRequestTypeDef",
     "UserContextTypeDef",
     "ListDataSourcesResponseTypeDef",
     "DataSourceSyncJobTypeDef",
+    "HierarchicalPrincipalOutputTypeDef",
     "ExperiencesSummaryTypeDef",
     "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
+    "DocumentAttributeConditionOutputTypeDef",
+    "DocumentAttributeOutputTypeDef",
+    "DocumentAttributeTargetOutputTypeDef",
+    "DocumentAttributeValueCountPairTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
-    "DocumentAttributeValueCountPairTypeDef",
+    "DocumentMetadataConfigurationOutputTypeDef",
     "DocumentRelevanceConfigurationTypeDef",
     "DocumentMetadataConfigurationTypeDef",
+    "S3DataSourceConfigurationOutputTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
+    "ExperienceConfigurationOutputTypeDef",
     "ExperienceConfigurationTypeDef",
     "ListFaqsResponseTypeDef",
+    "FeaturedResultsSetTypeDef",
     "ListFeaturedResultsSetsResponseTypeDef",
     "GetSnapshotsResponseTypeDef",
-    "ListDataSourceSyncJobsRequestRequestTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
+    "UserTokenConfigurationOutputTypeDef",
     "UserTokenConfigurationTypeDef",
+    "ListDataSourceSyncJobsRequestRequestTypeDef",
     "ListEntityPersonasResponseTypeDef",
     "ListQuerySuggestionsBlockListsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListThesauriResponseTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
+    "UrlsOutputTypeDef",
     "UrlsTypeDef",
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
+    "DatabaseConfigurationOutputTypeDef",
+    "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
+    "ServiceNowConfigurationOutputTypeDef",
+    "GitHubConfigurationOutputTypeDef",
+    "OneDriveConfigurationOutputTypeDef",
     "DatabaseConfigurationTypeDef",
     "SalesforceKnowledgeArticleConfigurationTypeDef",
     "ServiceNowConfigurationTypeDef",
     "GitHubConfigurationTypeDef",
     "OneDriveConfigurationTypeDef",
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    "ConfluenceConfigurationOutputTypeDef",
     "ConfluenceConfigurationTypeDef",
     "CreateAccessControlConfigurationRequestRequestTypeDef",
-    "DescribeAccessControlConfigurationResponseTypeDef",
     "UpdateAccessControlConfigurationRequestRequestTypeDef",
-    "CreateFeaturedResultsSetResponseTypeDef",
-    "UpdateFeaturedResultsSetResponseTypeDef",
     "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
+    "DescribeAccessControlConfigurationResponseTypeDef",
     "ListExperiencesResponseTypeDef",
+    "HookConfigurationOutputTypeDef",
+    "RetrieveResultItemTypeDef",
+    "SourceDocumentTypeDef",
+    "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
     "HookConfigurationTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     "AttributeFilterTypeDef",
     "DocumentInfoTypeDef",
     "DocumentTypeDef",
-    "RetrieveResultItemTypeDef",
-    "SourceDocumentTypeDef",
     "QueryRequestRequestTypeDef",
     "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
-    "CreateExperienceRequestRequestTypeDef",
     "DescribeExperienceResponseTypeDef",
+    "CreateExperienceRequestRequestTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
+    "CreateFeaturedResultsSetResponseTypeDef",
+    "UpdateFeaturedResultsSetResponseTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
-    "CreateIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
+    "CreateIndexRequestRequestTypeDef",
     "UpdateIndexRequestRequestTypeDef",
+    "WebCrawlerConfigurationOutputTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
+    "SalesforceConfigurationOutputTypeDef",
     "SalesforceConfigurationTypeDef",
     "GetQuerySuggestionsRequestRequestTypeDef",
+    "RetrieveResultTypeDef",
+    "CustomDocumentEnrichmentConfigurationOutputTypeDef",
     "CustomDocumentEnrichmentConfigurationTypeDef",
     "BatchGetDocumentStatusRequestRequestTypeDef",
-    "RetrieveResultTypeDef",
     "AdditionalResultAttributeTypeDef",
     "SuggestionTypeDef",
+    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "BatchPutDocumentRequestRequestTypeDef",
     "FeaturedResultsItemTypeDef",
     "QueryResultItemTypeDef",
     "GetQuerySuggestionsResponseTypeDef",
-    "CreateDataSourceRequestRequestTypeDef",
     "DescribeDataSourceResponseTypeDef",
+    "CreateDataSourceRequestRequestTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "QueryResultTypeDef",
 )
 
 AccessControlConfigurationSummaryTypeDef = TypedDict(
     "AccessControlConfigurationSummaryTypeDef",
     {
         "Id": str,
     },
 )
 
+AccessControlListConfigurationOutputTypeDef = TypedDict(
+    "AccessControlListConfigurationOutputTypeDef",
+    {
+        "KeyPath": str,
+    },
+    total=False,
+)
+
 AccessControlListConfigurationTypeDef = TypedDict(
     "AccessControlListConfigurationTypeDef",
     {
         "KeyPath": str,
     },
     total=False,
 )
 
+AclConfigurationOutputTypeDef = TypedDict(
+    "AclConfigurationOutputTypeDef",
+    {
+        "AllowedGroupsColumnName": str,
+    },
+)
+
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "AllowedGroupsColumnName": str,
     },
 )
 
+_RequiredDataSourceToIndexFieldMappingOutputTypeDef = TypedDict(
+    "_RequiredDataSourceToIndexFieldMappingOutputTypeDef",
+    {
+        "DataSourceFieldName": str,
+        "IndexFieldName": str,
+    },
+)
+_OptionalDataSourceToIndexFieldMappingOutputTypeDef = TypedDict(
+    "_OptionalDataSourceToIndexFieldMappingOutputTypeDef",
+    {
+        "DateFieldFormat": str,
+    },
+    total=False,
+)
+
+class DataSourceToIndexFieldMappingOutputTypeDef(
+    _RequiredDataSourceToIndexFieldMappingOutputTypeDef,
+    _OptionalDataSourceToIndexFieldMappingOutputTypeDef,
+):
+    pass
+
+DataSourceVpcConfigurationOutputTypeDef = TypedDict(
+    "DataSourceVpcConfigurationOutputTypeDef",
+    {
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+    },
+)
+
+S3PathOutputTypeDef = TypedDict(
+    "S3PathOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+
 _RequiredDataSourceToIndexFieldMappingTypeDef = TypedDict(
     "_RequiredDataSourceToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": str,
         "IndexFieldName": str,
     },
 )
@@ -384,21 +514,19 @@
     "_OptionalDataSourceToIndexFieldMappingTypeDef",
     {
         "DateFieldFormat": str,
     },
     total=False,
 )
 
-
 class DataSourceToIndexFieldMappingTypeDef(
     _RequiredDataSourceToIndexFieldMappingTypeDef, _OptionalDataSourceToIndexFieldMappingTypeDef
 ):
     pass
 
-
 DataSourceVpcConfigurationTypeDef = TypedDict(
     "DataSourceVpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
@@ -432,23 +560,41 @@
     "EntityPersonaConfigurationTypeDef",
     {
         "EntityId": str,
         "Persona": PersonaType,
     },
 )
 
+SuggestableConfigOutputTypeDef = TypedDict(
+    "SuggestableConfigOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Suggestable": bool,
+    },
+    total=False,
+)
+
 SuggestableConfigTypeDef = TypedDict(
     "SuggestableConfigTypeDef",
     {
         "AttributeName": str,
         "Suggestable": bool,
     },
     total=False,
 )
 
+BasicAuthenticationConfigurationOutputTypeDef = TypedDict(
+    "BasicAuthenticationConfigurationOutputTypeDef",
+    {
+        "Host": str,
+        "Port": int,
+        "Credentials": str,
+    },
+)
+
 BasicAuthenticationConfigurationTypeDef = TypedDict(
     "BasicAuthenticationConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
         "Credentials": str,
     },
@@ -464,21 +610,19 @@
     "_OptionalDataSourceSyncJobMetricTargetTypeDef",
     {
         "DataSourceSyncJobId": str,
     },
     total=False,
 )
 
-
 class DataSourceSyncJobMetricTargetTypeDef(
     _RequiredDataSourceSyncJobMetricTargetTypeDef, _OptionalDataSourceSyncJobMetricTargetTypeDef
 ):
     pass
 
-
 BatchDeleteDocumentResponseFailedDocumentTypeDef = TypedDict(
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     {
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
@@ -529,14 +673,22 @@
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+CapacityUnitsConfigurationOutputTypeDef = TypedDict(
+    "CapacityUnitsConfigurationOutputTypeDef",
+    {
+        "StorageCapacityUnits": int,
+        "QueryCapacityUnits": int,
+    },
+)
+
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
     {
         "StorageCapacityUnits": int,
         "QueryCapacityUnits": int,
     },
 )
@@ -552,34 +704,74 @@
     "ClickFeedbackTypeDef",
     {
         "ResultId": str,
         "ClickTime": Union[datetime, str],
     },
 )
 
+ConfluenceAttachmentToIndexFieldMappingOutputTypeDef = TypedDict(
+    "ConfluenceAttachmentToIndexFieldMappingOutputTypeDef",
+    {
+        "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
+        "DateFieldFormat": str,
+        "IndexFieldName": str,
+    },
+    total=False,
+)
+
 ConfluenceAttachmentToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
+ConfluenceBlogToIndexFieldMappingOutputTypeDef = TypedDict(
+    "ConfluenceBlogToIndexFieldMappingOutputTypeDef",
+    {
+        "DataSourceFieldName": ConfluenceBlogFieldNameType,
+        "DateFieldFormat": str,
+        "IndexFieldName": str,
+    },
+    total=False,
+)
+
 ConfluenceBlogToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceBlogToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceBlogFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
+_RequiredProxyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredProxyConfigurationOutputTypeDef",
+    {
+        "Host": str,
+        "Port": int,
+    },
+)
+_OptionalProxyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalProxyConfigurationOutputTypeDef",
+    {
+        "Credentials": str,
+    },
+    total=False,
+)
+
+class ProxyConfigurationOutputTypeDef(
+    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
     },
 )
@@ -587,52 +779,91 @@
     "_OptionalProxyConfigurationTypeDef",
     {
         "Credentials": str,
     },
     total=False,
 )
 
-
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
+ConfluencePageToIndexFieldMappingOutputTypeDef = TypedDict(
+    "ConfluencePageToIndexFieldMappingOutputTypeDef",
+    {
+        "DataSourceFieldName": ConfluencePageFieldNameType,
+        "DateFieldFormat": str,
+        "IndexFieldName": str,
+    },
+    total=False,
+)
 
 ConfluencePageToIndexFieldMappingTypeDef = TypedDict(
     "ConfluencePageToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluencePageFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
+ConfluenceSpaceToIndexFieldMappingOutputTypeDef = TypedDict(
+    "ConfluenceSpaceToIndexFieldMappingOutputTypeDef",
+    {
+        "DataSourceFieldName": ConfluenceSpaceFieldNameType,
+        "DateFieldFormat": str,
+        "IndexFieldName": str,
+    },
+    total=False,
+)
+
 ConfluenceSpaceToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceSpaceFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
+ConnectionConfigurationOutputTypeDef = TypedDict(
+    "ConnectionConfigurationOutputTypeDef",
+    {
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "DatabaseName": str,
+        "TableName": str,
+        "SecretArn": str,
+    },
+)
+
 ConnectionConfigurationTypeDef = TypedDict(
     "ConnectionConfigurationTypeDef",
     {
         "DatabaseHost": str,
         "DatabasePort": int,
         "DatabaseName": str,
         "TableName": str,
         "SecretArn": str,
     },
 )
 
+ContentSourceConfigurationOutputTypeDef = TypedDict(
+    "ContentSourceConfigurationOutputTypeDef",
+    {
+        "DataSourceIds": List[str],
+        "FaqIds": List[str],
+        "DirectPutContent": bool,
+    },
+    total=False,
+)
+
 ContentSourceConfigurationTypeDef = TypedDict(
     "ContentSourceConfigurationTypeDef",
     {
         "DataSourceIds": Sequence[str],
         "FaqIds": Sequence[str],
         "DirectPutContent": bool,
     },
@@ -662,19 +893,17 @@
     "_OptionalPrincipalTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
-
 class PrincipalTypeDef(_RequiredPrincipalTypeDef, _OptionalPrincipalTypeDef):
     pass
 
-
 CreateAccessControlConfigurationResponseTypeDef = TypedDict(
     "CreateAccessControlConfigurationResponseTypeDef",
     {
         "Id": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -754,14 +983,22 @@
     "CreateThesaurusResponseTypeDef",
     {
         "Id": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TemplateConfigurationOutputTypeDef = TypedDict(
+    "TemplateConfigurationOutputTypeDef",
+    {
+        "Template": Dict[str, Any],
+    },
+    total=False,
+)
+
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "Template": Mapping[str, Any],
     },
     total=False,
 )
@@ -796,14 +1033,22 @@
         "DocumentsDeleted": str,
         "DocumentsFailed": str,
         "DocumentsScanned": str,
     },
     total=False,
 )
 
+SqlConfigurationOutputTypeDef = TypedDict(
+    "SqlConfigurationOutputTypeDef",
+    {
+        "QueryIdentifiersEnclosingOption": QueryIdentifiersEnclosingOptionType,
+    },
+    total=False,
+)
+
 SqlConfigurationTypeDef = TypedDict(
     "SqlConfigurationTypeDef",
     {
         "QueryIdentifiersEnclosingOption": QueryIdentifiersEnclosingOptionType,
     },
     total=False,
 )
@@ -859,22 +1104,20 @@
     {
         "DataSourceId": str,
         "OrderingId": int,
     },
     total=False,
 )
 
-
 class DeletePrincipalMappingRequestRequestTypeDef(
     _RequiredDeletePrincipalMappingRequestRequestTypeDef,
     _OptionalDeletePrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
@@ -891,14 +1134,33 @@
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
 
+_RequiredPrincipalOutputTypeDef = TypedDict(
+    "_RequiredPrincipalOutputTypeDef",
+    {
+        "Name": str,
+        "Type": PrincipalTypeType,
+        "Access": ReadAccessTypeType,
+    },
+)
+_OptionalPrincipalOutputTypeDef = TypedDict(
+    "_OptionalPrincipalOutputTypeDef",
+    {
+        "DataSourceId": str,
+    },
+    total=False,
+)
+
+class PrincipalOutputTypeDef(_RequiredPrincipalOutputTypeDef, _OptionalPrincipalOutputTypeDef):
+    pass
+
 DescribeDataSourceRequestRequestTypeDef = TypedDict(
     "DescribeDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -957,14 +1219,29 @@
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+UserGroupResolutionConfigurationOutputTypeDef = TypedDict(
+    "UserGroupResolutionConfigurationOutputTypeDef",
+    {
+        "UserGroupResolutionMode": UserGroupResolutionModeType,
+    },
+)
+
 _RequiredDescribePrincipalMappingRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePrincipalMappingRequestRequestTypeDef",
     {
         "IndexId": str,
         "GroupId": str,
     },
 )
@@ -972,22 +1249,20 @@
     "_OptionalDescribePrincipalMappingRequestRequestTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
-
 class DescribePrincipalMappingRequestRequestTypeDef(
     _RequiredDescribePrincipalMappingRequestRequestTypeDef,
     _OptionalDescribePrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
-
 GroupOrderingIdSummaryTypeDef = TypedDict(
     "GroupOrderingIdSummaryTypeDef",
     {
         "Status": PrincipalMappingStatusType,
         "LastUpdatedAt": datetime,
         "ReceivedAt": datetime,
         "OrderingId": int,
@@ -1024,33 +1299,67 @@
     {
         "Id": str,
         "IndexId": str,
         "EntityIds": Sequence[str],
     },
 )
 
+DocumentAttributeValueOutputTypeDef = TypedDict(
+    "DocumentAttributeValueOutputTypeDef",
+    {
+        "StringValue": str,
+        "StringListValue": List[str],
+        "LongValue": int,
+        "DateValue": datetime,
+    },
+    total=False,
+)
+
 DocumentAttributeValueTypeDef = TypedDict(
     "DocumentAttributeValueTypeDef",
     {
         "StringValue": str,
         "StringListValue": Sequence[str],
         "LongValue": int,
         "DateValue": Union[datetime, str],
     },
     total=False,
 )
 
+RelevanceOutputTypeDef = TypedDict(
+    "RelevanceOutputTypeDef",
+    {
+        "Freshness": bool,
+        "Importance": int,
+        "Duration": str,
+        "RankOrder": OrderType,
+        "ValueImportanceMap": Dict[str, int],
+    },
+    total=False,
+)
+
+SearchOutputTypeDef = TypedDict(
+    "SearchOutputTypeDef",
+    {
+        "Facetable": bool,
+        "Searchable": bool,
+        "Displayable": bool,
+        "Sortable": bool,
+    },
+    total=False,
+)
+
 RelevanceTypeDef = TypedDict(
     "RelevanceTypeDef",
     {
         "Freshness": bool,
         "Importance": int,
         "Duration": str,
         "RankOrder": OrderType,
-        "ValueImportanceMap": Dict[str, int],
+        "ValueImportanceMap": Mapping[str, int],
     },
     total=False,
 )
 
 SearchTypeDef = TypedDict(
     "SearchTypeDef",
     {
@@ -1058,14 +1367,22 @@
         "Searchable": bool,
         "Displayable": bool,
         "Sortable": bool,
     },
     total=False,
 )
 
+DocumentsMetadataConfigurationOutputTypeDef = TypedDict(
+    "DocumentsMetadataConfigurationOutputTypeDef",
+    {
+        "S3Prefix": str,
+    },
+    total=False,
+)
+
 DocumentsMetadataConfigurationTypeDef = TypedDict(
     "DocumentsMetadataConfigurationTypeDef",
     {
         "S3Prefix": str,
     },
     total=False,
 )
@@ -1085,14 +1402,22 @@
         "IdentifiedUserName": str,
         "FirstName": str,
         "LastName": str,
     },
     total=False,
 )
 
+UserIdentityConfigurationOutputTypeDef = TypedDict(
+    "UserIdentityConfigurationOutputTypeDef",
+    {
+        "IdentityAttributeName": str,
+    },
+    total=False,
+)
+
 UserIdentityConfigurationTypeDef = TypedDict(
     "UserIdentityConfigurationTypeDef",
     {
         "IdentityAttributeName": str,
     },
     total=False,
 )
@@ -1134,14 +1459,22 @@
         "UpdatedAt": datetime,
         "FileFormat": FaqFileFormatType,
         "LanguageCode": str,
     },
     total=False,
 )
 
+FeaturedDocumentOutputTypeDef = TypedDict(
+    "FeaturedDocumentOutputTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
 FeaturedResultsSetSummaryTypeDef = TypedDict(
     "FeaturedResultsSetSummaryTypeDef",
     {
         "FeaturedResultsSetId": str,
         "FeaturedResultsSetName": str,
         "Status": FeaturedResultsSetStatusType,
         "LastUpdatedTimestamp": int,
@@ -1163,30 +1496,50 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetSnapshotsRequestRequestTypeDef(
     _RequiredGetSnapshotsRequestRequestTypeDef, _OptionalGetSnapshotsRequestRequestTypeDef
 ):
     pass
 
-
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
+TimeRangeOutputTypeDef = TypedDict(
+    "TimeRangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
+GitHubDocumentCrawlPropertiesOutputTypeDef = TypedDict(
+    "GitHubDocumentCrawlPropertiesOutputTypeDef",
+    {
+        "CrawlRepositoryDocuments": bool,
+        "CrawlIssue": bool,
+        "CrawlIssueComment": bool,
+        "CrawlIssueCommentAttachment": bool,
+        "CrawlPullRequest": bool,
+        "CrawlPullRequestComment": bool,
+        "CrawlPullRequestCommentAttachment": bool,
+    },
+    total=False,
+)
+
+SaaSConfigurationOutputTypeDef = TypedDict(
+    "SaaSConfigurationOutputTypeDef",
+    {
+        "OrganizationName": str,
+        "HostUrl": str,
+    },
+)
+
 GitHubDocumentCrawlPropertiesTypeDef = TypedDict(
     "GitHubDocumentCrawlPropertiesTypeDef",
     {
         "CrawlRepositoryDocuments": bool,
         "CrawlIssue": bool,
         "CrawlIssueComment": bool,
         "CrawlIssueCommentAttachment": bool,
@@ -1215,19 +1568,17 @@
     "_OptionalMemberGroupTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
-
 class MemberGroupTypeDef(_RequiredMemberGroupTypeDef, _OptionalMemberGroupTypeDef):
     pass
 
-
 MemberUserTypeDef = TypedDict(
     "MemberUserTypeDef",
     {
         "UserId": str,
     },
 )
 
@@ -1252,19 +1603,17 @@
     {
         "TopAnswer": bool,
         "Type": HighlightTypeType,
     },
     total=False,
 )
 
-
 class HighlightTypeDef(_RequiredHighlightTypeDef, _OptionalHighlightTypeDef):
     pass
 
-
 _RequiredIndexConfigurationSummaryTypeDef = TypedDict(
     "_RequiredIndexConfigurationSummaryTypeDef",
     {
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": IndexStatusType,
     },
@@ -1275,37 +1624,67 @@
         "Name": str,
         "Id": str,
         "Edition": IndexEditionType,
     },
     total=False,
 )
 
-
 class IndexConfigurationSummaryTypeDef(
     _RequiredIndexConfigurationSummaryTypeDef, _OptionalIndexConfigurationSummaryTypeDef
 ):
     pass
 
-
 TextDocumentStatisticsTypeDef = TypedDict(
     "TextDocumentStatisticsTypeDef",
     {
         "IndexedTextDocumentsCount": int,
         "IndexedTextBytes": int,
     },
 )
 
+JsonTokenTypeConfigurationOutputTypeDef = TypedDict(
+    "JsonTokenTypeConfigurationOutputTypeDef",
+    {
+        "UserNameAttributeField": str,
+        "GroupAttributeField": str,
+    },
+)
+
 JsonTokenTypeConfigurationTypeDef = TypedDict(
     "JsonTokenTypeConfigurationTypeDef",
     {
         "UserNameAttributeField": str,
         "GroupAttributeField": str,
     },
 )
 
+_RequiredJwtTokenTypeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredJwtTokenTypeConfigurationOutputTypeDef",
+    {
+        "KeyLocation": KeyLocationType,
+    },
+)
+_OptionalJwtTokenTypeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalJwtTokenTypeConfigurationOutputTypeDef",
+    {
+        "URL": str,
+        "SecretManagerArn": str,
+        "UserNameAttributeField": str,
+        "GroupAttributeField": str,
+        "Issuer": str,
+        "ClaimRegex": str,
+    },
+    total=False,
+)
+
+class JwtTokenTypeConfigurationOutputTypeDef(
+    _RequiredJwtTokenTypeConfigurationOutputTypeDef, _OptionalJwtTokenTypeConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredJwtTokenTypeConfigurationTypeDef = TypedDict(
     "_RequiredJwtTokenTypeConfigurationTypeDef",
     {
         "KeyLocation": KeyLocationType,
     },
 )
 _OptionalJwtTokenTypeConfigurationTypeDef = TypedDict(
@@ -1317,21 +1696,19 @@
         "GroupAttributeField": str,
         "Issuer": str,
         "ClaimRegex": str,
     },
     total=False,
 )
 
-
 class JwtTokenTypeConfigurationTypeDef(
     _RequiredJwtTokenTypeConfigurationTypeDef, _OptionalJwtTokenTypeConfigurationTypeDef
 ):
     pass
 
-
 _RequiredListAccessControlConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessControlConfigurationsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListAccessControlConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1339,21 +1716,28 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAccessControlConfigurationsRequestRequestTypeDef(
     _RequiredListAccessControlConfigurationsRequestRequestTypeDef,
     _OptionalListAccessControlConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+    total=False,
+)
 
 _RequiredListDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourcesRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
@@ -1362,21 +1746,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDataSourcesRequestRequestTypeDef(
     _RequiredListDataSourcesRequestRequestTypeDef, _OptionalListDataSourcesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListEntityPersonasRequestRequestTypeDef = TypedDict(
     "_RequiredListEntityPersonasRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -1385,22 +1767,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEntityPersonasRequestRequestTypeDef(
     _RequiredListEntityPersonasRequestRequestTypeDef,
     _OptionalListEntityPersonasRequestRequestTypeDef,
 ):
     pass
 
-
 PersonasSummaryTypeDef = TypedDict(
     "PersonasSummaryTypeDef",
     {
         "EntityId": str,
         "Persona": PersonaType,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
@@ -1419,22 +1799,20 @@
     "_OptionalListExperienceEntitiesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListExperienceEntitiesRequestRequestTypeDef(
     _RequiredListExperienceEntitiesRequestRequestTypeDef,
     _OptionalListExperienceEntitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListExperiencesRequestRequestTypeDef = TypedDict(
     "_RequiredListExperiencesRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListExperiencesRequestRequestTypeDef = TypedDict(
@@ -1442,21 +1820,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListExperiencesRequestRequestTypeDef(
     _RequiredListExperiencesRequestRequestTypeDef, _OptionalListExperiencesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListFaqsRequestRequestTypeDef = TypedDict(
     "_RequiredListFaqsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListFaqsRequestRequestTypeDef = TypedDict(
@@ -1464,21 +1840,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListFaqsRequestRequestTypeDef(
     _RequiredListFaqsRequestRequestTypeDef, _OptionalListFaqsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturedResultsSetsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
@@ -1486,22 +1860,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListFeaturedResultsSetsRequestRequestTypeDef(
     _RequiredListFeaturedResultsSetsRequestRequestTypeDef,
     _OptionalListFeaturedResultsSetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     {
         "IndexId": str,
         "OrderingId": int,
     },
 )
@@ -1511,22 +1883,20 @@
         "DataSourceId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListGroupsOlderThanOrderingIdRequestRequestTypeDef(
     _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     _OptionalListGroupsOlderThanOrderingIdRequestRequestTypeDef,
 ):
     pass
 
-
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1543,22 +1913,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListQuerySuggestionsBlockListsRequestRequestTypeDef(
     _RequiredListQuerySuggestionsBlockListsRequestRequestTypeDef,
     _OptionalListQuerySuggestionsBlockListsRequestRequestTypeDef,
 ):
     pass
 
-
 QuerySuggestionsBlockListSummaryTypeDef = TypedDict(
     "QuerySuggestionsBlockListSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": QuerySuggestionsBlockListStatusType,
         "CreatedAt": datetime,
@@ -1571,14 +1939,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 _RequiredListThesauriRequestRequestTypeDef = TypedDict(
     "_RequiredListThesauriRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListThesauriRequestRequestTypeDef = TypedDict(
@@ -1586,21 +1962,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListThesauriRequestRequestTypeDef(
     _RequiredListThesauriRequestRequestTypeDef, _OptionalListThesauriRequestRequestTypeDef
 ):
     pass
 
-
 ThesaurusSummaryTypeDef = TypedDict(
     "ThesaurusSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": ThesaurusStatusType,
         "CreatedAt": datetime,
@@ -1656,34 +2030,58 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredSeedUrlConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSeedUrlConfigurationOutputTypeDef",
+    {
+        "SeedUrls": List[str],
+    },
+)
+_OptionalSeedUrlConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSeedUrlConfigurationOutputTypeDef",
+    {
+        "WebCrawlerMode": WebCrawlerModeType,
+    },
+    total=False,
+)
+
+class SeedUrlConfigurationOutputTypeDef(
+    _RequiredSeedUrlConfigurationOutputTypeDef, _OptionalSeedUrlConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredSeedUrlConfigurationTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationTypeDef",
     {
         "SeedUrls": Sequence[str],
     },
 )
 _OptionalSeedUrlConfigurationTypeDef = TypedDict(
     "_OptionalSeedUrlConfigurationTypeDef",
     {
         "WebCrawlerMode": WebCrawlerModeType,
     },
     total=False,
 )
 
-
 class SeedUrlConfigurationTypeDef(
     _RequiredSeedUrlConfigurationTypeDef, _OptionalSeedUrlConfigurationTypeDef
 ):
     pass
 
+SiteMapsConfigurationOutputTypeDef = TypedDict(
+    "SiteMapsConfigurationOutputTypeDef",
+    {
+        "SiteMaps": List[str],
+    },
+)
 
 SiteMapsConfigurationTypeDef = TypedDict(
     "SiteMapsConfigurationTypeDef",
     {
         "SiteMaps": Sequence[str],
     },
 )
@@ -1745,14 +2143,480 @@
     {
         "NextToken": str,
         "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredColumnConfigurationOutputTypeDef = TypedDict(
+    "_RequiredColumnConfigurationOutputTypeDef",
+    {
+        "DocumentIdColumnName": str,
+        "DocumentDataColumnName": str,
+        "ChangeDetectingColumns": List[str],
+    },
+)
+_OptionalColumnConfigurationOutputTypeDef = TypedDict(
+    "_OptionalColumnConfigurationOutputTypeDef",
+    {
+        "DocumentTitleColumnName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class ColumnConfigurationOutputTypeDef(
+    _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredGoogleDriveConfigurationOutputTypeDef = TypedDict(
+    "_RequiredGoogleDriveConfigurationOutputTypeDef",
+    {
+        "SecretArn": str,
+    },
+)
+_OptionalGoogleDriveConfigurationOutputTypeDef = TypedDict(
+    "_OptionalGoogleDriveConfigurationOutputTypeDef",
+    {
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "ExcludeMimeTypes": List[str],
+        "ExcludeUserAccounts": List[str],
+        "ExcludeSharedDrives": List[str],
+    },
+    total=False,
+)
+
+class GoogleDriveConfigurationOutputTypeDef(
+    _RequiredGoogleDriveConfigurationOutputTypeDef, _OptionalGoogleDriveConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSalesforceChatterFeedConfigurationOutputTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSalesforceChatterFeedConfigurationOutputTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "IncludeFilterTypes": List[SalesforceChatterFeedIncludeFilterTypeType],
+    },
+    total=False,
+)
+
+class SalesforceChatterFeedConfigurationOutputTypeDef(
+    _RequiredSalesforceChatterFeedConfigurationOutputTypeDef,
+    _OptionalSalesforceChatterFeedConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef(
+    _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
+    _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef(
+    _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
+    _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
+):
+    pass
+
+SalesforceStandardObjectAttachmentConfigurationOutputTypeDef = TypedDict(
+    "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+_RequiredSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSalesforceStandardObjectConfigurationOutputTypeDef",
+    {
+        "Name": SalesforceStandardObjectNameType,
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSalesforceStandardObjectConfigurationOutputTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class SalesforceStandardObjectConfigurationOutputTypeDef(
+    _RequiredSalesforceStandardObjectConfigurationOutputTypeDef,
+    _OptionalSalesforceStandardObjectConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "IncludeAttachmentFilePatterns": List[str],
+        "ExcludeAttachmentFilePatterns": List[str],
+        "DocumentTitleFieldName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FilterQuery": str,
+    },
+    total=False,
+)
+
+class ServiceNowKnowledgeArticleConfigurationOutputTypeDef(
+    _RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef,
+    _OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "IncludeAttachmentFilePatterns": List[str],
+        "ExcludeAttachmentFilePatterns": List[str],
+        "DocumentTitleFieldName": str,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class ServiceNowServiceCatalogConfigurationOutputTypeDef(
+    _RequiredServiceNowServiceCatalogConfigurationOutputTypeDef,
+    _OptionalServiceNowServiceCatalogConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredWorkDocsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredWorkDocsConfigurationOutputTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalWorkDocsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalWorkDocsConfigurationOutputTypeDef",
+    {
+        "CrawlComments": bool,
+        "UseChangeLog": bool,
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class WorkDocsConfigurationOutputTypeDef(
+    _RequiredWorkDocsConfigurationOutputTypeDef, _OptionalWorkDocsConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredBoxConfigurationOutputTypeDef = TypedDict(
+    "_RequiredBoxConfigurationOutputTypeDef",
+    {
+        "EnterpriseId": str,
+        "SecretArn": str,
+    },
+)
+_OptionalBoxConfigurationOutputTypeDef = TypedDict(
+    "_OptionalBoxConfigurationOutputTypeDef",
+    {
+        "UseChangeLog": bool,
+        "CrawlComments": bool,
+        "CrawlTasks": bool,
+        "CrawlWebLinks": bool,
+        "FileFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "TaskFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "CommentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "WebLinkFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class BoxConfigurationOutputTypeDef(
+    _RequiredBoxConfigurationOutputTypeDef, _OptionalBoxConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredFsxConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFsxConfigurationOutputTypeDef",
+    {
+        "FileSystemId": str,
+        "FileSystemType": Literal["WINDOWS"],
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+    },
+)
+_OptionalFsxConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFsxConfigurationOutputTypeDef",
+    {
+        "SecretArn": str,
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class FsxConfigurationOutputTypeDef(
+    _RequiredFsxConfigurationOutputTypeDef, _OptionalFsxConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredJiraConfigurationOutputTypeDef = TypedDict(
+    "_RequiredJiraConfigurationOutputTypeDef",
+    {
+        "JiraAccountUrl": str,
+        "SecretArn": str,
+    },
+)
+_OptionalJiraConfigurationOutputTypeDef = TypedDict(
+    "_OptionalJiraConfigurationOutputTypeDef",
+    {
+        "UseChangeLog": bool,
+        "Project": List[str],
+        "IssueType": List[str],
+        "Status": List[str],
+        "IssueSubEntityFilter": List[IssueSubEntityType],
+        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "CommentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "IssueFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "ProjectFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "WorkLogFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class JiraConfigurationOutputTypeDef(
+    _RequiredJiraConfigurationOutputTypeDef, _OptionalJiraConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredQuipConfigurationOutputTypeDef = TypedDict(
+    "_RequiredQuipConfigurationOutputTypeDef",
+    {
+        "Domain": str,
+        "SecretArn": str,
+    },
+)
+_OptionalQuipConfigurationOutputTypeDef = TypedDict(
+    "_OptionalQuipConfigurationOutputTypeDef",
+    {
+        "CrawlFileComments": bool,
+        "CrawlChatRooms": bool,
+        "CrawlAttachments": bool,
+        "FolderIds": List[str],
+        "ThreadFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "MessageFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class QuipConfigurationOutputTypeDef(
+    _RequiredQuipConfigurationOutputTypeDef, _OptionalQuipConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredSlackConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSlackConfigurationOutputTypeDef",
+    {
+        "TeamId": str,
+        "SecretArn": str,
+        "SlackEntityList": List[SlackEntityType],
+        "SinceCrawlDate": str,
+    },
+)
+_OptionalSlackConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSlackConfigurationOutputTypeDef",
+    {
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "UseChangeLog": bool,
+        "CrawlBotMessage": bool,
+        "ExcludeArchived": bool,
+        "LookBackPeriod": int,
+        "PrivateChannelFilter": List[str],
+        "PublicChannelFilter": List[str],
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class SlackConfigurationOutputTypeDef(
+    _RequiredSlackConfigurationOutputTypeDef, _OptionalSlackConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredAlfrescoConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAlfrescoConfigurationOutputTypeDef",
+    {
+        "SiteUrl": str,
+        "SiteId": str,
+        "SecretArn": str,
+        "SslCertificateS3Path": S3PathOutputTypeDef,
+    },
+)
+_OptionalAlfrescoConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAlfrescoConfigurationOutputTypeDef",
+    {
+        "CrawlSystemFolders": bool,
+        "CrawlComments": bool,
+        "EntityFilter": List[AlfrescoEntityType],
+        "DocumentLibraryFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "BlogFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "WikiFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class AlfrescoConfigurationOutputTypeDef(
+    _RequiredAlfrescoConfigurationOutputTypeDef, _OptionalAlfrescoConfigurationOutputTypeDef
+):
+    pass
+
+DescribeFaqResponseTypeDef = TypedDict(
+    "DescribeFaqResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "S3Path": S3PathOutputTypeDef,
+        "Status": FaqStatusType,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "FileFormat": FaqFileFormatType,
+        "LanguageCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    {
+        "IndexId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "Status": QuerySuggestionsBlockListStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "SourceS3Path": S3PathOutputTypeDef,
+        "ItemCount": int,
+        "FileSizeBytes": int,
+        "RoleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeThesaurusResponseTypeDef = TypedDict(
+    "DescribeThesaurusResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Description": str,
+        "Status": ThesaurusStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "RoleArn": str,
+        "SourceS3Path": S3PathOutputTypeDef,
+        "FileSizeBytes": int,
+        "TermCount": int,
+        "SynonymRuleCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+OnPremiseConfigurationOutputTypeDef = TypedDict(
+    "OnPremiseConfigurationOutputTypeDef",
+    {
+        "HostUrl": str,
+        "OrganizationName": str,
+        "SslCertificateS3Path": S3PathOutputTypeDef,
+    },
+)
+
+OneDriveUsersOutputTypeDef = TypedDict(
+    "OneDriveUsersOutputTypeDef",
+    {
+        "OneDriveUserList": List[str],
+        "OneDriveUserS3Path": S3PathOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredColumnConfigurationTypeDef = TypedDict(
     "_RequiredColumnConfigurationTypeDef",
     {
         "DocumentIdColumnName": str,
         "DocumentDataColumnName": str,
         "ChangeDetectingColumns": Sequence[str],
     },
@@ -1762,21 +2626,19 @@
     {
         "DocumentTitleColumnName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class ColumnConfigurationTypeDef(
     _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGoogleDriveConfigurationTypeDef = TypedDict(
     "_RequiredGoogleDriveConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGoogleDriveConfigurationTypeDef = TypedDict(
@@ -1788,21 +2650,19 @@
         "ExcludeMimeTypes": Sequence[str],
         "ExcludeUserAccounts": Sequence[str],
         "ExcludeSharedDrives": Sequence[str],
     },
     total=False,
 )
 
-
 class GoogleDriveConfigurationTypeDef(
     _RequiredGoogleDriveConfigurationTypeDef, _OptionalGoogleDriveConfigurationTypeDef
 ):
     pass
 
-
 _RequiredSalesforceChatterFeedConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceChatterFeedConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceChatterFeedConfigurationTypeDef = TypedDict(
@@ -1811,22 +2671,20 @@
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
         "IncludeFilterTypes": Sequence[SalesforceChatterFeedIncludeFilterTypeType],
     },
     total=False,
 )
 
-
 class SalesforceChatterFeedConfigurationTypeDef(
     _RequiredSalesforceChatterFeedConfigurationTypeDef,
     _OptionalSalesforceChatterFeedConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     {
         "Name": str,
         "DocumentDataFieldName": str,
     },
 )
@@ -1835,22 +2693,20 @@
     {
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(
     _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
@@ -1858,22 +2714,20 @@
     {
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(
     _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
 ):
     pass
 
-
 SalesforceStandardObjectAttachmentConfigurationTypeDef = TypedDict(
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     {
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
@@ -1891,22 +2745,20 @@
     {
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SalesforceStandardObjectConfigurationTypeDef(
     _RequiredSalesforceStandardObjectConfigurationTypeDef,
     _OptionalSalesforceStandardObjectConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowKnowledgeArticleConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
@@ -1918,22 +2770,20 @@
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
         "FilterQuery": str,
     },
     total=False,
 )
 
-
 class ServiceNowKnowledgeArticleConfigurationTypeDef(
     _RequiredServiceNowKnowledgeArticleConfigurationTypeDef,
     _OptionalServiceNowKnowledgeArticleConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowServiceCatalogConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
@@ -1944,22 +2794,20 @@
         "ExcludeAttachmentFilePatterns": Sequence[str],
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class ServiceNowServiceCatalogConfigurationTypeDef(
     _RequiredServiceNowServiceCatalogConfigurationTypeDef,
     _OptionalServiceNowServiceCatalogConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredWorkDocsConfigurationTypeDef = TypedDict(
     "_RequiredWorkDocsConfigurationTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalWorkDocsConfigurationTypeDef = TypedDict(
@@ -1970,21 +2818,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class WorkDocsConfigurationTypeDef(
     _RequiredWorkDocsConfigurationTypeDef, _OptionalWorkDocsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredBoxConfigurationTypeDef = TypedDict(
     "_RequiredBoxConfigurationTypeDef",
     {
         "EnterpriseId": str,
         "SecretArn": str,
     },
 )
@@ -2002,19 +2848,17 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
     pass
 
-
 _RequiredFsxConfigurationTypeDef = TypedDict(
     "_RequiredFsxConfigurationTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
@@ -2026,19 +2870,17 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class FsxConfigurationTypeDef(_RequiredFsxConfigurationTypeDef, _OptionalFsxConfigurationTypeDef):
     pass
 
-
 _RequiredJiraConfigurationTypeDef = TypedDict(
     "_RequiredJiraConfigurationTypeDef",
     {
         "JiraAccountUrl": str,
         "SecretArn": str,
     },
 )
@@ -2058,21 +2900,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class JiraConfigurationTypeDef(
     _RequiredJiraConfigurationTypeDef, _OptionalJiraConfigurationTypeDef
 ):
     pass
 
-
 _RequiredQuipConfigurationTypeDef = TypedDict(
     "_RequiredQuipConfigurationTypeDef",
     {
         "Domain": str,
         "SecretArn": str,
     },
 )
@@ -2089,21 +2929,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class QuipConfigurationTypeDef(
     _RequiredQuipConfigurationTypeDef, _OptionalQuipConfigurationTypeDef
 ):
     pass
 
-
 _RequiredSlackConfigurationTypeDef = TypedDict(
     "_RequiredSlackConfigurationTypeDef",
     {
         "TeamId": str,
         "SecretArn": str,
         "SlackEntityList": Sequence[SlackEntityType],
         "SinceCrawlDate": str,
@@ -2122,21 +2960,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SlackConfigurationTypeDef(
     _RequiredSlackConfigurationTypeDef, _OptionalSlackConfigurationTypeDef
 ):
     pass
 
-
 _RequiredAlfrescoConfigurationTypeDef = TypedDict(
     "_RequiredAlfrescoConfigurationTypeDef",
     {
         "SiteUrl": str,
         "SiteId": str,
         "SecretArn": str,
         "SslCertificateS3Path": S3PathTypeDef,
@@ -2154,79 +2990,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class AlfrescoConfigurationTypeDef(
     _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
 ):
     pass
 
-
-DescribeFaqResponseTypeDef = TypedDict(
-    "DescribeFaqResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "S3Path": S3PathTypeDef,
-        "Status": FaqStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "FileFormat": FaqFileFormatType,
-        "LanguageCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "Status": QuerySuggestionsBlockListStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "SourceS3Path": S3PathTypeDef,
-        "ItemCount": int,
-        "FileSizeBytes": int,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeThesaurusResponseTypeDef = TypedDict(
-    "DescribeThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "Status": ThesaurusStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "RoleArn": str,
-        "SourceS3Path": S3PathTypeDef,
-        "FileSizeBytes": int,
-        "TermCount": int,
-        "SynonymRuleCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OnPremiseConfigurationTypeDef = TypedDict(
     "OnPremiseConfigurationTypeDef",
     {
         "HostUrl": str,
         "OrganizationName": str,
         "SslCertificateS3Path": S3PathTypeDef,
     },
@@ -2255,22 +3031,20 @@
         "Description": str,
         "SourceS3Path": S3PathTypeDef,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateQuerySuggestionsBlockListRequestRequestTypeDef(
     _RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
     _OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateThesaurusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThesaurusRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -2281,21 +3055,19 @@
         "Description": str,
         "RoleArn": str,
         "SourceS3Path": S3PathTypeDef,
     },
     total=False,
 )
 
-
 class UpdateThesaurusRequestRequestTypeDef(
     _RequiredUpdateThesaurusRequestRequestTypeDef, _OptionalUpdateThesaurusRequestRequestTypeDef
 ):
     pass
 
-
 AssociateEntitiesToExperienceRequestRequestTypeDef = TypedDict(
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
         "EntityList": Sequence[EntityConfigurationTypeDef],
     },
@@ -2350,29 +3122,37 @@
         "Personas": Sequence[EntityPersonaConfigurationTypeDef],
     },
 )
 
 AttributeSuggestionsDescribeConfigTypeDef = TypedDict(
     "AttributeSuggestionsDescribeConfigTypeDef",
     {
-        "SuggestableConfigList": List[SuggestableConfigTypeDef],
+        "SuggestableConfigList": List[SuggestableConfigOutputTypeDef],
         "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
     total=False,
 )
 
 AttributeSuggestionsUpdateConfigTypeDef = TypedDict(
     "AttributeSuggestionsUpdateConfigTypeDef",
     {
         "SuggestableConfigList": Sequence[SuggestableConfigTypeDef],
         "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
     total=False,
 )
 
+AuthenticationConfigurationOutputTypeDef = TypedDict(
+    "AuthenticationConfigurationOutputTypeDef",
+    {
+        "BasicAuthentication": List[BasicAuthenticationConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "BasicAuthentication": Sequence[BasicAuthenticationConfigurationTypeDef],
     },
     total=False,
 )
@@ -2388,22 +3168,20 @@
     "_OptionalBatchDeleteDocumentRequestRequestTypeDef",
     {
         "DataSourceSyncJobMetricTarget": DataSourceSyncJobMetricTargetTypeDef,
     },
     total=False,
 )
 
-
 class BatchDeleteDocumentRequestRequestTypeDef(
     _RequiredBatchDeleteDocumentRequestRequestTypeDef,
     _OptionalBatchDeleteDocumentRequestRequestTypeDef,
 ):
     pass
 
-
 BatchDeleteDocumentResponseTypeDef = TypedDict(
     "BatchDeleteDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchDeleteDocumentResponseFailedDocumentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2429,31 +3207,79 @@
     "BatchPutDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchPutDocumentResponseFailedDocumentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConfluenceAttachmentConfigurationOutputTypeDef = TypedDict(
+    "ConfluenceAttachmentConfigurationOutputTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 ConfluenceAttachmentConfigurationTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationTypeDef",
     {
         "CrawlAttachments": bool,
         "AttachmentFieldMappings": Sequence[ConfluenceAttachmentToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+ConfluenceBlogConfigurationOutputTypeDef = TypedDict(
+    "ConfluenceBlogConfigurationOutputTypeDef",
+    {
+        "BlogFieldMappings": List[ConfluenceBlogToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 ConfluenceBlogConfigurationTypeDef = TypedDict(
     "ConfluenceBlogConfigurationTypeDef",
     {
         "BlogFieldMappings": Sequence[ConfluenceBlogToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+_RequiredSharePointConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSharePointConfigurationOutputTypeDef",
+    {
+        "SharePointVersion": SharePointVersionType,
+        "Urls": List[str],
+        "SecretArn": str,
+    },
+)
+_OptionalSharePointConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSharePointConfigurationOutputTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "UseChangeLog": bool,
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "DocumentTitleFieldName": str,
+        "DisableLocalGroups": bool,
+        "SslCertificateS3Path": S3PathOutputTypeDef,
+        "AuthenticationType": SharePointOnlineAuthenticationTypeType,
+        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class SharePointConfigurationOutputTypeDef(
+    _RequiredSharePointConfigurationOutputTypeDef, _OptionalSharePointConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredSharePointConfigurationTypeDef = TypedDict(
     "_RequiredSharePointConfigurationTypeDef",
     {
         "SharePointVersion": SharePointVersionType,
         "Urls": Sequence[str],
         "SecretArn": str,
     },
@@ -2472,29 +3298,47 @@
         "SslCertificateS3Path": S3PathTypeDef,
         "AuthenticationType": SharePointOnlineAuthenticationTypeType,
         "ProxyConfiguration": ProxyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SharePointConfigurationTypeDef(
     _RequiredSharePointConfigurationTypeDef, _OptionalSharePointConfigurationTypeDef
 ):
     pass
 
+ConfluencePageConfigurationOutputTypeDef = TypedDict(
+    "ConfluencePageConfigurationOutputTypeDef",
+    {
+        "PageFieldMappings": List[ConfluencePageToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
 
 ConfluencePageConfigurationTypeDef = TypedDict(
     "ConfluencePageConfigurationTypeDef",
     {
         "PageFieldMappings": Sequence[ConfluencePageToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+ConfluenceSpaceConfigurationOutputTypeDef = TypedDict(
+    "ConfluenceSpaceConfigurationOutputTypeDef",
+    {
+        "CrawlPersonalSpaces": bool,
+        "CrawlArchivedSpaces": bool,
+        "IncludeSpaces": List[str],
+        "ExcludeSpaces": List[str],
+        "SpaceFieldMappings": List[ConfluenceSpaceToIndexFieldMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 ConfluenceSpaceConfigurationTypeDef = TypedDict(
     "ConfluenceSpaceConfigurationTypeDef",
     {
         "CrawlPersonalSpaces": bool,
         "CrawlArchivedSpaces": bool,
         "IncludeSpaces": Sequence[str],
         "ExcludeSpaces": Sequence[str],
@@ -2536,21 +3380,19 @@
         "FileFormat": FaqFileFormatType,
         "ClientToken": str,
         "LanguageCode": str,
     },
     total=False,
 )
 
-
 class CreateFaqRequestRequestTypeDef(
     _RequiredCreateFaqRequestRequestTypeDef, _OptionalCreateFaqRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
         "SourceS3Path": S3PathTypeDef,
         "RoleArn": str,
@@ -2562,22 +3404,20 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateQuerySuggestionsBlockListRequestRequestTypeDef(
     _RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef,
     _OptionalCreateQuerySuggestionsBlockListRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateThesaurusRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThesaurusRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
         "RoleArn": str,
         "SourceS3Path": S3PathTypeDef,
@@ -2589,29 +3429,19 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateThesaurusRequestRequestTypeDef(
     _RequiredCreateThesaurusRequestRequestTypeDef, _OptionalCreateThesaurusRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2632,37 +3462,20 @@
         "QueryTexts": Sequence[str],
         "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFeaturedResultsSetRequestRequestTypeDef(
     _RequiredCreateFeaturedResultsSetRequestRequestTypeDef,
     _OptionalCreateFeaturedResultsSetRequestRequestTypeDef,
 ):
     pass
 
-
-FeaturedResultsSetTypeDef = TypedDict(
-    "FeaturedResultsSetTypeDef",
-    {
-        "FeaturedResultsSetId": str,
-        "FeaturedResultsSetName": str,
-        "Description": str,
-        "Status": FeaturedResultsSetStatusType,
-        "QueryTexts": List[str],
-        "FeaturedDocuments": List[FeaturedDocumentTypeDef],
-        "LastUpdatedTimestamp": int,
-        "CreationTimestamp": int,
-    },
-    total=False,
-)
-
 _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFeaturedResultsSetRequestRequestTypeDef",
     {
         "IndexId": str,
         "FeaturedResultsSetId": str,
     },
 )
@@ -2674,22 +3487,20 @@
         "Status": FeaturedResultsSetStatusType,
         "QueryTexts": Sequence[str],
         "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
     },
     total=False,
 )
 
-
 class UpdateFeaturedResultsSetRequestRequestTypeDef(
     _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef,
     _OptionalUpdateFeaturedResultsSetRequestRequestTypeDef,
 ):
     pass
 
-
 UserContextTypeDef = TypedDict(
     "UserContextTypeDef",
     {
         "Token": str,
         "UserId": str,
         "Groups": Sequence[str],
         "DataSourceGroups": Sequence[DataSourceGroupTypeDef],
@@ -2717,14 +3528,21 @@
         "ErrorCode": ErrorCodeType,
         "DataSourceErrorCode": str,
         "Metrics": DataSourceSyncJobMetricsTypeDef,
     },
     total=False,
 )
 
+HierarchicalPrincipalOutputTypeDef = TypedDict(
+    "HierarchicalPrincipalOutputTypeDef",
+    {
+        "PrincipalList": List[PrincipalOutputTypeDef],
+    },
+)
+
 ExperiencesSummaryTypeDef = TypedDict(
     "ExperiencesSummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "CreatedAt": datetime,
         "Status": ExperienceStatusType,
@@ -2756,14 +3574,63 @@
         "DataSourceId": str,
         "GroupId": str,
         "GroupOrderingIdSummaries": List[GroupOrderingIdSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDocumentAttributeConditionOutputTypeDef = TypedDict(
+    "_RequiredDocumentAttributeConditionOutputTypeDef",
+    {
+        "ConditionDocumentAttributeKey": str,
+        "Operator": ConditionOperatorType,
+    },
+)
+_OptionalDocumentAttributeConditionOutputTypeDef = TypedDict(
+    "_OptionalDocumentAttributeConditionOutputTypeDef",
+    {
+        "ConditionOnValue": DocumentAttributeValueOutputTypeDef,
+    },
+    total=False,
+)
+
+class DocumentAttributeConditionOutputTypeDef(
+    _RequiredDocumentAttributeConditionOutputTypeDef,
+    _OptionalDocumentAttributeConditionOutputTypeDef,
+):
+    pass
+
+DocumentAttributeOutputTypeDef = TypedDict(
+    "DocumentAttributeOutputTypeDef",
+    {
+        "Key": str,
+        "Value": DocumentAttributeValueOutputTypeDef,
+    },
+)
+
+DocumentAttributeTargetOutputTypeDef = TypedDict(
+    "DocumentAttributeTargetOutputTypeDef",
+    {
+        "TargetDocumentAttributeKey": str,
+        "TargetDocumentAttributeValueDeletion": bool,
+        "TargetDocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
+    },
+    total=False,
+)
+
+DocumentAttributeValueCountPairTypeDef = TypedDict(
+    "DocumentAttributeValueCountPairTypeDef",
+    {
+        "DocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
+        "Count": int,
+        "FacetResults": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 _RequiredDocumentAttributeConditionTypeDef = TypedDict(
     "_RequiredDocumentAttributeConditionTypeDef",
     {
         "ConditionDocumentAttributeKey": str,
         "Operator": ConditionOperatorType,
     },
 )
@@ -2771,21 +3638,19 @@
     "_OptionalDocumentAttributeConditionTypeDef",
     {
         "ConditionOnValue": DocumentAttributeValueTypeDef,
     },
     total=False,
 )
 
-
 class DocumentAttributeConditionTypeDef(
     _RequiredDocumentAttributeConditionTypeDef, _OptionalDocumentAttributeConditionTypeDef
 ):
     pass
 
-
 DocumentAttributeTargetTypeDef = TypedDict(
     "DocumentAttributeTargetTypeDef",
     {
         "TargetDocumentAttributeKey": str,
         "TargetDocumentAttributeValueDeletion": bool,
         "TargetDocumentAttributeValue": DocumentAttributeValueTypeDef,
     },
@@ -2796,24 +3661,36 @@
     "DocumentAttributeTypeDef",
     {
         "Key": str,
         "Value": DocumentAttributeValueTypeDef,
     },
 )
 
-DocumentAttributeValueCountPairTypeDef = TypedDict(
-    "DocumentAttributeValueCountPairTypeDef",
+_RequiredDocumentMetadataConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDocumentMetadataConfigurationOutputTypeDef",
     {
-        "DocumentAttributeValue": DocumentAttributeValueTypeDef,
-        "Count": int,
-        "FacetResults": List[Dict[str, Any]],
+        "Name": str,
+        "Type": DocumentAttributeValueTypeType,
+    },
+)
+_OptionalDocumentMetadataConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDocumentMetadataConfigurationOutputTypeDef",
+    {
+        "Relevance": RelevanceOutputTypeDef,
+        "Search": SearchOutputTypeDef,
     },
     total=False,
 )
 
+class DocumentMetadataConfigurationOutputTypeDef(
+    _RequiredDocumentMetadataConfigurationOutputTypeDef,
+    _OptionalDocumentMetadataConfigurationOutputTypeDef,
+):
+    pass
+
 DocumentRelevanceConfigurationTypeDef = TypedDict(
     "DocumentRelevanceConfigurationTypeDef",
     {
         "Name": str,
         "Relevance": RelevanceTypeDef,
     },
 )
@@ -2830,20 +3707,41 @@
     {
         "Relevance": RelevanceTypeDef,
         "Search": SearchTypeDef,
     },
     total=False,
 )
 
-
 class DocumentMetadataConfigurationTypeDef(
     _RequiredDocumentMetadataConfigurationTypeDef, _OptionalDocumentMetadataConfigurationTypeDef
 ):
     pass
 
+_RequiredS3DataSourceConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3DataSourceConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+    },
+)
+_OptionalS3DataSourceConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3DataSourceConfigurationOutputTypeDef",
+    {
+        "InclusionPrefixes": List[str],
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationOutputTypeDef,
+        "AccessControlListConfiguration": AccessControlListConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3DataSourceConfigurationOutputTypeDef(
+    _RequiredS3DataSourceConfigurationOutputTypeDef, _OptionalS3DataSourceConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredS3DataSourceConfigurationTypeDef = TypedDict(
     "_RequiredS3DataSourceConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
@@ -2855,31 +3753,38 @@
         "ExclusionPatterns": Sequence[str],
         "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationTypeDef,
         "AccessControlListConfiguration": AccessControlListConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class S3DataSourceConfigurationTypeDef(
     _RequiredS3DataSourceConfigurationTypeDef, _OptionalS3DataSourceConfigurationTypeDef
 ):
     pass
 
-
 ExperienceEntitiesSummaryTypeDef = TypedDict(
     "ExperienceEntitiesSummaryTypeDef",
     {
         "EntityId": str,
         "EntityType": EntityTypeType,
         "DisplayData": EntityDisplayDataTypeDef,
     },
     total=False,
 )
 
+ExperienceConfigurationOutputTypeDef = TypedDict(
+    "ExperienceConfigurationOutputTypeDef",
+    {
+        "ContentSourceConfiguration": ContentSourceConfigurationOutputTypeDef,
+        "UserIdentityConfiguration": UserIdentityConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ExperienceConfigurationTypeDef = TypedDict(
     "ExperienceConfigurationTypeDef",
     {
         "ContentSourceConfiguration": ContentSourceConfigurationTypeDef,
         "UserIdentityConfiguration": UserIdentityConfigurationTypeDef,
     },
     total=False,
@@ -2890,60 +3795,49 @@
     {
         "NextToken": str,
         "FaqSummaryItems": List[FaqSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FeaturedResultsSetTypeDef = TypedDict(
+    "FeaturedResultsSetTypeDef",
+    {
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": List[str],
+        "FeaturedDocuments": List[FeaturedDocumentOutputTypeDef],
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
+    },
+    total=False,
+)
+
 ListFeaturedResultsSetsResponseTypeDef = TypedDict(
     "ListFeaturedResultsSetsResponseTypeDef",
     {
         "FeaturedResultsSetSummaryItems": List[FeaturedResultsSetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSnapshotsResponseTypeDef = TypedDict(
     "GetSnapshotsResponseTypeDef",
     {
-        "SnapShotTimeFilter": TimeRangeTypeDef,
+        "SnapShotTimeFilter": TimeRangeOutputTypeDef,
         "SnapshotsDataHeader": List[str],
         "SnapshotsData": List[List[str]],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-    },
-)
-_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTimeFilter": TimeRangeTypeDef,
-        "StatusFilter": DataSourceSyncJobStatusType,
-    },
-    total=False,
-)
-
-
-class ListDataSourceSyncJobsRequestRequestTypeDef(
-    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
-    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
-):
-    pass
-
-
 GroupMembersTypeDef = TypedDict(
     "GroupMembersTypeDef",
     {
         "MemberGroups": Sequence[MemberGroupTypeDef],
         "MemberUsers": Sequence[MemberUserTypeDef],
         "S3PathforGroupMembers": S3PathTypeDef,
     },
@@ -2981,23 +3875,56 @@
     "IndexStatisticsTypeDef",
     {
         "FaqStatistics": FaqStatisticsTypeDef,
         "TextDocumentStatistics": TextDocumentStatisticsTypeDef,
     },
 )
 
+UserTokenConfigurationOutputTypeDef = TypedDict(
+    "UserTokenConfigurationOutputTypeDef",
+    {
+        "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationOutputTypeDef,
+        "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 UserTokenConfigurationTypeDef = TypedDict(
     "UserTokenConfigurationTypeDef",
     {
         "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationTypeDef,
         "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+    },
+)
+_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTimeFilter": TimeRangeTypeDef,
+        "StatusFilter": DataSourceSyncJobStatusType,
+    },
+    total=False,
+)
+
+class ListDataSourceSyncJobsRequestRequestTypeDef(
+    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
+    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
+):
+    pass
+
 ListEntityPersonasResponseTypeDef = TypedDict(
     "ListEntityPersonasResponseTypeDef",
     {
         "SummaryItems": List[PersonasSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3008,14 +3935,22 @@
     {
         "BlockListSummaryItems": List[QuerySuggestionsBlockListSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListThesauriResponseTypeDef = TypedDict(
     "ListThesauriResponseTypeDef",
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3033,20 +3968,27 @@
     {
         "ClickFeedbackItems": Sequence[ClickFeedbackTypeDef],
         "RelevanceFeedbackItems": Sequence[RelevanceFeedbackTypeDef],
     },
     total=False,
 )
 
-
 class SubmitFeedbackRequestRequestTypeDef(
     _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
 ):
     pass
 
+UrlsOutputTypeDef = TypedDict(
+    "UrlsOutputTypeDef",
+    {
+        "SeedUrlConfiguration": SeedUrlConfigurationOutputTypeDef,
+        "SiteMapsConfiguration": SiteMapsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
 
 UrlsTypeDef = TypedDict(
     "UrlsTypeDef",
     {
         "SeedUrlConfiguration": SeedUrlConfigurationTypeDef,
         "SiteMapsConfiguration": SiteMapsConfigurationTypeDef,
     },
@@ -3066,14 +4008,162 @@
     "TableRowTypeDef",
     {
         "Cells": List[TableCellTypeDef],
     },
     total=False,
 )
 
+_RequiredDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDatabaseConfigurationOutputTypeDef",
+    {
+        "DatabaseEngineType": DatabaseEngineTypeType,
+        "ConnectionConfiguration": ConnectionConfigurationOutputTypeDef,
+        "ColumnConfiguration": ColumnConfigurationOutputTypeDef,
+    },
+)
+_OptionalDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDatabaseConfigurationOutputTypeDef",
+    {
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "AclConfiguration": AclConfigurationOutputTypeDef,
+        "SqlConfiguration": SqlConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class DatabaseConfigurationOutputTypeDef(
+    _RequiredDatabaseConfigurationOutputTypeDef, _OptionalDatabaseConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef",
+    {
+        "IncludedStates": List[SalesforceKnowledgeArticleStateType],
+    },
+)
+_OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef",
+    {
+        "StandardKnowledgeArticleTypeConfiguration": (
+            SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef
+        ),
+        "CustomKnowledgeArticleTypeConfigurations": List[
+            SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef
+        ],
+    },
+    total=False,
+)
+
+class SalesforceKnowledgeArticleConfigurationOutputTypeDef(
+    _RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef,
+    _OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredServiceNowConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceNowConfigurationOutputTypeDef",
+    {
+        "HostUrl": str,
+        "SecretArn": str,
+        "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
+    },
+)
+_OptionalServiceNowConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceNowConfigurationOutputTypeDef",
+    {
+        "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
+        "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationOutputTypeDef,
+        "AuthenticationType": ServiceNowAuthenticationTypeType,
+    },
+    total=False,
+)
+
+class ServiceNowConfigurationOutputTypeDef(
+    _RequiredServiceNowConfigurationOutputTypeDef, _OptionalServiceNowConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredGitHubConfigurationOutputTypeDef = TypedDict(
+    "_RequiredGitHubConfigurationOutputTypeDef",
+    {
+        "SecretArn": str,
+    },
+)
+_OptionalGitHubConfigurationOutputTypeDef = TypedDict(
+    "_OptionalGitHubConfigurationOutputTypeDef",
+    {
+        "SaaSConfiguration": SaaSConfigurationOutputTypeDef,
+        "OnPremiseConfiguration": OnPremiseConfigurationOutputTypeDef,
+        "Type": TypeType,
+        "UseChangeLog": bool,
+        "GitHubDocumentCrawlProperties": GitHubDocumentCrawlPropertiesOutputTypeDef,
+        "RepositoryFilter": List[str],
+        "InclusionFolderNamePatterns": List[str],
+        "InclusionFileTypePatterns": List[str],
+        "InclusionFileNamePatterns": List[str],
+        "ExclusionFolderNamePatterns": List[str],
+        "ExclusionFileTypePatterns": List[str],
+        "ExclusionFileNamePatterns": List[str],
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "GitHubRepositoryConfigurationFieldMappings": List[
+            DataSourceToIndexFieldMappingOutputTypeDef
+        ],
+        "GitHubCommitConfigurationFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "GitHubIssueDocumentConfigurationFieldMappings": List[
+            DataSourceToIndexFieldMappingOutputTypeDef
+        ],
+        "GitHubIssueCommentConfigurationFieldMappings": List[
+            DataSourceToIndexFieldMappingOutputTypeDef
+        ],
+        "GitHubIssueAttachmentConfigurationFieldMappings": List[
+            DataSourceToIndexFieldMappingOutputTypeDef
+        ],
+        "GitHubPullRequestCommentConfigurationFieldMappings": List[
+            DataSourceToIndexFieldMappingOutputTypeDef
+        ],
+        "GitHubPullRequestDocumentConfigurationFieldMappings": List[
+            DataSourceToIndexFieldMappingOutputTypeDef
+        ],
+        "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": List[
+            DataSourceToIndexFieldMappingOutputTypeDef
+        ],
+    },
+    total=False,
+)
+
+class GitHubConfigurationOutputTypeDef(
+    _RequiredGitHubConfigurationOutputTypeDef, _OptionalGitHubConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredOneDriveConfigurationOutputTypeDef = TypedDict(
+    "_RequiredOneDriveConfigurationOutputTypeDef",
+    {
+        "TenantDomain": str,
+        "SecretArn": str,
+        "OneDriveUsers": OneDriveUsersOutputTypeDef,
+    },
+)
+_OptionalOneDriveConfigurationOutputTypeDef = TypedDict(
+    "_OptionalOneDriveConfigurationOutputTypeDef",
+    {
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "DisableLocalGroups": bool,
+    },
+    total=False,
+)
+
+class OneDriveConfigurationOutputTypeDef(
+    _RequiredOneDriveConfigurationOutputTypeDef, _OptionalOneDriveConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredDatabaseConfigurationTypeDef",
     {
         "DatabaseEngineType": DatabaseEngineTypeType,
         "ConnectionConfiguration": ConnectionConfigurationTypeDef,
         "ColumnConfiguration": ColumnConfigurationTypeDef,
     },
@@ -3084,21 +4174,19 @@
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
         "AclConfiguration": AclConfigurationTypeDef,
         "SqlConfiguration": SqlConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseConfigurationTypeDef(
     _RequiredDatabaseConfigurationTypeDef, _OptionalDatabaseConfigurationTypeDef
 ):
     pass
 
-
 _RequiredSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceKnowledgeArticleConfigurationTypeDef",
     {
         "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
     },
 )
 _OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
@@ -3110,22 +4198,20 @@
         "CustomKnowledgeArticleTypeConfigurations": Sequence[
             SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef
         ],
     },
     total=False,
 )
 
-
 class SalesforceKnowledgeArticleConfigurationTypeDef(
     _RequiredSalesforceKnowledgeArticleConfigurationTypeDef,
     _OptionalSalesforceKnowledgeArticleConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredServiceNowConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowConfigurationTypeDef",
     {
         "HostUrl": str,
         "SecretArn": str,
         "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
     },
@@ -3136,21 +4222,19 @@
         "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationTypeDef,
         "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationTypeDef,
         "AuthenticationType": ServiceNowAuthenticationTypeType,
     },
     total=False,
 )
 
-
 class ServiceNowConfigurationTypeDef(
     _RequiredServiceNowConfigurationTypeDef, _OptionalServiceNowConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGitHubConfigurationTypeDef = TypedDict(
     "_RequiredGitHubConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGitHubConfigurationTypeDef = TypedDict(
@@ -3191,21 +4275,19 @@
         "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": Sequence[
             DataSourceToIndexFieldMappingTypeDef
         ],
     },
     total=False,
 )
 
-
 class GitHubConfigurationTypeDef(
     _RequiredGitHubConfigurationTypeDef, _OptionalGitHubConfigurationTypeDef
 ):
     pass
 
-
 _RequiredOneDriveConfigurationTypeDef = TypedDict(
     "_RequiredOneDriveConfigurationTypeDef",
     {
         "TenantDomain": str,
         "SecretArn": str,
         "OneDriveUsers": OneDriveUsersTypeDef,
     },
@@ -3217,21 +4299,19 @@
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
         "DisableLocalGroups": bool,
     },
     total=False,
 )
 
-
 class OneDriveConfigurationTypeDef(
     _RequiredOneDriveConfigurationTypeDef, _OptionalOneDriveConfigurationTypeDef
 ):
     pass
 
-
 DescribeQuerySuggestionsConfigResponseTypeDef = TypedDict(
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     {
         "Mode": ModeType,
         "Status": QuerySuggestionsStatusType,
         "QueryLogLookBackWindowInDays": int,
         "IncludeQueriesWithoutUserInformation": bool,
@@ -3260,21 +4340,48 @@
         "MinimumNumberOfQueryingUsers": int,
         "MinimumQueryCount": int,
         "AttributeSuggestionsConfig": AttributeSuggestionsUpdateConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
     _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
     _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
 ):
     pass
 
+_RequiredConfluenceConfigurationOutputTypeDef = TypedDict(
+    "_RequiredConfluenceConfigurationOutputTypeDef",
+    {
+        "ServerUrl": str,
+        "SecretArn": str,
+        "Version": ConfluenceVersionType,
+    },
+)
+_OptionalConfluenceConfigurationOutputTypeDef = TypedDict(
+    "_OptionalConfluenceConfigurationOutputTypeDef",
+    {
+        "SpaceConfiguration": ConfluenceSpaceConfigurationOutputTypeDef,
+        "PageConfiguration": ConfluencePageConfigurationOutputTypeDef,
+        "BlogConfiguration": ConfluenceBlogConfigurationOutputTypeDef,
+        "AttachmentConfiguration": ConfluenceAttachmentConfigurationOutputTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "AuthenticationType": ConfluenceAuthenticationTypeType,
+    },
+    total=False,
+)
+
+class ConfluenceConfigurationOutputTypeDef(
+    _RequiredConfluenceConfigurationOutputTypeDef, _OptionalConfluenceConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredConfluenceConfigurationTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
@@ -3292,21 +4399,19 @@
         "ExclusionPatterns": Sequence[str],
         "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationType": ConfluenceAuthenticationTypeType,
     },
     total=False,
 )
 
-
 class ConfluenceConfigurationTypeDef(
     _RequiredConfluenceConfigurationTypeDef, _OptionalConfluenceConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
     },
 )
@@ -3317,34 +4422,20 @@
         "AccessControlList": Sequence[PrincipalTypeDef],
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
-    "DescribeAccessControlConfigurationResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "ErrorMessage": str,
-        "AccessControlList": List[PrincipalTypeDef],
-        "HierarchicalAccessControlList": List[HierarchicalPrincipalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
@@ -3355,38 +4446,20 @@
         "Description": str,
         "AccessControlList": Sequence[PrincipalTypeDef],
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
     },
     total=False,
 )
 
-
 class UpdateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-CreateFeaturedResultsSetResponseTypeDef = TypedDict(
-    "CreateFeaturedResultsSetResponseTypeDef",
-    {
-        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
-    "UpdateFeaturedResultsSetResponseTypeDef",
-    {
-        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeSuggestionsGetConfigTypeDef = TypedDict(
     "AttributeSuggestionsGetConfigTypeDef",
     {
         "SuggestionAttributes": Sequence[str],
         "AdditionalResponseAttributes": Sequence[str],
         "AttributeFilter": "AttributeFilterTypeDef",
         "UserContext": UserContextTypeDef,
@@ -3399,23 +4472,88 @@
     {
         "History": List[DataSourceSyncJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccessControlConfigurationResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "ErrorMessage": str,
+        "AccessControlList": List[PrincipalOutputTypeDef],
+        "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListExperiencesResponseTypeDef = TypedDict(
     "ListExperiencesResponseTypeDef",
     {
         "SummaryItems": List[ExperiencesSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredHookConfigurationOutputTypeDef = TypedDict(
+    "_RequiredHookConfigurationOutputTypeDef",
+    {
+        "LambdaArn": str,
+        "S3Bucket": str,
+    },
+)
+_OptionalHookConfigurationOutputTypeDef = TypedDict(
+    "_OptionalHookConfigurationOutputTypeDef",
+    {
+        "InvocationCondition": DocumentAttributeConditionOutputTypeDef,
+    },
+    total=False,
+)
+
+class HookConfigurationOutputTypeDef(
+    _RequiredHookConfigurationOutputTypeDef, _OptionalHookConfigurationOutputTypeDef
+):
+    pass
+
+RetrieveResultItemTypeDef = TypedDict(
+    "RetrieveResultItemTypeDef",
+    {
+        "Id": str,
+        "DocumentId": str,
+        "DocumentTitle": str,
+        "Content": str,
+        "DocumentURI": str,
+        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
+SourceDocumentTypeDef = TypedDict(
+    "SourceDocumentTypeDef",
+    {
+        "DocumentId": str,
+        "SuggestionAttributes": List[str],
+        "AdditionalAttributes": List[DocumentAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
+InlineCustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
+    "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
+    {
+        "Condition": DocumentAttributeConditionOutputTypeDef,
+        "Target": DocumentAttributeTargetOutputTypeDef,
+        "DocumentContentDeletion": bool,
+    },
+    total=False,
+)
+
 _RequiredHookConfigurationTypeDef = TypedDict(
     "_RequiredHookConfigurationTypeDef",
     {
         "LambdaArn": str,
         "S3Bucket": str,
     },
 )
@@ -3423,21 +4561,19 @@
     "_OptionalHookConfigurationTypeDef",
     {
         "InvocationCondition": DocumentAttributeConditionTypeDef,
     },
     total=False,
 )
 
-
 class HookConfigurationTypeDef(
     _RequiredHookConfigurationTypeDef, _OptionalHookConfigurationTypeDef
 ):
     pass
 
-
 InlineCustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     {
         "Condition": DocumentAttributeConditionTypeDef,
         "Target": DocumentAttributeTargetTypeDef,
         "DocumentContentDeletion": bool,
     },
@@ -3471,19 +4607,17 @@
     "_OptionalDocumentInfoTypeDef",
     {
         "Attributes": Sequence[DocumentAttributeTypeDef],
     },
     total=False,
 )
 
-
 class DocumentInfoTypeDef(_RequiredDocumentInfoTypeDef, _OptionalDocumentInfoTypeDef):
     pass
 
-
 _RequiredDocumentTypeDef = TypedDict(
     "_RequiredDocumentTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDocumentTypeDef = TypedDict(
@@ -3497,42 +4631,17 @@
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
         "ContentType": ContentTypeType,
         "AccessControlConfigurationId": str,
     },
     total=False,
 )
 
-
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
-
-RetrieveResultItemTypeDef = TypedDict(
-    "RetrieveResultItemTypeDef",
-    {
-        "Id": str,
-        "DocumentId": str,
-        "DocumentTitle": str,
-        "Content": str,
-        "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeTypeDef],
-    },
-    total=False,
-)
-
-SourceDocumentTypeDef = TypedDict(
-    "SourceDocumentTypeDef",
-    {
-        "DocumentId": str,
-        "SuggestionAttributes": List[str],
-        "AdditionalAttributes": List[DocumentAttributeTypeDef],
-    },
-    total=False,
-)
-
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -3550,21 +4659,19 @@
         "UserContext": UserContextTypeDef,
         "VisitorId": str,
         "SpellCorrectionConfiguration": SpellCorrectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredRetrieveRequestRequestTypeDef = TypedDict(
     "_RequiredRetrieveRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -3577,30 +4684,46 @@
         "PageNumber": int,
         "PageSize": int,
         "UserContext": UserContextTypeDef,
     },
     total=False,
 )
 
-
 class RetrieveRequestRequestTypeDef(
     _RequiredRetrieveRequestRequestTypeDef, _OptionalRetrieveRequestRequestTypeDef
 ):
     pass
 
-
 ListExperienceEntitiesResponseTypeDef = TypedDict(
     "ListExperienceEntitiesResponseTypeDef",
     {
         "SummaryItems": List[ExperienceEntitiesSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeExperienceResponseTypeDef = TypedDict(
+    "DescribeExperienceResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Endpoints": List[ExperienceEndpointTypeDef],
+        "Configuration": ExperienceConfigurationOutputTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Description": str,
+        "Status": ExperienceStatusType,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperienceRequestRequestTypeDef",
     {
         "Name": str,
         "IndexId": str,
     },
 )
@@ -3611,39 +4734,19 @@
         "Configuration": ExperienceConfigurationTypeDef,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateExperienceRequestRequestTypeDef(
     _RequiredCreateExperienceRequestRequestTypeDef, _OptionalCreateExperienceRequestRequestTypeDef
 ):
     pass
 
-
-DescribeExperienceResponseTypeDef = TypedDict(
-    "DescribeExperienceResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Endpoints": List[ExperienceEndpointTypeDef],
-        "Configuration": ExperienceConfigurationTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Description": str,
-        "Status": ExperienceStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -3654,20 +4757,34 @@
         "RoleArn": str,
         "Configuration": ExperienceConfigurationTypeDef,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateExperienceRequestRequestTypeDef(
     _RequiredUpdateExperienceRequestRequestTypeDef, _OptionalUpdateExperienceRequestRequestTypeDef
 ):
     pass
 
+CreateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "CreateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "UpdateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredPutPrincipalMappingRequestRequestTypeDef = TypedDict(
     "_RequiredPutPrincipalMappingRequestRequestTypeDef",
     {
         "IndexId": str,
         "GroupId": str,
         "GroupMembers": GroupMembersTypeDef,
@@ -3679,30 +4796,51 @@
         "DataSourceId": str,
         "OrderingId": int,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class PutPrincipalMappingRequestRequestTypeDef(
     _RequiredPutPrincipalMappingRequestRequestTypeDef,
     _OptionalPutPrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
-
 AdditionalResultAttributeValueTypeDef = TypedDict(
     "AdditionalResultAttributeValueTypeDef",
     {
         "TextWithHighlightsValue": TextWithHighlightsTypeDef,
     },
     total=False,
 )
 
+DescribeIndexResponseTypeDef = TypedDict(
+    "DescribeIndexResponseTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Edition": IndexEditionType,
+        "RoleArn": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "Status": IndexStatusType,
+        "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationOutputTypeDef],
+        "IndexStatistics": IndexStatisticsTypeDef,
+        "ErrorMessage": str,
+        "CapacityUnits": CapacityUnitsConfigurationOutputTypeDef,
+        "UserTokenConfigurations": List[UserTokenConfigurationOutputTypeDef],
+        "UserContextPolicy": UserContextPolicyType,
+        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIndexRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -3717,44 +4855,19 @@
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
-
-DescribeIndexResponseTypeDef = TypedDict(
-    "DescribeIndexResponseTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Edition": IndexEditionType,
-        "RoleArn": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "Status": IndexStatusType,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationTypeDef],
-        "IndexStatistics": IndexStatisticsTypeDef,
-        "ErrorMessage": str,
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
-        "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
-        "UserContextPolicy": UserContextPolicyType,
-        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
@@ -3768,20 +4881,44 @@
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateIndexRequestRequestTypeDef(
     _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
 ):
     pass
 
+_RequiredWebCrawlerConfigurationOutputTypeDef = TypedDict(
+    "_RequiredWebCrawlerConfigurationOutputTypeDef",
+    {
+        "Urls": UrlsOutputTypeDef,
+    },
+)
+_OptionalWebCrawlerConfigurationOutputTypeDef = TypedDict(
+    "_OptionalWebCrawlerConfigurationOutputTypeDef",
+    {
+        "CrawlDepth": int,
+        "MaxLinksPerPage": int,
+        "MaxContentSizePerPageInMegaBytes": float,
+        "MaxUrlsPerMinuteCrawlRate": int,
+        "UrlInclusionPatterns": List[str],
+        "UrlExclusionPatterns": List[str],
+        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class WebCrawlerConfigurationOutputTypeDef(
+    _RequiredWebCrawlerConfigurationOutputTypeDef, _OptionalWebCrawlerConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredWebCrawlerConfigurationTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationTypeDef",
     {
         "Urls": UrlsTypeDef,
     },
 )
@@ -3796,21 +4933,19 @@
         "UrlExclusionPatterns": Sequence[str],
         "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class WebCrawlerConfigurationTypeDef(
     _RequiredWebCrawlerConfigurationTypeDef, _OptionalWebCrawlerConfigurationTypeDef
 ):
     pass
 
-
 SuggestionValueTypeDef = TypedDict(
     "SuggestionValueTypeDef",
     {
         "Text": SuggestionTextWithHighlightsTypeDef,
     },
     total=False,
 )
@@ -3820,14 +4955,42 @@
     {
         "Rows": List[TableRowTypeDef],
         "TotalNumberOfRows": int,
     },
     total=False,
 )
 
+_RequiredSalesforceConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSalesforceConfigurationOutputTypeDef",
+    {
+        "ServerUrl": str,
+        "SecretArn": str,
+    },
+)
+_OptionalSalesforceConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSalesforceConfigurationOutputTypeDef",
+    {
+        "StandardObjectConfigurations": List[SalesforceStandardObjectConfigurationOutputTypeDef],
+        "KnowledgeArticleConfiguration": SalesforceKnowledgeArticleConfigurationOutputTypeDef,
+        "ChatterFeedConfiguration": SalesforceChatterFeedConfigurationOutputTypeDef,
+        "CrawlAttachments": bool,
+        "StandardObjectAttachmentConfiguration": (
+            SalesforceStandardObjectAttachmentConfigurationOutputTypeDef
+        ),
+        "IncludeAttachmentFilePatterns": List[str],
+        "ExcludeAttachmentFilePatterns": List[str],
+    },
+    total=False,
+)
+
+class SalesforceConfigurationOutputTypeDef(
+    _RequiredSalesforceConfigurationOutputTypeDef, _OptionalSalesforceConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredSalesforceConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
     },
 )
@@ -3843,21 +5006,19 @@
         ),
         "IncludeAttachmentFilePatterns": Sequence[str],
         "ExcludeAttachmentFilePatterns": Sequence[str],
     },
     total=False,
 )
 
-
 class SalesforceConfigurationTypeDef(
     _RequiredSalesforceConfigurationTypeDef, _OptionalSalesforceConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -3867,21 +5028,39 @@
         "MaxSuggestionsCount": int,
         "SuggestionTypes": Sequence[SuggestionTypeType],
         "AttributeSuggestionsConfig": AttributeSuggestionsGetConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetQuerySuggestionsRequestRequestTypeDef(
     _RequiredGetQuerySuggestionsRequestRequestTypeDef,
     _OptionalGetQuerySuggestionsRequestRequestTypeDef,
 ):
     pass
 
+RetrieveResultTypeDef = TypedDict(
+    "RetrieveResultTypeDef",
+    {
+        "QueryId": str,
+        "ResultItems": List[RetrieveResultItemTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
+    "CustomDocumentEnrichmentConfigurationOutputTypeDef",
+    {
+        "InlineConfigurations": List[InlineCustomDocumentEnrichmentConfigurationOutputTypeDef],
+        "PreExtractionHookConfiguration": HookConfigurationOutputTypeDef,
+        "PostExtractionHookConfiguration": HookConfigurationOutputTypeDef,
+        "RoleArn": str,
+    },
+    total=False,
+)
 
 CustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "CustomDocumentEnrichmentConfigurationTypeDef",
     {
         "InlineConfigurations": Sequence[InlineCustomDocumentEnrichmentConfigurationTypeDef],
         "PreExtractionHookConfiguration": HookConfigurationTypeDef,
         "PostExtractionHookConfiguration": HookConfigurationTypeDef,
@@ -3894,23 +5073,14 @@
     "BatchGetDocumentStatusRequestRequestTypeDef",
     {
         "IndexId": str,
         "DocumentInfoList": Sequence[DocumentInfoTypeDef],
     },
 )
 
-RetrieveResultTypeDef = TypedDict(
-    "RetrieveResultTypeDef",
-    {
-        "QueryId": str,
-        "ResultItems": List[RetrieveResultItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AdditionalResultAttributeTypeDef = TypedDict(
     "AdditionalResultAttributeTypeDef",
     {
         "Key": str,
         "ValueType": Literal["TEXT_WITH_HIGHLIGHTS_VALUE"],
         "Value": AdditionalResultAttributeValueTypeDef,
     },
@@ -3922,14 +5092,39 @@
         "Id": str,
         "Value": SuggestionValueTypeDef,
         "SourceDocuments": List[SourceDocumentTypeDef],
     },
     total=False,
 )
 
+DataSourceConfigurationOutputTypeDef = TypedDict(
+    "DataSourceConfigurationOutputTypeDef",
+    {
+        "S3Configuration": S3DataSourceConfigurationOutputTypeDef,
+        "SharePointConfiguration": SharePointConfigurationOutputTypeDef,
+        "DatabaseConfiguration": DatabaseConfigurationOutputTypeDef,
+        "SalesforceConfiguration": SalesforceConfigurationOutputTypeDef,
+        "OneDriveConfiguration": OneDriveConfigurationOutputTypeDef,
+        "ServiceNowConfiguration": ServiceNowConfigurationOutputTypeDef,
+        "ConfluenceConfiguration": ConfluenceConfigurationOutputTypeDef,
+        "GoogleDriveConfiguration": GoogleDriveConfigurationOutputTypeDef,
+        "WebCrawlerConfiguration": WebCrawlerConfigurationOutputTypeDef,
+        "WorkDocsConfiguration": WorkDocsConfigurationOutputTypeDef,
+        "FsxConfiguration": FsxConfigurationOutputTypeDef,
+        "SlackConfiguration": SlackConfigurationOutputTypeDef,
+        "BoxConfiguration": BoxConfigurationOutputTypeDef,
+        "QuipConfiguration": QuipConfigurationOutputTypeDef,
+        "JiraConfiguration": JiraConfigurationOutputTypeDef,
+        "GitHubConfiguration": GitHubConfigurationOutputTypeDef,
+        "AlfrescoConfiguration": AlfrescoConfigurationOutputTypeDef,
+        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "S3Configuration": S3DataSourceConfigurationTypeDef,
         "SharePointConfiguration": SharePointConfigurationTypeDef,
         "DatabaseConfiguration": DatabaseConfigurationTypeDef,
         "SalesforceConfiguration": SalesforceConfigurationTypeDef,
@@ -3963,32 +5158,30 @@
     {
         "RoleArn": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class BatchPutDocumentRequestRequestTypeDef(
     _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
 ):
     pass
 
-
 FeaturedResultsItemTypeDef = TypedDict(
     "FeaturedResultsItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
         "DocumentTitle": TextWithHighlightsTypeDef,
         "DocumentExcerpt": TextWithHighlightsTypeDef,
         "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeTypeDef],
+        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
         "FeedbackToken": str,
     },
     total=False,
 )
 
 QueryResultItemTypeDef = TypedDict(
     "QueryResultItemTypeDef",
@@ -3997,15 +5190,15 @@
         "Type": QueryResultTypeType,
         "Format": QueryResultFormatType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
         "DocumentTitle": TextWithHighlightsTypeDef,
         "DocumentExcerpt": TextWithHighlightsTypeDef,
         "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeTypeDef],
+        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
         "ScoreAttributes": ScoreAttributesTypeDef,
         "FeedbackToken": str,
         "TableExcerpt": TableExcerptTypeDef,
     },
     total=False,
 )
 
@@ -4014,14 +5207,36 @@
     {
         "QuerySuggestionsId": str,
         "Suggestions": List[SuggestionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeDataSourceResponseTypeDef = TypedDict(
+    "DescribeDataSourceResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Type": DataSourceTypeType,
+        "Configuration": DataSourceConfigurationOutputTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Description": str,
+        "Status": DataSourceStatusType,
+        "Schedule": str,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "LanguageCode": str,
+        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "Name": str,
         "IndexId": str,
         "Type": DataSourceTypeType,
     },
@@ -4038,43 +5253,19 @@
         "ClientToken": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
     pass
 
-
-DescribeDataSourceResponseTypeDef = TypedDict(
-    "DescribeDataSourceResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Type": DataSourceTypeType,
-        "Configuration": DataSourceConfigurationTypeDef,
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Description": str,
-        "Status": DataSourceStatusType,
-        "Schedule": str,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "LanguageCode": str,
-        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4089,21 +5280,19 @@
         "RoleArn": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDataSourceRequestRequestTypeDef(
     _RequiredUpdateDataSourceRequestRequestTypeDef, _OptionalUpdateDataSourceRequestRequestTypeDef
 ):
     pass
 
-
 QueryResultTypeDef = TypedDict(
     "QueryResultTypeDef",
     {
         "QueryId": str,
         "ResultItems": List[QueryResultItemTypeDef],
         "FacetResults": List["FacetResultTypeDef"],
         "TotalNumberOfResults": int,
```

### Comparing `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/SOURCES.txt` & `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.0/setup.py` & `mypy-boto3-kendra-1.28.12/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.kendra 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.kendra 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

