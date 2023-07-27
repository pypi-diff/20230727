# Comparing `tmp/mypy-boto3-iotanalytics-1.28.0.tar.gz` & `tmp/mypy-boto3-iotanalytics-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotanalytics-1.28.0.tar", last modified: Thu Jul  6 20:59:47 2023, max compression
+gzip compressed data, was "mypy-boto3-iotanalytics-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
```

## Comparing `mypy-boto3-iotanalytics-1.28.0.tar` & `mypy-boto3-iotanalytics-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.442329 mypy-boto3-iotanalytics-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-07-06 20:59:47.442329 mypy-boto3-iotanalytics-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.434329 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-06 20:43:38.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-07-06 20:43:38.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-06 20:43:38.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-06 20:43:38.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-06 20:43:38.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-06 20:43:38.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-07-06 20:43:41.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46164 2023-07-06 20:43:40.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.438329 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-07-06 20:59:47.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:47.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:47.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:47.000000 mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:47.442329 mypy-boto3-iotanalytics-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:43:37.000000 mypy-boto3-iotanalytics-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.096484 mypy-boto3-iotanalytics-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-07-27 05:34:49.092484 mypy-boto3-iotanalytics-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.088484 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64203 2023-07-27 05:23:59.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64094 2023-07-27 05:23:59.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:58.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.092484 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:48.000000 mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.096484 mypy-boto3-iotanalytics-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:23:57.000000 mypy-boto3-iotanalytics-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotanalytics-1.28.0/LICENSE` & `mypy-boto3-iotanalytics-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.12/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTAnalytics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-iotanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,154 +344,203 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotanalytics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
+    AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
+    ChannelActivityOutputTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
+    CustomerManagedChannelS3StorageOutputTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
-    RetentionPeriodTypeDef,
+    RetentionPeriodOutputTypeDef,
+    ColumnOutputTypeDef,
     ColumnTypeDef,
+    ResourceConfigurationOutputTypeDef,
     ResourceConfigurationTypeDef,
+    RetentionPeriodTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
     CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
     CreatePipelineResponseTypeDef,
+    CustomerManagedDatastoreS3StorageOutputTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
+    IotEventsDestinationConfigurationOutputTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
+    DatasetContentVersionValueOutputTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
+    ScheduleOutputTypeDef,
+    TriggeringDatasetOutputTypeDef,
     ScheduleTypeDef,
     TriggeringDatasetTypeDef,
+    VersioningConfigurationOutputTypeDef,
+    DatastoreActivityOutputTypeDef,
     DatastoreActivityTypeDef,
+    IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
+    PartitionOutputTypeDef,
+    TimestampPartitionOutputTypeDef,
     PartitionTypeDef,
     TimestampPartitionTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteDatasetContentRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeletePipelineRequestRequestTypeDef,
+    DeltaTimeOutputTypeDef,
+    DeltaTimeSessionWindowConfigurationOutputTypeDef,
     DeltaTimeSessionWindowConfigurationTypeDef,
     DeltaTimeTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsOutputTypeDef,
     DescribePipelineRequestRequestTypeDef,
+    DeviceRegistryEnrichActivityOutputTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
+    DeviceShadowEnrichActivityOutputTypeDef,
     DeviceShadowEnrichActivityTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterActivityOutputTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
+    GlueConfigurationOutputTypeDef,
     GlueConfigurationTypeDef,
+    LambdaActivityOutputTypeDef,
     LambdaActivityTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    LoggingOptionsTypeDef,
+    MathActivityOutputTypeDef,
     MathActivityTypeDef,
+    OutputFileUriValueOutputTypeDef,
     OutputFileUriValueTypeDef,
     PaginatorConfigTypeDef,
+    RemoveAttributesActivityOutputTypeDef,
+    SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
     ResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchPutMessageRequestRequestTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
+    DatasetTriggerOutputTypeDef,
     DatasetTriggerTypeDef,
+    DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
+    DatastorePartitionOutputTypeDef,
     DatastorePartitionTypeDef,
+    QueryFilterOutputTypeDef,
+    LateDataRuleConfigurationOutputTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
+    VariableOutputTypeDef,
     VariableTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
-    ChannelSummaryTypeDef,
     ChannelTypeDef,
+    ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageSummaryTypeDef,
     DatastoreStorageTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
+    LateDataRuleOutputTypeDef,
     LateDataRuleTypeDef,
     SqlQueryDatasetActionTypeDef,
+    DatasetContentDeliveryDestinationOutputTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
+    ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
-    ListChannelsResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
     DatastoreSummaryTypeDef,
+    DatasetContentDeliveryRuleOutputTypeDef,
     DatasetContentDeliveryRuleTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
-    CreateDatastoreRequestRequestTypeDef,
     DatastoreTypeDef,
+    CreateDatastoreRequestRequestTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityTypeDef:
+def get_structure() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotanalytics-1.28.0/README.md` & `mypy-boto3-iotanalytics-1.28.12/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-iotanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,154 +312,203 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotanalytics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
+    AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
+    ChannelActivityOutputTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
+    CustomerManagedChannelS3StorageOutputTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
-    RetentionPeriodTypeDef,
+    RetentionPeriodOutputTypeDef,
+    ColumnOutputTypeDef,
     ColumnTypeDef,
+    ResourceConfigurationOutputTypeDef,
     ResourceConfigurationTypeDef,
+    RetentionPeriodTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
     CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
     CreatePipelineResponseTypeDef,
+    CustomerManagedDatastoreS3StorageOutputTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
+    IotEventsDestinationConfigurationOutputTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
+    DatasetContentVersionValueOutputTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
+    ScheduleOutputTypeDef,
+    TriggeringDatasetOutputTypeDef,
     ScheduleTypeDef,
     TriggeringDatasetTypeDef,
+    VersioningConfigurationOutputTypeDef,
+    DatastoreActivityOutputTypeDef,
     DatastoreActivityTypeDef,
+    IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
+    PartitionOutputTypeDef,
+    TimestampPartitionOutputTypeDef,
     PartitionTypeDef,
     TimestampPartitionTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteDatasetContentRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeletePipelineRequestRequestTypeDef,
+    DeltaTimeOutputTypeDef,
+    DeltaTimeSessionWindowConfigurationOutputTypeDef,
     DeltaTimeSessionWindowConfigurationTypeDef,
     DeltaTimeTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsOutputTypeDef,
     DescribePipelineRequestRequestTypeDef,
+    DeviceRegistryEnrichActivityOutputTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
+    DeviceShadowEnrichActivityOutputTypeDef,
     DeviceShadowEnrichActivityTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterActivityOutputTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
+    GlueConfigurationOutputTypeDef,
     GlueConfigurationTypeDef,
+    LambdaActivityOutputTypeDef,
     LambdaActivityTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    LoggingOptionsTypeDef,
+    MathActivityOutputTypeDef,
     MathActivityTypeDef,
+    OutputFileUriValueOutputTypeDef,
     OutputFileUriValueTypeDef,
     PaginatorConfigTypeDef,
+    RemoveAttributesActivityOutputTypeDef,
+    SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
     ResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchPutMessageRequestRequestTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
+    DatasetTriggerOutputTypeDef,
     DatasetTriggerTypeDef,
+    DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
+    DatastorePartitionOutputTypeDef,
     DatastorePartitionTypeDef,
+    QueryFilterOutputTypeDef,
+    LateDataRuleConfigurationOutputTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
+    VariableOutputTypeDef,
     VariableTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
-    ChannelSummaryTypeDef,
     ChannelTypeDef,
+    ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageSummaryTypeDef,
     DatastoreStorageTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
+    LateDataRuleOutputTypeDef,
     LateDataRuleTypeDef,
     SqlQueryDatasetActionTypeDef,
+    DatasetContentDeliveryDestinationOutputTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
+    ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
-    ListChannelsResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
     DatastoreSummaryTypeDef,
+    DatasetContentDeliveryRuleOutputTypeDef,
     DatasetContentDeliveryRuleTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
-    CreateDatastoreRequestRequestTypeDef,
     DatastoreTypeDef,
+    CreateDatastoreRequestRequestTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityTypeDef:
+def get_structure() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/__init__.py` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/__init__.pyi` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/__main__.py` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTAnalytics 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTAnalytics 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics\nOther"
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

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/client.py` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/client.pyi` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/literals.py` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,15 @@
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
@@ -258,26 +259,28 @@
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

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/literals.pyi` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
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
@@ -256,26 +257,28 @@
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

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/paginator.py` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/paginator.pyi` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/type_defs.py` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotanalytics.type_defs import AddAttributesActivityTypeDef
+    from mypy_boto3_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
 
