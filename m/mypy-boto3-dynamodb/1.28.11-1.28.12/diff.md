# Comparing `tmp/mypy-boto3-dynamodb-1.28.11.tar.gz` & `tmp/mypy-boto3-dynamodb-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.28.12.tar", last modified: Thu Jul 27 05:34:36 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.28.11.tar` & `mypy-boto3-dynamodb-1.28.12.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.853034 mypy-boto3-dynamodb-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-07-25 19:49:13.841034 mypy-boto3-dynamodb-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.841034 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   152329 2023-07-25 19:47:09.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   152192 2023-07-25 19:47:07.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-25 19:47:05.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.841034 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 19:49:13.000000 mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.853034 mypy-boto3-dynamodb-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 19:47:04.000000 mypy-boto3-dynamodb-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   158324 2023-07-27 05:20:41.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158157 2023-07-27 05:20:40.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.28.11/LICENSE` & `mypy-boto3-dynamodb-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/PKG-INFO` & `mypy-boto3-dynamodb-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.11
-Summary: Type annotations for boto3.DynamoDB 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.DynamoDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-dynamodb"></a>
 
 # mypy-boto3-dynamodb
 
 [![PyPI - mypy-boto3-dynamodb](https://img.shields.io/pypi/v/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,15 +481,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ResponseMetadataTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
     AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
@@ -501,14 +501,15 @@
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
     KeysAndAttributesServiceResourceOutputTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -553,19 +554,21 @@
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
     KeySchemaElementTableOutputTypeDef,
     ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
     KeySchemaElementOutputTypeDef,
@@ -573,57 +576,57 @@
     ProvisionedThroughputDescriptionTypeDef,
     ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
     ReplicaOutputTypeDef,
     S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
     TagOutputTypeDef,
+    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
     ProvisionedThroughputOverrideOutputTypeDef,
     ProvisionedThroughputOverrideTableOutputTypeDef,
     PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
     StreamSpecificationOutputTypeDef,
     StreamSpecificationTableOutputTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    DescribeLimitsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestOutputTypeDef,
@@ -647,15 +650,17 @@
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
+    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
@@ -688,19 +693,14 @@
     GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexOutputTypeDef,
     SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
     GlobalTableTypeDef,
     ImportSummaryTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
     ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
@@ -806,15 +806,15 @@
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> ArchivalSummaryTableResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.11/README.md` & `mypy-boto3-dynamodb-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dynamodb"></a>
 
 # mypy-boto3-dynamodb
 
 [![PyPI - mypy-boto3-dynamodb](https://img.shields.io/pypi/v/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -449,15 +449,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ResponseMetadataTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
     AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
@@ -469,14 +469,15 @@
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
     KeysAndAttributesServiceResourceOutputTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -521,19 +522,21 @@
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
     KeySchemaElementTableOutputTypeDef,
     ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
     KeySchemaElementOutputTypeDef,
@@ -541,57 +544,57 @@
     ProvisionedThroughputDescriptionTypeDef,
     ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
     ReplicaOutputTypeDef,
     S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
     TagOutputTypeDef,
+    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
     ProvisionedThroughputOverrideOutputTypeDef,
     ProvisionedThroughputOverrideTableOutputTypeDef,
     PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
     StreamSpecificationOutputTypeDef,
     StreamSpecificationTableOutputTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    DescribeLimitsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestOutputTypeDef,
@@ -615,15 +618,17 @@
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
+    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
@@ -656,19 +661,14 @@
     GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexOutputTypeDef,
     SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
     GlobalTableTypeDef,
     ImportSummaryTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
     ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
@@ -774,15 +774,15 @@
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> ArchivalSummaryTableResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.28.11\nVersion:         1.28.11\nBuilder version:"
-        " 7.15.1\nDocs:           "
+        "Type annotations for boto3.DynamoDB 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.11")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,15 @@
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
@@ -359,14 +360,15 @@
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
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,15 @@
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
@@ -357,14 +358,15 @@
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
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,45 +77,45 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
 
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
         """
 
 
 class ListTagsOfResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 
@@ -157,15 +157,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
 
@@ -206,13 +206,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,43 +74,43 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
         """
 
 class ListTagsOfResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 class QueryPaginator(Paginator):
@@ -151,15 +151,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
 class ScanPaginator(Paginator):
@@ -199,13 +199,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_dynamodb.type_defs import ArchivalSummaryTableResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ArchivalSummaryTableResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -60,15 +60,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "ArchivalSummaryTableResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionOutputTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
     "AttributeDefinitionTableOutputTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
@@ -80,14 +80,15 @@
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
     "KeysAndAttributesServiceResourceOutputTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
+    "BillingModeSummaryTableResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -132,19 +133,21 @@
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
     "KeySchemaElementTableOutputTypeDef",
     "ProjectionTableOutputTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
     "KeySchemaElementOutputTypeDef",
@@ -152,57 +155,57 @@
     "ProvisionedThroughputDescriptionTypeDef",
     "ProvisionedThroughputOutputTypeDef",
     "ProjectionServiceResourceTypeDef",
     "ReplicaOutputTypeDef",
     "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
     "TagOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
     "ProvisionedThroughputOverrideOutputTypeDef",
     "ProvisionedThroughputOverrideTableOutputTypeDef",
     "PutRequestServiceResourceOutputTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
+    "ResponseMetadataTypeDef",
+    "RestoreSummaryTableResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
+    "SSEDescriptionTableResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
     "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
     "StreamSpecificationOutputTypeDef",
     "StreamSpecificationTableOutputTypeDef",
+    "StreamSpecificationTableResponseMetadataTypeDef",
     "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
+    "TableClassSummaryTableResponseMetadataTypeDef",
     "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    "BillingModeSummaryTableResponseMetadataTypeDef",
-    "DescribeLimitsOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    "StreamSpecificationTableResponseMetadataTypeDef",
-    "TableClassSummaryTableResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementErrorTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestOutputTypeDef",
@@ -226,15 +229,17 @@
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
+    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
@@ -267,19 +272,14 @@
     "GlobalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexOutputTypeDef",
     "SourceTableDetailsTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
     "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
     "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     "WriteRequestServiceResourceOutputTypeDef",
     "WriteRequestServiceResourceTypeDef",
@@ -384,41 +384,42 @@
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryTableResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
+    total=False,
 )
 
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
+    total=False,
 )
 
 AttributeDefinitionOutputTypeDef = TypedDict(
     "AttributeDefinitionOutputTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
@@ -467,14 +468,15 @@
         "NS": List[str],
         "BS": List[bytes],
         "M": Dict[str, Dict[str, Any]],
         "L": List[Dict[str, Any]],
         "NULL": bool,
         "BOOL": bool,
     },
+    total=False,
 )
 
 AttributeValueTableTypeDef = TypedDict(
     "AttributeValueTableTypeDef",
     {
         "S": str,
         "N": str,
@@ -483,14 +485,15 @@
         "NS": List[str],
         "BS": List[bytes],
         "M": Dict[str, Dict[str, Any]],
         "L": List[Dict[str, Any]],
         "NULL": bool,
         "BOOL": bool,
     },
+    total=False,
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
@@ -526,24 +529,38 @@
             None,
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
-AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
-        "TargetValue": float,
     },
