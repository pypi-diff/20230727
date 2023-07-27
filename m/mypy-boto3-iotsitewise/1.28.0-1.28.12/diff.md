# Comparing `tmp/mypy-boto3-iotsitewise-1.28.0.tar.gz` & `tmp/mypy-boto3-iotsitewise-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsitewise-1.28.0.tar", last modified: Thu Jul  6 20:59:50 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsitewise-1.28.12.tar", last modified: Thu Jul 27 05:34:50 2023, max compression
```

## Comparing `mypy-boto3-iotsitewise-1.28.0.tar` & `mypy-boto3-iotsitewise-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.402335 mypy-boto3-iotsitewise-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28382 2023-07-06 20:59:50.398335 mypy-boto3-iotsitewise-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26881 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.390335 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62559 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-07-06 20:43:59.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-07-06 20:43:59.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-07-06 20:43:59.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-07-06 20:43:59.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   105875 2023-07-06 20:44:04.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105674 2023-07-06 20:44:00.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-06 20:43:59.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-06 20:43:59.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.398335 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28382 2023-07-06 20:59:50.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 20:59:50.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:50.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:50.000000 mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:50.402335 mypy-boto3-iotsitewise-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:43:58.000000 mypy-boto3-iotsitewise-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29685 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62559 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-27 05:24:11.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   117425 2023-07-27 05:24:14.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117201 2023-07-27 05:24:13.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29685 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:50.000000 mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:50.784478 mypy-boto3-iotsitewise-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:24:10.000000 mypy-boto3-iotsitewise-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotsitewise-1.28.0/LICENSE` & `mypy-boto3-iotsitewise-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTSiteWise 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTSiteWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsitewise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsitewise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -471,25 +471,30 @@
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
+    AlarmsOutputTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
     AssetHierarchyTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
+    AssetModelHierarchyOutputTypeDef,
     AssetModelHierarchyTypeDef,
     PropertyNotificationTypeDef,
+    TimeInNanosOutputTypeDef,
+    VariantOutputTypeDef,
     TimeInNanosTypeDef,
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
@@ -506,15 +511,17 @@
     CreateBulkImportJobResponseTypeDef,
     CreateDashboardRequestRequestTypeDef,
     CreateDashboardResponseTypeDef,
     CreateGatewayResponseTypeDef,
     ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
+    CsvOutputTypeDef,
     CsvTypeDef,
+    CustomerManagedS3StorageOutputTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDashboardRequestRequestTypeDef,
     DeleteGatewayRequestRequestTypeDef,
@@ -523,46 +530,56 @@
     DeleteTimeSeriesRequestRequestTypeDef,
     DescribeAccessPolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribeBulkImportJobRequestRequestTypeDef,
+    ErrorReportLocationOutputTypeDef,
+    FileOutputTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardResponseTypeDef,
     DescribeGatewayCapabilityConfigurationRequestRequestTypeDef,
     DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     GatewayCapabilitySummaryTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsOutputTypeDef,
     DescribePortalRequestRequestTypeDef,
     ImageLocationTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
-    RetentionPeriodTypeDef,
+    RetentionPeriodOutputTypeDef,
     DescribeTimeSeriesRequestRequestTypeDef,
     DescribeTimeSeriesResponseTypeDef,
     DetailedErrorTypeDef,
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    VariableValueOutputTypeDef,
     VariableValueTypeDef,
+    ForwardingConfigOutputTypeDef,
     ForwardingConfigTypeDef,
+    GreengrassOutputTypeDef,
+    GreengrassV2OutputTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
     GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
     GetAssetPropertyAggregatesRequestRequestTypeDef,
     GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
     GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
     GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
+    GroupIdentityOutputTypeDef,
     GroupIdentityTypeDef,
+    IAMRoleIdentityOutputTypeDef,
     IAMRoleIdentityTypeDef,
+    IAMUserIdentityOutputTypeDef,
     IAMUserIdentityTypeDef,
+    UserIdentityOutputTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
     ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     ListAssetModelPropertiesRequestRequestTypeDef,
     ListAssetModelsRequestListAssetModelsPaginateTypeDef,
@@ -590,21 +607,27 @@
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     ListTimeSeriesRequestRequestTypeDef,
     TimeSeriesSummaryTypeDef,
+    LoggingOptionsTypeDef,
+    MetricProcessingConfigOutputTypeDef,
     MetricProcessingConfigTypeDef,
+    TumblingWindowOutputTypeDef,
     TumblingWindowTypeDef,
     MonitorErrorDetailsTypeDef,
     PaginatorConfigTypeDef,
+    PortalResourceOutputTypeDef,
     PortalResourceTypeDef,
+    ProjectResourceOutputTypeDef,
     ProjectResourceTypeDef,
     PutDefaultEncryptionConfigurationRequestRequestTypeDef,
+    RetentionPeriodTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetPropertyRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     UpdateGatewayCapabilityConfigurationRequestRequestTypeDef,
@@ -614,120 +637,137 @@
     AggregatedValueTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     AssetRelationshipSummaryTypeDef,
     AssetPropertySummaryTypeDef,
     AssetPropertyTypeDef,
     BatchPutAssetPropertyErrorTypeDef,
-    AssetPropertyValueTypeDef,
+    AssetPropertyValueOutputTypeDef,
     InterpolatedAssetPropertyValueTypeDef,
+    AssetPropertyValueTypeDef,
     BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
     BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     ConfigurationStatusTypeDef,
     CreatePortalRequestRequestTypeDef,
     ImageTypeDef,
+    FileFormatOutputTypeDef,
     FileFormatTypeDef,
+    MultiLayerStorageOutputTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
     DescribeAssetRequestAssetNotExistsWaitTypeDef,
     DescribePortalRequestPortalActiveWaitTypeDef,
     DescribePortalRequestPortalNotExistsWaitTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
     ErrorDetailsTypeDef,
+    ExpressionVariableOutputTypeDef,
     ExpressionVariableTypeDef,
+    MeasurementProcessingConfigOutputTypeDef,
+    TransformProcessingConfigOutputTypeDef,
     MeasurementProcessingConfigTypeDef,
     TransformProcessingConfigTypeDef,
+    GatewayPlatformOutputTypeDef,
     GatewayPlatformTypeDef,
+    IdentityOutputTypeDef,
     IdentityTypeDef,
     ListBulkImportJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
+    MetricWindowOutputTypeDef,
     MetricWindowTypeDef,
     PortalStatusTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     BatchGetAssetPropertyAggregatesSuccessEntryTypeDef,
     GetAssetPropertyAggregatesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     AssetCompositeModelTypeDef,
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
-    PutAssetPropertyValueEntryTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
+    PutAssetPropertyValueEntryTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     UpdatePortalRequestRequestTypeDef,
+    JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
-    PutStorageConfigurationRequestRequestTypeDef,
     PutStorageConfigurationResponseTypeDef,
+    PutStorageConfigurationRequestRequestTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
+    MeasurementOutputTypeDef,
+    TransformOutputTypeDef,
     MeasurementTypeDef,
     TransformTypeDef,
-    CreateGatewayRequestRequestTypeDef,
     DescribeGatewayResponseTypeDef,
     GatewaySummaryTypeDef,
+    CreateGatewayRequestRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     CreatePortalResponseTypeDef,
     DeletePortalResponseTypeDef,
     DescribePortalResponseTypeDef,
     PortalSummaryTypeDef,
     UpdatePortalResponseTypeDef,
     AccessPolicySummaryTypeDef,
-    CreateAccessPolicyRequestRequestTypeDef,
     DescribeAccessPolicyResponseTypeDef,
+    CreateAccessPolicyRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
-    CreateBulkImportJobRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
+    CreateBulkImportJobRequestRequestTypeDef,
     AssetModelSummaryTypeDef,
     CreateAssetModelResponseTypeDef,
     DeleteAssetModelResponseTypeDef,
     UpdateAssetModelResponseTypeDef,
     AssetSummaryTypeDef,
     AssociatedAssetsSummaryTypeDef,
     CreateAssetResponseTypeDef,
     DeleteAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
     UpdateAssetResponseTypeDef,
     ListGatewaysResponseTypeDef,
+    PropertyTypeOutputTypeDef,
     PropertyTypeTypeDef,
     ListPortalsResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetsResponseTypeDef,
     ListAssociatedAssetsResponseTypeDef,
-    AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyOutputTypeDef,
     AssetModelPropertySummaryTypeDef,
-    AssetModelPropertyTypeDef,
     PropertyTypeDef,
-    AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyTypeDef,
+    AssetModelCompositeModelOutputTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
-    AssetModelCompositeModelTypeDef,
     CompositeModelPropertyTypeDef,
-    CreateAssetModelRequestRequestTypeDef,
+    AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelCompositeModelTypeDef,
     DescribeAssetModelResponseTypeDef,
-    UpdateAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyResponseTypeDef,
+    CreateAssetModelRequestRequestTypeDef,
+    UpdateAssetModelRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AggregatesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotsitewise-1.28.0/README.md` & `mypy-boto3-iotsitewise-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsitewise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsitewise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,25 +439,30 @@
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
+    AlarmsOutputTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
     AssetHierarchyTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
+    AssetModelHierarchyOutputTypeDef,
     AssetModelHierarchyTypeDef,
     PropertyNotificationTypeDef,
+    TimeInNanosOutputTypeDef,
+    VariantOutputTypeDef,
     TimeInNanosTypeDef,
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
@@ -474,15 +479,17 @@
     CreateBulkImportJobResponseTypeDef,
     CreateDashboardRequestRequestTypeDef,
     CreateDashboardResponseTypeDef,
     CreateGatewayResponseTypeDef,
     ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
+    CsvOutputTypeDef,
     CsvTypeDef,
+    CustomerManagedS3StorageOutputTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDashboardRequestRequestTypeDef,
     DeleteGatewayRequestRequestTypeDef,
@@ -491,46 +498,56 @@
     DeleteTimeSeriesRequestRequestTypeDef,
     DescribeAccessPolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribeBulkImportJobRequestRequestTypeDef,
+    ErrorReportLocationOutputTypeDef,
+    FileOutputTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardResponseTypeDef,
     DescribeGatewayCapabilityConfigurationRequestRequestTypeDef,
     DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     GatewayCapabilitySummaryTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsOutputTypeDef,
     DescribePortalRequestRequestTypeDef,
     ImageLocationTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
-    RetentionPeriodTypeDef,
+    RetentionPeriodOutputTypeDef,
     DescribeTimeSeriesRequestRequestTypeDef,
     DescribeTimeSeriesResponseTypeDef,
     DetailedErrorTypeDef,
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    VariableValueOutputTypeDef,
     VariableValueTypeDef,
+    ForwardingConfigOutputTypeDef,
     ForwardingConfigTypeDef,
+    GreengrassOutputTypeDef,
+    GreengrassV2OutputTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
     GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
     GetAssetPropertyAggregatesRequestRequestTypeDef,
     GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
     GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
     GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
+    GroupIdentityOutputTypeDef,
     GroupIdentityTypeDef,
+    IAMRoleIdentityOutputTypeDef,
     IAMRoleIdentityTypeDef,
+    IAMUserIdentityOutputTypeDef,
     IAMUserIdentityTypeDef,
+    UserIdentityOutputTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
     ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     ListAssetModelPropertiesRequestRequestTypeDef,
     ListAssetModelsRequestListAssetModelsPaginateTypeDef,
@@ -558,21 +575,27 @@
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     ListTimeSeriesRequestRequestTypeDef,
     TimeSeriesSummaryTypeDef,
+    LoggingOptionsTypeDef,
+    MetricProcessingConfigOutputTypeDef,
     MetricProcessingConfigTypeDef,
+    TumblingWindowOutputTypeDef,
     TumblingWindowTypeDef,
     MonitorErrorDetailsTypeDef,
     PaginatorConfigTypeDef,
+    PortalResourceOutputTypeDef,
     PortalResourceTypeDef,
+    ProjectResourceOutputTypeDef,
     ProjectResourceTypeDef,
     PutDefaultEncryptionConfigurationRequestRequestTypeDef,
+    RetentionPeriodTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetPropertyRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     UpdateGatewayCapabilityConfigurationRequestRequestTypeDef,
@@ -582,120 +605,137 @@
     AggregatedValueTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     AssetRelationshipSummaryTypeDef,
     AssetPropertySummaryTypeDef,
     AssetPropertyTypeDef,
     BatchPutAssetPropertyErrorTypeDef,
-    AssetPropertyValueTypeDef,
+    AssetPropertyValueOutputTypeDef,
     InterpolatedAssetPropertyValueTypeDef,
+    AssetPropertyValueTypeDef,
     BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
     BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     ConfigurationStatusTypeDef,
     CreatePortalRequestRequestTypeDef,
     ImageTypeDef,
+    FileFormatOutputTypeDef,
     FileFormatTypeDef,
+    MultiLayerStorageOutputTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
     DescribeAssetRequestAssetNotExistsWaitTypeDef,
     DescribePortalRequestPortalActiveWaitTypeDef,
     DescribePortalRequestPortalNotExistsWaitTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
     ErrorDetailsTypeDef,
+    ExpressionVariableOutputTypeDef,
     ExpressionVariableTypeDef,
+    MeasurementProcessingConfigOutputTypeDef,
+    TransformProcessingConfigOutputTypeDef,
     MeasurementProcessingConfigTypeDef,
     TransformProcessingConfigTypeDef,
+    GatewayPlatformOutputTypeDef,
     GatewayPlatformTypeDef,
+    IdentityOutputTypeDef,
     IdentityTypeDef,
     ListBulkImportJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
+    MetricWindowOutputTypeDef,
     MetricWindowTypeDef,
     PortalStatusTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     BatchGetAssetPropertyAggregatesSuccessEntryTypeDef,
     GetAssetPropertyAggregatesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     AssetCompositeModelTypeDef,
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
-    PutAssetPropertyValueEntryTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
+    PutAssetPropertyValueEntryTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     UpdatePortalRequestRequestTypeDef,
+    JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
-    PutStorageConfigurationRequestRequestTypeDef,
     PutStorageConfigurationResponseTypeDef,
+    PutStorageConfigurationRequestRequestTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
+    MeasurementOutputTypeDef,
+    TransformOutputTypeDef,
     MeasurementTypeDef,
     TransformTypeDef,
-    CreateGatewayRequestRequestTypeDef,
     DescribeGatewayResponseTypeDef,
     GatewaySummaryTypeDef,
+    CreateGatewayRequestRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     CreatePortalResponseTypeDef,
     DeletePortalResponseTypeDef,
     DescribePortalResponseTypeDef,
     PortalSummaryTypeDef,
     UpdatePortalResponseTypeDef,
     AccessPolicySummaryTypeDef,
-    CreateAccessPolicyRequestRequestTypeDef,
     DescribeAccessPolicyResponseTypeDef,
+    CreateAccessPolicyRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
-    CreateBulkImportJobRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
+    CreateBulkImportJobRequestRequestTypeDef,
     AssetModelSummaryTypeDef,
     CreateAssetModelResponseTypeDef,
     DeleteAssetModelResponseTypeDef,
     UpdateAssetModelResponseTypeDef,
     AssetSummaryTypeDef,
     AssociatedAssetsSummaryTypeDef,
     CreateAssetResponseTypeDef,
     DeleteAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
     UpdateAssetResponseTypeDef,
     ListGatewaysResponseTypeDef,