-    data: AddAttributesActivityTypeDef = {...}
+    data: AddAttributesActivityOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -35,152 +35,223 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "MessageTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
+    "ChannelActivityOutputTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
+    "CustomerManagedChannelS3StorageOutputTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
-    "RetentionPeriodTypeDef",
+    "RetentionPeriodOutputTypeDef",
+    "ColumnOutputTypeDef",
     "ColumnTypeDef",
+    "ResourceConfigurationOutputTypeDef",
     "ResourceConfigurationTypeDef",
+    "RetentionPeriodTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
     "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
     "CreatePipelineResponseTypeDef",
+    "CustomerManagedDatastoreS3StorageOutputTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
+    "IotEventsDestinationConfigurationOutputTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
+    "DatasetContentVersionValueOutputTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
+    "ScheduleOutputTypeDef",
+    "TriggeringDatasetOutputTypeDef",
     "ScheduleTypeDef",
     "TriggeringDatasetTypeDef",
+    "VersioningConfigurationOutputTypeDef",
+    "DatastoreActivityOutputTypeDef",
     "DatastoreActivityTypeDef",
+    "IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
+    "PartitionOutputTypeDef",
+    "TimestampPartitionOutputTypeDef",
     "PartitionTypeDef",
     "TimestampPartitionTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteDatasetContentRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
     "DeletePipelineRequestRequestTypeDef",
+    "DeltaTimeOutputTypeDef",
+    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
     "DeltaTimeSessionWindowConfigurationTypeDef",
     "DeltaTimeTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
-    "LoggingOptionsTypeDef",
+    "LoggingOptionsOutputTypeDef",
     "DescribePipelineRequestRequestTypeDef",
+    "DeviceRegistryEnrichActivityOutputTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
+    "DeviceShadowEnrichActivityOutputTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "FilterActivityOutputTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
+    "GlueConfigurationOutputTypeDef",
     "GlueConfigurationTypeDef",
+    "LambdaActivityOutputTypeDef",
     "LambdaActivityTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "LoggingOptionsTypeDef",
+    "MathActivityOutputTypeDef",
     "MathActivityTypeDef",
+    "OutputFileUriValueOutputTypeDef",
     "OutputFileUriValueTypeDef",
     "PaginatorConfigTypeDef",
+    "RemoveAttributesActivityOutputTypeDef",
+    "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataRequestRequestTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "BatchPutMessageRequestRequestTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
+    "ChannelStorageOutputTypeDef",
     "ChannelStorageSummaryTypeDef",
     "ChannelStorageTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
+    "DatasetTriggerOutputTypeDef",
     "DatasetTriggerTypeDef",
+    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
+    "DatastorePartitionOutputTypeDef",
     "DatastorePartitionTypeDef",
+    "QueryFilterOutputTypeDef",
+    "LateDataRuleConfigurationOutputTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "PutLoggingOptionsRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutLoggingOptionsRequestRequestTypeDef",
+    "VariableOutputTypeDef",
     "VariableTypeDef",
+    "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
-    "ChannelSummaryTypeDef",
     "ChannelTypeDef",
+    "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
+    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageSummaryTypeDef",
     "DatastoreStorageTypeDef",
+    "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
+    "SqlQueryDatasetActionOutputTypeDef",
+    "LateDataRuleOutputTypeDef",
     "LateDataRuleTypeDef",
     "SqlQueryDatasetActionTypeDef",
+    "DatasetContentDeliveryDestinationOutputTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
+    "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
-    "ListChannelsResponseTypeDef",
     "DescribeChannelResponseTypeDef",
+    "ListChannelsResponseTypeDef",
+    "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
     "DatastoreSummaryTypeDef",
+    "DatasetContentDeliveryRuleOutputTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
+    "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
-    "CreateDatastoreRequestRequestTypeDef",
     "DatastoreTypeDef",
+    "CreateDatastoreRequestRequestTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
+_RequiredAddAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredAddAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": Dict[str, str],
+    },
+)
+_OptionalAddAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalAddAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class AddAttributesActivityOutputTypeDef(
+    _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -221,14 +292,36 @@
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
 
+_RequiredChannelActivityOutputTypeDef = TypedDict(
+    "_RequiredChannelActivityOutputTypeDef",
+    {
+        "name": str,
+        "channelName": str,
+    },
+)
+_OptionalChannelActivityOutputTypeDef = TypedDict(
+    "_OptionalChannelActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class ChannelActivityOutputTypeDef(
+    _RequiredChannelActivityOutputTypeDef, _OptionalChannelActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredChannelActivityTypeDef = TypedDict(
     "_RequiredChannelActivityTypeDef",
     {
         "name": str,
         "channelName": str,
     },
 )
@@ -258,14 +351,37 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
+_RequiredCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
+    "_RequiredCustomerManagedChannelS3StorageOutputTypeDef",
+    {
+        "bucket": str,
+        "roleArn": str,
+    },
+)
+_OptionalCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
+    "_OptionalCustomerManagedChannelS3StorageOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+
+class CustomerManagedChannelS3StorageOutputTypeDef(
+    _RequiredCustomerManagedChannelS3StorageOutputTypeDef,
+    _OptionalCustomerManagedChannelS3StorageOutputTypeDef,
+):
+    pass
+
+
 CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -290,39 +406,64 @@
 
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
     total=False,
 )
 
+ColumnOutputTypeDef = TypedDict(
+    "ColumnOutputTypeDef",
+    {
+        "name": str,
+        "type": str,
+    },
+)
+
 ColumnTypeDef = TypedDict(
     "ColumnTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
+ResourceConfigurationOutputTypeDef = TypedDict(
+    "ResourceConfigurationOutputTypeDef",
+    {
+        "computeType": ComputeTypeType,
+        "volumeSizeInGB": int,
+    },
+)
+
 ResourceConfigurationTypeDef = TypedDict(
     "ResourceConfigurationTypeDef",
     {
         "computeType": ComputeTypeType,
         "volumeSizeInGB": int,
     },
 )
 
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
+    {
+        "unlimited": bool,
+        "numberOfDays": int,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -371,14 +512,37 @@
     {
         "pipelineName": str,
         "pipelineArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "bucket": str,
+        "roleArn": str,
+    },
+)
+_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+
+class CustomerManagedDatastoreS3StorageOutputTypeDef(
+    _RequiredCustomerManagedDatastoreS3StorageOutputTypeDef,
+    _OptionalCustomerManagedDatastoreS3StorageOutputTypeDef,
+):
+    pass
+
+
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -413,14 +577,22 @@
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
 )
 
+IotEventsDestinationConfigurationOutputTypeDef = TypedDict(
+    "IotEventsDestinationConfigurationOutputTypeDef",
+    {
+        "inputName": str,
+        "roleArn": str,
+    },
+)
+
 IotEventsDestinationConfigurationTypeDef = TypedDict(
     "IotEventsDestinationConfigurationTypeDef",
     {
         "inputName": str,
         "roleArn": str,
     },
 )
@@ -430,14 +602,21 @@
     {
         "state": DatasetContentStateType,
         "reason": str,
     },
     total=False,
 )
 
+DatasetContentVersionValueOutputTypeDef = TypedDict(
+    "DatasetContentVersionValueOutputTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+
 DatasetContentVersionValueTypeDef = TypedDict(
     "DatasetContentVersionValueTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -446,14 +625,29 @@
     {
         "entryName": str,
         "dataURI": str,
     },
     total=False,
 )
 
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "expression": str,
+    },
+    total=False,
+)
+
+TriggeringDatasetOutputTypeDef = TypedDict(
+    "TriggeringDatasetOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "expression": str,
     },
     total=False,
 )
@@ -461,22 +655,61 @@
 TriggeringDatasetTypeDef = TypedDict(
     "TriggeringDatasetTypeDef",
     {
         "name": str,
     },
 )
 
+VersioningConfigurationOutputTypeDef = TypedDict(
+    "VersioningConfigurationOutputTypeDef",
+    {
+        "unlimited": bool,
+        "maxVersions": int,
+    },
+    total=False,
+)
+
+DatastoreActivityOutputTypeDef = TypedDict(
+    "DatastoreActivityOutputTypeDef",
+    {
+        "name": str,
+        "datastoreName": str,
+    },
+)
+
 DatastoreActivityTypeDef = TypedDict(
     "DatastoreActivityTypeDef",
     {
         "name": str,
         "datastoreName": str,
     },
 )
 