+    total=False,
 )
 
+
+class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
+    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+):
+    pass
+
+
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -560,41 +577,53 @@
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
 
-BackupDetailsTypeDef = TypedDict(
-    "BackupDetailsTypeDef",
+_RequiredBackupDetailsTypeDef = TypedDict(
+    "_RequiredBackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
-        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
+    },
+)
+_OptionalBackupDetailsTypeDef = TypedDict(
+    "_OptionalBackupDetailsTypeDef",
+    {
+        "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
+    total=False,
 )
 
+
+class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
+    pass
+
+
 BackupSummaryTableTypeDef = TypedDict(
     "BackupSummaryTableTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
+    total=False,
 )
 
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
@@ -603,14 +632,15 @@
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
+    total=False,
 )
 
 _RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
     "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -650,74 +680,103 @@
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
 
-KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
-    "KeysAndAttributesServiceResourceOutputTypeDef",
+_RequiredKeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesServiceResourceOutputTypeDef",
     {
         "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
+    },
+)
+_OptionalKeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesServiceResourceOutputTypeDef",
+    {
         "AttributesToGet": List[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Dict[str, str],
     },
+    total=False,
 )
 
+
+class KeysAndAttributesServiceResourceOutputTypeDef(
+    _RequiredKeysAndAttributesServiceResourceOutputTypeDef,
+    _OptionalKeysAndAttributesServiceResourceOutputTypeDef,
+):
+    pass
+
+
 ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
     "ItemCollectionMetricsServiceResourceTypeDef",
     {
         "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
+)
+
+BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
+    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
+    total=False,
 )
 
 CapacityServiceResourceTypeDef = TypedDict(
     "CapacityServiceResourceTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
+    total=False,
 )
 
 CapacityTableTypeDef = TypedDict(
     "CapacityTableTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
+    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
+    total=False,
 )
 
 _RequiredConditionTableTypeDef = TypedDict(
     "_RequiredConditionTableTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -755,23 +814,25 @@
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
+    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
+    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
@@ -956,14 +1017,15 @@
 
 CsvOptionsOutputTypeDef = TypedDict(
     "CsvOptionsOutputTypeDef",
     {
         "Delimiter": str,
         "HeaderList": List[str],
     },
+    total=False,
 )
 
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderList": Sequence[str],
@@ -1037,14 +1099,15 @@
 
 ItemCollectionMetricsTableTypeDef = TypedDict(
     "ItemCollectionMetricsTableTypeDef",
     {
         "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
 )
 
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
@@ -1141,14 +1204,15 @@
 
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
+    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1181,14 +1245,15 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
+    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1218,14 +1283,26 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
+    total=False,
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1256,22 +1333,31 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
+    total=False,
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
+    total=False,
 )
 
 _RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
         "TableArn": str,
         "S3Bucket": str,
@@ -1352,25 +1438,27 @@
 
 ProjectionTableOutputTypeDef = TypedDict(
     "ProjectionTableOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
+    total=False,
 )
 
 ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTableTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
+    total=False,
 )
 
 KeySchemaElementOutputTypeDef = TypedDict(
     "KeySchemaElementOutputTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
@@ -1379,25 +1467,27 @@
 
 ProjectionOutputTypeDef = TypedDict(
     "ProjectionOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
+    total=False,
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
+    total=False,
 )
 
 ProvisionedThroughputOutputTypeDef = TypedDict(
     "ProvisionedThroughputOutputTypeDef",
     {
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
@@ -1414,25 +1504,39 @@
 )
 
 ReplicaOutputTypeDef = TypedDict(
     "ReplicaOutputTypeDef",
     {
         "RegionName": str,
     },
+    total=False,
 )
 
-S3BucketSourceOutputTypeDef = TypedDict(
-    "S3BucketSourceOutputTypeDef",
+_RequiredS3BucketSourceOutputTypeDef = TypedDict(
+    "_RequiredS3BucketSourceOutputTypeDef",
     {
-        "S3BucketOwner": str,
         "S3Bucket": str,
+    },
+)
+_OptionalS3BucketSourceOutputTypeDef = TypedDict(
+    "_OptionalS3BucketSourceOutputTypeDef",
+    {
+        "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
+    total=False,
 )
 
+
+class S3BucketSourceOutputTypeDef(
+    _RequiredS3BucketSourceOutputTypeDef, _OptionalS3BucketSourceOutputTypeDef
+):
+    pass
+
+
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1453,20 +1557,32 @@
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1516,23 +1632,71 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
@@ -1562,33 +1726,57 @@
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
+ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
     "ProvisionedThroughputOverrideOutputTypeDef",
     {
         "ReadCapacityUnits": int,
     },
+    total=False,
 )
 
 ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
     "ProvisionedThroughputOverrideTableOutputTypeDef",
     {
         "ReadCapacityUnits": int,
     },
+    total=False,
 )
 
 PutRequestServiceResourceOutputTypeDef = TypedDict(
     "PutRequestServiceResourceOutputTypeDef",
     {
         "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
     },
@@ -1621,96 +1809,193 @@
 
 TableClassSummaryTableTypeDef = TypedDict(
     "TableClassSummaryTableTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
+    total=False,
 )
 
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
+    total=False,
 )
 
-RestoreSummaryTableTypeDef = TypedDict(
-    "RestoreSummaryTableTypeDef",
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
+RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryTableResponseMetadataTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RestoreSummaryTypeDef = TypedDict(
-    "RestoreSummaryTypeDef",
+_RequiredRestoreSummaryTableTypeDef = TypedDict(
+    "_RequiredRestoreSummaryTableTypeDef",
+    {
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+    },
+)
+_OptionalRestoreSummaryTableTypeDef = TypedDict(
+    "_OptionalRestoreSummaryTableTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
+    },
+    total=False,
+)
+
+
+class RestoreSummaryTableTypeDef(
+    _RequiredRestoreSummaryTableTypeDef, _OptionalRestoreSummaryTableTypeDef
+):
+    pass
+
+
+_RequiredRestoreSummaryTypeDef = TypedDict(
+    "_RequiredRestoreSummaryTypeDef",
+    {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
+_OptionalRestoreSummaryTypeDef = TypedDict(
+    "_OptionalRestoreSummaryTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+    },
+    total=False,
+)
+
+
+class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
+    pass
+
+
+SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 SSEDescriptionTableTypeDef = TypedDict(
     "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
+    total=False,
 )
 
 SSEDescriptionTypeDef = TypedDict(
     "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
+    total=False,
 )
 
 SSESpecificationOutputTypeDef = TypedDict(
     "SSESpecificationOutputTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
+    total=False,
 )
 
 SSESpecificationTableTypeDef = TypedDict(
     "SSESpecificationTableTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
-StreamSpecificationOutputTypeDef = TypedDict(
-    "StreamSpecificationOutputTypeDef",
+_RequiredStreamSpecificationOutputTypeDef = TypedDict(
+    "_RequiredStreamSpecificationOutputTypeDef",
+    {
+        "StreamEnabled": bool,
+    },
+)
+_OptionalStreamSpecificationOutputTypeDef = TypedDict(
+    "_OptionalStreamSpecificationOutputTypeDef",
+    {
+        "StreamViewType": StreamViewTypeType,
+    },
+    total=False,
+)
+
+
+class StreamSpecificationOutputTypeDef(
+    _RequiredStreamSpecificationOutputTypeDef, _OptionalStreamSpecificationOutputTypeDef
+):
+    pass
+
+
+_RequiredStreamSpecificationTableOutputTypeDef = TypedDict(
+    "_RequiredStreamSpecificationTableOutputTypeDef",
     {
         "StreamEnabled": bool,
+    },
+)
+_OptionalStreamSpecificationTableOutputTypeDef = TypedDict(
+    "_OptionalStreamSpecificationTableOutputTypeDef",
+    {
         "StreamViewType": StreamViewTypeType,
     },
+    total=False,
 )
 
-StreamSpecificationTableOutputTypeDef = TypedDict(
-    "StreamSpecificationTableOutputTypeDef",
+
+class StreamSpecificationTableOutputTypeDef(
+    _RequiredStreamSpecificationTableOutputTypeDef, _OptionalStreamSpecificationTableOutputTypeDef
+):
+    pass
+
+
+StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationTableResponseMetadataTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
@@ -1735,14 +2020,23 @@
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
+TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryTableResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeToLiveSpecificationOutputTypeDef = TypedDict(
     "TimeToLiveSpecificationOutputTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
@@ -1782,138 +2076,21 @@
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
 
-ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryTableResponseMetadataTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationTableResponseMetadataTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryTableResponseMetadataTypeDef",
-    {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1943,14 +2120,15 @@
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
+    total=False,
 )
 
 _RequiredBatchStatementRequestTypeDef = TypedDict(
     "_RequiredBatchStatementRequestTypeDef",
     {
         "Statement": str,
     },
@@ -2382,34 +2560,49 @@
 
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
     },
+    total=False,
 )
 
-KeysAndAttributesOutputTypeDef = TypedDict(
-    "KeysAndAttributesOutputTypeDef",
+_RequiredKeysAndAttributesOutputTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesOutputTypeDef",
     {
         "Keys": List[Dict[str, AttributeValueTypeDef]],
+    },
+)
+_OptionalKeysAndAttributesOutputTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesOutputTypeDef",
+    {
         "AttributesToGet": List[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Dict[str, str],
     },
+    total=False,
 )
 
+
+class KeysAndAttributesOutputTypeDef(
+    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
+):
+    pass
+
+
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[
             Mapping[
                 str,
                 Union[
@@ -2665,14 +2858,15 @@
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
         ),
     },
+    total=False,
 )
 
 _RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
@@ -2694,33 +2888,33 @@
     pass
 
 
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2749,42 +2943,98 @@
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityServiceResourceTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
     },
+    total=False,
 )
 
 ConsumedCapacityTableTypeDef = TypedDict(
     "ConsumedCapacityTableTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTableTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
     },
+    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
+    total=False,
 )
 
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2836,14 +3086,66 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2894,28 +3196,41 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-ContinuousBackupsDescriptionTypeDef = TypedDict(
-    "ContinuousBackupsDescriptionTypeDef",
+_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_RequiredContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
+    },
+)
+_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_OptionalContinuousBackupsDescriptionTypeDef",
+    {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
+    total=False,
 )
 
+
+class ContinuousBackupsDescriptionTypeDef(
+    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
+):
+    pass
+
+
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
@@ -3071,14 +3386,15 @@
 )
 
 InputFormatOptionsOutputTypeDef = TypedDict(
     "InputFormatOptionsOutputTypeDef",
     {
         "Csv": CsvOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
@@ -3296,48 +3612,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3381,37 +3697,38 @@
     pass
 
 
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "LocalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTableOutputTypeDef],
         "Projection": ProjectionTableOutputTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTableOutputTypeDef],
@@ -3419,35 +3736,38 @@
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 LocalSecondaryIndexDescriptionTypeDef = TypedDict(
     "LocalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 LocalSecondaryIndexInfoTypeDef = TypedDict(
     "LocalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
@@ -3455,51 +3775,79 @@
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexInfoTypeDef = TypedDict(
     "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
     },
+    total=False,
 )
 
-GlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "GlobalSecondaryIndexOutputTypeDef",
+_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_RequiredGlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
+    },
+)
+_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_OptionalGlobalSecondaryIndexOutputTypeDef",
+    {
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
     },
+    total=False,
 )
 
-SourceTableDetailsTypeDef = TypedDict(
-    "SourceTableDetailsTypeDef",
+
+class GlobalSecondaryIndexOutputTypeDef(
+    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
+):
+    pass
+
+
+_RequiredSourceTableDetailsTypeDef = TypedDict(
+    "_RequiredSourceTableDetailsTypeDef",
     {
         "TableName": str,
         "TableId": str,
-        "TableArn": str,
-        "TableSizeBytes": int,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "TableCreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+_OptionalSourceTableDetailsTypeDef = TypedDict(
+    "_OptionalSourceTableDetailsTypeDef",
+    {
+        "TableArn": str,
+        "TableSizeBytes": int,
         "ItemCount": int,
         "BillingMode": BillingModeType,
     },
+    total=False,
 )
 
+
+class SourceTableDetailsTypeDef(
+    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
+):
+    pass
+
+
 _RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
         "Projection": ProjectionServiceResourceTypeDef,
     },
@@ -3531,192 +3879,47 @@
 
 GlobalTableTypeDef = TypedDict(
     "GlobalTableTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": List[ReplicaOutputTypeDef],
     },
+    total=False,
 )
 
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
         "S3BucketSource": S3BucketSourceOutputTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
-)
-
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
-
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
     total=False,
 )
 
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
@@ -3726,30 +3929,33 @@
 
 ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
     },