+    PropertyTypeOutputTypeDef,
     PropertyTypeTypeDef,
     ListPortalsResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetsResponseTypeDef,
     ListAssociatedAssetsResponseTypeDef,
-    AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyOutputTypeDef,
     AssetModelPropertySummaryTypeDef,
-    AssetModelPropertyTypeDef,
     PropertyTypeDef,
-    AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyTypeDef,
+    AssetModelCompositeModelOutputTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
-    AssetModelCompositeModelTypeDef,
     CompositeModelPropertyTypeDef,
-    CreateAssetModelRequestRequestTypeDef,
+    AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelCompositeModelTypeDef,
     DescribeAssetModelResponseTypeDef,
-    UpdateAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyResponseTypeDef,
+    CreateAssetModelRequestRequestTypeDef,
+    UpdateAssetModelRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AggregatesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/__init__.py` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/__init__.pyi` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/__main__.py` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSiteWise 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTSiteWise 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise\nOther"
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

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/client.py` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/client.pyi` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/literals.py` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,15 @@
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
@@ -388,26 +389,28 @@
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

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/literals.pyi` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,15 @@
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
@@ -386,26 +387,28 @@
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

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/paginator.py` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/paginator.pyi` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/type_defs.py` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,25 +64,30 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AggregatesTypeDef",
+    "AlarmsOutputTypeDef",
     "AlarmsTypeDef",
     "AssetErrorDetailsTypeDef",
     "AssetHierarchyInfoTypeDef",
     "AssetHierarchyTypeDef",
     "AssetModelHierarchyDefinitionTypeDef",
+    "AssetModelHierarchyOutputTypeDef",
     "AssetModelHierarchyTypeDef",
     "PropertyNotificationTypeDef",
+    "TimeInNanosOutputTypeDef",
+    "VariantOutputTypeDef",
     "TimeInNanosTypeDef",
     "VariantTypeDef",
     "AssociateAssetsRequestRequestTypeDef",
     "AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "BatchAssociateProjectAssetsRequestRequestTypeDef",
     "BatchDisassociateProjectAssetsRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorInfoTypeDef",
     "BatchGetAssetPropertyValueEntryTypeDef",
@@ -99,15 +104,17 @@
     "CreateBulkImportJobResponseTypeDef",
     "CreateDashboardRequestRequestTypeDef",
     "CreateDashboardResponseTypeDef",
     "CreateGatewayResponseTypeDef",
     "ImageFileTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
+    "CsvOutputTypeDef",
     "CsvTypeDef",
+    "CustomerManagedS3StorageOutputTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
@@ -116,46 +123,56 @@
     "DeleteTimeSeriesRequestRequestTypeDef",
     "DescribeAccessPolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAssetModelRequestRequestTypeDef",
     "DescribeAssetPropertyRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribeBulkImportJobRequestRequestTypeDef",
+    "ErrorReportLocationOutputTypeDef",
+    "FileOutputTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardResponseTypeDef",
     "DescribeGatewayCapabilityConfigurationRequestRequestTypeDef",
     "DescribeGatewayCapabilityConfigurationResponseTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "GatewayCapabilitySummaryTypeDef",
-    "LoggingOptionsTypeDef",
+    "LoggingOptionsOutputTypeDef",
     "DescribePortalRequestRequestTypeDef",
     "ImageLocationTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
-    "RetentionPeriodTypeDef",
+    "RetentionPeriodOutputTypeDef",
     "DescribeTimeSeriesRequestRequestTypeDef",
     "DescribeTimeSeriesResponseTypeDef",
     "DetailedErrorTypeDef",
     "DisassociateAssetsRequestRequestTypeDef",
     "DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "VariableValueOutputTypeDef",
     "VariableValueTypeDef",
+    "ForwardingConfigOutputTypeDef",
     "ForwardingConfigTypeDef",
+    "GreengrassOutputTypeDef",
+    "GreengrassV2OutputTypeDef",
     "GreengrassTypeDef",
     "GreengrassV2TypeDef",
     "GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     "GetAssetPropertyAggregatesRequestRequestTypeDef",
     "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "GetAssetPropertyValueRequestRequestTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
+    "GroupIdentityOutputTypeDef",
     "GroupIdentityTypeDef",
+    "IAMRoleIdentityOutputTypeDef",
     "IAMRoleIdentityTypeDef",
+    "IAMUserIdentityOutputTypeDef",
     "IAMUserIdentityTypeDef",
+    "UserIdentityOutputTypeDef",
     "UserIdentityTypeDef",
     "JobSummaryTypeDef",
     "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
     "ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
     "ListAssetModelPropertiesRequestRequestTypeDef",
     "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
@@ -183,21 +200,27 @@
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     "ListTimeSeriesRequestRequestTypeDef",
     "TimeSeriesSummaryTypeDef",
+    "LoggingOptionsTypeDef",
+    "MetricProcessingConfigOutputTypeDef",
     "MetricProcessingConfigTypeDef",
+    "TumblingWindowOutputTypeDef",
     "TumblingWindowTypeDef",
     "MonitorErrorDetailsTypeDef",
     "PaginatorConfigTypeDef",
+    "PortalResourceOutputTypeDef",
     "PortalResourceTypeDef",
+    "ProjectResourceOutputTypeDef",
     "ProjectResourceTypeDef",
     "PutDefaultEncryptionConfigurationRequestRequestTypeDef",
+    "RetentionPeriodTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetPropertyRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "UpdateGatewayCapabilityConfigurationRequestRequestTypeDef",
@@ -207,120 +230,137 @@
     "AggregatedValueTypeDef",
     "BatchAssociateProjectAssetsResponseTypeDef",
     "BatchDisassociateProjectAssetsResponseTypeDef",
     "AssetRelationshipSummaryTypeDef",
     "AssetPropertySummaryTypeDef",
     "AssetPropertyTypeDef",
     "BatchPutAssetPropertyErrorTypeDef",
-    "AssetPropertyValueTypeDef",
+    "AssetPropertyValueOutputTypeDef",
     "InterpolatedAssetPropertyValueTypeDef",
+    "AssetPropertyValueTypeDef",
     "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     "ConfigurationStatusTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "ImageTypeDef",
+    "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
+    "MultiLayerStorageOutputTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
     "DescribeAssetRequestAssetNotExistsWaitTypeDef",
     "DescribePortalRequestPortalActiveWaitTypeDef",
     "DescribePortalRequestPortalNotExistsWaitTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "PutLoggingOptionsRequestRequestTypeDef",
     "ErrorDetailsTypeDef",
+    "ExpressionVariableOutputTypeDef",
     "ExpressionVariableTypeDef",
+    "MeasurementProcessingConfigOutputTypeDef",
+    "TransformProcessingConfigOutputTypeDef",
     "MeasurementProcessingConfigTypeDef",
     "TransformProcessingConfigTypeDef",
+    "GatewayPlatformOutputTypeDef",
     "GatewayPlatformTypeDef",
+    "IdentityOutputTypeDef",
     "IdentityTypeDef",
     "ListBulkImportJobsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ListTimeSeriesResponseTypeDef",
+    "PutLoggingOptionsRequestRequestTypeDef",
+    "MetricWindowOutputTypeDef",
     "MetricWindowTypeDef",
     "PortalStatusTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetAssetPropertyAggregatesSuccessEntryTypeDef",
     "GetAssetPropertyAggregatesResponseTypeDef",
     "ListAssetRelationshipsResponseTypeDef",
     "ListAssetPropertiesResponseTypeDef",
     "AssetCompositeModelTypeDef",
     "BatchPutAssetPropertyErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     "BatchGetAssetPropertyValueSuccessEntryTypeDef",
     "GetAssetPropertyValueHistoryResponseTypeDef",
     "GetAssetPropertyValueResponseTypeDef",
-    "PutAssetPropertyValueEntryTypeDef",
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    "PutAssetPropertyValueEntryTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
     "UpdatePortalRequestRequestTypeDef",
+    "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
-    "PutStorageConfigurationRequestRequestTypeDef",
     "PutStorageConfigurationResponseTypeDef",
+    "PutStorageConfigurationRequestRequestTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
+    "MeasurementOutputTypeDef",
+    "TransformOutputTypeDef",
     "MeasurementTypeDef",
     "TransformTypeDef",
-    "CreateGatewayRequestRequestTypeDef",
     "DescribeGatewayResponseTypeDef",
     "GatewaySummaryTypeDef",
+    "CreateGatewayRequestRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
     "CreatePortalResponseTypeDef",
     "DeletePortalResponseTypeDef",
     "DescribePortalResponseTypeDef",
     "PortalSummaryTypeDef",
     "UpdatePortalResponseTypeDef",
     "AccessPolicySummaryTypeDef",
-    "CreateAccessPolicyRequestRequestTypeDef",
     "DescribeAccessPolicyResponseTypeDef",
+    "CreateAccessPolicyRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
-    "CreateBulkImportJobRequestRequestTypeDef",
     "DescribeBulkImportJobResponseTypeDef",
+    "CreateBulkImportJobRequestRequestTypeDef",
     "AssetModelSummaryTypeDef",
     "CreateAssetModelResponseTypeDef",
     "DeleteAssetModelResponseTypeDef",
     "UpdateAssetModelResponseTypeDef",
     "AssetSummaryTypeDef",
     "AssociatedAssetsSummaryTypeDef",
     "CreateAssetResponseTypeDef",
     "DeleteAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListGatewaysResponseTypeDef",
+    "PropertyTypeOutputTypeDef",
     "PropertyTypeTypeDef",
     "ListPortalsResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
     "ListAssetModelsResponseTypeDef",
     "ListAssetsResponseTypeDef",
     "ListAssociatedAssetsResponseTypeDef",
-    "AssetModelPropertyDefinitionTypeDef",
+    "AssetModelPropertyOutputTypeDef",
     "AssetModelPropertySummaryTypeDef",
-    "AssetModelPropertyTypeDef",
     "PropertyTypeDef",
-    "AssetModelCompositeModelDefinitionTypeDef",
+    "AssetModelPropertyDefinitionTypeDef",
+    "AssetModelPropertyTypeDef",
+    "AssetModelCompositeModelOutputTypeDef",
     "ListAssetModelPropertiesResponseTypeDef",
-    "AssetModelCompositeModelTypeDef",
     "CompositeModelPropertyTypeDef",
-    "CreateAssetModelRequestRequestTypeDef",
+    "AssetModelCompositeModelDefinitionTypeDef",
+    "AssetModelCompositeModelTypeDef",
     "DescribeAssetModelResponseTypeDef",
-    "UpdateAssetModelRequestRequestTypeDef",
     "DescribeAssetPropertyResponseTypeDef",
+    "CreateAssetModelRequestRequestTypeDef",
+    "UpdateAssetModelRequestRequestTypeDef",
 )
 
 AggregatesTypeDef = TypedDict(
     "AggregatesTypeDef",
     {
         "average": float,
         "count": float,
@@ -328,14 +368,33 @@
         "minimum": float,
         "sum": float,
         "standardDeviation": float,
     },
     total=False,
 )
 