+_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "bucket": str,
+    },
+)
+_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+
+class IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef(
+    _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
+    _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
+):
+    pass
+
+
 IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -500,14 +733,42 @@
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
 
+PartitionOutputTypeDef = TypedDict(
+    "PartitionOutputTypeDef",
+    {
+        "attributeName": str,
+    },
+)
+
+_RequiredTimestampPartitionOutputTypeDef = TypedDict(
+    "_RequiredTimestampPartitionOutputTypeDef",
+    {
+        "attributeName": str,
+    },
+)
+_OptionalTimestampPartitionOutputTypeDef = TypedDict(
+    "_OptionalTimestampPartitionOutputTypeDef",
+    {
+        "timestampFormat": str,
+    },
+    total=False,
+)
+
+
+class TimestampPartitionOutputTypeDef(
+    _RequiredTimestampPartitionOutputTypeDef, _OptionalTimestampPartitionOutputTypeDef
+):
+    pass
+
+
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -578,14 +839,29 @@
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
+DeltaTimeOutputTypeDef = TypedDict(
+    "DeltaTimeOutputTypeDef",
+    {
+        "offsetSeconds": int,
+        "timeExpression": str,
+    },
+)
+
+DeltaTimeSessionWindowConfigurationOutputTypeDef = TypedDict(
+    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
+    {
+        "timeoutInMinutes": int,
+    },
+)
+
 DeltaTimeSessionWindowConfigurationTypeDef = TypedDict(
     "DeltaTimeSessionWindowConfigurationTypeDef",
     {
         "timeoutInMinutes": int,
     },
 )
 
@@ -642,30 +918,55 @@
 
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
 
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
+LoggingOptionsOutputTypeDef = TypedDict(
+    "LoggingOptionsOutputTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
 )
 
 DescribePipelineRequestRequestTypeDef = TypedDict(
     "DescribePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
+_RequiredDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
+    "_RequiredDeviceRegistryEnrichActivityOutputTypeDef",
+    {
+        "name": str,
+        "attribute": str,
+        "thingName": str,
+        "roleArn": str,
+    },
+)
+_OptionalDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
+    "_OptionalDeviceRegistryEnrichActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class DeviceRegistryEnrichActivityOutputTypeDef(
+    _RequiredDeviceRegistryEnrichActivityOutputTypeDef,
+    _OptionalDeviceRegistryEnrichActivityOutputTypeDef,
+):
+    pass
+
+
 _RequiredDeviceRegistryEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceRegistryEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -682,14 +983,39 @@
 
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
 
+_RequiredDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
+    "_RequiredDeviceShadowEnrichActivityOutputTypeDef",
+    {
+        "name": str,
+        "attribute": str,
+        "thingName": str,
+        "roleArn": str,
+    },
+)
+_OptionalDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
+    "_OptionalDeviceShadowEnrichActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class DeviceShadowEnrichActivityOutputTypeDef(
+    _RequiredDeviceShadowEnrichActivityOutputTypeDef,
+    _OptionalDeviceShadowEnrichActivityOutputTypeDef,
+):
+    pass
+
+
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -713,14 +1039,36 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFilterActivityOutputTypeDef = TypedDict(
+    "_RequiredFilterActivityOutputTypeDef",
+    {
+        "name": str,
+        "filter": str,
+    },
+)
+_OptionalFilterActivityOutputTypeDef = TypedDict(
+    "_OptionalFilterActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class FilterActivityOutputTypeDef(
+    _RequiredFilterActivityOutputTypeDef, _OptionalFilterActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -754,22 +1102,53 @@
 
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
 
+GlueConfigurationOutputTypeDef = TypedDict(
+    "GlueConfigurationOutputTypeDef",
+    {
+        "tableName": str,
+        "databaseName": str,
+    },
+)
+
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
+_RequiredLambdaActivityOutputTypeDef = TypedDict(
+    "_RequiredLambdaActivityOutputTypeDef",
+    {
+        "name": str,
+        "lambdaName": str,
+        "batchSize": int,
+    },
+)
+_OptionalLambdaActivityOutputTypeDef = TypedDict(
+    "_OptionalLambdaActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class LambdaActivityOutputTypeDef(
+    _RequiredLambdaActivityOutputTypeDef, _OptionalLambdaActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredLambdaActivityTypeDef = TypedDict(
     "_RequiredLambdaActivityTypeDef",
     {
         "name": str,
         "lambdaName": str,
         "batchSize": int,
     },
@@ -907,14 +1286,54 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
+    {
+        "roleArn": str,
+        "level": Literal["ERROR"],
+        "enabled": bool,
+    },
+)
+
+_RequiredMathActivityOutputTypeDef = TypedDict(
+    "_RequiredMathActivityOutputTypeDef",
+    {
+        "name": str,
+        "attribute": str,
+        "math": str,
+    },
+)
+_OptionalMathActivityOutputTypeDef = TypedDict(
+    "_OptionalMathActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class MathActivityOutputTypeDef(
+    _RequiredMathActivityOutputTypeDef, _OptionalMathActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredMathActivityTypeDef = TypedDict(
     "_RequiredMathActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "math": str,
     },
@@ -928,14 +1347,21 @@
 )
 
 
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
 
+OutputFileUriValueOutputTypeDef = TypedDict(
+    "OutputFileUriValueOutputTypeDef",
+    {
+        "fileName": str,
+    },
+)
+
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
@@ -945,14 +1371,58 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredRemoveAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalRemoveAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class RemoveAttributesActivityOutputTypeDef(
+    _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
+):
+    pass
+
+
+_RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredSelectAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalSelectAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class SelectAttributesActivityOutputTypeDef(
+    _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -1122,14 +1592,23 @@
     "DatastoreStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
 
+ChannelStorageOutputTypeDef = TypedDict(
+    "ChannelStorageOutputTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageOutputTypeDef,
+    },
+    total=False,
+)
+
 ChannelStorageSummaryTypeDef = TypedDict(
     "ChannelStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
     },
     total=False,
@@ -1145,53 +1624,53 @@
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SchemaDefinitionTypeDef = TypedDict(
-    "SchemaDefinitionTypeDef",
+SchemaDefinitionOutputTypeDef = TypedDict(
+    "SchemaDefinitionOutputTypeDef",
     {
-        "columns": Sequence[ColumnTypeDef],
+        "columns": List[ColumnOutputTypeDef],
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+SchemaDefinitionTypeDef = TypedDict(
+    "SchemaDefinitionTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "columns": Sequence[ColumnTypeDef],
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
@@ -1216,23 +1695,39 @@
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatasetTriggerOutputTypeDef = TypedDict(
+    "DatasetTriggerOutputTypeDef",
+    {
+        "schedule": ScheduleOutputTypeDef,
+        "dataset": TriggeringDatasetOutputTypeDef,
+    },
+    total=False,
+)
+
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
         "dataset": TriggeringDatasetTypeDef,
     },
     total=False,
 )
 
+DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef = TypedDict(
+    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
+    {
+        "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
+    },
+)
+
 DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     },
     total=False,
 )
@@ -1240,23 +1735,48 @@
 DatastoreIotSiteWiseMultiLayerStorageTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     },
 )
 
+DatastorePartitionOutputTypeDef = TypedDict(
+    "DatastorePartitionOutputTypeDef",
+    {
+        "attributePartition": PartitionOutputTypeDef,
+        "timestampPartition": TimestampPartitionOutputTypeDef,
+    },
+    total=False,
+)
+
 DatastorePartitionTypeDef = TypedDict(
     "DatastorePartitionTypeDef",
     {
         "attributePartition": PartitionTypeDef,
         "timestampPartition": TimestampPartitionTypeDef,
     },
     total=False,
 )
 