+    total=False,
 )
 
 ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
     },
+    total=False,
 )
 
 WriteRequestServiceResourceOutputTypeDef = TypedDict(
     "WriteRequestServiceResourceOutputTypeDef",
     {
         "PutRequest": PutRequestServiceResourceOutputTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
     },
+    total=False,
 )
 
 WriteRequestServiceResourceTypeDef = TypedDict(
     "WriteRequestServiceResourceTypeDef",
     {
         "PutRequest": PutRequestServiceResourceTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceTypeDef,
@@ -3757,15 +3963,15 @@
     total=False,
 )
 
 UpdateTimeToLiveOutputTypeDef = TypedDict(
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTimeToLiveInputRequestTypeDef = TypedDict(
     "UpdateTimeToLiveInputRequestTypeDef",
     {
         "TableName": str,
@@ -3776,14 +3982,15 @@
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
+    total=False,
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
@@ -4227,14 +4434,15 @@
 
 WriteRequestOutputTypeDef = TypedDict(
     "WriteRequestOutputTypeDef",
     {
         "PutRequest": PutRequestOutputTypeDef,
         "DeleteRequest": DeleteRequestOutputTypeDef,
     },
+    total=False,
 )
 
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
@@ -4258,14 +4466,15 @@
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
+    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
@@ -4278,205 +4487,205 @@
 
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
         "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
         "Item": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
         "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
         "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
         "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
         "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
@@ -4723,29 +4932,43 @@
     {
         "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
         "StreamDescription": StreamSpecificationOutputTypeDef,
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
     },
+    total=False,
 )
 
-TableCreationParametersOutputTypeDef = TypedDict(
-    "TableCreationParametersOutputTypeDef",
+_RequiredTableCreationParametersOutputTypeDef = TypedDict(
+    "_RequiredTableCreationParametersOutputTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "KeySchema": List[KeySchemaElementOutputTypeDef],
+    },
+)
+_OptionalTableCreationParametersOutputTypeDef = TypedDict(
+    "_OptionalTableCreationParametersOutputTypeDef",
+    {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
         "SSESpecification": SSESpecificationOutputTypeDef,
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
     },
+    total=False,
 )
 
+
+class TableCreationParametersOutputTypeDef(
+    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
+):
+    pass
+
+
 _RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
@@ -4775,24 +4998,24 @@
 
 
 ListGlobalTablesOutputTypeDef = TypedDict(
     "ListGlobalTablesOutputTypeDef",
     {
         "GlobalTables": List[GlobalTableTypeDef],
         "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicaDescriptionTypeDef = TypedDict(
     "ReplicaDescriptionTypeDef",
     {
         "RegionName": str,
@@ -4801,14 +5024,15 @@
         "ReplicaStatusPercentProgress": str,
         "KMSMasterKeyId": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
         "ReplicaInaccessibleDateTime": datetime,
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
+    total=False,
 )
 
 ReplicaDescriptionTableTypeDef = TypedDict(
     "ReplicaDescriptionTableTypeDef",
     {
         "RegionName": str,
         "ReplicaStatus": ReplicaStatusType,
@@ -4816,23 +5040,24 @@
         "ReplicaStatusPercentProgress": str,
         "KMSMasterKeyId": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
         "ReplicaInaccessibleDateTime": datetime,
         "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
     },
+    total=False,
 )
 
 BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
     "BatchWriteItemOutputServiceResourceTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4856,15 +5081,15 @@
 
 
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
@@ -4887,15 +5112,15 @@
 
 BatchWriteItemOutputTypeDef = TypedDict(
     "BatchWriteItemOutputTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputRequestTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
@@ -4944,28 +5169,43 @@
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
-ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
+    },
+)
+_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
+
+class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
+    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+):
+    pass
+
+
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -5074,14 +5314,15 @@
 BackupDescriptionTypeDef = TypedDict(
     "BackupDescriptionTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
         "SourceTableDetails": SourceTableDetailsTypeDef,
         "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
     },
+    total=False,
 )
 
 ImportTableDescriptionTypeDef = TypedDict(
     "ImportTableDescriptionTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
@@ -5099,25 +5340,27 @@
         "EndTime": datetime,
         "ProcessedSizeBytes": int,
         "ProcessedItemCount": int,
         "ImportedItemCount": int,
         "FailureCode": str,
         "FailureMessage": str,
     },
+    total=False,
 )
 
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
+    total=False,
 )
 
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
         "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "TableName": str,