+_RequiredAlarmsOutputTypeDef = TypedDict(
+    "_RequiredAlarmsOutputTypeDef",
+    {
+        "alarmRoleArn": str,
+    },
+)
+_OptionalAlarmsOutputTypeDef = TypedDict(
+    "_OptionalAlarmsOutputTypeDef",
+    {
+        "notificationLambdaArn": str,
+    },
+    total=False,
+)
+
+
+class AlarmsOutputTypeDef(_RequiredAlarmsOutputTypeDef, _OptionalAlarmsOutputTypeDef):
+    pass
+
+
 _RequiredAlarmsTypeDef = TypedDict(
     "_RequiredAlarmsTypeDef",
     {
         "alarmRoleArn": str,
     },
 )
 _OptionalAlarmsTypeDef = TypedDict(
@@ -392,14 +451,36 @@
     "AssetModelHierarchyDefinitionTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
 
+_RequiredAssetModelHierarchyOutputTypeDef = TypedDict(
+    "_RequiredAssetModelHierarchyOutputTypeDef",
+    {
+        "name": str,
+        "childAssetModelId": str,
+    },
+)
+_OptionalAssetModelHierarchyOutputTypeDef = TypedDict(
+    "_OptionalAssetModelHierarchyOutputTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+
+class AssetModelHierarchyOutputTypeDef(
+    _RequiredAssetModelHierarchyOutputTypeDef, _OptionalAssetModelHierarchyOutputTypeDef
+):
+    pass
+
+
 _RequiredAssetModelHierarchyTypeDef = TypedDict(
     "_RequiredAssetModelHierarchyTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
@@ -422,14 +503,46 @@
     "PropertyNotificationTypeDef",
     {
         "topic": str,
         "state": PropertyNotificationStateType,
     },
 )
 
+_RequiredTimeInNanosOutputTypeDef = TypedDict(
+    "_RequiredTimeInNanosOutputTypeDef",
+    {
+        "timeInSeconds": int,
+    },
+)
+_OptionalTimeInNanosOutputTypeDef = TypedDict(
+    "_OptionalTimeInNanosOutputTypeDef",
+    {
+        "offsetInNanos": int,
+    },
+    total=False,
+)
+
+
+class TimeInNanosOutputTypeDef(
+    _RequiredTimeInNanosOutputTypeDef, _OptionalTimeInNanosOutputTypeDef
+):
+    pass
+
+
+VariantOutputTypeDef = TypedDict(
+    "VariantOutputTypeDef",
+    {
+        "stringValue": str,
+        "integerValue": int,
+        "doubleValue": float,
+        "booleanValue": bool,
+    },
+    total=False,
+)
+
 _RequiredTimeInNanosTypeDef = TypedDict(
     "_RequiredTimeInNanosTypeDef",
     {
         "timeInSeconds": int,
     },
 )
 _OptionalTimeInNanosTypeDef = TypedDict(
@@ -499,14 +612,22 @@
 class AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef(
     _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     _OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
 
+AttributeOutputTypeDef = TypedDict(
+    "AttributeOutputTypeDef",
+    {
+        "defaultValue": str,
+    },
+    total=False,
+)
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "defaultValue": str,
     },
     total=False,
 )
@@ -848,22 +969,38 @@
     {
         "projectId": str,
         "projectArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CsvOutputTypeDef = TypedDict(
+    "CsvOutputTypeDef",
+    {
+        "columnNames": List[ColumnNameType],
+    },
+    total=False,
+)
+
 CsvTypeDef = TypedDict(
     "CsvTypeDef",
     {
         "columnNames": Sequence[ColumnNameType],
     },
     total=False,
 )
 
+CustomerManagedS3StorageOutputTypeDef = TypedDict(
+    "CustomerManagedS3StorageOutputTypeDef",
+    {
+        "s3ResourceArn": str,
+        "roleArn": str,
+    },
+)
+
 CustomerManagedS3StorageTypeDef = TypedDict(
     "CustomerManagedS3StorageTypeDef",
     {
         "s3ResourceArn": str,
         "roleArn": str,
     },
 )
@@ -1105,14 +1242,42 @@
 DescribeBulkImportJobRequestRequestTypeDef = TypedDict(
     "DescribeBulkImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
+ErrorReportLocationOutputTypeDef = TypedDict(
+    "ErrorReportLocationOutputTypeDef",
+    {
+        "bucket": str,
+        "prefix": str,
+    },
+)
+
+_RequiredFileOutputTypeDef = TypedDict(
+    "_RequiredFileOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+    },
+)
+_OptionalFileOutputTypeDef = TypedDict(
+    "_OptionalFileOutputTypeDef",
+    {
+        "versionId": str,
+    },
+    total=False,
+)
+
+
+class FileOutputTypeDef(_RequiredFileOutputTypeDef, _OptionalFileOutputTypeDef):
+    pass
+
+
 DescribeDashboardRequestRequestTypeDef = TypedDict(
     "DescribeDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
     },
 )
 
@@ -1161,16 +1326,16 @@
     "GatewayCapabilitySummaryTypeDef",
     {
         "capabilityNamespace": str,
         "capabilitySyncStatus": CapabilitySyncStatusType,
     },
 )
 
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
+LoggingOptionsOutputTypeDef = TypedDict(
+    "LoggingOptionsOutputTypeDef",
     {
         "level": LoggingLevelType,
     },
 )
 
 DescribePortalRequestRequestTypeDef = TypedDict(
     "DescribePortalRequestRequestTypeDef",
@@ -1204,16 +1369,16 @@
         "projectDescription": str,
         "projectCreationDate": datetime,
         "projectLastUpdateDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
     {
         "numberOfDays": int,
         "unlimited": bool,
     },
     total=False,
 )
 
@@ -1302,14 +1467,35 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredVariableValueOutputTypeDef = TypedDict(
+    "_RequiredVariableValueOutputTypeDef",
+    {
+        "propertyId": str,
+    },
+)
+_OptionalVariableValueOutputTypeDef = TypedDict(
+    "_OptionalVariableValueOutputTypeDef",
+    {
+        "hierarchyId": str,
+    },
+    total=False,
+)
+
+
+class VariableValueOutputTypeDef(
+    _RequiredVariableValueOutputTypeDef, _OptionalVariableValueOutputTypeDef
+):
+    pass
+
+
 _RequiredVariableValueTypeDef = TypedDict(
     "_RequiredVariableValueTypeDef",
     {
         "propertyId": str,
     },
 )
 _OptionalVariableValueTypeDef = TypedDict(
@@ -1321,21 +1507,42 @@
 )
 
 
 class VariableValueTypeDef(_RequiredVariableValueTypeDef, _OptionalVariableValueTypeDef):
     pass
 
 
+ForwardingConfigOutputTypeDef = TypedDict(
+    "ForwardingConfigOutputTypeDef",
+    {
+        "state": ForwardingConfigStateType,
+    },
+)
+
 ForwardingConfigTypeDef = TypedDict(
     "ForwardingConfigTypeDef",
     {
         "state": ForwardingConfigStateType,
     },
 )
 
+GreengrassOutputTypeDef = TypedDict(
+    "GreengrassOutputTypeDef",
+    {
+        "groupArn": str,
+    },
+)
+
+GreengrassV2OutputTypeDef = TypedDict(
+    "GreengrassV2OutputTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+
 GreengrassTypeDef = TypedDict(
     "GreengrassTypeDef",
     {
         "groupArn": str,
     },
 )
 
@@ -1509,35 +1716,63 @@
 class GetInterpolatedAssetPropertyValuesRequestRequestTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
 ):
     pass
 
 
+GroupIdentityOutputTypeDef = TypedDict(
+    "GroupIdentityOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 GroupIdentityTypeDef = TypedDict(
     "GroupIdentityTypeDef",
     {
         "id": str,
     },
 )
 
+IAMRoleIdentityOutputTypeDef = TypedDict(
+    "IAMRoleIdentityOutputTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 IAMRoleIdentityTypeDef = TypedDict(
     "IAMRoleIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
+IAMUserIdentityOutputTypeDef = TypedDict(
+    "IAMUserIdentityOutputTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 IAMUserIdentityTypeDef = TypedDict(
     "IAMUserIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
+UserIdentityOutputTypeDef = TypedDict(
+    "UserIdentityOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "id": str,
     },
 )
 
@@ -2083,21 +2318,56 @@
 
 class TimeSeriesSummaryTypeDef(
     _RequiredTimeSeriesSummaryTypeDef, _OptionalTimeSeriesSummaryTypeDef
 ):
     pass
 
 
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
+    {
+        "level": LoggingLevelType,
+    },
+)
+
+MetricProcessingConfigOutputTypeDef = TypedDict(
+    "MetricProcessingConfigOutputTypeDef",
+    {
+        "computeLocation": ComputeLocationType,
+    },
+)
+
 MetricProcessingConfigTypeDef = TypedDict(
     "MetricProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
 
+_RequiredTumblingWindowOutputTypeDef = TypedDict(
+    "_RequiredTumblingWindowOutputTypeDef",
+    {
+        "interval": str,
+    },
+)
+_OptionalTumblingWindowOutputTypeDef = TypedDict(
+    "_OptionalTumblingWindowOutputTypeDef",
+    {
+        "offset": str,
+    },
+    total=False,
+)
+
+
+class TumblingWindowOutputTypeDef(
+    _RequiredTumblingWindowOutputTypeDef, _OptionalTumblingWindowOutputTypeDef
+):
+    pass
+
+
 _RequiredTumblingWindowTypeDef = TypedDict(
     "_RequiredTumblingWindowTypeDef",
     {
         "interval": str,
     },
 )
 _OptionalTumblingWindowTypeDef = TypedDict(
@@ -2128,21 +2398,35 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PortalResourceOutputTypeDef = TypedDict(
+    "PortalResourceOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 PortalResourceTypeDef = TypedDict(
     "PortalResourceTypeDef",
     {
         "id": str,
     },
 )
 
+ProjectResourceOutputTypeDef = TypedDict(
+    "ProjectResourceOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 ProjectResourceTypeDef = TypedDict(
     "ProjectResourceTypeDef",
     {
         "id": str,
     },
 )
 
@@ -2164,14 +2448,23 @@
 class PutDefaultEncryptionConfigurationRequestRequestTypeDef(
     _RequiredPutDefaultEncryptionConfigurationRequestRequestTypeDef,
     _OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
+    {
+        "numberOfDays": int,
+        "unlimited": bool,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -2411,15 +2704,45 @@
 
 
 BatchPutAssetPropertyErrorTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorTypeDef",
     {
         "errorCode": BatchPutAssetPropertyValueErrorCodeType,
         "errorMessage": str,
-        "timestamps": List[TimeInNanosTypeDef],
+        "timestamps": List[TimeInNanosOutputTypeDef],
+    },
+)
+
+_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueOutputTypeDef",
+    {
+        "value": VariantOutputTypeDef,
+        "timestamp": TimeInNanosOutputTypeDef,
+    },
+)
+_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueOutputTypeDef",
+    {
+        "quality": QualityType,
+    },
+    total=False,
+)
+
+
+class AssetPropertyValueOutputTypeDef(
+    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
+):
+    pass
+
+
+InterpolatedAssetPropertyValueTypeDef = TypedDict(
+    "InterpolatedAssetPropertyValueTypeDef",
+    {
+        "timestamp": TimeInNanosOutputTypeDef,
+        "value": VariantOutputTypeDef,
     },
 )
 
 _RequiredAssetPropertyValueTypeDef = TypedDict(
     "_RequiredAssetPropertyValueTypeDef",
     {
         "value": VariantTypeDef,
@@ -2437,22 +2760,14 @@
 
 class AssetPropertyValueTypeDef(
     _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
 
-InterpolatedAssetPropertyValueTypeDef = TypedDict(
-    "InterpolatedAssetPropertyValueTypeDef",
-    {
-        "timestamp": TimeInNanosTypeDef,
-        "value": VariantTypeDef,
-    },
-)
-
 _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
     },
 )
 _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
@@ -2641,22 +2956,37 @@
     {
         "id": str,
         "file": ImageFileTypeDef,
     },
     total=False,
 )
 
+FileFormatOutputTypeDef = TypedDict(
+    "FileFormatOutputTypeDef",
+    {
+        "csv": CsvOutputTypeDef,
+    },
+    total=False,
+)
+
 FileFormatTypeDef = TypedDict(
     "FileFormatTypeDef",
     {
         "csv": CsvTypeDef,
     },
     total=False,
 )
 
+MultiLayerStorageOutputTypeDef = TypedDict(
+    "MultiLayerStorageOutputTypeDef",
+    {
+        "customerManagedS3Storage": CustomerManagedS3StorageOutputTypeDef,
+    },
+)
+
 MultiLayerStorageTypeDef = TypedDict(
     "MultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": CustomerManagedS3StorageTypeDef,
     },
 )
 
@@ -2804,26 +3134,19 @@
 ):
     pass
 
 
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
-    {
-        "loggingOptions": LoggingOptionsTypeDef,
-    },
-)
-
 _RequiredErrorDetailsTypeDef = TypedDict(
     "_RequiredErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
         "message": str,
     },
 )
@@ -2836,22 +3159,58 @@
 )
 
 
 class ErrorDetailsTypeDef(_RequiredErrorDetailsTypeDef, _OptionalErrorDetailsTypeDef):
     pass
 
 
+ExpressionVariableOutputTypeDef = TypedDict(
+    "ExpressionVariableOutputTypeDef",
+    {
+        "name": str,
+        "value": VariableValueOutputTypeDef,
+    },
+)
+
 ExpressionVariableTypeDef = TypedDict(
     "ExpressionVariableTypeDef",
     {
         "name": str,
         "value": VariableValueTypeDef,
     },
 )
 
+MeasurementProcessingConfigOutputTypeDef = TypedDict(
+    "MeasurementProcessingConfigOutputTypeDef",
+    {
+        "forwardingConfig": ForwardingConfigOutputTypeDef,
+    },
+)
+
+_RequiredTransformProcessingConfigOutputTypeDef = TypedDict(
+    "_RequiredTransformProcessingConfigOutputTypeDef",
+    {
+        "computeLocation": ComputeLocationType,
+    },
+)
+_OptionalTransformProcessingConfigOutputTypeDef = TypedDict(
+    "_OptionalTransformProcessingConfigOutputTypeDef",
+    {
+        "forwardingConfig": ForwardingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TransformProcessingConfigOutputTypeDef(
+    _RequiredTransformProcessingConfigOutputTypeDef, _OptionalTransformProcessingConfigOutputTypeDef
+):
+    pass
+
+
 MeasurementProcessingConfigTypeDef = TypedDict(
     "MeasurementProcessingConfigTypeDef",
     {
         "forwardingConfig": ForwardingConfigTypeDef,
     },
 )
 
@@ -2872,23 +3231,43 @@
 
 class TransformProcessingConfigTypeDef(
     _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
 ):
     pass
 
 
+GatewayPlatformOutputTypeDef = TypedDict(
+    "GatewayPlatformOutputTypeDef",
+    {
+        "greengrass": GreengrassOutputTypeDef,
+        "greengrassV2": GreengrassV2OutputTypeDef,
+    },
+    total=False,
+)
+
 GatewayPlatformTypeDef = TypedDict(
     "GatewayPlatformTypeDef",
     {
         "greengrass": GreengrassTypeDef,
         "greengrassV2": GreengrassV2TypeDef,
     },
     total=False,
 )
 
+IdentityOutputTypeDef = TypedDict(
+    "IdentityOutputTypeDef",
+    {
+        "user": UserIdentityOutputTypeDef,
+        "group": GroupIdentityOutputTypeDef,
+        "iamUser": IAMUserIdentityOutputTypeDef,
+        "iamRole": IAMRoleIdentityOutputTypeDef,
+    },
+    total=False,
+)
+
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "user": UserIdentityTypeDef,
         "group": GroupIdentityTypeDef,
         "iamUser": IAMUserIdentityTypeDef,
         "iamRole": IAMRoleIdentityTypeDef,
@@ -2919,14 +3298,29 @@
     {
         "TimeSeriesSummaries": List[TimeSeriesSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
+    {
+        "loggingOptions": LoggingOptionsTypeDef,
+    },
+)
+
+MetricWindowOutputTypeDef = TypedDict(
+    "MetricWindowOutputTypeDef",
+    {
+        "tumbling": TumblingWindowOutputTypeDef,
+    },
+    total=False,
+)
+
 MetricWindowTypeDef = TypedDict(
     "MetricWindowTypeDef",
     {
         "tumbling": TumblingWindowTypeDef,
     },
     total=False,
 )
@@ -2946,14 +3340,23 @@
 )
 
 
 class PortalStatusTypeDef(_RequiredPortalStatusTypeDef, _OptionalPortalStatusTypeDef):
     pass
 
 
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "portal": PortalResourceOutputTypeDef,
+        "project": ProjectResourceOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "portal": PortalResourceTypeDef,
         "project": ProjectResourceTypeDef,
     },
     total=False,
@@ -3026,28 +3429,28 @@
     },
 )
 
 BatchGetAssetPropertyValueHistorySuccessEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     {
         "entryId": str,
-        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
     },
 )
 
 _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
         "entryId": str,
     },
 )
 _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
-        "assetPropertyValue": AssetPropertyValueTypeDef,
+        "assetPropertyValue": AssetPropertyValueOutputTypeDef,
     },
     total=False,
 )
 
 
 class BatchGetAssetPropertyValueSuccessEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef,