+QueryFilterOutputTypeDef = TypedDict(
+    "QueryFilterOutputTypeDef",
+    {
+        "deltaTime": DeltaTimeOutputTypeDef,
+    },
+    total=False,
+)
+
+LateDataRuleConfigurationOutputTypeDef = TypedDict(
+    "LateDataRuleConfigurationOutputTypeDef",
+    {
+        "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LateDataRuleConfigurationTypeDef = TypedDict(
     "LateDataRuleConfigurationTypeDef",
     {
         "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationTypeDef,
     },
     total=False,
 )
@@ -1268,25 +1788,42 @@
     },
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
+        "loggingOptions": LoggingOptionsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutLoggingOptionsRequestRequestTypeDef = TypedDict(
-    "PutLoggingOptionsRequestRequestTypeDef",
+_RequiredS3DestinationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationConfigurationOutputTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
+        "bucket": str,
+        "key": str,
+        "roleArn": str,
     },
 )
+_OptionalS3DestinationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationConfigurationOutputTypeDef",
+    {
+        "glueConfiguration": GlueConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class S3DestinationConfigurationOutputTypeDef(
+    _RequiredS3DestinationConfigurationOutputTypeDef,
+    _OptionalS3DestinationConfigurationOutputTypeDef,
+):
+    pass
+
 
 _RequiredS3DestinationConfigurationTypeDef = TypedDict(
     "_RequiredS3DestinationConfigurationTypeDef",
     {
         "bucket": str,
         "key": str,
         "roleArn": str,
@@ -1303,14 +1840,51 @@
 
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
+    {
+        "loggingOptions": LoggingOptionsTypeDef,
+    },
+)
+
+_RequiredVariableOutputTypeDef = TypedDict(
+    "_RequiredVariableOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalVariableOutputTypeDef = TypedDict(
+    "_OptionalVariableOutputTypeDef",
+    {
+        "stringValue": str,
+        "doubleValue": float,
+        "datasetContentVersionValue": DatasetContentVersionValueOutputTypeDef,
+        "outputFileUriValue": OutputFileUriValueOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VariableOutputTypeDef(_RequiredVariableOutputTypeDef, _OptionalVariableOutputTypeDef):
+    pass
+
+
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalVariableTypeDef = TypedDict(
@@ -1325,14 +1899,31 @@
 )
 
 
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
 
+PipelineActivityOutputTypeDef = TypedDict(
+    "PipelineActivityOutputTypeDef",
+    {
+        "channel": ChannelActivityOutputTypeDef,
+        "lambda": LambdaActivityOutputTypeDef,
+        "datastore": DatastoreActivityOutputTypeDef,
+        "addAttributes": AddAttributesActivityOutputTypeDef,
+        "removeAttributes": RemoveAttributesActivityOutputTypeDef,
+        "selectAttributes": SelectAttributesActivityOutputTypeDef,
+        "filter": FilterActivityOutputTypeDef,
+        "math": MathActivityOutputTypeDef,
+        "deviceRegistryEnrich": DeviceRegistryEnrichActivityOutputTypeDef,
+        "deviceShadowEnrich": DeviceShadowEnrichActivityOutputTypeDef,
+    },
+    total=False,
+)
+
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityTypeDef,
@@ -1353,35 +1944,35 @@
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
     {
-        "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
+        "name": str,
+        "storage": ChannelStorageOutputTypeDef,
+        "arn": str,
         "status": ChannelStatusType,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
-ChannelTypeDef = TypedDict(
-    "ChannelTypeDef",
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
     {
-        "name": str,
-        "storage": ChannelStorageTypeDef,
-        "arn": str,
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
         "status": ChannelStatusType,
-        "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
@@ -1426,14 +2017,22 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
+ParquetConfigurationOutputTypeDef = TypedDict(
+    "ParquetConfigurationOutputTypeDef",
+    {
+        "schemaDefinition": SchemaDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 ParquetConfigurationTypeDef = TypedDict(
     "ParquetConfigurationTypeDef",
     {
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1450,20 +2049,30 @@
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
         "status": DatasetStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
-        "triggers": List[DatasetTriggerTypeDef],
+        "triggers": List[DatasetTriggerOutputTypeDef],
         "actions": List[DatasetActionSummaryTypeDef],
     },
     total=False,
 )
 
+DatastoreStorageOutputTypeDef = TypedDict(
+    "DatastoreStorageOutputTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedDatastoreS3StorageOutputTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
+    },
+    total=False,
+)
+
 DatastoreStorageSummaryTypeDef = TypedDict(
     "DatastoreStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
@@ -1476,22 +2085,72 @@
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsOutputTypeDef = TypedDict(
+    "DatastorePartitionsOutputTypeDef",
+    {
+        "partitions": List[DatastorePartitionOutputTypeDef],
+    },
+    total=False,
+)
+
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
 
+_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredSqlQueryDatasetActionOutputTypeDef",
+    {
+        "sqlQuery": str,
+    },
+)
+_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalSqlQueryDatasetActionOutputTypeDef",
+    {
+        "filters": List[QueryFilterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class SqlQueryDatasetActionOutputTypeDef(
+    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
+):
+    pass
+
+
+_RequiredLateDataRuleOutputTypeDef = TypedDict(
+    "_RequiredLateDataRuleOutputTypeDef",
+    {
+        "ruleConfiguration": LateDataRuleConfigurationOutputTypeDef,
+    },
+)
+_OptionalLateDataRuleOutputTypeDef = TypedDict(
+    "_OptionalLateDataRuleOutputTypeDef",
+    {
+        "ruleName": str,
+    },
+    total=False,
+)
+
+
+class LateDataRuleOutputTypeDef(
+    _RequiredLateDataRuleOutputTypeDef, _OptionalLateDataRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredLateDataRuleTypeDef = TypedDict(
     "_RequiredLateDataRuleTypeDef",
     {
         "ruleConfiguration": LateDataRuleConfigurationTypeDef,
     },
 )
 _OptionalLateDataRuleTypeDef = TypedDict(
@@ -1524,23 +2183,55 @@
 
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
 
+DatasetContentDeliveryDestinationOutputTypeDef = TypedDict(
+    "DatasetContentDeliveryDestinationOutputTypeDef",
+    {
+        "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationOutputTypeDef,
+        "s3DestinationConfiguration": S3DestinationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredContainerDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionOutputTypeDef",
+    {
+        "image": str,
+        "executionRoleArn": str,
+        "resourceConfiguration": ResourceConfigurationOutputTypeDef,
+    },
+)
+_OptionalContainerDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionOutputTypeDef",
+    {
+        "variables": List[VariableOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ContainerDatasetActionOutputTypeDef(
+    _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
+):
+    pass
+
+
 _RequiredContainerDatasetActionTypeDef = TypedDict(
     "_RequiredContainerDatasetActionTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
@@ -1556,14 +2247,27 @@
 
 class ContainerDatasetActionTypeDef(
     _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
 
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "activities": List[PipelineActivityOutputTypeDef],
+        "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineActivities": Sequence[PipelineActivityTypeDef],
     },
 )
@@ -1578,27 +2282,14 @@
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "activities": List[PipelineActivityTypeDef],
-        "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-    },
-    total=False,
-)
-
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
         "payloads": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
 )
@@ -1616,30 +2307,39 @@
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "statistics": ChannelStatisticsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
+FileFormatConfigurationOutputTypeDef = TypedDict(
+    "FileFormatConfigurationOutputTypeDef",
     {
-        "channel": ChannelTypeDef,
-        "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jsonConfiguration": Dict[str, Any],
+        "parquetConfiguration": ParquetConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
         "parquetConfiguration": ParquetConfigurationTypeDef,
@@ -1662,19 +2362,41 @@
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
-        "datastorePartitions": DatastorePartitionsTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
+    "_RequiredDatasetContentDeliveryRuleOutputTypeDef",
+    {
+        "destination": DatasetContentDeliveryDestinationOutputTypeDef,
+    },
+)
+_OptionalDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
+    "_OptionalDatasetContentDeliveryRuleOutputTypeDef",
+    {
+        "entryName": str,
     },
     total=False,
 )
 
+
+class DatasetContentDeliveryRuleOutputTypeDef(
+    _RequiredDatasetContentDeliveryRuleOutputTypeDef,
+    _OptionalDatasetContentDeliveryRuleOutputTypeDef,
+):
+    pass
+
+
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
@@ -1688,14 +2410,24 @@
 
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
 
+DatasetActionOutputTypeDef = TypedDict(
+    "DatasetActionOutputTypeDef",
+    {
+        "actionName": str,
+        "queryAction": SqlQueryDatasetActionOutputTypeDef,
+        "containerAction": ContainerDatasetActionOutputTypeDef,
+    },
+    total=False,
+)
+
 DatasetActionTypeDef = TypedDict(
     "DatasetActionTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionTypeDef,
         "containerAction": ContainerDatasetActionTypeDef,
     },
@@ -1706,14 +2438,31 @@
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatastoreTypeDef = TypedDict(
+    "DatastoreTypeDef",
+    {
+        "name": str,
+        "storage": DatastoreStorageOutputTypeDef,
+        "arn": str,
+        "status": DatastoreStatusType,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+        "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1731,31 +2480,14 @@
 
 class CreateDatastoreRequestRequestTypeDef(
     _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
 
-DatastoreTypeDef = TypedDict(
-    "DatastoreTypeDef",
-    {
-        "name": str,
-        "storage": DatastoreStorageTypeDef,
-        "arn": str,
-        "status": DatastoreStatusType,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
-        "fileFormatConfiguration": FileFormatConfigurationTypeDef,
-        "datastorePartitions": DatastorePartitionsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1780,14 +2512,32 @@
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "actions": List[DatasetActionOutputTypeDef],
+        "triggers": List[DatasetTriggerOutputTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleOutputTypeDef],
+        "status": DatasetStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "versioningConfiguration": VersioningConfigurationOutputTypeDef,
+        "lateDataRules": List[LateDataRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
         "actions": Sequence[DatasetActionTypeDef],
     },
 )
@@ -1807,32 +2557,14 @@
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "actions": List[DatasetActionTypeDef],
-        "triggers": List[DatasetTriggerTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
-        "status": DatasetStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "versioningConfiguration": VersioningConfigurationTypeDef,
-        "lateDataRules": List[LateDataRuleTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
         "actions": Sequence[DatasetActionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics/type_defs.pyi` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotanalytics.type_defs import AddAttributesActivityTypeDef
+    from mypy_boto3_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
 
-    data: AddAttributesActivityTypeDef = {...}
+    data: AddAttributesActivityOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -34,152 +34,221 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "MessageTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
+    "ChannelActivityOutputTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
+    "CustomerManagedChannelS3StorageOutputTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
-    "RetentionPeriodTypeDef",
+    "RetentionPeriodOutputTypeDef",
+    "ColumnOutputTypeDef",
     "ColumnTypeDef",
+    "ResourceConfigurationOutputTypeDef",
     "ResourceConfigurationTypeDef",
+    "RetentionPeriodTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
     "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
     "CreatePipelineResponseTypeDef",
+    "CustomerManagedDatastoreS3StorageOutputTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
+    "IotEventsDestinationConfigurationOutputTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
+    "DatasetContentVersionValueOutputTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
+    "ScheduleOutputTypeDef",
+    "TriggeringDatasetOutputTypeDef",
     "ScheduleTypeDef",
     "TriggeringDatasetTypeDef",
+    "VersioningConfigurationOutputTypeDef",
+    "DatastoreActivityOutputTypeDef",
     "DatastoreActivityTypeDef",
+    "IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     "IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
+    "PartitionOutputTypeDef",
+    "TimestampPartitionOutputTypeDef",
     "PartitionTypeDef",
     "TimestampPartitionTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteDatasetContentRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
     "DeletePipelineRequestRequestTypeDef",
+    "DeltaTimeOutputTypeDef",
+    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
     "DeltaTimeSessionWindowConfigurationTypeDef",
     "DeltaTimeTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
-    "LoggingOptionsTypeDef",
+    "LoggingOptionsOutputTypeDef",
     "DescribePipelineRequestRequestTypeDef",
+    "DeviceRegistryEnrichActivityOutputTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
+    "DeviceShadowEnrichActivityOutputTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "FilterActivityOutputTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
+    "GlueConfigurationOutputTypeDef",
     "GlueConfigurationTypeDef",
+    "LambdaActivityOutputTypeDef",
     "LambdaActivityTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "LoggingOptionsTypeDef",
+    "MathActivityOutputTypeDef",
     "MathActivityTypeDef",
+    "OutputFileUriValueOutputTypeDef",
     "OutputFileUriValueTypeDef",
     "PaginatorConfigTypeDef",
+    "RemoveAttributesActivityOutputTypeDef",
+    "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataRequestRequestTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "BatchPutMessageRequestRequestTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
+    "ChannelStorageOutputTypeDef",
     "ChannelStorageSummaryTypeDef",
     "ChannelStorageTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
+    "DatasetTriggerOutputTypeDef",
     "DatasetTriggerTypeDef",
+    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
+    "DatastorePartitionOutputTypeDef",
     "DatastorePartitionTypeDef",
+    "QueryFilterOutputTypeDef",
+    "LateDataRuleConfigurationOutputTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "PutLoggingOptionsRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutLoggingOptionsRequestRequestTypeDef",
+    "VariableOutputTypeDef",
     "VariableTypeDef",
+    "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
-    "ChannelSummaryTypeDef",
     "ChannelTypeDef",
+    "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
+    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageSummaryTypeDef",
     "DatastoreStorageTypeDef",
+    "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
+    "SqlQueryDatasetActionOutputTypeDef",
+    "LateDataRuleOutputTypeDef",
     "LateDataRuleTypeDef",
     "SqlQueryDatasetActionTypeDef",
+    "DatasetContentDeliveryDestinationOutputTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
+    "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
-    "ListChannelsResponseTypeDef",
     "DescribeChannelResponseTypeDef",
+    "ListChannelsResponseTypeDef",
+    "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
     "DatastoreSummaryTypeDef",
+    "DatasetContentDeliveryRuleOutputTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
+    "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
-    "CreateDatastoreRequestRequestTypeDef",
     "DatastoreTypeDef",
+    "CreateDatastoreRequestRequestTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
+_RequiredAddAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredAddAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": Dict[str, str],
+    },
+)
+_OptionalAddAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalAddAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class AddAttributesActivityOutputTypeDef(
+    _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
+):
+    pass
+
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -218,14 +287,34 @@
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
 
+_RequiredChannelActivityOutputTypeDef = TypedDict(
+    "_RequiredChannelActivityOutputTypeDef",
+    {
+        "name": str,
+        "channelName": str,
+    },
+)
+_OptionalChannelActivityOutputTypeDef = TypedDict(
+    "_OptionalChannelActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class ChannelActivityOutputTypeDef(
+    _RequiredChannelActivityOutputTypeDef, _OptionalChannelActivityOutputTypeDef
+):
+    pass
+
 _RequiredChannelActivityTypeDef = TypedDict(
     "_RequiredChannelActivityTypeDef",
     {
         "name": str,
         "channelName": str,
     },
 )
@@ -253,14 +342,35 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
+_RequiredCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
+    "_RequiredCustomerManagedChannelS3StorageOutputTypeDef",
+    {
+        "bucket": str,
+        "roleArn": str,
+    },
+)
+_OptionalCustomerManagedChannelS3StorageOutputTypeDef = TypedDict(
+    "_OptionalCustomerManagedChannelS3StorageOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+class CustomerManagedChannelS3StorageOutputTypeDef(
+    _RequiredCustomerManagedChannelS3StorageOutputTypeDef,
+    _OptionalCustomerManagedChannelS3StorageOutputTypeDef,
+):
+    pass
+
 CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedChannelS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -283,39 +393,64 @@
 )
 
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
     total=False,
 )
 
+ColumnOutputTypeDef = TypedDict(
+    "ColumnOutputTypeDef",
+    {
+        "name": str,
+        "type": str,
+    },
+)
+
 ColumnTypeDef = TypedDict(
     "ColumnTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
+ResourceConfigurationOutputTypeDef = TypedDict(
+    "ResourceConfigurationOutputTypeDef",
+    {
+        "computeType": ComputeTypeType,
+        "volumeSizeInGB": int,
+    },
+)
+
 ResourceConfigurationTypeDef = TypedDict(
     "ResourceConfigurationTypeDef",
     {
         "computeType": ComputeTypeType,
         "volumeSizeInGB": int,
     },
 )
 
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
+    {
+        "unlimited": bool,
+        "numberOfDays": int,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -362,14 +497,35 @@
     {
         "pipelineName": str,
         "pipelineArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_RequiredCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "bucket": str,
+        "roleArn": str,
+    },
+)
+_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_OptionalCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+class CustomerManagedDatastoreS3StorageOutputTypeDef(
+    _RequiredCustomerManagedDatastoreS3StorageOutputTypeDef,
+    _OptionalCustomerManagedDatastoreS3StorageOutputTypeDef,
+):
+    pass
+
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -402,14 +558,22 @@
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
 )
 
+IotEventsDestinationConfigurationOutputTypeDef = TypedDict(
+    "IotEventsDestinationConfigurationOutputTypeDef",
+    {
+        "inputName": str,
+        "roleArn": str,
+    },
+)
+
 IotEventsDestinationConfigurationTypeDef = TypedDict(
     "IotEventsDestinationConfigurationTypeDef",
     {
         "inputName": str,
         "roleArn": str,
     },
 )
@@ -419,14 +583,21 @@
     {
         "state": DatasetContentStateType,
         "reason": str,
     },
     total=False,
 )
 
+DatasetContentVersionValueOutputTypeDef = TypedDict(
+    "DatasetContentVersionValueOutputTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+
 DatasetContentVersionValueTypeDef = TypedDict(
     "DatasetContentVersionValueTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -435,14 +606,29 @@
     {
         "entryName": str,
         "dataURI": str,
     },
     total=False,
 )
 
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "expression": str,
+    },
+    total=False,
+)
+
+TriggeringDatasetOutputTypeDef = TypedDict(
+    "TriggeringDatasetOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "expression": str,
     },
     total=False,
 )
@@ -450,22 +636,59 @@
 TriggeringDatasetTypeDef = TypedDict(
     "TriggeringDatasetTypeDef",
     {
         "name": str,
     },
 )
 
+VersioningConfigurationOutputTypeDef = TypedDict(
+    "VersioningConfigurationOutputTypeDef",
+    {
+        "unlimited": bool,
+        "maxVersions": int,
+    },
+    total=False,
+)
+
+DatastoreActivityOutputTypeDef = TypedDict(
+    "DatastoreActivityOutputTypeDef",
+    {
+        "name": str,
+        "datastoreName": str,
+    },
+)
+
 DatastoreActivityTypeDef = TypedDict(
     "DatastoreActivityTypeDef",
     {
         "name": str,
         "datastoreName": str,
     },
 )
 
+_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "bucket": str,
+    },
+)
+_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef = TypedDict(
+    "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+class IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef(
+    _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
+    _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
+):
+    pass
+
 IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -487,14 +710,40 @@
 
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
+PartitionOutputTypeDef = TypedDict(
+    "PartitionOutputTypeDef",
+    {
+        "attributeName": str,
+    },
+)
+
+_RequiredTimestampPartitionOutputTypeDef = TypedDict(
+    "_RequiredTimestampPartitionOutputTypeDef",
+    {
+        "attributeName": str,
+    },
+)
+_OptionalTimestampPartitionOutputTypeDef = TypedDict(
+    "_OptionalTimestampPartitionOutputTypeDef",
+    {
+        "timestampFormat": str,
+    },
+    total=False,
+)
+
+class TimestampPartitionOutputTypeDef(
+    _RequiredTimestampPartitionOutputTypeDef, _OptionalTimestampPartitionOutputTypeDef
+):
+    pass
+
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -561,14 +810,29 @@
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
+DeltaTimeOutputTypeDef = TypedDict(
+    "DeltaTimeOutputTypeDef",
+    {
+        "offsetSeconds": int,
+        "timeExpression": str,
+    },
+)
+
+DeltaTimeSessionWindowConfigurationOutputTypeDef = TypedDict(
+    "DeltaTimeSessionWindowConfigurationOutputTypeDef",
+    {
+        "timeoutInMinutes": int,
+    },
+)
+
 DeltaTimeSessionWindowConfigurationTypeDef = TypedDict(
     "DeltaTimeSessionWindowConfigurationTypeDef",
     {
         "timeoutInMinutes": int,
     },
 )
 
@@ -621,30 +885,53 @@
 )
 
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
+LoggingOptionsOutputTypeDef = TypedDict(
+    "LoggingOptionsOutputTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
 )
 
 DescribePipelineRequestRequestTypeDef = TypedDict(
     "DescribePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 
+_RequiredDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
+    "_RequiredDeviceRegistryEnrichActivityOutputTypeDef",
+    {
+        "name": str,
+        "attribute": str,
+        "thingName": str,
+        "roleArn": str,
+    },
+)
+_OptionalDeviceRegistryEnrichActivityOutputTypeDef = TypedDict(
+    "_OptionalDeviceRegistryEnrichActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class DeviceRegistryEnrichActivityOutputTypeDef(
+    _RequiredDeviceRegistryEnrichActivityOutputTypeDef,
+    _OptionalDeviceRegistryEnrichActivityOutputTypeDef,
+):
+    pass
+
 _RequiredDeviceRegistryEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceRegistryEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -659,14 +946,37 @@
 )
 
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
+_RequiredDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
+    "_RequiredDeviceShadowEnrichActivityOutputTypeDef",
+    {
+        "name": str,
+        "attribute": str,
+        "thingName": str,
+        "roleArn": str,
+    },
+)
+_OptionalDeviceShadowEnrichActivityOutputTypeDef = TypedDict(
+    "_OptionalDeviceShadowEnrichActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class DeviceShadowEnrichActivityOutputTypeDef(
+    _RequiredDeviceShadowEnrichActivityOutputTypeDef,
+    _OptionalDeviceShadowEnrichActivityOutputTypeDef,
+):
+    pass
+
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -688,14 +998,34 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFilterActivityOutputTypeDef = TypedDict(
+    "_RequiredFilterActivityOutputTypeDef",
+    {
+        "name": str,
+        "filter": str,
+    },
+)
+_OptionalFilterActivityOutputTypeDef = TypedDict(
+    "_OptionalFilterActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class FilterActivityOutputTypeDef(
+    _RequiredFilterActivityOutputTypeDef, _OptionalFilterActivityOutputTypeDef
+):
+    pass
+
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -725,22 +1055,51 @@
 )
 
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
+GlueConfigurationOutputTypeDef = TypedDict(
+    "GlueConfigurationOutputTypeDef",
+    {
+        "tableName": str,
+        "databaseName": str,
+    },
+)
+
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
+_RequiredLambdaActivityOutputTypeDef = TypedDict(
+    "_RequiredLambdaActivityOutputTypeDef",
+    {
+        "name": str,
+        "lambdaName": str,
+        "batchSize": int,
+    },
+)
+_OptionalLambdaActivityOutputTypeDef = TypedDict(
+    "_OptionalLambdaActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class LambdaActivityOutputTypeDef(
+    _RequiredLambdaActivityOutputTypeDef, _OptionalLambdaActivityOutputTypeDef
+):
+    pass
+
 _RequiredLambdaActivityTypeDef = TypedDict(
     "_RequiredLambdaActivityTypeDef",
     {
         "name": str,
         "lambdaName": str,
         "batchSize": int,
     },
@@ -872,14 +1231,52 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
+    {
+        "roleArn": str,
+        "level": Literal["ERROR"],
+        "enabled": bool,
+    },
+)
+
+_RequiredMathActivityOutputTypeDef = TypedDict(
+    "_RequiredMathActivityOutputTypeDef",
+    {
+        "name": str,
+        "attribute": str,
+        "math": str,
+    },
+)
+_OptionalMathActivityOutputTypeDef = TypedDict(
+    "_OptionalMathActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class MathActivityOutputTypeDef(
+    _RequiredMathActivityOutputTypeDef, _OptionalMathActivityOutputTypeDef
+):
+    pass
+
 _RequiredMathActivityTypeDef = TypedDict(
     "_RequiredMathActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "math": str,
     },
@@ -891,14 +1288,21 @@
     },
     total=False,
 )
 
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
+OutputFileUriValueOutputTypeDef = TypedDict(
+    "OutputFileUriValueOutputTypeDef",
+    {
+        "fileName": str,
+    },
+)
+
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
@@ -908,14 +1312,54 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredRemoveAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalRemoveAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class RemoveAttributesActivityOutputTypeDef(
+    _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
+):
+    pass
+
+_RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredSelectAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalSelectAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class SelectAttributesActivityOutputTypeDef(
+    _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
+):
+    pass
+
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -1077,14 +1521,23 @@
     "DatastoreStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
 
+ChannelStorageOutputTypeDef = TypedDict(
+    "ChannelStorageOutputTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageOutputTypeDef,
+    },
+    total=False,
+)
+
 ChannelStorageSummaryTypeDef = TypedDict(
     "ChannelStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
     },
     total=False,
@@ -1100,53 +1553,53 @@
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SchemaDefinitionTypeDef = TypedDict(
-    "SchemaDefinitionTypeDef",
+SchemaDefinitionOutputTypeDef = TypedDict(
+    "SchemaDefinitionOutputTypeDef",
     {
-        "columns": Sequence[ColumnTypeDef],
+        "columns": List[ColumnOutputTypeDef],
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+SchemaDefinitionTypeDef = TypedDict(
+    "SchemaDefinitionTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "columns": Sequence[ColumnTypeDef],
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
@@ -1171,23 +1624,39 @@
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatasetTriggerOutputTypeDef = TypedDict(
+    "DatasetTriggerOutputTypeDef",
+    {
+        "schedule": ScheduleOutputTypeDef,
+        "dataset": TriggeringDatasetOutputTypeDef,
+    },
+    total=False,
+)
+
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
         "dataset": TriggeringDatasetTypeDef,
     },
     total=False,
 )
 
+DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef = TypedDict(
+    "DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef",
+    {
+        "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
+    },
+)
+
 DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     },
     total=False,
 )
@@ -1195,23 +1664,48 @@
 DatastoreIotSiteWiseMultiLayerStorageTypeDef = TypedDict(
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     },
 )
 
+DatastorePartitionOutputTypeDef = TypedDict(
+    "DatastorePartitionOutputTypeDef",
+    {
+        "attributePartition": PartitionOutputTypeDef,
+        "timestampPartition": TimestampPartitionOutputTypeDef,
+    },
+    total=False,
+)
+
 DatastorePartitionTypeDef = TypedDict(
     "DatastorePartitionTypeDef",
     {
         "attributePartition": PartitionTypeDef,
         "timestampPartition": TimestampPartitionTypeDef,
     },
     total=False,
 )
 
+QueryFilterOutputTypeDef = TypedDict(
+    "QueryFilterOutputTypeDef",
+    {
+        "deltaTime": DeltaTimeOutputTypeDef,
+    },
+    total=False,
+)
+
+LateDataRuleConfigurationOutputTypeDef = TypedDict(
+    "LateDataRuleConfigurationOutputTypeDef",
+    {
+        "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LateDataRuleConfigurationTypeDef = TypedDict(
     "LateDataRuleConfigurationTypeDef",
     {
         "deltaTimeSessionWindowConfiguration": DeltaTimeSessionWindowConfigurationTypeDef,
     },
     total=False,
 )
@@ -1223,26 +1717,41 @@
     },
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
+        "loggingOptions": LoggingOptionsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutLoggingOptionsRequestRequestTypeDef = TypedDict(
-    "PutLoggingOptionsRequestRequestTypeDef",
+_RequiredS3DestinationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationConfigurationOutputTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
+        "bucket": str,
+        "key": str,
+        "roleArn": str,
+    },
+)
+_OptionalS3DestinationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationConfigurationOutputTypeDef",
+    {
+        "glueConfiguration": GlueConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+class S3DestinationConfigurationOutputTypeDef(
+    _RequiredS3DestinationConfigurationOutputTypeDef,
+    _OptionalS3DestinationConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredS3DestinationConfigurationTypeDef = TypedDict(
     "_RequiredS3DestinationConfigurationTypeDef",
     {
         "bucket": str,
         "key": str,
         "roleArn": str,
     },
@@ -1256,14 +1765,49 @@
 )
 
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
+    {
+        "loggingOptions": LoggingOptionsTypeDef,
+    },
+)
+
+_RequiredVariableOutputTypeDef = TypedDict(
+    "_RequiredVariableOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalVariableOutputTypeDef = TypedDict(
+    "_OptionalVariableOutputTypeDef",
+    {
+        "stringValue": str,
+        "doubleValue": float,
+        "datasetContentVersionValue": DatasetContentVersionValueOutputTypeDef,
+        "outputFileUriValue": OutputFileUriValueOutputTypeDef,
+    },
+    total=False,
+)
+
+class VariableOutputTypeDef(_RequiredVariableOutputTypeDef, _OptionalVariableOutputTypeDef):
+    pass
+
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalVariableTypeDef = TypedDict(
@@ -1276,14 +1820,31 @@
     },
     total=False,
 )
 
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
+PipelineActivityOutputTypeDef = TypedDict(
+    "PipelineActivityOutputTypeDef",
+    {
+        "channel": ChannelActivityOutputTypeDef,
+        "lambda": LambdaActivityOutputTypeDef,
+        "datastore": DatastoreActivityOutputTypeDef,
+        "addAttributes": AddAttributesActivityOutputTypeDef,
+        "removeAttributes": RemoveAttributesActivityOutputTypeDef,
+        "selectAttributes": SelectAttributesActivityOutputTypeDef,
+        "filter": FilterActivityOutputTypeDef,
+        "math": MathActivityOutputTypeDef,
+        "deviceRegistryEnrich": DeviceRegistryEnrichActivityOutputTypeDef,
+        "deviceShadowEnrich": DeviceShadowEnrichActivityOutputTypeDef,
+    },
+    total=False,
+)
+
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityTypeDef,
@@ -1304,35 +1865,35 @@
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
     {
-        "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
+        "name": str,
+        "storage": ChannelStorageOutputTypeDef,
+        "arn": str,
         "status": ChannelStatusType,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
-ChannelTypeDef = TypedDict(
-    "ChannelTypeDef",
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
     {
-        "name": str,
-        "storage": ChannelStorageTypeDef,
-        "arn": str,
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
         "status": ChannelStatusType,
-        "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
@@ -1373,14 +1934,22 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+ParquetConfigurationOutputTypeDef = TypedDict(
+    "ParquetConfigurationOutputTypeDef",
+    {
+        "schemaDefinition": SchemaDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 ParquetConfigurationTypeDef = TypedDict(
     "ParquetConfigurationTypeDef",
     {
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1397,20 +1966,30 @@
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
         "status": DatasetStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
-        "triggers": List[DatasetTriggerTypeDef],
+        "triggers": List[DatasetTriggerOutputTypeDef],
         "actions": List[DatasetActionSummaryTypeDef],
     },
     total=False,
 )
 
+DatastoreStorageOutputTypeDef = TypedDict(
+    "DatastoreStorageOutputTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedDatastoreS3StorageOutputTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
+    },
+    total=False,
+)
+
 DatastoreStorageSummaryTypeDef = TypedDict(
     "DatastoreStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
@@ -1423,22 +2002,68 @@
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsOutputTypeDef = TypedDict(
+    "DatastorePartitionsOutputTypeDef",
+    {
+        "partitions": List[DatastorePartitionOutputTypeDef],
+    },
+    total=False,
+)
+
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
 
+_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredSqlQueryDatasetActionOutputTypeDef",
+    {
+        "sqlQuery": str,
+    },
+)
+_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalSqlQueryDatasetActionOutputTypeDef",
+    {
+        "filters": List[QueryFilterOutputTypeDef],
+    },
+    total=False,
+)
+
+class SqlQueryDatasetActionOutputTypeDef(
+    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
+):
+    pass
+
+_RequiredLateDataRuleOutputTypeDef = TypedDict(
+    "_RequiredLateDataRuleOutputTypeDef",
+    {
+        "ruleConfiguration": LateDataRuleConfigurationOutputTypeDef,
+    },
+)
+_OptionalLateDataRuleOutputTypeDef = TypedDict(
+    "_OptionalLateDataRuleOutputTypeDef",
+    {
+        "ruleName": str,
+    },
+    total=False,
+)
+
+class LateDataRuleOutputTypeDef(
+    _RequiredLateDataRuleOutputTypeDef, _OptionalLateDataRuleOutputTypeDef
+):
+    pass
+
 _RequiredLateDataRuleTypeDef = TypedDict(
     "_RequiredLateDataRuleTypeDef",
     {
         "ruleConfiguration": LateDataRuleConfigurationTypeDef,
     },
 )
 _OptionalLateDataRuleTypeDef = TypedDict(
@@ -1467,23 +2092,53 @@
 )
 
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
+DatasetContentDeliveryDestinationOutputTypeDef = TypedDict(
+    "DatasetContentDeliveryDestinationOutputTypeDef",
+    {
+        "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationOutputTypeDef,
+        "s3DestinationConfiguration": S3DestinationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredContainerDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionOutputTypeDef",
+    {
+        "image": str,
+        "executionRoleArn": str,
+        "resourceConfiguration": ResourceConfigurationOutputTypeDef,
+    },
+)
+_OptionalContainerDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionOutputTypeDef",
+    {
+        "variables": List[VariableOutputTypeDef],
+    },
+    total=False,
+)
+
+class ContainerDatasetActionOutputTypeDef(
+    _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
+):
+    pass
+
 _RequiredContainerDatasetActionTypeDef = TypedDict(
     "_RequiredContainerDatasetActionTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
@@ -1497,14 +2152,27 @@
 )
 
 class ContainerDatasetActionTypeDef(
     _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "activities": List[PipelineActivityOutputTypeDef],
+        "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineActivities": Sequence[PipelineActivityTypeDef],
     },
 )
@@ -1517,27 +2185,14 @@
 )
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "activities": List[PipelineActivityTypeDef],
-        "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-    },
-    total=False,
-)
-
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
         "payloads": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
 )
@@ -1555,30 +2210,39 @@
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "statistics": ChannelStatisticsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
+FileFormatConfigurationOutputTypeDef = TypedDict(
+    "FileFormatConfigurationOutputTypeDef",
     {
-        "channel": ChannelTypeDef,
-        "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jsonConfiguration": Dict[str, Any],
+        "parquetConfiguration": ParquetConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
         "parquetConfiguration": ParquetConfigurationTypeDef,
@@ -1601,19 +2265,39 @@
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
-        "datastorePartitions": DatastorePartitionsTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
+    "_RequiredDatasetContentDeliveryRuleOutputTypeDef",
+    {
+        "destination": DatasetContentDeliveryDestinationOutputTypeDef,
+    },
+)
+_OptionalDatasetContentDeliveryRuleOutputTypeDef = TypedDict(
+    "_OptionalDatasetContentDeliveryRuleOutputTypeDef",
+    {
+        "entryName": str,
+    },
+    total=False,
+)
+
+class DatasetContentDeliveryRuleOutputTypeDef(
+    _RequiredDatasetContentDeliveryRuleOutputTypeDef,
+    _OptionalDatasetContentDeliveryRuleOutputTypeDef,
+):
+    pass
+
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
@@ -1625,14 +2309,24 @@
 )
 
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
+DatasetActionOutputTypeDef = TypedDict(
+    "DatasetActionOutputTypeDef",
+    {
+        "actionName": str,
+        "queryAction": SqlQueryDatasetActionOutputTypeDef,
+        "containerAction": ContainerDatasetActionOutputTypeDef,
+    },
+    total=False,
+)
+
 DatasetActionTypeDef = TypedDict(
     "DatasetActionTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionTypeDef,
         "containerAction": ContainerDatasetActionTypeDef,
     },
@@ -1643,14 +2337,31 @@
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatastoreTypeDef = TypedDict(
+    "DatastoreTypeDef",
+    {
+        "name": str,
+        "storage": DatastoreStorageOutputTypeDef,
+        "arn": str,
+        "status": DatastoreStatusType,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+        "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1666,31 +2377,14 @@
 )
 
 class CreateDatastoreRequestRequestTypeDef(
     _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
-DatastoreTypeDef = TypedDict(
-    "DatastoreTypeDef",
-    {
-        "name": str,
-        "storage": DatastoreStorageTypeDef,
-        "arn": str,
-        "status": DatastoreStatusType,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
-        "fileFormatConfiguration": FileFormatConfigurationTypeDef,
-        "datastorePartitions": DatastorePartitionsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1713,14 +2407,32 @@
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "actions": List[DatasetActionOutputTypeDef],
+        "triggers": List[DatasetTriggerOutputTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleOutputTypeDef],
+        "status": DatasetStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "versioningConfiguration": VersioningConfigurationOutputTypeDef,
+        "lateDataRules": List[LateDataRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
         "actions": Sequence[DatasetActionTypeDef],
     },
 )
@@ -1738,32 +2450,14 @@
 )
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "actions": List[DatasetActionTypeDef],
-        "triggers": List[DatasetTriggerTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
-        "status": DatasetStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "versioningConfiguration": VersioningConfigurationTypeDef,
-        "lateDataRules": List[LateDataRuleTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
         "actions": Sequence[DatasetActionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTAnalytics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotanalytics"></a>
 
 # mypy-boto3-iotanalytics
 
 [![PyPI - mypy-boto3-iotanalytics](https://img.shields.io/pypi/v/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-iotanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotanalytics)](https://pepy.tech/project/mypy-boto3-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTAnalytics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[boto3.IoTAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,154 +344,203 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotanalytics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotanalytics.type_defs import (
+    AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     MessageTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
+    ChannelActivityOutputTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
+    CustomerManagedChannelS3StorageOutputTypeDef,
     CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
-    RetentionPeriodTypeDef,
+    RetentionPeriodOutputTypeDef,
+    ColumnOutputTypeDef,
     ColumnTypeDef,
+    ResourceConfigurationOutputTypeDef,
     ResourceConfigurationTypeDef,
+    RetentionPeriodTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
     CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
     CreatePipelineResponseTypeDef,
+    CustomerManagedDatastoreS3StorageOutputTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
+    IotEventsDestinationConfigurationOutputTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
+    DatasetContentVersionValueOutputTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
+    ScheduleOutputTypeDef,
+    TriggeringDatasetOutputTypeDef,
     ScheduleTypeDef,
     TriggeringDatasetTypeDef,
+    VersioningConfigurationOutputTypeDef,
+    DatastoreActivityOutputTypeDef,
     DatastoreActivityTypeDef,
+    IotSiteWiseCustomerManagedDatastoreS3StorageOutputTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef,
     IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
+    PartitionOutputTypeDef,
+    TimestampPartitionOutputTypeDef,
     PartitionTypeDef,
     TimestampPartitionTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteDatasetContentRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeletePipelineRequestRequestTypeDef,
+    DeltaTimeOutputTypeDef,
+    DeltaTimeSessionWindowConfigurationOutputTypeDef,
     DeltaTimeSessionWindowConfigurationTypeDef,
     DeltaTimeTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsOutputTypeDef,
     DescribePipelineRequestRequestTypeDef,
+    DeviceRegistryEnrichActivityOutputTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
+    DeviceShadowEnrichActivityOutputTypeDef,
     DeviceShadowEnrichActivityTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterActivityOutputTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
+    GlueConfigurationOutputTypeDef,
     GlueConfigurationTypeDef,
+    LambdaActivityOutputTypeDef,
     LambdaActivityTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
     ListDatasetContentsRequestRequestTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    LoggingOptionsTypeDef,
+    MathActivityOutputTypeDef,
     MathActivityTypeDef,
+    OutputFileUriValueOutputTypeDef,
     OutputFileUriValueTypeDef,
     PaginatorConfigTypeDef,
+    RemoveAttributesActivityOutputTypeDef,
+    SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
     ResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchPutMessageRequestRequestTypeDef,
     StartPipelineReprocessingRequestRequestTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageSummaryTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
+    DatasetTriggerOutputTypeDef,
     DatasetTriggerTypeDef,
+    DatastoreIotSiteWiseMultiLayerStorageOutputTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
+    DatastorePartitionOutputTypeDef,
     DatastorePartitionTypeDef,
+    QueryFilterOutputTypeDef,
+    LateDataRuleConfigurationOutputTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
+    VariableOutputTypeDef,
     VariableTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
-    ChannelSummaryTypeDef,
     ChannelTypeDef,
+    ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageSummaryTypeDef,
     DatastoreStorageTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
+    LateDataRuleOutputTypeDef,
     LateDataRuleTypeDef,
     SqlQueryDatasetActionTypeDef,
+    DatasetContentDeliveryDestinationOutputTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
+    ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
-    ListChannelsResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
     DatastoreSummaryTypeDef,
+    DatasetContentDeliveryRuleOutputTypeDef,
     DatasetContentDeliveryRuleTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
-    CreateDatastoreRequestRequestTypeDef,
     DatastoreTypeDef,
+    CreateDatastoreRequestRequestTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityTypeDef:
+def get_structure() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotanalytics-1.28.0/mypy_boto3_iotanalytics.egg-info/SOURCES.txt` & `mypy-boto3-iotanalytics-1.28.12/mypy_boto3_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.0/setup.py` & `mypy-boto3-iotanalytics-1.28.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotanalytics",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTAnalytics 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTAnalytics 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