@@ -5139,14 +5382,15 @@
         "Replicas": List[ReplicaDescriptionTypeDef],
         "RestoreSummary": RestoreSummaryTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
         "ArchivalSummary": ArchivalSummaryTypeDef,
         "TableClassSummary": TableClassSummaryTypeDef,
         "DeletionProtectionEnabled": bool,
     },
+    total=False,
 )
 
 TableDescriptionTableTypeDef = TypedDict(
     "TableDescriptionTableTypeDef",
     {
         "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
         "TableName": str,
@@ -5168,44 +5412,59 @@
         "Replicas": List[ReplicaDescriptionTableTypeDef],
         "RestoreSummary": RestoreSummaryTableTypeDef,
         "SSEDescription": SSEDescriptionTableTypeDef,
         "ArchivalSummary": ArchivalSummaryTableTypeDef,
         "TableClassSummary": TableClassSummaryTableTypeDef,
         "DeletionProtectionEnabled": bool,
     },
+    total=False,
 )
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
+    total=False,
 )
 
-ReplicaSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaSettingsDescriptionTypeDef",
+_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
+    },
+)
+_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaSettingsDescriptionTypeDef",
+    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
+    total=False,
 )
 
+
+class ReplicaSettingsDescriptionTypeDef(
+    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
+):
+    pass
+
+
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5297,146 +5556,147 @@
     pass
 
 
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTableTypeDef = TypedDict(
     "DeleteTableOutputTableTypeDef",
     {
         "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
+    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5490,18 +5750,18 @@
     pass
 
 
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/type_defs.pyi` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_dynamodb.type_defs import ArchivalSummaryTableResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ArchivalSummaryTableResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -59,15 +59,15 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "ArchivalSummaryTableResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionOutputTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
     "AttributeDefinitionTableOutputTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
@@ -79,14 +79,15 @@
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
     "KeysAndAttributesServiceResourceOutputTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
+    "BillingModeSummaryTableResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -131,19 +132,21 @@
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
     "KeySchemaElementTableOutputTypeDef",
     "ProjectionTableOutputTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
     "KeySchemaElementOutputTypeDef",
@@ -151,57 +154,57 @@
     "ProvisionedThroughputDescriptionTypeDef",
     "ProvisionedThroughputOutputTypeDef",
     "ProjectionServiceResourceTypeDef",
     "ReplicaOutputTypeDef",
     "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
     "TagOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
     "ProvisionedThroughputOverrideOutputTypeDef",
     "ProvisionedThroughputOverrideTableOutputTypeDef",
     "PutRequestServiceResourceOutputTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
+    "ResponseMetadataTypeDef",
+    "RestoreSummaryTableResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
+    "SSEDescriptionTableResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
     "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
     "StreamSpecificationOutputTypeDef",
     "StreamSpecificationTableOutputTypeDef",
+    "StreamSpecificationTableResponseMetadataTypeDef",
     "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
+    "TableClassSummaryTableResponseMetadataTypeDef",
     "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    "BillingModeSummaryTableResponseMetadataTypeDef",
-    "DescribeLimitsOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    "StreamSpecificationTableResponseMetadataTypeDef",
-    "TableClassSummaryTableResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementErrorTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestOutputTypeDef",
@@ -225,15 +228,17 @@
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
+    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
@@ -266,19 +271,14 @@
     "GlobalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexOutputTypeDef",
     "SourceTableDetailsTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
     "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
     "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     "WriteRequestServiceResourceOutputTypeDef",
     "WriteRequestServiceResourceTypeDef",
@@ -383,41 +383,42 @@
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryTableResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
+    total=False,
 )
 
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
+    total=False,
 )
 
 AttributeDefinitionOutputTypeDef = TypedDict(
     "AttributeDefinitionOutputTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
@@ -466,14 +467,15 @@
         "NS": List[str],
         "BS": List[bytes],
         "M": Dict[str, Dict[str, Any]],
         "L": List[Dict[str, Any]],
         "NULL": bool,
         "BOOL": bool,
     },
+    total=False,
 )
 
 AttributeValueTableTypeDef = TypedDict(
     "AttributeValueTableTypeDef",
     {
         "S": str,
         "N": str,
@@ -482,14 +484,15 @@
         "NS": List[str],
         "BS": List[bytes],
         "M": Dict[str, Dict[str, Any]],
         "L": List[Dict[str, Any]],
         "NULL": bool,
         "BOOL": bool,
     },
+    total=False,
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
@@ -525,24 +528,36 @@
             None,
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
-AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
-        "TargetValue": float,
     },
+    total=False,
 )
 
+class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
+    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+):
+    pass
+
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -557,41 +572,51 @@
 
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
-BackupDetailsTypeDef = TypedDict(
-    "BackupDetailsTypeDef",
+_RequiredBackupDetailsTypeDef = TypedDict(
+    "_RequiredBackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
-        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
+    },
+)
+_OptionalBackupDetailsTypeDef = TypedDict(
+    "_OptionalBackupDetailsTypeDef",
+    {
+        "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
+    total=False,
 )
 
+class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
+    pass
+
 BackupSummaryTableTypeDef = TypedDict(
     "BackupSummaryTableTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
+    total=False,
 )
 
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
@@ -600,14 +625,15 @@
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
+    total=False,
 )
 
 _RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
     "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -645,74 +671,101 @@
 
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
-KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
-    "KeysAndAttributesServiceResourceOutputTypeDef",
+_RequiredKeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesServiceResourceOutputTypeDef",
     {
         "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
+    },
+)
+_OptionalKeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesServiceResourceOutputTypeDef",
+    {
         "AttributesToGet": List[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Dict[str, str],
     },
+    total=False,
 )
 
+class KeysAndAttributesServiceResourceOutputTypeDef(
+    _RequiredKeysAndAttributesServiceResourceOutputTypeDef,
+    _OptionalKeysAndAttributesServiceResourceOutputTypeDef,
+):
+    pass
+
 ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
     "ItemCollectionMetricsServiceResourceTypeDef",
     {
         "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
+)
+
+BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
+    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
+    total=False,
 )
 
 CapacityServiceResourceTypeDef = TypedDict(
     "CapacityServiceResourceTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
+    total=False,
 )
 
 CapacityTableTypeDef = TypedDict(
     "CapacityTableTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
+    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
+    total=False,
 )
 
 _RequiredConditionTableTypeDef = TypedDict(
     "_RequiredConditionTableTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -748,23 +801,25 @@
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
+    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
+    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
@@ -945,14 +1000,15 @@
 
 CsvOptionsOutputTypeDef = TypedDict(
     "CsvOptionsOutputTypeDef",
     {
         "Delimiter": str,
         "HeaderList": List[str],
     },
+    total=False,
 )
 
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderList": Sequence[str],
@@ -1026,14 +1082,15 @@
 
 ItemCollectionMetricsTableTypeDef = TypedDict(
     "ItemCollectionMetricsTableTypeDef",
     {
         "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
 )
 
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
@@ -1128,14 +1185,15 @@
 
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
+    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1168,14 +1226,15 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
+    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1205,14 +1264,26 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
+    total=False,
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1243,22 +1314,31 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
+    total=False,
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
+    total=False,
 )
 
 _RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
         "TableArn": str,
         "S3Bucket": str,
@@ -1335,25 +1415,27 @@
 
 ProjectionTableOutputTypeDef = TypedDict(
     "ProjectionTableOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
+    total=False,
 )
 
 ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTableTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
+    total=False,
 )
 
 KeySchemaElementOutputTypeDef = TypedDict(
     "KeySchemaElementOutputTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
@@ -1362,25 +1444,27 @@
 
 ProjectionOutputTypeDef = TypedDict(
     "ProjectionOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
+    total=False,
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
+    total=False,
 )
 
 ProvisionedThroughputOutputTypeDef = TypedDict(
     "ProvisionedThroughputOutputTypeDef",
     {
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
@@ -1397,25 +1481,37 @@
 )
 
 ReplicaOutputTypeDef = TypedDict(
     "ReplicaOutputTypeDef",
     {
         "RegionName": str,
     },
+    total=False,
 )
 
-S3BucketSourceOutputTypeDef = TypedDict(
-    "S3BucketSourceOutputTypeDef",
+_RequiredS3BucketSourceOutputTypeDef = TypedDict(
+    "_RequiredS3BucketSourceOutputTypeDef",
     {
-        "S3BucketOwner": str,
         "S3Bucket": str,
+    },
+)
+_OptionalS3BucketSourceOutputTypeDef = TypedDict(
+    "_OptionalS3BucketSourceOutputTypeDef",
+    {
+        "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
+    total=False,
 )
 
+class S3BucketSourceOutputTypeDef(
+    _RequiredS3BucketSourceOutputTypeDef, _OptionalS3BucketSourceOutputTypeDef
+):
+    pass
+
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1434,20 +1530,32 @@
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1497,23 +1605,69 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
@@ -1541,33 +1695,57 @@
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
+ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
     "ProvisionedThroughputOverrideOutputTypeDef",
     {
         "ReadCapacityUnits": int,
     },
+    total=False,
 )
 
 ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
     "ProvisionedThroughputOverrideTableOutputTypeDef",
     {
         "ReadCapacityUnits": int,
     },
+    total=False,
 )
 
 PutRequestServiceResourceOutputTypeDef = TypedDict(
     "PutRequestServiceResourceOutputTypeDef",
     {
         "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
     },
@@ -1600,96 +1778,185 @@
 
 TableClassSummaryTableTypeDef = TypedDict(
     "TableClassSummaryTableTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
+    total=False,
 )
 
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
+    total=False,
 )
 
-RestoreSummaryTableTypeDef = TypedDict(
-    "RestoreSummaryTableTypeDef",
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
+RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryTableResponseMetadataTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RestoreSummaryTypeDef = TypedDict(
-    "RestoreSummaryTypeDef",
+_RequiredRestoreSummaryTableTypeDef = TypedDict(
+    "_RequiredRestoreSummaryTableTypeDef",
+    {
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+    },
+)
+_OptionalRestoreSummaryTableTypeDef = TypedDict(
+    "_OptionalRestoreSummaryTableTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
+    },
+    total=False,
+)
+
+class RestoreSummaryTableTypeDef(
+    _RequiredRestoreSummaryTableTypeDef, _OptionalRestoreSummaryTableTypeDef
+):
+    pass
+
+_RequiredRestoreSummaryTypeDef = TypedDict(
+    "_RequiredRestoreSummaryTypeDef",
+    {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
+_OptionalRestoreSummaryTypeDef = TypedDict(
+    "_OptionalRestoreSummaryTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+    },
+    total=False,
+)
+
+class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
+    pass
+
+SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 SSEDescriptionTableTypeDef = TypedDict(
     "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
+    total=False,
 )
 
 SSEDescriptionTypeDef = TypedDict(
     "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
+    total=False,
 )
 
 SSESpecificationOutputTypeDef = TypedDict(
     "SSESpecificationOutputTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
+    total=False,
 )
 
 SSESpecificationTableTypeDef = TypedDict(
     "SSESpecificationTableTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
-StreamSpecificationOutputTypeDef = TypedDict(
-    "StreamSpecificationOutputTypeDef",
+_RequiredStreamSpecificationOutputTypeDef = TypedDict(
+    "_RequiredStreamSpecificationOutputTypeDef",
+    {
+        "StreamEnabled": bool,
+    },
+)
+_OptionalStreamSpecificationOutputTypeDef = TypedDict(
+    "_OptionalStreamSpecificationOutputTypeDef",
+    {
+        "StreamViewType": StreamViewTypeType,
+    },
+    total=False,
+)
+
+class StreamSpecificationOutputTypeDef(
+    _RequiredStreamSpecificationOutputTypeDef, _OptionalStreamSpecificationOutputTypeDef
+):
+    pass
+
+_RequiredStreamSpecificationTableOutputTypeDef = TypedDict(
+    "_RequiredStreamSpecificationTableOutputTypeDef",
     {
         "StreamEnabled": bool,
+    },
+)
+_OptionalStreamSpecificationTableOutputTypeDef = TypedDict(
+    "_OptionalStreamSpecificationTableOutputTypeDef",
+    {
         "StreamViewType": StreamViewTypeType,
     },
+    total=False,
 )
 
-StreamSpecificationTableOutputTypeDef = TypedDict(
-    "StreamSpecificationTableOutputTypeDef",
+class StreamSpecificationTableOutputTypeDef(
+    _RequiredStreamSpecificationTableOutputTypeDef, _OptionalStreamSpecificationTableOutputTypeDef
+):
+    pass
+
+StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationTableResponseMetadataTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
@@ -1712,14 +1979,23 @@
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
+TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryTableResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeToLiveSpecificationOutputTypeDef = TypedDict(
     "TimeToLiveSpecificationOutputTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
@@ -1757,138 +2033,21 @@
 
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
-ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryTableResponseMetadataTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationTableResponseMetadataTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryTableResponseMetadataTypeDef",
-    {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1918,14 +2077,15 @@
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
+    total=False,
 )
 
 _RequiredBatchStatementRequestTypeDef = TypedDict(
     "_RequiredBatchStatementRequestTypeDef",
     {
         "Statement": str,
     },
@@ -2343,34 +2503,47 @@
 
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
     },
+    total=False,
 )
 
-KeysAndAttributesOutputTypeDef = TypedDict(
-    "KeysAndAttributesOutputTypeDef",
+_RequiredKeysAndAttributesOutputTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesOutputTypeDef",
     {
         "Keys": List[Dict[str, AttributeValueTypeDef]],
+    },
+)
+_OptionalKeysAndAttributesOutputTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesOutputTypeDef",
+    {
         "AttributesToGet": List[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Dict[str, str],
     },
+    total=False,
 )
 
+class KeysAndAttributesOutputTypeDef(
+    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
+):
+    pass
+
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[
             Mapping[
                 str,
                 Union[
@@ -2618,14 +2791,15 @@
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
         ),
     },
+    total=False,
 )
 
 _RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
@@ -2645,33 +2819,33 @@
 ):
     pass
 
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2698,42 +2872,96 @@
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityServiceResourceTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
     },
+    total=False,
 )
 
 ConsumedCapacityTableTypeDef = TypedDict(
     "ConsumedCapacityTableTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTableTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
     },
+    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
+    total=False,
+)
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
 )
 
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2785,14 +3013,64 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2843,28 +3121,39 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-ContinuousBackupsDescriptionTypeDef = TypedDict(
-    "ContinuousBackupsDescriptionTypeDef",
+_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_RequiredContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
+    },
+)
+_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_OptionalContinuousBackupsDescriptionTypeDef",
+    {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
+    total=False,
 )
 
+class ContinuousBackupsDescriptionTypeDef(
+    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
+):
+    pass
+
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
@@ -3010,14 +3299,15 @@
 )
 
 InputFormatOptionsOutputTypeDef = TypedDict(
     "InputFormatOptionsOutputTypeDef",
     {
         "Csv": CsvOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
@@ -3229,48 +3519,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3310,37 +3600,38 @@
 ):
     pass
 
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "LocalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTableOutputTypeDef],
         "Projection": ProjectionTableOutputTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTableOutputTypeDef],
@@ -3348,35 +3639,38 @@
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 LocalSecondaryIndexDescriptionTypeDef = TypedDict(
     "LocalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 LocalSecondaryIndexInfoTypeDef = TypedDict(
     "LocalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
@@ -3384,51 +3678,75 @@
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexInfoTypeDef = TypedDict(
     "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
     },
+    total=False,
 )
 
-GlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "GlobalSecondaryIndexOutputTypeDef",
+_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_RequiredGlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "Projection": ProjectionOutputTypeDef,
+    },
+)
+_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_OptionalGlobalSecondaryIndexOutputTypeDef",
+    {
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
     },
+    total=False,
 )
 
-SourceTableDetailsTypeDef = TypedDict(
-    "SourceTableDetailsTypeDef",
+class GlobalSecondaryIndexOutputTypeDef(
+    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
+):
+    pass
+
+_RequiredSourceTableDetailsTypeDef = TypedDict(
+    "_RequiredSourceTableDetailsTypeDef",
     {
         "TableName": str,
         "TableId": str,
-        "TableArn": str,
-        "TableSizeBytes": int,
         "KeySchema": List[KeySchemaElementOutputTypeDef],
         "TableCreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+_OptionalSourceTableDetailsTypeDef = TypedDict(
+    "_OptionalSourceTableDetailsTypeDef",
+    {
+        "TableArn": str,
+        "TableSizeBytes": int,
         "ItemCount": int,
         "BillingMode": BillingModeType,
     },
+    total=False,
 )
 
+class SourceTableDetailsTypeDef(
+    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
+):
+    pass
+
 _RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
         "Projection": ProjectionServiceResourceTypeDef,
     },
@@ -3458,186 +3776,47 @@
 
 GlobalTableTypeDef = TypedDict(
     "GlobalTableTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": List[ReplicaOutputTypeDef],
     },
+    total=False,
 )
 
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
         "S3BucketSource": S3BucketSourceOutputTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
-)
-
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
     total=False,
 )
 
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
@@ -3647,30 +3826,33 @@
 
 ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
     },
+    total=False,
 )
 
 ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
     },
+    total=False,
 )
 
 WriteRequestServiceResourceOutputTypeDef = TypedDict(
     "WriteRequestServiceResourceOutputTypeDef",
     {
         "PutRequest": PutRequestServiceResourceOutputTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
     },
+    total=False,
 )
 
 WriteRequestServiceResourceTypeDef = TypedDict(
     "WriteRequestServiceResourceTypeDef",
     {
         "PutRequest": PutRequestServiceResourceTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceTypeDef,
@@ -3678,15 +3860,15 @@
     total=False,
 )
 
 UpdateTimeToLiveOutputTypeDef = TypedDict(
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTimeToLiveInputRequestTypeDef = TypedDict(
     "UpdateTimeToLiveInputRequestTypeDef",
     {
         "TableName": str,
@@ -3697,14 +3879,15 @@
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
+    total=False,
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
@@ -4132,14 +4315,15 @@
 
 WriteRequestOutputTypeDef = TypedDict(
     "WriteRequestOutputTypeDef",
     {
         "PutRequest": PutRequestOutputTypeDef,
         "DeleteRequest": DeleteRequestOutputTypeDef,
     },
+    total=False,
 )
 
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
@@ -4163,14 +4347,15 @@
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
+    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
@@ -4183,205 +4368,205 @@
 
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
         "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
         "Item": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
         "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
         "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
         "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
         "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
@@ -4612,29 +4797,41 @@
     {
         "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
         "StreamDescription": StreamSpecificationOutputTypeDef,
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
     },
+    total=False,
 )
 
-TableCreationParametersOutputTypeDef = TypedDict(
-    "TableCreationParametersOutputTypeDef",
+_RequiredTableCreationParametersOutputTypeDef = TypedDict(
+    "_RequiredTableCreationParametersOutputTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "KeySchema": List[KeySchemaElementOutputTypeDef],
+    },
+)
+_OptionalTableCreationParametersOutputTypeDef = TypedDict(
+    "_OptionalTableCreationParametersOutputTypeDef",
+    {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
         "SSESpecification": SSESpecificationOutputTypeDef,
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
     },
+    total=False,
 )
 
+class TableCreationParametersOutputTypeDef(
+    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
+):
+    pass
+
 _RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
@@ -4662,24 +4859,24 @@
     pass
 
 ListGlobalTablesOutputTypeDef = TypedDict(
     "ListGlobalTablesOutputTypeDef",
     {
         "GlobalTables": List[GlobalTableTypeDef],
         "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicaDescriptionTypeDef = TypedDict(
     "ReplicaDescriptionTypeDef",
     {
         "RegionName": str,
@@ -4688,14 +4885,15 @@
         "ReplicaStatusPercentProgress": str,
         "KMSMasterKeyId": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
         "ReplicaInaccessibleDateTime": datetime,
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
+    total=False,
 )
 
 ReplicaDescriptionTableTypeDef = TypedDict(
     "ReplicaDescriptionTableTypeDef",
     {
         "RegionName": str,
         "ReplicaStatus": ReplicaStatusType,
@@ -4703,23 +4901,24 @@
         "ReplicaStatusPercentProgress": str,
         "KMSMasterKeyId": str,
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
         "ReplicaInaccessibleDateTime": datetime,
         "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
     },
+    total=False,
 )
 
 BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
     "BatchWriteItemOutputServiceResourceTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4741,15 +4940,15 @@
     pass
 
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
@@ -4770,15 +4969,15 @@
 
 BatchWriteItemOutputTypeDef = TypedDict(
     "BatchWriteItemOutputTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputRequestTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
@@ -4823,28 +5022,41 @@
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
-ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
+    },
+)
+_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
+class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
+    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+):
+    pass
+
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -4947,14 +5159,15 @@
 BackupDescriptionTypeDef = TypedDict(
     "BackupDescriptionTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
         "SourceTableDetails": SourceTableDetailsTypeDef,
         "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
     },
+    total=False,
 )
 
 ImportTableDescriptionTypeDef = TypedDict(
     "ImportTableDescriptionTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
@@ -4972,25 +5185,27 @@
         "EndTime": datetime,
         "ProcessedSizeBytes": int,
         "ProcessedItemCount": int,
         "ImportedItemCount": int,
         "FailureCode": str,
         "FailureMessage": str,
     },
+    total=False,
 )
 
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
+    total=False,
 )
 
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
         "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "TableName": str,
@@ -5012,14 +5227,15 @@
         "Replicas": List[ReplicaDescriptionTypeDef],
         "RestoreSummary": RestoreSummaryTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
         "ArchivalSummary": ArchivalSummaryTypeDef,
         "TableClassSummary": TableClassSummaryTypeDef,
         "DeletionProtectionEnabled": bool,
     },
+    total=False,
 )
 
 TableDescriptionTableTypeDef = TypedDict(
     "TableDescriptionTableTypeDef",
     {
         "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
         "TableName": str,
@@ -5041,44 +5257,57 @@
         "Replicas": List[ReplicaDescriptionTableTypeDef],
         "RestoreSummary": RestoreSummaryTableTypeDef,
         "SSEDescription": SSEDescriptionTableTypeDef,
         "ArchivalSummary": ArchivalSummaryTableTypeDef,
         "TableClassSummary": TableClassSummaryTableTypeDef,
         "DeletionProtectionEnabled": bool,
     },
+    total=False,
 )
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
+    total=False,
 )
 
-ReplicaSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaSettingsDescriptionTypeDef",
+_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
+    },
+)
+_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaSettingsDescriptionTypeDef",
+    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
+    total=False,
 )
 
+class ReplicaSettingsDescriptionTypeDef(
+    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
+):
+    pass
+
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5164,146 +5393,147 @@
 ):
     pass
 
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTableTypeDef = TypedDict(
     "DeleteTableOutputTableTypeDef",
     {
         "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
+    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5353,18 +5583,18 @@
 ):
     pass
 
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.11
-Summary: Type annotations for boto3.DynamoDB 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.DynamoDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-dynamodb"></a>
 
 # mypy-boto3-dynamodb
 
 [![PyPI - mypy-boto3-dynamodb](https://img.shields.io/pypi/v/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,15 +481,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ResponseMetadataTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
     AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
@@ -501,14 +501,15 @@
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
     KeysAndAttributesServiceResourceOutputTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -553,19 +554,21 @@
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
     KeySchemaElementTableOutputTypeDef,
     ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
     KeySchemaElementOutputTypeDef,
@@ -573,57 +576,57 @@
     ProvisionedThroughputDescriptionTypeDef,
     ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
     ReplicaOutputTypeDef,
     S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
     TagOutputTypeDef,
+    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
     ProvisionedThroughputOverrideOutputTypeDef,
     ProvisionedThroughputOverrideTableOutputTypeDef,
     PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
     StreamSpecificationOutputTypeDef,
     StreamSpecificationTableOutputTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    DescribeLimitsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestOutputTypeDef,
@@ -647,15 +650,17 @@
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
+    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
@@ -688,19 +693,14 @@
     GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexOutputTypeDef,
     SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
     GlobalTableTypeDef,
     ImportSummaryTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
     ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
@@ -806,15 +806,15 @@
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> ArchivalSummaryTableResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.11/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.11/setup.py` & `mypy-boto3-dynamodb-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDB 1.28.11 service generated with mypy-boto3-builder"
-        " 7.15.1"
+        "Type annotations for boto3.DynamoDB 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