@@ -3055,24 +3458,33 @@
 ):
     pass
 
 
 GetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryResponseTypeDef",
     {
-        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssetPropertyValueResponseTypeDef = TypedDict(
     "GetAssetPropertyValueResponseTypeDef",
     {
-        "propertyValue": AssetPropertyValueTypeDef,
+        "propertyValue": AssetPropertyValueOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
+    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    {
+        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
@@ -3093,23 +3505,14 @@
 
 class PutAssetPropertyValueEntryTypeDef(
     _RequiredPutAssetPropertyValueEntryTypeDef, _OptionalPutAssetPropertyValueEntryTypeDef
 ):
     pass
 
 
-GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
-    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
-    {
-        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     {
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -3150,34 +3553,53 @@
 
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
 
+JobConfigurationOutputTypeDef = TypedDict(
+    "JobConfigurationOutputTypeDef",
+    {
+        "fileFormat": FileFormatOutputTypeDef,
+    },
+)
+
 JobConfigurationTypeDef = TypedDict(
     "JobConfigurationTypeDef",
     {
         "fileFormat": FileFormatTypeDef,
     },
 )
 
 DescribeStorageConfigurationResponseTypeDef = TypedDict(
     "DescribeStorageConfigurationResponseTypeDef",
     {
         "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageTypeDef,
+        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "configurationStatus": ConfigurationStatusTypeDef,
         "lastUpdateDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutStorageConfigurationResponseTypeDef = TypedDict(
+    "PutStorageConfigurationResponseTypeDef",
+    {
+        "storageType": StorageTypeType,
+        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
+        "disassociatedDataStorage": DisassociatedDataStorageStateType,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutStorageConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageConfigurationRequestRequestTypeDef",
     {
         "storageType": StorageTypeType,
     },
 )
 _OptionalPutStorageConfigurationRequestRequestTypeDef = TypedDict(
@@ -3194,26 +3616,14 @@
 class PutStorageConfigurationRequestRequestTypeDef(
     _RequiredPutStorageConfigurationRequestRequestTypeDef,
     _OptionalPutStorageConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-PutStorageConfigurationResponseTypeDef = TypedDict(
-    "PutStorageConfigurationResponseTypeDef",
-    {
-        "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageTypeDef,
-        "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssetModelStatusTypeDef = TypedDict(
     "_RequiredAssetModelStatusTypeDef",
     {
         "state": AssetModelStateType,
     },
 )
 _OptionalAssetModelStatusTypeDef = TypedDict(
@@ -3244,71 +3654,77 @@
 )
 
 
 class AssetStatusTypeDef(_RequiredAssetStatusTypeDef, _OptionalAssetStatusTypeDef):
     pass
 
 
-MeasurementTypeDef = TypedDict(
-    "MeasurementTypeDef",
+MeasurementOutputTypeDef = TypedDict(
+    "MeasurementOutputTypeDef",
     {
-        "processingConfig": MeasurementProcessingConfigTypeDef,
+        "processingConfig": MeasurementProcessingConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredTransformTypeDef = TypedDict(
-    "_RequiredTransformTypeDef",
+_RequiredTransformOutputTypeDef = TypedDict(
+    "_RequiredTransformOutputTypeDef",
     {
         "expression": str,
-        "variables": Sequence[ExpressionVariableTypeDef],
+        "variables": List[ExpressionVariableOutputTypeDef],
     },
 )
-_OptionalTransformTypeDef = TypedDict(
-    "_OptionalTransformTypeDef",
+_OptionalTransformOutputTypeDef = TypedDict(
+    "_OptionalTransformOutputTypeDef",
     {
-        "processingConfig": TransformProcessingConfigTypeDef,
+        "processingConfig": TransformProcessingConfigOutputTypeDef,
     },
     total=False,
 )
 
 
-class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
+class TransformOutputTypeDef(_RequiredTransformOutputTypeDef, _OptionalTransformOutputTypeDef):
     pass
 
 
-_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateGatewayRequestRequestTypeDef",
+MeasurementTypeDef = TypedDict(
+    "MeasurementTypeDef",
     {
-        "gatewayName": str,
-        "gatewayPlatform": GatewayPlatformTypeDef,
+        "processingConfig": MeasurementProcessingConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateGatewayRequestRequestTypeDef",
+
+_RequiredTransformTypeDef = TypedDict(
+    "_RequiredTransformTypeDef",
     {
-        "tags": Mapping[str, str],
+        "expression": str,
+        "variables": Sequence[ExpressionVariableTypeDef],
+    },
+)
+_OptionalTransformTypeDef = TypedDict(
+    "_OptionalTransformTypeDef",
+    {
+        "processingConfig": TransformProcessingConfigTypeDef,
     },
     total=False,
 )
 
 
-class CreateGatewayRequestRequestTypeDef(
-    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
-):
+class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
     pass
 
 
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
         "gatewayArn": str,
-        "gatewayPlatform": GatewayPlatformTypeDef,
+        "gatewayPlatform": GatewayPlatformOutputTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
         "creationDate": datetime,
         "lastUpdateDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3320,25 +3736,68 @@
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
 )
 _OptionalGatewaySummaryTypeDef = TypedDict(
     "_OptionalGatewaySummaryTypeDef",
     {
-        "gatewayPlatform": GatewayPlatformTypeDef,
+        "gatewayPlatform": GatewayPlatformOutputTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
     },
     total=False,
 )
 
 
 class GatewaySummaryTypeDef(_RequiredGatewaySummaryTypeDef, _OptionalGatewaySummaryTypeDef):
     pass
 
 
+_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateGatewayRequestRequestTypeDef",
+    {
+        "gatewayName": str,
+        "gatewayPlatform": GatewayPlatformTypeDef,
+    },
+)
+_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateGatewayRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateGatewayRequestRequestTypeDef(
+    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "expression": str,
+        "variables": List[ExpressionVariableOutputTypeDef],
+        "window": MetricWindowOutputTypeDef,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "processingConfig": MetricProcessingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
+
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
         "window": MetricWindowTypeDef,
     },
@@ -3389,15 +3848,15 @@
         "portalStatus": PortalStatusTypeDef,
         "portalCreationDate": datetime,
         "portalLastUpdateDate": datetime,
         "portalLogoImageLocation": ImageLocationTypeDef,
         "roleArn": str,
         "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
-        "alarms": AlarmsTypeDef,
+        "alarms": AlarmsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPortalSummaryTypeDef = TypedDict(
     "_RequiredPortalSummaryTypeDef",
     {
@@ -3431,16 +3890,16 @@
     },
 )
 
 _RequiredAccessPolicySummaryTypeDef = TypedDict(
     "_RequiredAccessPolicySummaryTypeDef",
     {
         "id": str,
-        "identity": IdentityTypeDef,
-        "resource": ResourceTypeDef,
+        "identity": IdentityOutputTypeDef,
+        "resource": ResourceOutputTypeDef,
         "permission": PermissionType,
     },
 )
 _OptionalAccessPolicySummaryTypeDef = TypedDict(
     "_OptionalAccessPolicySummaryTypeDef",
     {
         "creationDate": datetime,
@@ -3452,14 +3911,28 @@
 
 class AccessPolicySummaryTypeDef(
     _RequiredAccessPolicySummaryTypeDef, _OptionalAccessPolicySummaryTypeDef
 ):
     pass
 
 
+DescribeAccessPolicyResponseTypeDef = TypedDict(
+    "DescribeAccessPolicyResponseTypeDef",
+    {
+        "accessPolicyId": str,
+        "accessPolicyArn": str,
+        "accessPolicyIdentity": IdentityOutputTypeDef,
+        "accessPolicyResource": ResourceOutputTypeDef,
+        "accessPolicyPermission": PermissionType,
+        "accessPolicyCreationDate": datetime,
+        "accessPolicyLastUpdateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
     },
@@ -3477,28 +3950,14 @@
 class CreateAccessPolicyRequestRequestTypeDef(
     _RequiredCreateAccessPolicyRequestRequestTypeDef,
     _OptionalCreateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAccessPolicyResponseTypeDef = TypedDict(
-    "DescribeAccessPolicyResponseTypeDef",
-    {
-        "accessPolicyId": str,
-        "accessPolicyArn": str,
-        "accessPolicyIdentity": IdentityTypeDef,
-        "accessPolicyResource": ResourceTypeDef,
-        "accessPolicyPermission": PermissionType,
-        "accessPolicyCreationDate": datetime,
-        "accessPolicyLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyId": str,
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
@@ -3564,38 +4023,38 @@
 BatchPutAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[PutAssetPropertyValueEntryTypeDef],
     },
 )
 
-CreateBulkImportJobRequestRequestTypeDef = TypedDict(
-    "CreateBulkImportJobRequestRequestTypeDef",
+DescribeBulkImportJobResponseTypeDef = TypedDict(
+    "DescribeBulkImportJobResponseTypeDef",
     {
+        "jobId": str,
         "jobName": str,
+        "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": Sequence[FileTypeDef],
-        "errorReportLocation": ErrorReportLocationTypeDef,
-        "jobConfiguration": JobConfigurationTypeDef,
+        "files": List[FileOutputTypeDef],
+        "errorReportLocation": ErrorReportLocationOutputTypeDef,
+        "jobConfiguration": JobConfigurationOutputTypeDef,
+        "jobCreationDate": datetime,
+        "jobLastUpdateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeBulkImportJobResponseTypeDef = TypedDict(
-    "DescribeBulkImportJobResponseTypeDef",
+CreateBulkImportJobRequestRequestTypeDef = TypedDict(
+    "CreateBulkImportJobRequestRequestTypeDef",
     {
-        "jobId": str,
         "jobName": str,
-        "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": List[FileTypeDef],
+        "files": Sequence[FileTypeDef],
         "errorReportLocation": ErrorReportLocationTypeDef,
         "jobConfiguration": JobConfigurationTypeDef,
-        "jobCreationDate": datetime,
-        "jobLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssetModelSummaryTypeDef = TypedDict(
     "AssetModelSummaryTypeDef",
     {
         "id": str,
@@ -3737,14 +4196,25 @@
     {
         "gatewaySummaries": List[GatewaySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PropertyTypeOutputTypeDef = TypedDict(
+    "PropertyTypeOutputTypeDef",
+    {
+        "attribute": AttributeOutputTypeDef,
+        "measurement": MeasurementOutputTypeDef,
+        "transform": TransformOutputTypeDef,
+        "metric": MetricOutputTypeDef,
+    },
+    total=False,
+)
+
 PropertyTypeTypeDef = TypedDict(
     "PropertyTypeTypeDef",
     {
         "attribute": AttributeTypeDef,
         "measurement": MeasurementTypeDef,
         "transform": TransformTypeDef,
         "metric": MetricTypeDef,
@@ -3793,44 +4263,45 @@
     {
         "assetSummaries": List[AssociatedAssetsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_RequiredAssetModelPropertyDefinitionTypeDef",
+_RequiredAssetModelPropertyOutputTypeDef = TypedDict(
+    "_RequiredAssetModelPropertyOutputTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeTypeDef,
+        "type": PropertyTypeOutputTypeDef,
     },
 )
-_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_OptionalAssetModelPropertyDefinitionTypeDef",
+_OptionalAssetModelPropertyOutputTypeDef = TypedDict(
+    "_OptionalAssetModelPropertyOutputTypeDef",
     {
+        "id": str,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
 
-class AssetModelPropertyDefinitionTypeDef(
-    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
+class AssetModelPropertyOutputTypeDef(
+    _RequiredAssetModelPropertyOutputTypeDef, _OptionalAssetModelPropertyOutputTypeDef
 ):
     pass
 
 
 _RequiredAssetModelPropertySummaryTypeDef = TypedDict(
     "_RequiredAssetModelPropertySummaryTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeTypeDef,
+        "type": PropertyTypeOutputTypeDef,
     },
 )
 _OptionalAssetModelPropertySummaryTypeDef = TypedDict(
     "_OptionalAssetModelPropertySummaryTypeDef",
     {
         "id": str,
         "dataTypeSpec": str,
@@ -3843,14 +4314,62 @@
 
 class AssetModelPropertySummaryTypeDef(
     _RequiredAssetModelPropertySummaryTypeDef, _OptionalAssetModelPropertySummaryTypeDef
 ):
     pass
 
 
+_RequiredPropertyTypeDef = TypedDict(
+    "_RequiredPropertyTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "dataType": PropertyDataTypeType,
+    },
+)
+_OptionalPropertyTypeDef = TypedDict(
+    "_OptionalPropertyTypeDef",
+    {
+        "alias": str,
+        "notification": PropertyNotificationTypeDef,
+        "unit": str,
+        "type": PropertyTypeOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
+    pass
+
+
+_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_RequiredAssetModelPropertyDefinitionTypeDef",
+    {
+        "name": str,
+        "dataType": PropertyDataTypeType,
+        "type": PropertyTypeTypeDef,
+    },
+)
+_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_OptionalAssetModelPropertyDefinitionTypeDef",
+    {
+        "dataTypeSpec": str,
+        "unit": str,
+    },
+    total=False,
+)
+
+
+class AssetModelPropertyDefinitionTypeDef(
+    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
+):
+    pass
+
+
 _RequiredAssetModelPropertyTypeDef = TypedDict(
     "_RequiredAssetModelPropertyTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
         "type": PropertyTypeTypeDef,
     },
@@ -3868,35 +4387,67 @@
 
 class AssetModelPropertyTypeDef(
     _RequiredAssetModelPropertyTypeDef, _OptionalAssetModelPropertyTypeDef
 ):
     pass
 
 
-_RequiredPropertyTypeDef = TypedDict(
-    "_RequiredPropertyTypeDef",
+_RequiredAssetModelCompositeModelOutputTypeDef = TypedDict(
+    "_RequiredAssetModelCompositeModelOutputTypeDef",
     {
+        "name": str,
+        "type": str,
+    },
+)
+_OptionalAssetModelCompositeModelOutputTypeDef = TypedDict(
+    "_OptionalAssetModelCompositeModelOutputTypeDef",
+    {
+        "description": str,
+        "properties": List[AssetModelPropertyOutputTypeDef],
         "id": str,
+    },
+    total=False,
+)
+
+
+class AssetModelCompositeModelOutputTypeDef(
+    _RequiredAssetModelCompositeModelOutputTypeDef, _OptionalAssetModelCompositeModelOutputTypeDef
+):
+    pass
+
+
+ListAssetModelPropertiesResponseTypeDef = TypedDict(
+    "ListAssetModelPropertiesResponseTypeDef",
+    {
+        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCompositeModelPropertyTypeDef = TypedDict(
+    "_RequiredCompositeModelPropertyTypeDef",
+    {
         "name": str,
-        "dataType": PropertyDataTypeType,
+        "type": str,
+        "assetProperty": PropertyTypeDef,
     },
 )
-_OptionalPropertyTypeDef = TypedDict(
-    "_OptionalPropertyTypeDef",
+_OptionalCompositeModelPropertyTypeDef = TypedDict(
+    "_OptionalCompositeModelPropertyTypeDef",
     {
-        "alias": str,
-        "notification": PropertyNotificationTypeDef,
-        "unit": str,
-        "type": PropertyTypeTypeDef,
+        "id": str,
     },
     total=False,
 )
 
 
-class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
+class CompositeModelPropertyTypeDef(
+    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
+):
     pass
 
 
 _RequiredAssetModelCompositeModelDefinitionTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelDefinitionTypeDef",
     {
         "name": str,
@@ -3916,70 +4467,67 @@
 class AssetModelCompositeModelDefinitionTypeDef(
     _RequiredAssetModelCompositeModelDefinitionTypeDef,
     _OptionalAssetModelCompositeModelDefinitionTypeDef,
 ):
     pass
 
 
-ListAssetModelPropertiesResponseTypeDef = TypedDict(
-    "ListAssetModelPropertiesResponseTypeDef",
-    {
-        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssetModelCompositeModelTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 _OptionalAssetModelCompositeModelTypeDef = TypedDict(
     "_OptionalAssetModelCompositeModelTypeDef",
     {
         "description": str,
-        "properties": List[AssetModelPropertyTypeDef],
+        "properties": Sequence[AssetModelPropertyTypeDef],
         "id": str,
     },
     total=False,
 )
 
 
 class AssetModelCompositeModelTypeDef(
     _RequiredAssetModelCompositeModelTypeDef, _OptionalAssetModelCompositeModelTypeDef
 ):
     pass
 
 
-_RequiredCompositeModelPropertyTypeDef = TypedDict(
-    "_RequiredCompositeModelPropertyTypeDef",
+DescribeAssetModelResponseTypeDef = TypedDict(
+    "DescribeAssetModelResponseTypeDef",
     {
-        "name": str,
-        "type": str,
-        "assetProperty": PropertyTypeDef,
+        "assetModelId": str,
+        "assetModelArn": str,
+        "assetModelName": str,
+        "assetModelDescription": str,
+        "assetModelProperties": List[AssetModelPropertyOutputTypeDef],
+        "assetModelHierarchies": List[AssetModelHierarchyOutputTypeDef],
+        "assetModelCompositeModels": List[AssetModelCompositeModelOutputTypeDef],
+        "assetModelCreationDate": datetime,
+        "assetModelLastUpdateDate": datetime,
+        "assetModelStatus": AssetModelStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCompositeModelPropertyTypeDef = TypedDict(
-    "_OptionalCompositeModelPropertyTypeDef",
+
+DescribeAssetPropertyResponseTypeDef = TypedDict(
+    "DescribeAssetPropertyResponseTypeDef",
     {
-        "id": str,
+        "assetId": str,
+        "assetName": str,
+        "assetModelId": str,
+        "assetProperty": PropertyTypeDef,
+        "compositeModel": CompositeModelPropertyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class CompositeModelPropertyTypeDef(
-    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
-):
-    pass
-
-
 _RequiredCreateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetModelRequestRequestTypeDef",
     {
         "assetModelName": str,
     },
 )
 _OptionalCreateAssetModelRequestRequestTypeDef = TypedDict(
@@ -3998,31 +4546,14 @@
 
 class CreateAssetModelRequestRequestTypeDef(
     _RequiredCreateAssetModelRequestRequestTypeDef, _OptionalCreateAssetModelRequestRequestTypeDef
 ):
     pass
 
 
-DescribeAssetModelResponseTypeDef = TypedDict(
-    "DescribeAssetModelResponseTypeDef",
-    {
-        "assetModelId": str,
-        "assetModelArn": str,
-        "assetModelName": str,
-        "assetModelDescription": str,
-        "assetModelProperties": List[AssetModelPropertyTypeDef],
-        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": List[AssetModelCompositeModelTypeDef],
-        "assetModelCreationDate": datetime,
-        "assetModelLastUpdateDate": datetime,
-        "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
         "assetModelName": str,
     },
 )
@@ -4039,20 +4570,7 @@
 )
 
 
 class UpdateAssetModelRequestRequestTypeDef(
     _RequiredUpdateAssetModelRequestRequestTypeDef, _OptionalUpdateAssetModelRequestRequestTypeDef
 ):
     pass
-
-
-DescribeAssetPropertyResponseTypeDef = TypedDict(
-    "DescribeAssetPropertyResponseTypeDef",
-    {
-        "assetId": str,
-        "assetName": str,
-        "assetModelId": str,
-        "assetProperty": PropertyTypeDef,
-        "compositeModel": CompositeModelPropertyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/type_defs.pyi` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -63,25 +63,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AggregatesTypeDef",
+    "AlarmsOutputTypeDef",
     "AlarmsTypeDef",
     "AssetErrorDetailsTypeDef",
     "AssetHierarchyInfoTypeDef",
     "AssetHierarchyTypeDef",
     "AssetModelHierarchyDefinitionTypeDef",
+    "AssetModelHierarchyOutputTypeDef",
     "AssetModelHierarchyTypeDef",
     "PropertyNotificationTypeDef",
+    "TimeInNanosOutputTypeDef",
+    "VariantOutputTypeDef",
     "TimeInNanosTypeDef",
     "VariantTypeDef",
     "AssociateAssetsRequestRequestTypeDef",
     "AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "BatchAssociateProjectAssetsRequestRequestTypeDef",
     "BatchDisassociateProjectAssetsRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     "BatchGetAssetPropertyAggregatesErrorInfoTypeDef",
     "BatchGetAssetPropertyValueEntryTypeDef",
@@ -98,15 +103,17 @@
     "CreateBulkImportJobResponseTypeDef",
     "CreateDashboardRequestRequestTypeDef",
     "CreateDashboardResponseTypeDef",
     "CreateGatewayResponseTypeDef",
     "ImageFileTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
+    "CsvOutputTypeDef",
     "CsvTypeDef",
+    "CustomerManagedS3StorageOutputTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
@@ -115,46 +122,56 @@
     "DeleteTimeSeriesRequestRequestTypeDef",
     "DescribeAccessPolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAssetModelRequestRequestTypeDef",
     "DescribeAssetPropertyRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribeBulkImportJobRequestRequestTypeDef",
+    "ErrorReportLocationOutputTypeDef",
+    "FileOutputTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardResponseTypeDef",
     "DescribeGatewayCapabilityConfigurationRequestRequestTypeDef",
     "DescribeGatewayCapabilityConfigurationResponseTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "GatewayCapabilitySummaryTypeDef",
-    "LoggingOptionsTypeDef",
+    "LoggingOptionsOutputTypeDef",
     "DescribePortalRequestRequestTypeDef",
     "ImageLocationTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
-    "RetentionPeriodTypeDef",
+    "RetentionPeriodOutputTypeDef",
     "DescribeTimeSeriesRequestRequestTypeDef",
     "DescribeTimeSeriesResponseTypeDef",
     "DetailedErrorTypeDef",
     "DisassociateAssetsRequestRequestTypeDef",
     "DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "VariableValueOutputTypeDef",
     "VariableValueTypeDef",
+    "ForwardingConfigOutputTypeDef",
     "ForwardingConfigTypeDef",
+    "GreengrassOutputTypeDef",
+    "GreengrassV2OutputTypeDef",
     "GreengrassTypeDef",
     "GreengrassV2TypeDef",
     "GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef",
     "GetAssetPropertyAggregatesRequestRequestTypeDef",
     "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "GetAssetPropertyValueRequestRequestTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef",
     "GetInterpolatedAssetPropertyValuesRequestRequestTypeDef",
+    "GroupIdentityOutputTypeDef",
     "GroupIdentityTypeDef",
+    "IAMRoleIdentityOutputTypeDef",
     "IAMRoleIdentityTypeDef",
+    "IAMUserIdentityOutputTypeDef",
     "IAMUserIdentityTypeDef",
+    "UserIdentityOutputTypeDef",
     "UserIdentityTypeDef",
     "JobSummaryTypeDef",
     "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
     "ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef",
     "ListAssetModelPropertiesRequestRequestTypeDef",
     "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
@@ -182,21 +199,27 @@
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     "ListTimeSeriesRequestRequestTypeDef",
     "TimeSeriesSummaryTypeDef",
+    "LoggingOptionsTypeDef",
+    "MetricProcessingConfigOutputTypeDef",
     "MetricProcessingConfigTypeDef",
+    "TumblingWindowOutputTypeDef",
     "TumblingWindowTypeDef",
     "MonitorErrorDetailsTypeDef",
     "PaginatorConfigTypeDef",
+    "PortalResourceOutputTypeDef",
     "PortalResourceTypeDef",
+    "ProjectResourceOutputTypeDef",
     "ProjectResourceTypeDef",
     "PutDefaultEncryptionConfigurationRequestRequestTypeDef",
+    "RetentionPeriodTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetPropertyRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "UpdateGatewayCapabilityConfigurationRequestRequestTypeDef",
@@ -206,120 +229,137 @@
     "AggregatedValueTypeDef",
     "BatchAssociateProjectAssetsResponseTypeDef",
     "BatchDisassociateProjectAssetsResponseTypeDef",
     "AssetRelationshipSummaryTypeDef",
     "AssetPropertySummaryTypeDef",
     "AssetPropertyTypeDef",
     "BatchPutAssetPropertyErrorTypeDef",
-    "AssetPropertyValueTypeDef",
+    "AssetPropertyValueOutputTypeDef",
     "InterpolatedAssetPropertyValueTypeDef",
+    "AssetPropertyValueTypeDef",
     "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     "ConfigurationStatusTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "ImageTypeDef",
+    "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
+    "MultiLayerStorageOutputTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
     "DescribeAssetRequestAssetNotExistsWaitTypeDef",
     "DescribePortalRequestPortalActiveWaitTypeDef",
     "DescribePortalRequestPortalNotExistsWaitTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "PutLoggingOptionsRequestRequestTypeDef",
     "ErrorDetailsTypeDef",
+    "ExpressionVariableOutputTypeDef",
     "ExpressionVariableTypeDef",
+    "MeasurementProcessingConfigOutputTypeDef",
+    "TransformProcessingConfigOutputTypeDef",
     "MeasurementProcessingConfigTypeDef",
     "TransformProcessingConfigTypeDef",
+    "GatewayPlatformOutputTypeDef",
     "GatewayPlatformTypeDef",
+    "IdentityOutputTypeDef",
     "IdentityTypeDef",
     "ListBulkImportJobsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ListTimeSeriesResponseTypeDef",
+    "PutLoggingOptionsRequestRequestTypeDef",
+    "MetricWindowOutputTypeDef",
     "MetricWindowTypeDef",
     "PortalStatusTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetAssetPropertyAggregatesSuccessEntryTypeDef",
     "GetAssetPropertyAggregatesResponseTypeDef",
     "ListAssetRelationshipsResponseTypeDef",
     "ListAssetPropertiesResponseTypeDef",
     "AssetCompositeModelTypeDef",
     "BatchPutAssetPropertyErrorEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     "BatchGetAssetPropertyValueSuccessEntryTypeDef",
     "GetAssetPropertyValueHistoryResponseTypeDef",
     "GetAssetPropertyValueResponseTypeDef",
-    "PutAssetPropertyValueEntryTypeDef",
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    "PutAssetPropertyValueEntryTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
     "UpdatePortalRequestRequestTypeDef",
+    "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
-    "PutStorageConfigurationRequestRequestTypeDef",
     "PutStorageConfigurationResponseTypeDef",
+    "PutStorageConfigurationRequestRequestTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
+    "MeasurementOutputTypeDef",
+    "TransformOutputTypeDef",
     "MeasurementTypeDef",
     "TransformTypeDef",
-    "CreateGatewayRequestRequestTypeDef",
     "DescribeGatewayResponseTypeDef",
     "GatewaySummaryTypeDef",
+    "CreateGatewayRequestRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
     "CreatePortalResponseTypeDef",
     "DeletePortalResponseTypeDef",
     "DescribePortalResponseTypeDef",
     "PortalSummaryTypeDef",
     "UpdatePortalResponseTypeDef",
     "AccessPolicySummaryTypeDef",
-    "CreateAccessPolicyRequestRequestTypeDef",
     "DescribeAccessPolicyResponseTypeDef",
+    "CreateAccessPolicyRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
-    "CreateBulkImportJobRequestRequestTypeDef",
     "DescribeBulkImportJobResponseTypeDef",
+    "CreateBulkImportJobRequestRequestTypeDef",
     "AssetModelSummaryTypeDef",
     "CreateAssetModelResponseTypeDef",
     "DeleteAssetModelResponseTypeDef",
     "UpdateAssetModelResponseTypeDef",
     "AssetSummaryTypeDef",
     "AssociatedAssetsSummaryTypeDef",
     "CreateAssetResponseTypeDef",
     "DeleteAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListGatewaysResponseTypeDef",
+    "PropertyTypeOutputTypeDef",
     "PropertyTypeTypeDef",
     "ListPortalsResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
     "ListAssetModelsResponseTypeDef",
     "ListAssetsResponseTypeDef",
     "ListAssociatedAssetsResponseTypeDef",
-    "AssetModelPropertyDefinitionTypeDef",
+    "AssetModelPropertyOutputTypeDef",
     "AssetModelPropertySummaryTypeDef",
-    "AssetModelPropertyTypeDef",
     "PropertyTypeDef",
-    "AssetModelCompositeModelDefinitionTypeDef",
+    "AssetModelPropertyDefinitionTypeDef",
+    "AssetModelPropertyTypeDef",
+    "AssetModelCompositeModelOutputTypeDef",
     "ListAssetModelPropertiesResponseTypeDef",
-    "AssetModelCompositeModelTypeDef",
     "CompositeModelPropertyTypeDef",
-    "CreateAssetModelRequestRequestTypeDef",
+    "AssetModelCompositeModelDefinitionTypeDef",
+    "AssetModelCompositeModelTypeDef",
     "DescribeAssetModelResponseTypeDef",
-    "UpdateAssetModelRequestRequestTypeDef",
     "DescribeAssetPropertyResponseTypeDef",
+    "CreateAssetModelRequestRequestTypeDef",
+    "UpdateAssetModelRequestRequestTypeDef",
 )
 
 AggregatesTypeDef = TypedDict(
     "AggregatesTypeDef",
     {
         "average": float,
         "count": float,
@@ -327,14 +367,31 @@
         "minimum": float,
         "sum": float,
         "standardDeviation": float,
     },
     total=False,
 )
 
+_RequiredAlarmsOutputTypeDef = TypedDict(
+    "_RequiredAlarmsOutputTypeDef",
+    {
+        "alarmRoleArn": str,
+    },
+)
+_OptionalAlarmsOutputTypeDef = TypedDict(
+    "_OptionalAlarmsOutputTypeDef",
+    {
+        "notificationLambdaArn": str,
+    },
+    total=False,
+)
+
+class AlarmsOutputTypeDef(_RequiredAlarmsOutputTypeDef, _OptionalAlarmsOutputTypeDef):
+    pass
+
 _RequiredAlarmsTypeDef = TypedDict(
     "_RequiredAlarmsTypeDef",
     {
         "alarmRoleArn": str,
     },
 )
 _OptionalAlarmsTypeDef = TypedDict(
@@ -387,14 +444,34 @@
     "AssetModelHierarchyDefinitionTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
 
+_RequiredAssetModelHierarchyOutputTypeDef = TypedDict(
+    "_RequiredAssetModelHierarchyOutputTypeDef",
+    {
+        "name": str,
+        "childAssetModelId": str,
+    },
+)
+_OptionalAssetModelHierarchyOutputTypeDef = TypedDict(
+    "_OptionalAssetModelHierarchyOutputTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+class AssetModelHierarchyOutputTypeDef(
+    _RequiredAssetModelHierarchyOutputTypeDef, _OptionalAssetModelHierarchyOutputTypeDef
+):
+    pass
+
 _RequiredAssetModelHierarchyTypeDef = TypedDict(
     "_RequiredAssetModelHierarchyTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
@@ -415,14 +492,44 @@
     "PropertyNotificationTypeDef",
     {
         "topic": str,
         "state": PropertyNotificationStateType,
     },
 )
 
+_RequiredTimeInNanosOutputTypeDef = TypedDict(
+    "_RequiredTimeInNanosOutputTypeDef",
+    {
+        "timeInSeconds": int,
+    },
+)
+_OptionalTimeInNanosOutputTypeDef = TypedDict(
+    "_OptionalTimeInNanosOutputTypeDef",
+    {
+        "offsetInNanos": int,
+    },
+    total=False,
+)
+
+class TimeInNanosOutputTypeDef(
+    _RequiredTimeInNanosOutputTypeDef, _OptionalTimeInNanosOutputTypeDef
+):
+    pass
+
+VariantOutputTypeDef = TypedDict(
+    "VariantOutputTypeDef",
+    {
+        "stringValue": str,
+        "integerValue": int,
+        "doubleValue": float,
+        "booleanValue": bool,
+    },
+    total=False,
+)
+
 _RequiredTimeInNanosTypeDef = TypedDict(
     "_RequiredTimeInNanosTypeDef",
     {
         "timeInSeconds": int,
     },
 )
 _OptionalTimeInNanosTypeDef = TypedDict(
@@ -486,14 +593,22 @@
 
 class AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef(
     _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     _OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
+AttributeOutputTypeDef = TypedDict(
+    "AttributeOutputTypeDef",
+    {
+        "defaultValue": str,
+    },
+    total=False,
+)
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "defaultValue": str,
     },
     total=False,
 )
@@ -817,22 +932,38 @@
     {
         "projectId": str,
         "projectArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CsvOutputTypeDef = TypedDict(
+    "CsvOutputTypeDef",
+    {
+        "columnNames": List[ColumnNameType],
+    },
+    total=False,
+)
+
 CsvTypeDef = TypedDict(
     "CsvTypeDef",
     {
         "columnNames": Sequence[ColumnNameType],
     },
     total=False,
 )
 
+CustomerManagedS3StorageOutputTypeDef = TypedDict(
+    "CustomerManagedS3StorageOutputTypeDef",
+    {
+        "s3ResourceArn": str,
+        "roleArn": str,
+    },
+)
+
 CustomerManagedS3StorageTypeDef = TypedDict(
     "CustomerManagedS3StorageTypeDef",
     {
         "s3ResourceArn": str,
         "roleArn": str,
     },
 )
@@ -1056,14 +1187,40 @@
 DescribeBulkImportJobRequestRequestTypeDef = TypedDict(
     "DescribeBulkImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
+ErrorReportLocationOutputTypeDef = TypedDict(
+    "ErrorReportLocationOutputTypeDef",
+    {
+        "bucket": str,
+        "prefix": str,
+    },
+)
+
+_RequiredFileOutputTypeDef = TypedDict(
+    "_RequiredFileOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+    },
+)
+_OptionalFileOutputTypeDef = TypedDict(
+    "_OptionalFileOutputTypeDef",
+    {
+        "versionId": str,
+    },
+    total=False,
+)
+
+class FileOutputTypeDef(_RequiredFileOutputTypeDef, _OptionalFileOutputTypeDef):
+    pass
+
 DescribeDashboardRequestRequestTypeDef = TypedDict(
     "DescribeDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
     },
 )
 
@@ -1112,16 +1269,16 @@
     "GatewayCapabilitySummaryTypeDef",
     {
         "capabilityNamespace": str,
         "capabilitySyncStatus": CapabilitySyncStatusType,
     },
 )
 
-LoggingOptionsTypeDef = TypedDict(
-    "LoggingOptionsTypeDef",
+LoggingOptionsOutputTypeDef = TypedDict(
+    "LoggingOptionsOutputTypeDef",
     {
         "level": LoggingLevelType,
     },
 )
 
 DescribePortalRequestRequestTypeDef = TypedDict(
     "DescribePortalRequestRequestTypeDef",
@@ -1155,16 +1312,16 @@
         "projectDescription": str,
         "projectCreationDate": datetime,
         "projectLastUpdateDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
     {
         "numberOfDays": int,
         "unlimited": bool,
     },
     total=False,
 )
 
@@ -1249,14 +1406,33 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredVariableValueOutputTypeDef = TypedDict(
+    "_RequiredVariableValueOutputTypeDef",
+    {
+        "propertyId": str,
+    },
+)
+_OptionalVariableValueOutputTypeDef = TypedDict(
+    "_OptionalVariableValueOutputTypeDef",
+    {
+        "hierarchyId": str,
+    },
+    total=False,
+)
+
+class VariableValueOutputTypeDef(
+    _RequiredVariableValueOutputTypeDef, _OptionalVariableValueOutputTypeDef
+):
+    pass
+
 _RequiredVariableValueTypeDef = TypedDict(
     "_RequiredVariableValueTypeDef",
     {
         "propertyId": str,
     },
 )
 _OptionalVariableValueTypeDef = TypedDict(
@@ -1266,21 +1442,42 @@
     },
     total=False,
 )
 
 class VariableValueTypeDef(_RequiredVariableValueTypeDef, _OptionalVariableValueTypeDef):
     pass
 
+ForwardingConfigOutputTypeDef = TypedDict(
+    "ForwardingConfigOutputTypeDef",
+    {
+        "state": ForwardingConfigStateType,
+    },
+)
+
 ForwardingConfigTypeDef = TypedDict(
     "ForwardingConfigTypeDef",
     {
         "state": ForwardingConfigStateType,
     },
 )
 
+GreengrassOutputTypeDef = TypedDict(
+    "GreengrassOutputTypeDef",
+    {
+        "groupArn": str,
+    },
+)
+
+GreengrassV2OutputTypeDef = TypedDict(
+    "GreengrassV2OutputTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+
 GreengrassTypeDef = TypedDict(
     "GreengrassTypeDef",
     {
         "groupArn": str,
     },
 )
 
@@ -1446,35 +1643,63 @@
 
 class GetInterpolatedAssetPropertyValuesRequestRequestTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
 ):
     pass
 
+GroupIdentityOutputTypeDef = TypedDict(
+    "GroupIdentityOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 GroupIdentityTypeDef = TypedDict(
     "GroupIdentityTypeDef",
     {
         "id": str,
     },
 )
 
+IAMRoleIdentityOutputTypeDef = TypedDict(
+    "IAMRoleIdentityOutputTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 IAMRoleIdentityTypeDef = TypedDict(
     "IAMRoleIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
+IAMUserIdentityOutputTypeDef = TypedDict(
+    "IAMUserIdentityOutputTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 IAMUserIdentityTypeDef = TypedDict(
     "IAMUserIdentityTypeDef",
     {
         "arn": str,
     },
 )
 
+UserIdentityOutputTypeDef = TypedDict(
+    "UserIdentityOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1988,21 +2213,54 @@
 )
 
 class TimeSeriesSummaryTypeDef(
     _RequiredTimeSeriesSummaryTypeDef, _OptionalTimeSeriesSummaryTypeDef
 ):
     pass
 
+LoggingOptionsTypeDef = TypedDict(
+    "LoggingOptionsTypeDef",
+    {
+        "level": LoggingLevelType,
+    },
+)
+
+MetricProcessingConfigOutputTypeDef = TypedDict(
+    "MetricProcessingConfigOutputTypeDef",
+    {
+        "computeLocation": ComputeLocationType,
+    },
+)
+
 MetricProcessingConfigTypeDef = TypedDict(
     "MetricProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
 
+_RequiredTumblingWindowOutputTypeDef = TypedDict(
+    "_RequiredTumblingWindowOutputTypeDef",
+    {
+        "interval": str,
+    },
+)
+_OptionalTumblingWindowOutputTypeDef = TypedDict(
+    "_OptionalTumblingWindowOutputTypeDef",
+    {
+        "offset": str,
+    },
+    total=False,
+)
+
+class TumblingWindowOutputTypeDef(
+    _RequiredTumblingWindowOutputTypeDef, _OptionalTumblingWindowOutputTypeDef
+):
+    pass
+
 _RequiredTumblingWindowTypeDef = TypedDict(
     "_RequiredTumblingWindowTypeDef",
     {
         "interval": str,
     },
 )
 _OptionalTumblingWindowTypeDef = TypedDict(
@@ -2031,21 +2289,35 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PortalResourceOutputTypeDef = TypedDict(
+    "PortalResourceOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 PortalResourceTypeDef = TypedDict(
     "PortalResourceTypeDef",
     {
         "id": str,
     },
 )
 
+ProjectResourceOutputTypeDef = TypedDict(
+    "ProjectResourceOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 ProjectResourceTypeDef = TypedDict(
     "ProjectResourceTypeDef",
     {
         "id": str,
     },
 )
 
@@ -2065,14 +2337,23 @@
 
 class PutDefaultEncryptionConfigurationRequestRequestTypeDef(
     _RequiredPutDefaultEncryptionConfigurationRequestRequestTypeDef,
     _OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
+    {
+        "numberOfDays": int,
+        "unlimited": bool,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -2298,15 +2579,43 @@
     pass
 
 BatchPutAssetPropertyErrorTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorTypeDef",
     {
         "errorCode": BatchPutAssetPropertyValueErrorCodeType,
         "errorMessage": str,
-        "timestamps": List[TimeInNanosTypeDef],
+        "timestamps": List[TimeInNanosOutputTypeDef],
+    },
+)
+
+_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueOutputTypeDef",
+    {
+        "value": VariantOutputTypeDef,
+        "timestamp": TimeInNanosOutputTypeDef,
+    },
+)
+_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueOutputTypeDef",
+    {
+        "quality": QualityType,
+    },
+    total=False,
+)
+
+class AssetPropertyValueOutputTypeDef(
+    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
+):
+    pass
+
+InterpolatedAssetPropertyValueTypeDef = TypedDict(
+    "InterpolatedAssetPropertyValueTypeDef",
+    {
+        "timestamp": TimeInNanosOutputTypeDef,
+        "value": VariantOutputTypeDef,
     },
 )
 
 _RequiredAssetPropertyValueTypeDef = TypedDict(
     "_RequiredAssetPropertyValueTypeDef",
     {
         "value": VariantTypeDef,
@@ -2322,22 +2631,14 @@
 )
 
 class AssetPropertyValueTypeDef(
     _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
-InterpolatedAssetPropertyValueTypeDef = TypedDict(
-    "InterpolatedAssetPropertyValueTypeDef",
-    {
-        "timestamp": TimeInNanosTypeDef,
-        "value": VariantTypeDef,
-    },
-)
-
 _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],
     },
 )
 _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
@@ -2510,22 +2811,37 @@
     {
         "id": str,
         "file": ImageFileTypeDef,
     },
     total=False,
 )
 
+FileFormatOutputTypeDef = TypedDict(
+    "FileFormatOutputTypeDef",
+    {
+        "csv": CsvOutputTypeDef,
+    },
+    total=False,
+)
+
 FileFormatTypeDef = TypedDict(
     "FileFormatTypeDef",
     {
         "csv": CsvTypeDef,
     },
     total=False,
 )
 
+MultiLayerStorageOutputTypeDef = TypedDict(
+    "MultiLayerStorageOutputTypeDef",
+    {
+        "customerManagedS3Storage": CustomerManagedS3StorageOutputTypeDef,
+    },
+)
+
 MultiLayerStorageTypeDef = TypedDict(
     "MultiLayerStorageTypeDef",
     {
         "customerManagedS3Storage": CustomerManagedS3StorageTypeDef,
     },
 )
 
@@ -2661,26 +2977,19 @@
     _OptionalDescribePortalRequestPortalNotExistsWaitTypeDef,
 ):
     pass
 
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
-    {
-        "loggingOptions": LoggingOptionsTypeDef,
-    },
-)
-
 _RequiredErrorDetailsTypeDef = TypedDict(
     "_RequiredErrorDetailsTypeDef",
     {
         "code": ErrorCodeType,
         "message": str,
     },
 )
@@ -2691,22 +3000,56 @@
     },
     total=False,
 )
 
 class ErrorDetailsTypeDef(_RequiredErrorDetailsTypeDef, _OptionalErrorDetailsTypeDef):
     pass
 
+ExpressionVariableOutputTypeDef = TypedDict(
+    "ExpressionVariableOutputTypeDef",
+    {
+        "name": str,
+        "value": VariableValueOutputTypeDef,
+    },
+)
+
 ExpressionVariableTypeDef = TypedDict(
     "ExpressionVariableTypeDef",
     {
         "name": str,
         "value": VariableValueTypeDef,
     },
 )
 
+MeasurementProcessingConfigOutputTypeDef = TypedDict(
+    "MeasurementProcessingConfigOutputTypeDef",
+    {
+        "forwardingConfig": ForwardingConfigOutputTypeDef,
+    },
+)
+
+_RequiredTransformProcessingConfigOutputTypeDef = TypedDict(
+    "_RequiredTransformProcessingConfigOutputTypeDef",
+    {
+        "computeLocation": ComputeLocationType,
+    },
+)
+_OptionalTransformProcessingConfigOutputTypeDef = TypedDict(
+    "_OptionalTransformProcessingConfigOutputTypeDef",
+    {
+        "forwardingConfig": ForwardingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class TransformProcessingConfigOutputTypeDef(
+    _RequiredTransformProcessingConfigOutputTypeDef, _OptionalTransformProcessingConfigOutputTypeDef
+):
+    pass
+
 MeasurementProcessingConfigTypeDef = TypedDict(
     "MeasurementProcessingConfigTypeDef",
     {
         "forwardingConfig": ForwardingConfigTypeDef,
     },
 )
 
@@ -2725,23 +3068,43 @@
 )
 
 class TransformProcessingConfigTypeDef(
     _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
 ):
     pass
 
+GatewayPlatformOutputTypeDef = TypedDict(
+    "GatewayPlatformOutputTypeDef",
+    {
+        "greengrass": GreengrassOutputTypeDef,
+        "greengrassV2": GreengrassV2OutputTypeDef,
+    },
+    total=False,
+)
+
 GatewayPlatformTypeDef = TypedDict(
     "GatewayPlatformTypeDef",
     {
         "greengrass": GreengrassTypeDef,
         "greengrassV2": GreengrassV2TypeDef,
     },
     total=False,
 )
 
+IdentityOutputTypeDef = TypedDict(
+    "IdentityOutputTypeDef",
+    {
+        "user": UserIdentityOutputTypeDef,
+        "group": GroupIdentityOutputTypeDef,
+        "iamUser": IAMUserIdentityOutputTypeDef,
+        "iamRole": IAMRoleIdentityOutputTypeDef,
+    },
+    total=False,
+)
+
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "user": UserIdentityTypeDef,
         "group": GroupIdentityTypeDef,
         "iamUser": IAMUserIdentityTypeDef,
         "iamRole": IAMRoleIdentityTypeDef,
@@ -2772,14 +3135,29 @@
     {
         "TimeSeriesSummaries": List[TimeSeriesSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutLoggingOptionsRequestRequestTypeDef = TypedDict(
+    "PutLoggingOptionsRequestRequestTypeDef",
+    {
+        "loggingOptions": LoggingOptionsTypeDef,
+    },
+)
+
+MetricWindowOutputTypeDef = TypedDict(
+    "MetricWindowOutputTypeDef",
+    {
+        "tumbling": TumblingWindowOutputTypeDef,
+    },
+    total=False,
+)
+
 MetricWindowTypeDef = TypedDict(
     "MetricWindowTypeDef",
     {
         "tumbling": TumblingWindowTypeDef,
     },
     total=False,
 )
@@ -2797,14 +3175,23 @@
     },
     total=False,
 )
 
 class PortalStatusTypeDef(_RequiredPortalStatusTypeDef, _OptionalPortalStatusTypeDef):
     pass
 
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "portal": PortalResourceOutputTypeDef,
+        "project": ProjectResourceOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "portal": PortalResourceTypeDef,
         "project": ProjectResourceTypeDef,
     },
     total=False,
@@ -2875,51 +3262,60 @@
     },
 )
 
 BatchGetAssetPropertyValueHistorySuccessEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueHistorySuccessEntryTypeDef",
     {
         "entryId": str,
-        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
     },
 )
 
 _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
         "entryId": str,
     },
 )
 _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef = TypedDict(
     "_OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
-        "assetPropertyValue": AssetPropertyValueTypeDef,
+        "assetPropertyValue": AssetPropertyValueOutputTypeDef,
     },
     total=False,
 )
 
 class BatchGetAssetPropertyValueSuccessEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef,
 ):
     pass
 
 GetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryResponseTypeDef",
     {
-        "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
+        "assetPropertyValueHistory": List[AssetPropertyValueOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssetPropertyValueResponseTypeDef = TypedDict(
     "GetAssetPropertyValueResponseTypeDef",
     {
-        "propertyValue": AssetPropertyValueTypeDef,
+        "propertyValue": AssetPropertyValueOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
+    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
+    {
+        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
@@ -2938,23 +3334,14 @@
 )
 
 class PutAssetPropertyValueEntryTypeDef(
     _RequiredPutAssetPropertyValueEntryTypeDef, _OptionalPutAssetPropertyValueEntryTypeDef
 ):
     pass
 
-GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
-    "GetInterpolatedAssetPropertyValuesResponseTypeDef",
-    {
-        "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDefaultEncryptionConfigurationResponseTypeDef = TypedDict(
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     {
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2993,34 +3380,53 @@
 )
 
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
+JobConfigurationOutputTypeDef = TypedDict(
+    "JobConfigurationOutputTypeDef",
+    {
+        "fileFormat": FileFormatOutputTypeDef,
+    },
+)
+
 JobConfigurationTypeDef = TypedDict(
     "JobConfigurationTypeDef",
     {
         "fileFormat": FileFormatTypeDef,
     },
 )
 
 DescribeStorageConfigurationResponseTypeDef = TypedDict(
     "DescribeStorageConfigurationResponseTypeDef",
     {
         "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageTypeDef,
+        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodTypeDef,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
         "configurationStatus": ConfigurationStatusTypeDef,
         "lastUpdateDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutStorageConfigurationResponseTypeDef = TypedDict(
+    "PutStorageConfigurationResponseTypeDef",
+    {
+        "storageType": StorageTypeType,
+        "multiLayerStorage": MultiLayerStorageOutputTypeDef,
+        "disassociatedDataStorage": DisassociatedDataStorageStateType,
+        "retentionPeriod": RetentionPeriodOutputTypeDef,
+        "configurationStatus": ConfigurationStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutStorageConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageConfigurationRequestRequestTypeDef",
     {
         "storageType": StorageTypeType,
     },
 )
 _OptionalPutStorageConfigurationRequestRequestTypeDef = TypedDict(
@@ -3035,26 +3441,14 @@
 
 class PutStorageConfigurationRequestRequestTypeDef(
     _RequiredPutStorageConfigurationRequestRequestTypeDef,
     _OptionalPutStorageConfigurationRequestRequestTypeDef,
 ):
     pass
 
-PutStorageConfigurationResponseTypeDef = TypedDict(
-    "PutStorageConfigurationResponseTypeDef",
-    {
-        "storageType": StorageTypeType,
-        "multiLayerStorage": MultiLayerStorageTypeDef,
-        "disassociatedDataStorage": DisassociatedDataStorageStateType,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "configurationStatus": ConfigurationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssetModelStatusTypeDef = TypedDict(
     "_RequiredAssetModelStatusTypeDef",
     {
         "state": AssetModelStateType,
     },
 )
 _OptionalAssetModelStatusTypeDef = TypedDict(
@@ -3081,67 +3475,73 @@
     },
     total=False,
 )
 
 class AssetStatusTypeDef(_RequiredAssetStatusTypeDef, _OptionalAssetStatusTypeDef):
     pass
 
-MeasurementTypeDef = TypedDict(
-    "MeasurementTypeDef",
+MeasurementOutputTypeDef = TypedDict(
+    "MeasurementOutputTypeDef",
     {
-        "processingConfig": MeasurementProcessingConfigTypeDef,
+        "processingConfig": MeasurementProcessingConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredTransformTypeDef = TypedDict(
-    "_RequiredTransformTypeDef",
+_RequiredTransformOutputTypeDef = TypedDict(
+    "_RequiredTransformOutputTypeDef",
     {
         "expression": str,
-        "variables": Sequence[ExpressionVariableTypeDef],
+        "variables": List[ExpressionVariableOutputTypeDef],
     },
 )
-_OptionalTransformTypeDef = TypedDict(
-    "_OptionalTransformTypeDef",
+_OptionalTransformOutputTypeDef = TypedDict(
+    "_OptionalTransformOutputTypeDef",
     {
-        "processingConfig": TransformProcessingConfigTypeDef,
+        "processingConfig": TransformProcessingConfigOutputTypeDef,
     },
     total=False,
 )
 
-class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
+class TransformOutputTypeDef(_RequiredTransformOutputTypeDef, _OptionalTransformOutputTypeDef):
     pass
 
-_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateGatewayRequestRequestTypeDef",
+MeasurementTypeDef = TypedDict(
+    "MeasurementTypeDef",
     {
-        "gatewayName": str,
-        "gatewayPlatform": GatewayPlatformTypeDef,
+        "processingConfig": MeasurementProcessingConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateGatewayRequestRequestTypeDef",
+
+_RequiredTransformTypeDef = TypedDict(
+    "_RequiredTransformTypeDef",
     {
-        "tags": Mapping[str, str],
+        "expression": str,
+        "variables": Sequence[ExpressionVariableTypeDef],
+    },
+)
+_OptionalTransformTypeDef = TypedDict(
+    "_OptionalTransformTypeDef",
+    {
+        "processingConfig": TransformProcessingConfigTypeDef,
     },
     total=False,
 )
 
-class CreateGatewayRequestRequestTypeDef(
-    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
-):
+class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
     pass
 
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
         "gatewayArn": str,
-        "gatewayPlatform": GatewayPlatformTypeDef,
+        "gatewayPlatform": GatewayPlatformOutputTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
         "creationDate": datetime,
         "lastUpdateDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3153,23 +3553,62 @@
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
 )
 _OptionalGatewaySummaryTypeDef = TypedDict(
     "_OptionalGatewaySummaryTypeDef",
     {
-        "gatewayPlatform": GatewayPlatformTypeDef,
+        "gatewayPlatform": GatewayPlatformOutputTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
     },
     total=False,
 )
 
 class GatewaySummaryTypeDef(_RequiredGatewaySummaryTypeDef, _OptionalGatewaySummaryTypeDef):
     pass
 
+_RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateGatewayRequestRequestTypeDef",
+    {
+        "gatewayName": str,
+        "gatewayPlatform": GatewayPlatformTypeDef,
+    },
+)
+_OptionalCreateGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateGatewayRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateGatewayRequestRequestTypeDef(
+    _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
+):
+    pass
+
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "expression": str,
+        "variables": List[ExpressionVariableOutputTypeDef],
+        "window": MetricWindowOutputTypeDef,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "processingConfig": MetricProcessingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
         "window": MetricWindowTypeDef,
     },
@@ -3218,15 +3657,15 @@
         "portalStatus": PortalStatusTypeDef,
         "portalCreationDate": datetime,
         "portalLastUpdateDate": datetime,
         "portalLogoImageLocation": ImageLocationTypeDef,
         "roleArn": str,
         "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
-        "alarms": AlarmsTypeDef,
+        "alarms": AlarmsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPortalSummaryTypeDef = TypedDict(
     "_RequiredPortalSummaryTypeDef",
     {
@@ -3258,16 +3697,16 @@
     },
 )
 
 _RequiredAccessPolicySummaryTypeDef = TypedDict(
     "_RequiredAccessPolicySummaryTypeDef",
     {
         "id": str,
-        "identity": IdentityTypeDef,
-        "resource": ResourceTypeDef,
+        "identity": IdentityOutputTypeDef,
+        "resource": ResourceOutputTypeDef,
         "permission": PermissionType,
     },
 )
 _OptionalAccessPolicySummaryTypeDef = TypedDict(
     "_OptionalAccessPolicySummaryTypeDef",
     {
         "creationDate": datetime,
@@ -3277,14 +3716,28 @@
 )
 
 class AccessPolicySummaryTypeDef(
     _RequiredAccessPolicySummaryTypeDef, _OptionalAccessPolicySummaryTypeDef
 ):
     pass
 
+DescribeAccessPolicyResponseTypeDef = TypedDict(
+    "DescribeAccessPolicyResponseTypeDef",
+    {
+        "accessPolicyId": str,
+        "accessPolicyArn": str,
+        "accessPolicyIdentity": IdentityOutputTypeDef,
+        "accessPolicyResource": ResourceOutputTypeDef,
+        "accessPolicyPermission": PermissionType,
+        "accessPolicyCreationDate": datetime,
+        "accessPolicyLastUpdateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
     },
@@ -3300,28 +3753,14 @@
 
 class CreateAccessPolicyRequestRequestTypeDef(
     _RequiredCreateAccessPolicyRequestRequestTypeDef,
     _OptionalCreateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
-DescribeAccessPolicyResponseTypeDef = TypedDict(
-    "DescribeAccessPolicyResponseTypeDef",
-    {
-        "accessPolicyId": str,
-        "accessPolicyArn": str,
-        "accessPolicyIdentity": IdentityTypeDef,
-        "accessPolicyResource": ResourceTypeDef,
-        "accessPolicyPermission": PermissionType,
-        "accessPolicyCreationDate": datetime,
-        "accessPolicyLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyId": str,
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
@@ -3385,38 +3824,38 @@
 BatchPutAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[PutAssetPropertyValueEntryTypeDef],
     },
 )
 
-CreateBulkImportJobRequestRequestTypeDef = TypedDict(
-    "CreateBulkImportJobRequestRequestTypeDef",
+DescribeBulkImportJobResponseTypeDef = TypedDict(
+    "DescribeBulkImportJobResponseTypeDef",
     {
+        "jobId": str,
         "jobName": str,
+        "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": Sequence[FileTypeDef],
-        "errorReportLocation": ErrorReportLocationTypeDef,
-        "jobConfiguration": JobConfigurationTypeDef,
+        "files": List[FileOutputTypeDef],
+        "errorReportLocation": ErrorReportLocationOutputTypeDef,
+        "jobConfiguration": JobConfigurationOutputTypeDef,
+        "jobCreationDate": datetime,
+        "jobLastUpdateDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeBulkImportJobResponseTypeDef = TypedDict(
-    "DescribeBulkImportJobResponseTypeDef",
+CreateBulkImportJobRequestRequestTypeDef = TypedDict(
+    "CreateBulkImportJobRequestRequestTypeDef",
     {
-        "jobId": str,
         "jobName": str,
-        "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": List[FileTypeDef],
+        "files": Sequence[FileTypeDef],
         "errorReportLocation": ErrorReportLocationTypeDef,
         "jobConfiguration": JobConfigurationTypeDef,
-        "jobCreationDate": datetime,
-        "jobLastUpdateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssetModelSummaryTypeDef = TypedDict(
     "AssetModelSummaryTypeDef",
     {
         "id": str,
@@ -3554,14 +3993,25 @@
     {
         "gatewaySummaries": List[GatewaySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PropertyTypeOutputTypeDef = TypedDict(
+    "PropertyTypeOutputTypeDef",
+    {
+        "attribute": AttributeOutputTypeDef,
+        "measurement": MeasurementOutputTypeDef,
+        "transform": TransformOutputTypeDef,
+        "metric": MetricOutputTypeDef,
+    },
+    total=False,
+)
+
 PropertyTypeTypeDef = TypedDict(
     "PropertyTypeTypeDef",
     {
         "attribute": AttributeTypeDef,
         "measurement": MeasurementTypeDef,
         "transform": TransformTypeDef,
         "metric": MetricTypeDef,
@@ -3610,42 +4060,43 @@
     {
         "assetSummaries": List[AssociatedAssetsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_RequiredAssetModelPropertyDefinitionTypeDef",
+_RequiredAssetModelPropertyOutputTypeDef = TypedDict(
+    "_RequiredAssetModelPropertyOutputTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeTypeDef,
+        "type": PropertyTypeOutputTypeDef,
     },
 )
-_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_OptionalAssetModelPropertyDefinitionTypeDef",
+_OptionalAssetModelPropertyOutputTypeDef = TypedDict(
+    "_OptionalAssetModelPropertyOutputTypeDef",
     {
+        "id": str,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
-class AssetModelPropertyDefinitionTypeDef(
-    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
+class AssetModelPropertyOutputTypeDef(
+    _RequiredAssetModelPropertyOutputTypeDef, _OptionalAssetModelPropertyOutputTypeDef
 ):
     pass
 
 _RequiredAssetModelPropertySummaryTypeDef = TypedDict(
     "_RequiredAssetModelPropertySummaryTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeTypeDef,
+        "type": PropertyTypeOutputTypeDef,
     },
 )
 _OptionalAssetModelPropertySummaryTypeDef = TypedDict(
     "_OptionalAssetModelPropertySummaryTypeDef",
     {
         "id": str,
         "dataTypeSpec": str,
@@ -3656,14 +4107,58 @@
 )
 
 class AssetModelPropertySummaryTypeDef(
     _RequiredAssetModelPropertySummaryTypeDef, _OptionalAssetModelPropertySummaryTypeDef
 ):
     pass
 
+_RequiredPropertyTypeDef = TypedDict(
+    "_RequiredPropertyTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "dataType": PropertyDataTypeType,
+    },
+)
+_OptionalPropertyTypeDef = TypedDict(
+    "_OptionalPropertyTypeDef",
+    {
+        "alias": str,
+        "notification": PropertyNotificationTypeDef,
+        "unit": str,
+        "type": PropertyTypeOutputTypeDef,
+    },
+    total=False,
+)
+
+class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
+    pass
+
+_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_RequiredAssetModelPropertyDefinitionTypeDef",
+    {
+        "name": str,
+        "dataType": PropertyDataTypeType,
+        "type": PropertyTypeTypeDef,
+    },
+)
+_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_OptionalAssetModelPropertyDefinitionTypeDef",
+    {
+        "dataTypeSpec": str,
+        "unit": str,
+    },
+    total=False,
+)
+
+class AssetModelPropertyDefinitionTypeDef(
+    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
+):
+    pass
+
 _RequiredAssetModelPropertyTypeDef = TypedDict(
     "_RequiredAssetModelPropertyTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
         "type": PropertyTypeTypeDef,
     },
@@ -3679,34 +4174,64 @@
 )
 
 class AssetModelPropertyTypeDef(
     _RequiredAssetModelPropertyTypeDef, _OptionalAssetModelPropertyTypeDef
 ):
     pass
 
-_RequiredPropertyTypeDef = TypedDict(
-    "_RequiredPropertyTypeDef",
+_RequiredAssetModelCompositeModelOutputTypeDef = TypedDict(
+    "_RequiredAssetModelCompositeModelOutputTypeDef",
+    {
+        "name": str,
+        "type": str,
+    },
+)
+_OptionalAssetModelCompositeModelOutputTypeDef = TypedDict(
+    "_OptionalAssetModelCompositeModelOutputTypeDef",
     {
+        "description": str,
+        "properties": List[AssetModelPropertyOutputTypeDef],
         "id": str,
+    },
+    total=False,
+)
+
+class AssetModelCompositeModelOutputTypeDef(
+    _RequiredAssetModelCompositeModelOutputTypeDef, _OptionalAssetModelCompositeModelOutputTypeDef
+):
+    pass
+
+ListAssetModelPropertiesResponseTypeDef = TypedDict(
+    "ListAssetModelPropertiesResponseTypeDef",
+    {
+        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCompositeModelPropertyTypeDef = TypedDict(
+    "_RequiredCompositeModelPropertyTypeDef",
+    {
         "name": str,
-        "dataType": PropertyDataTypeType,
+        "type": str,
+        "assetProperty": PropertyTypeDef,
     },
 )
-_OptionalPropertyTypeDef = TypedDict(
-    "_OptionalPropertyTypeDef",
+_OptionalCompositeModelPropertyTypeDef = TypedDict(
+    "_OptionalCompositeModelPropertyTypeDef",
     {
-        "alias": str,
-        "notification": PropertyNotificationTypeDef,
-        "unit": str,
-        "type": PropertyTypeTypeDef,
+        "id": str,
     },
     total=False,
 )
 
-class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
+class CompositeModelPropertyTypeDef(
+    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
+):
     pass
 
 _RequiredAssetModelCompositeModelDefinitionTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelDefinitionTypeDef",
     {
         "name": str,
         "type": str,
@@ -3723,66 +4248,65 @@
 
 class AssetModelCompositeModelDefinitionTypeDef(
     _RequiredAssetModelCompositeModelDefinitionTypeDef,
     _OptionalAssetModelCompositeModelDefinitionTypeDef,
 ):
     pass
 
-ListAssetModelPropertiesResponseTypeDef = TypedDict(
-    "ListAssetModelPropertiesResponseTypeDef",
-    {
-        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssetModelCompositeModelTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 _OptionalAssetModelCompositeModelTypeDef = TypedDict(
     "_OptionalAssetModelCompositeModelTypeDef",
     {
         "description": str,
-        "properties": List[AssetModelPropertyTypeDef],
+        "properties": Sequence[AssetModelPropertyTypeDef],
         "id": str,
     },
     total=False,
 )
 
 class AssetModelCompositeModelTypeDef(
     _RequiredAssetModelCompositeModelTypeDef, _OptionalAssetModelCompositeModelTypeDef
 ):
     pass
 
-_RequiredCompositeModelPropertyTypeDef = TypedDict(
-    "_RequiredCompositeModelPropertyTypeDef",
+DescribeAssetModelResponseTypeDef = TypedDict(
+    "DescribeAssetModelResponseTypeDef",
     {
-        "name": str,
-        "type": str,
-        "assetProperty": PropertyTypeDef,
+        "assetModelId": str,
+        "assetModelArn": str,
+        "assetModelName": str,
+        "assetModelDescription": str,
+        "assetModelProperties": List[AssetModelPropertyOutputTypeDef],
+        "assetModelHierarchies": List[AssetModelHierarchyOutputTypeDef],
+        "assetModelCompositeModels": List[AssetModelCompositeModelOutputTypeDef],
+        "assetModelCreationDate": datetime,
+        "assetModelLastUpdateDate": datetime,
+        "assetModelStatus": AssetModelStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCompositeModelPropertyTypeDef = TypedDict(
-    "_OptionalCompositeModelPropertyTypeDef",
+
+DescribeAssetPropertyResponseTypeDef = TypedDict(
+    "DescribeAssetPropertyResponseTypeDef",
     {
-        "id": str,
+        "assetId": str,
+        "assetName": str,
+        "assetModelId": str,
+        "assetProperty": PropertyTypeDef,
+        "compositeModel": CompositeModelPropertyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class CompositeModelPropertyTypeDef(
-    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
-):
-    pass
-
 _RequiredCreateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetModelRequestRequestTypeDef",
     {
         "assetModelName": str,
     },
 )
 _OptionalCreateAssetModelRequestRequestTypeDef = TypedDict(
@@ -3799,31 +4323,14 @@
 )
 
 class CreateAssetModelRequestRequestTypeDef(
     _RequiredCreateAssetModelRequestRequestTypeDef, _OptionalCreateAssetModelRequestRequestTypeDef
 ):
     pass
 
-DescribeAssetModelResponseTypeDef = TypedDict(
-    "DescribeAssetModelResponseTypeDef",
-    {
-        "assetModelId": str,
-        "assetModelArn": str,
-        "assetModelName": str,
-        "assetModelDescription": str,
-        "assetModelProperties": List[AssetModelPropertyTypeDef],
-        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": List[AssetModelCompositeModelTypeDef],
-        "assetModelCreationDate": datetime,
-        "assetModelLastUpdateDate": datetime,
-        "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
         "assetModelName": str,
     },
 )
@@ -3839,19 +4346,7 @@
     total=False,
 )
 
 class UpdateAssetModelRequestRequestTypeDef(
     _RequiredUpdateAssetModelRequestRequestTypeDef, _OptionalUpdateAssetModelRequestRequestTypeDef
 ):
     pass
-
-DescribeAssetPropertyResponseTypeDef = TypedDict(
-    "DescribeAssetPropertyResponseTypeDef",
-    {
-        "assetId": str,
-        "assetName": str,
-        "assetModelId": str,
-        "assetProperty": PropertyTypeDef,
-        "compositeModel": CompositeModelPropertyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/waiter.py` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise/waiter.pyi` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTSiteWise 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTSiteWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotsitewise"></a>
 
 # mypy-boto3-iotsitewise
 
 [![PyPI - mypy-boto3-iotsitewise](https://img.shields.io/pypi/v/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsitewise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsitewise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsitewise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsitewise)](https://pepy.tech/project/mypy-boto3-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSiteWise 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[boto3.IoTSiteWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -471,25 +471,30 @@
 
 `mypy_boto3_iotsitewise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsitewise.type_defs import (
     AggregatesTypeDef,
+    AlarmsOutputTypeDef,
     AlarmsTypeDef,
     AssetErrorDetailsTypeDef,
     AssetHierarchyInfoTypeDef,
     AssetHierarchyTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
+    AssetModelHierarchyOutputTypeDef,
     AssetModelHierarchyTypeDef,
     PropertyNotificationTypeDef,
+    TimeInNanosOutputTypeDef,
+    VariantOutputTypeDef,
     TimeInNanosTypeDef,
     VariantTypeDef,
     AssociateAssetsRequestRequestTypeDef,
     AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     BatchAssociateProjectAssetsRequestRequestTypeDef,
     BatchDisassociateProjectAssetsRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorEntryTypeDef,
     BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
@@ -506,15 +511,17 @@
     CreateBulkImportJobResponseTypeDef,
     CreateDashboardRequestRequestTypeDef,
     CreateDashboardResponseTypeDef,
     CreateGatewayResponseTypeDef,
     ImageFileTypeDef,
     CreateProjectRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
+    CsvOutputTypeDef,
     CsvTypeDef,
+    CustomerManagedS3StorageOutputTypeDef,
     CustomerManagedS3StorageTypeDef,
     DashboardSummaryTypeDef,
     DeleteAccessPolicyRequestRequestTypeDef,
     DeleteAssetModelRequestRequestTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDashboardRequestRequestTypeDef,
     DeleteGatewayRequestRequestTypeDef,
@@ -523,46 +530,56 @@
     DeleteTimeSeriesRequestRequestTypeDef,
     DescribeAccessPolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribeBulkImportJobRequestRequestTypeDef,
+    ErrorReportLocationOutputTypeDef,
+    FileOutputTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardResponseTypeDef,
     DescribeGatewayCapabilityConfigurationRequestRequestTypeDef,
     DescribeGatewayCapabilityConfigurationResponseTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     GatewayCapabilitySummaryTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsOutputTypeDef,
     DescribePortalRequestRequestTypeDef,
     ImageLocationTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
-    RetentionPeriodTypeDef,
+    RetentionPeriodOutputTypeDef,
     DescribeTimeSeriesRequestRequestTypeDef,
     DescribeTimeSeriesResponseTypeDef,
     DetailedErrorTypeDef,
     DisassociateAssetsRequestRequestTypeDef,
     DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    VariableValueOutputTypeDef,
     VariableValueTypeDef,
+    ForwardingConfigOutputTypeDef,
     ForwardingConfigTypeDef,
+    GreengrassOutputTypeDef,
+    GreengrassV2OutputTypeDef,
     GreengrassTypeDef,
     GreengrassV2TypeDef,
     GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
     GetAssetPropertyAggregatesRequestRequestTypeDef,
     GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef,
     GetAssetPropertyValueHistoryRequestRequestTypeDef,
     GetAssetPropertyValueRequestRequestTypeDef,
     GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     GetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
+    GroupIdentityOutputTypeDef,
     GroupIdentityTypeDef,
+    IAMRoleIdentityOutputTypeDef,
     IAMRoleIdentityTypeDef,
+    IAMUserIdentityOutputTypeDef,
     IAMUserIdentityTypeDef,
+    UserIdentityOutputTypeDef,
     UserIdentityTypeDef,
     JobSummaryTypeDef,
     ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     ListAssetModelPropertiesRequestRequestTypeDef,
     ListAssetModelsRequestListAssetModelsPaginateTypeDef,
@@ -590,21 +607,27 @@
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimeSeriesRequestListTimeSeriesPaginateTypeDef,
     ListTimeSeriesRequestRequestTypeDef,
     TimeSeriesSummaryTypeDef,
+    LoggingOptionsTypeDef,
+    MetricProcessingConfigOutputTypeDef,
     MetricProcessingConfigTypeDef,
+    TumblingWindowOutputTypeDef,
     TumblingWindowTypeDef,
     MonitorErrorDetailsTypeDef,
     PaginatorConfigTypeDef,
+    PortalResourceOutputTypeDef,
     PortalResourceTypeDef,
+    ProjectResourceOutputTypeDef,
     ProjectResourceTypeDef,
     PutDefaultEncryptionConfigurationRequestRequestTypeDef,
+    RetentionPeriodTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetPropertyRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     UpdateGatewayCapabilityConfigurationRequestRequestTypeDef,
@@ -614,120 +637,137 @@
     AggregatedValueTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     AssetRelationshipSummaryTypeDef,
     AssetPropertySummaryTypeDef,
     AssetPropertyTypeDef,
     BatchPutAssetPropertyErrorTypeDef,
-    AssetPropertyValueTypeDef,
+    AssetPropertyValueOutputTypeDef,
     InterpolatedAssetPropertyValueTypeDef,
+    AssetPropertyValueTypeDef,
     BatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     BatchGetAssetPropertyValueRequestRequestTypeDef,
     BatchGetAssetPropertyValueSkippedEntryTypeDef,
     BatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     BatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     ConfigurationStatusTypeDef,
     CreatePortalRequestRequestTypeDef,
     ImageTypeDef,
+    FileFormatOutputTypeDef,
     FileFormatTypeDef,
+    MultiLayerStorageOutputTypeDef,
     MultiLayerStorageTypeDef,
     ListDashboardsResponseTypeDef,
     DescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     DescribeAssetRequestAssetActiveWaitTypeDef,
     DescribeAssetRequestAssetNotExistsWaitTypeDef,
     DescribePortalRequestPortalActiveWaitTypeDef,
     DescribePortalRequestPortalNotExistsWaitTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    PutLoggingOptionsRequestRequestTypeDef,
     ErrorDetailsTypeDef,
+    ExpressionVariableOutputTypeDef,
     ExpressionVariableTypeDef,
+    MeasurementProcessingConfigOutputTypeDef,
+    TransformProcessingConfigOutputTypeDef,
     MeasurementProcessingConfigTypeDef,
     TransformProcessingConfigTypeDef,
+    GatewayPlatformOutputTypeDef,
     GatewayPlatformTypeDef,
+    IdentityOutputTypeDef,
     IdentityTypeDef,
     ListBulkImportJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTimeSeriesResponseTypeDef,
+    PutLoggingOptionsRequestRequestTypeDef,
+    MetricWindowOutputTypeDef,
     MetricWindowTypeDef,
     PortalStatusTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     BatchGetAssetPropertyAggregatesSuccessEntryTypeDef,
     GetAssetPropertyAggregatesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     AssetCompositeModelTypeDef,
     BatchPutAssetPropertyErrorEntryTypeDef,
     BatchGetAssetPropertyValueHistorySuccessEntryTypeDef,
     BatchGetAssetPropertyValueSuccessEntryTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
-    PutAssetPropertyValueEntryTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
+    PutAssetPropertyValueEntryTypeDef,
     DescribeDefaultEncryptionConfigurationResponseTypeDef,
     PutDefaultEncryptionConfigurationResponseTypeDef,
     UpdatePortalRequestRequestTypeDef,
+    JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     DescribeStorageConfigurationResponseTypeDef,
-    PutStorageConfigurationRequestRequestTypeDef,
     PutStorageConfigurationResponseTypeDef,
+    PutStorageConfigurationRequestRequestTypeDef,
     AssetModelStatusTypeDef,
     AssetStatusTypeDef,
+    MeasurementOutputTypeDef,
+    TransformOutputTypeDef,
     MeasurementTypeDef,
     TransformTypeDef,
-    CreateGatewayRequestRequestTypeDef,
     DescribeGatewayResponseTypeDef,
     GatewaySummaryTypeDef,
+    CreateGatewayRequestRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     CreatePortalResponseTypeDef,
     DeletePortalResponseTypeDef,
     DescribePortalResponseTypeDef,
     PortalSummaryTypeDef,
     UpdatePortalResponseTypeDef,
     AccessPolicySummaryTypeDef,
-    CreateAccessPolicyRequestRequestTypeDef,
     DescribeAccessPolicyResponseTypeDef,
+    CreateAccessPolicyRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchPutAssetPropertyValueResponseTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
     BatchGetAssetPropertyValueResponseTypeDef,
     BatchPutAssetPropertyValueRequestRequestTypeDef,
-    CreateBulkImportJobRequestRequestTypeDef,
     DescribeBulkImportJobResponseTypeDef,
+    CreateBulkImportJobRequestRequestTypeDef,
     AssetModelSummaryTypeDef,
     CreateAssetModelResponseTypeDef,
     DeleteAssetModelResponseTypeDef,
     UpdateAssetModelResponseTypeDef,
     AssetSummaryTypeDef,
     AssociatedAssetsSummaryTypeDef,
     CreateAssetResponseTypeDef,
     DeleteAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
     UpdateAssetResponseTypeDef,
     ListGatewaysResponseTypeDef,
+    PropertyTypeOutputTypeDef,
     PropertyTypeTypeDef,
     ListPortalsResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetsResponseTypeDef,
     ListAssociatedAssetsResponseTypeDef,
-    AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyOutputTypeDef,
     AssetModelPropertySummaryTypeDef,
-    AssetModelPropertyTypeDef,
     PropertyTypeDef,
-    AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyTypeDef,
+    AssetModelCompositeModelOutputTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
-    AssetModelCompositeModelTypeDef,
     CompositeModelPropertyTypeDef,
-    CreateAssetModelRequestRequestTypeDef,
+    AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelCompositeModelTypeDef,
     DescribeAssetModelResponseTypeDef,
-    UpdateAssetModelRequestRequestTypeDef,
     DescribeAssetPropertyResponseTypeDef,
+    CreateAssetModelRequestRequestTypeDef,
+    UpdateAssetModelRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AggregatesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotsitewise-1.28.0/mypy_boto3_iotsitewise.egg-info/SOURCES.txt` & `mypy-boto3-iotsitewise-1.28.12/mypy_boto3_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.0/setup.py` & `mypy-boto3-iotsitewise-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsitewise",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSiteWise 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTSiteWise 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

