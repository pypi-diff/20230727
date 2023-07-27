# Comparing `tmp/mypy-boto3-kinesisanalyticsv2-1.28.0.tar.gz` & `tmp/mypy-boto3-kinesisanalyticsv2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.0.tar", last modified: Thu Jul  6 20:59:55 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.12.tar", last modified: Thu Jul 27 05:34:54 2023, max compression
```

## Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0.tar` & `mypy-boto3-kinesisanalyticsv2-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.562346 mypy-boto3-kinesisanalyticsv2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21247 2023-07-06 20:59:55.558346 mypy-boto3-kinesisanalyticsv2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.550346 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-06 20:44:53.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27513 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-06 20:44:53.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-06 20:44:53.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-06 20:44:53.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-06 20:44:53.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69096 2023-07-06 20:44:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68995 2023-07-06 20:44:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.558346 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21247 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:55.562346 mypy-boto3-kinesisanalyticsv2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-06 20:44:52.000000 mypy-boto3-kinesisanalyticsv2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.240465 mypy-boto3-kinesisanalyticsv2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-07-27 05:34:54.228466 mypy-boto3-kinesisanalyticsv2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.228466 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27513 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-27 05:24:45.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74032 2023-07-27 05:24:47.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73919 2023-07-27 05:24:47.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.228466 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:54.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:54.240465 mypy-boto3-kinesisanalyticsv2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalyticsv2-1.28.12/setup.py
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/LICENSE` & `mypy-boto3-kinesisanalyticsv2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.0
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kinesisanalyticsv2"></a>
 
 # mypy-boto3-kinesisanalyticsv2
 
 [![PyPI - mypy-boto3-kinesisanalyticsv2](https://img.shields.io/pypi/v/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisanalyticsv2?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisanalyticsv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,17 +350,19 @@
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
+    ApplicationRestoreConfigurationOutputTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
@@ -368,14 +370,16 @@
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
     CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
+    MavenReferenceOutputTypeDef,
+    S3ContentLocationOutputTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
@@ -387,37 +391,43 @@
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
+    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
+    PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
+    FlinkRunConfigurationOutputTypeDef,
     FlinkRunConfigurationTypeDef,
-    InputParallelismTypeDef,
+    InputParallelismOutputTypeDef,
+    InputStartingPositionConfigurationOutputTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
     InputLambdaProcessorDescriptionTypeDef,
     InputLambdaProcessorTypeDef,
     InputLambdaProcessorUpdateTypeDef,
+    InputParallelismTypeDef,
     InputParallelismUpdateTypeDef,
     RecordColumnTypeDef,
     KinesisFirehoseInputTypeDef,
     KinesisStreamsInputTypeDef,
     KinesisFirehoseInputUpdateTypeDef,
     KinesisStreamsInputUpdateTypeDef,
+    JSONMappingParametersOutputTypeDef,
     JSONMappingParametersTypeDef,
     KinesisFirehoseOutputDescriptionTypeDef,
     KinesisFirehoseOutputTypeDef,
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
@@ -426,15 +436,17 @@
     LambdaOutputUpdateTypeDef,
     ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
     ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -452,66 +464,69 @@
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
     CatalogConfigurationTypeDef,
     CatalogConfigurationUpdateTypeDef,
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
-    EnvironmentPropertyDescriptionsTypeDef,
     EnvironmentPropertyUpdatesTypeDef,
+    EnvironmentPropertyDescriptionsTypeDef,
     FlinkApplicationConfigurationDescriptionTypeDef,
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
+    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
     AddApplicationInputProcessingConfigurationResponseTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
+    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
+    SourceSchemaOutputTypeDef,
     InputSchemaUpdateTypeDef,
     SourceSchemaTypeDef,
-    InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputUpdateTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
+    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     SqlApplicationConfigurationTypeDef,
     SqlApplicationConfigurationUpdateTypeDef,
     ApplicationConfigurationDescriptionTypeDef,
     ApplicationConfigurationTypeDef,
     ApplicationConfigurationUpdateTypeDef,
     ApplicationDetailTypeDef,
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/README.md` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-kinesisanalyticsv2
+Version: 1.28.12
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-kinesisanalyticsv2"></a>
 
 # mypy-boto3-kinesisanalyticsv2
 
 [![PyPI - mypy-boto3-kinesisanalyticsv2](https://img.shields.io/pypi/v/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisanalyticsv2?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisanalyticsv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,17 +350,19 @@
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
+    ApplicationRestoreConfigurationOutputTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
@@ -336,14 +370,16 @@
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
     CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
+    MavenReferenceOutputTypeDef,
+    S3ContentLocationOutputTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
@@ -355,37 +391,43 @@
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
+    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
+    PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
+    FlinkRunConfigurationOutputTypeDef,
     FlinkRunConfigurationTypeDef,
-    InputParallelismTypeDef,
+    InputParallelismOutputTypeDef,
+    InputStartingPositionConfigurationOutputTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
     InputLambdaProcessorDescriptionTypeDef,
     InputLambdaProcessorTypeDef,
     InputLambdaProcessorUpdateTypeDef,
+    InputParallelismTypeDef,
     InputParallelismUpdateTypeDef,
     RecordColumnTypeDef,
     KinesisFirehoseInputTypeDef,
     KinesisStreamsInputTypeDef,
     KinesisFirehoseInputUpdateTypeDef,
     KinesisStreamsInputUpdateTypeDef,
+    JSONMappingParametersOutputTypeDef,
     JSONMappingParametersTypeDef,
     KinesisFirehoseOutputDescriptionTypeDef,
     KinesisFirehoseOutputTypeDef,
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
@@ -394,15 +436,17 @@
     LambdaOutputUpdateTypeDef,
     ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
     ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -420,66 +464,69 @@
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
     CatalogConfigurationTypeDef,
     CatalogConfigurationUpdateTypeDef,
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
-    EnvironmentPropertyDescriptionsTypeDef,
     EnvironmentPropertyUpdatesTypeDef,
+    EnvironmentPropertyDescriptionsTypeDef,
     FlinkApplicationConfigurationDescriptionTypeDef,
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
+    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
     AddApplicationInputProcessingConfigurationResponseTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
+    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
+    SourceSchemaOutputTypeDef,
     InputSchemaUpdateTypeDef,
     SourceSchemaTypeDef,
-    InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputUpdateTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
+    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     SqlApplicationConfigurationTypeDef,
     SqlApplicationConfigurationUpdateTypeDef,
     ApplicationConfigurationDescriptionTypeDef,
     ApplicationConfigurationTypeDef,
     ApplicationConfigurationUpdateTypeDef,
     ApplicationDetailTypeDef,
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/__init__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/__init__.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/__main__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisAnalyticsV2 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.KinesisAnalyticsV2 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/client.py` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/client.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/literals.py` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,15 @@
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
@@ -284,26 +285,28 @@
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

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/literals.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
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
@@ -282,26 +283,28 @@
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

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/paginator.py` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/paginator.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/type_defs.py` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,30 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationTypeDef",
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
+    "ApplicationRestoreConfigurationOutputTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
+    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
@@ -64,14 +65,16 @@
     "S3ApplicationCodeLocationDescriptionTypeDef",
     "S3ContentLocationTypeDef",
     "S3ContentLocationUpdateTypeDef",
     "CreateApplicationPresignedUrlRequestRequestTypeDef",
     "CreateApplicationPresignedUrlResponseTypeDef",
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
+    "MavenReferenceOutputTypeDef",
+    "S3ContentLocationOutputTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationOutputResponseTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
@@ -83,37 +86,43 @@
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
+    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
+    "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
+    "FlinkRunConfigurationOutputTypeDef",
     "FlinkRunConfigurationTypeDef",
-    "InputParallelismTypeDef",
+    "InputParallelismOutputTypeDef",
+    "InputStartingPositionConfigurationOutputTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
     "InputLambdaProcessorDescriptionTypeDef",
     "InputLambdaProcessorTypeDef",
     "InputLambdaProcessorUpdateTypeDef",
+    "InputParallelismTypeDef",
     "InputParallelismUpdateTypeDef",
     "RecordColumnTypeDef",
     "KinesisFirehoseInputTypeDef",
     "KinesisStreamsInputTypeDef",
     "KinesisFirehoseInputUpdateTypeDef",
     "KinesisStreamsInputUpdateTypeDef",
+    "JSONMappingParametersOutputTypeDef",
     "JSONMappingParametersTypeDef",
     "KinesisFirehoseOutputDescriptionTypeDef",
     "KinesisFirehoseOutputTypeDef",
     "KinesisFirehoseOutputUpdateTypeDef",
     "KinesisStreamsOutputDescriptionTypeDef",
     "KinesisStreamsOutputTypeDef",
     "KinesisStreamsOutputUpdateTypeDef",
@@ -122,15 +131,17 @@
     "LambdaOutputUpdateTypeDef",
     "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
     "ListApplicationSnapshotsRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
     "ResponseMetadataTypeDef",
     "RollbackApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -148,66 +159,69 @@
     "ListApplicationVersionsResponseTypeDef",
     "CatalogConfigurationDescriptionTypeDef",
     "CatalogConfigurationTypeDef",
     "CatalogConfigurationUpdateTypeDef",
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
-    "EnvironmentPropertyDescriptionsTypeDef",
     "EnvironmentPropertyUpdatesTypeDef",
+    "EnvironmentPropertyDescriptionsTypeDef",
     "FlinkApplicationConfigurationDescriptionTypeDef",
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
+    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ApplicationCodeConfigurationDescriptionTypeDef",
     "ApplicationCodeConfigurationTypeDef",
     "ApplicationCodeConfigurationUpdateTypeDef",
     "ZeppelinApplicationConfigurationDescriptionTypeDef",
     "ZeppelinApplicationConfigurationTypeDef",
     "ZeppelinApplicationConfigurationUpdateTypeDef",
     "RunConfigurationTypeDef",
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
+    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "SourceSchemaOutputTypeDef",
     "InputSchemaUpdateTypeDef",
     "SourceSchemaTypeDef",
-    "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "InputTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
+    "InputUpdateTypeDef",
+    "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
-    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
+    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "SqlApplicationConfigurationTypeDef",
     "SqlApplicationConfigurationUpdateTypeDef",
     "ApplicationConfigurationDescriptionTypeDef",
     "ApplicationConfigurationTypeDef",
     "ApplicationConfigurationUpdateTypeDef",
     "ApplicationDetailTypeDef",
@@ -238,22 +252,20 @@
     {
         "CloudWatchLoggingOptionId": str,
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
-
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
@@ -300,21 +312,19 @@
     {
         "SubnetIdUpdates": Sequence[str],
         "SecurityGroupIdUpdates": Sequence[str],
     },
     total=False,
 )
 
-
 class VpcConfigurationUpdateTypeDef(
     _RequiredVpcConfigurationUpdateTypeDef, _OptionalVpcConfigurationUpdateTypeDef
 ):
     pass
 
-
 ApplicationMaintenanceConfigurationDescriptionTypeDef = TypedDict(
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     {
         "ApplicationMaintenanceWindowStartTime": str,
         "ApplicationMaintenanceWindowEndTime": str,
     },
 )
@@ -322,35 +332,53 @@
 ApplicationMaintenanceConfigurationUpdateTypeDef = TypedDict(
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     {
         "ApplicationMaintenanceWindowStartTimeUpdate": str,
     },
 )
 
+_RequiredApplicationRestoreConfigurationOutputTypeDef = TypedDict(
+    "_RequiredApplicationRestoreConfigurationOutputTypeDef",
+    {
+        "ApplicationRestoreType": ApplicationRestoreTypeType,
+    },
+)
+_OptionalApplicationRestoreConfigurationOutputTypeDef = TypedDict(
+    "_OptionalApplicationRestoreConfigurationOutputTypeDef",
+    {
+        "SnapshotName": str,
+    },
+    total=False,
+)
+
+class ApplicationRestoreConfigurationOutputTypeDef(
+    _RequiredApplicationRestoreConfigurationOutputTypeDef,
+    _OptionalApplicationRestoreConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredApplicationRestoreConfigurationTypeDef = TypedDict(
     "_RequiredApplicationRestoreConfigurationTypeDef",
     {
         "ApplicationRestoreType": ApplicationRestoreTypeType,
     },
 )
 _OptionalApplicationRestoreConfigurationTypeDef = TypedDict(
     "_OptionalApplicationRestoreConfigurationTypeDef",
     {
         "SnapshotName": str,
     },
     total=False,
 )
 
-
 class ApplicationRestoreConfigurationTypeDef(
     _RequiredApplicationRestoreConfigurationTypeDef, _OptionalApplicationRestoreConfigurationTypeDef
 ):
     pass
 
-
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
         "ApplicationVersionId": int,
@@ -361,29 +389,35 @@
     "_OptionalApplicationSummaryTypeDef",
     {
         "ApplicationMode": ApplicationModeType,
     },
     total=False,
 )
 
-
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
-
 ApplicationVersionSummaryTypeDef = TypedDict(
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
+CSVMappingParametersOutputTypeDef = TypedDict(
+    "CSVMappingParametersOutputTypeDef",
+    {
+        "RecordRowDelimiter": str,
+        "RecordColumnDelimiter": str,
+    },
+)
+
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -432,21 +466,19 @@
         "CheckpointingEnabled": bool,
         "CheckpointInterval": int,
         "MinPauseBetweenCheckpoints": int,
     },
     total=False,
 )
 
-
 class CheckpointConfigurationTypeDef(
     _RequiredCheckpointConfigurationTypeDef, _OptionalCheckpointConfigurationTypeDef
 ):
     pass
 
-
 CheckpointConfigurationUpdateTypeDef = TypedDict(
     "CheckpointConfigurationUpdateTypeDef",
     {
         "ConfigurationTypeUpdate": ConfigurationTypeType,
         "CheckpointingEnabledUpdate": bool,
         "CheckpointIntervalUpdate": int,
         "MinPauseBetweenCheckpointsUpdate": int,
@@ -464,21 +496,19 @@
     "_OptionalCloudWatchLoggingOptionUpdateTypeDef",
     {
         "LogStreamARNUpdate": str,
     },
     total=False,
 )
 
-
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
-
 _RequiredS3ApplicationCodeLocationDescriptionTypeDef = TypedDict(
     "_RequiredS3ApplicationCodeLocationDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -486,22 +516,20 @@
     "_OptionalS3ApplicationCodeLocationDescriptionTypeDef",
     {
         "ObjectVersion": str,
     },
     total=False,
 )
 
-
 class S3ApplicationCodeLocationDescriptionTypeDef(
     _RequiredS3ApplicationCodeLocationDescriptionTypeDef,
     _OptionalS3ApplicationCodeLocationDescriptionTypeDef,
 ):
     pass
 
-
 _RequiredS3ContentLocationTypeDef = TypedDict(
     "_RequiredS3ContentLocationTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -509,21 +537,19 @@
     "_OptionalS3ContentLocationTypeDef",
     {
         "ObjectVersion": str,
     },
     total=False,
 )
 
-
 class S3ContentLocationTypeDef(
     _RequiredS3ContentLocationTypeDef, _OptionalS3ContentLocationTypeDef
 ):
     pass
 
-
 S3ContentLocationUpdateTypeDef = TypedDict(
     "S3ContentLocationUpdateTypeDef",
     {
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
         "ObjectVersionUpdate": str,
     },
@@ -541,22 +567,20 @@
     "_OptionalCreateApplicationPresignedUrlRequestRequestTypeDef",
     {
         "SessionExpirationDurationInSeconds": int,
     },
     total=False,
 )
 
-
 class CreateApplicationPresignedUrlRequestRequestTypeDef(
     _RequiredCreateApplicationPresignedUrlRequestRequestTypeDef,
     _OptionalCreateApplicationPresignedUrlRequestRequestTypeDef,
 ):
     pass
 
-
 CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
     "CreateApplicationPresignedUrlResponseTypeDef",
     {
         "AuthorizedUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -571,27 +595,54 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 CreateApplicationSnapshotRequestRequestTypeDef = TypedDict(
     "CreateApplicationSnapshotRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "SnapshotName": str,
     },
 )
 
+MavenReferenceOutputTypeDef = TypedDict(
+    "MavenReferenceOutputTypeDef",
+    {
+        "GroupId": str,
+        "ArtifactId": str,
+        "Version": str,
+    },
+)
+
+_RequiredS3ContentLocationOutputTypeDef = TypedDict(
+    "_RequiredS3ContentLocationOutputTypeDef",
+    {
+        "BucketARN": str,
+        "FileKey": str,
+    },
+)
+_OptionalS3ContentLocationOutputTypeDef = TypedDict(
+    "_OptionalS3ContentLocationOutputTypeDef",
+    {
+        "ObjectVersion": str,
+    },
+    total=False,
+)
+
+class S3ContentLocationOutputTypeDef(
+    _RequiredS3ContentLocationOutputTypeDef, _OptionalS3ContentLocationOutputTypeDef
+):
+    pass
+
 MavenReferenceTypeDef = TypedDict(
     "MavenReferenceTypeDef",
     {
         "GroupId": str,
         "ArtifactId": str,
         "Version": str,
     },
@@ -609,22 +660,20 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
-
 class DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef(
     _RequiredDeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     _OptionalDeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "InputId": str,
     },
@@ -704,22 +753,20 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
-
 class DeleteApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalDeleteApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "DeleteApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -735,43 +782,39 @@
     "_OptionalS3ContentBaseLocationDescriptionTypeDef",
     {
         "BasePath": str,
     },
     total=False,
 )
 
-
 class S3ContentBaseLocationDescriptionTypeDef(
     _RequiredS3ContentBaseLocationDescriptionTypeDef,
     _OptionalS3ContentBaseLocationDescriptionTypeDef,
 ):
     pass
 
-
 _RequiredS3ContentBaseLocationTypeDef = TypedDict(
     "_RequiredS3ContentBaseLocationTypeDef",
     {
         "BucketARN": str,
     },
 )
 _OptionalS3ContentBaseLocationTypeDef = TypedDict(
     "_OptionalS3ContentBaseLocationTypeDef",
     {
         "BasePath": str,
     },
     total=False,
 )
 
-
 class S3ContentBaseLocationTypeDef(
     _RequiredS3ContentBaseLocationTypeDef, _OptionalS3ContentBaseLocationTypeDef
 ):
     pass
 
-
 S3ContentBaseLocationUpdateTypeDef = TypedDict(
     "S3ContentBaseLocationUpdateTypeDef",
     {
         "BucketARNUpdate": str,
         "BasePathUpdate": str,
     },
     total=False,
@@ -787,22 +830,20 @@
     "_OptionalDescribeApplicationRequestRequestTypeDef",
     {
         "IncludeAdditionalDetails": bool,
     },
     total=False,
 )
 
-
 class DescribeApplicationRequestRequestTypeDef(
     _RequiredDescribeApplicationRequestRequestTypeDef,
     _OptionalDescribeApplicationRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeApplicationSnapshotRequestRequestTypeDef = TypedDict(
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "SnapshotName": str,
     },
 )
@@ -819,27 +860,32 @@
     "_OptionalSnapshotDetailsTypeDef",
     {
         "SnapshotCreationTimestamp": datetime,
     },
     total=False,
 )
 
-
 class SnapshotDetailsTypeDef(_RequiredSnapshotDetailsTypeDef, _OptionalSnapshotDetailsTypeDef):
     pass
 
-
 DescribeApplicationVersionRequestRequestTypeDef = TypedDict(
     "DescribeApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "ApplicationVersionId": int,
     },
 )
 
+DestinationSchemaOutputTypeDef = TypedDict(
+    "DestinationSchemaOutputTypeDef",
+    {
+        "RecordFormatType": RecordFormatTypeType,
+    },
+)
+
 DestinationSchemaTypeDef = TypedDict(
     "DestinationSchemaTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 
@@ -863,14 +909,22 @@
     "PropertyGroupTypeDef",
     {
         "PropertyGroupId": str,
         "PropertyMap": Mapping[str, str],
     },
 )
 
+PropertyGroupOutputTypeDef = TypedDict(
+    "PropertyGroupOutputTypeDef",
+    {
+        "PropertyGroupId": str,
+        "PropertyMap": Dict[str, str],
+    },
+)
+
 MonitoringConfigurationDescriptionTypeDef = TypedDict(
     "MonitoringConfigurationDescriptionTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
@@ -900,21 +954,19 @@
     {
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
     total=False,
 )
 
-
 class MonitoringConfigurationTypeDef(
     _RequiredMonitoringConfigurationTypeDef, _OptionalMonitoringConfigurationTypeDef
 ):
     pass
 
-
 _RequiredParallelismConfigurationTypeDef = TypedDict(
     "_RequiredParallelismConfigurationTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
     },
 )
 _OptionalParallelismConfigurationTypeDef = TypedDict(
@@ -923,21 +975,19 @@
         "Parallelism": int,
         "ParallelismPerKPU": int,
         "AutoScalingEnabled": bool,
     },
     total=False,
 )
 
-
 class ParallelismConfigurationTypeDef(
     _RequiredParallelismConfigurationTypeDef, _OptionalParallelismConfigurationTypeDef
 ):
     pass
 
-
 MonitoringConfigurationUpdateTypeDef = TypedDict(
     "MonitoringConfigurationUpdateTypeDef",
     {
         "ConfigurationTypeUpdate": ConfigurationTypeType,
         "MetricsLevelUpdate": MetricsLevelType,
         "LogLevelUpdate": LogLevelType,
     },
@@ -951,107 +1001,125 @@
         "ParallelismUpdate": int,
         "ParallelismPerKPUUpdate": int,
         "AutoScalingEnabledUpdate": bool,
     },
     total=False,
 )
 
+FlinkRunConfigurationOutputTypeDef = TypedDict(
+    "FlinkRunConfigurationOutputTypeDef",
+    {
+        "AllowNonRestoredState": bool,
+    },
+    total=False,
+)
+
 FlinkRunConfigurationTypeDef = TypedDict(
     "FlinkRunConfigurationTypeDef",
     {
         "AllowNonRestoredState": bool,
     },
     total=False,
 )
 
-InputParallelismTypeDef = TypedDict(
-    "InputParallelismTypeDef",
+InputParallelismOutputTypeDef = TypedDict(
+    "InputParallelismOutputTypeDef",
     {
         "Count": int,
     },
     total=False,
 )
 
+InputStartingPositionConfigurationOutputTypeDef = TypedDict(
+    "InputStartingPositionConfigurationOutputTypeDef",
+    {
+        "InputStartingPosition": InputStartingPositionType,
+    },
+    total=False,
+)
+
 _RequiredKinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "_RequiredKinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalKinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "_OptionalKinesisFirehoseInputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class KinesisFirehoseInputDescriptionTypeDef(
     _RequiredKinesisFirehoseInputDescriptionTypeDef, _OptionalKinesisFirehoseInputDescriptionTypeDef
 ):
     pass
 
-
 _RequiredKinesisStreamsInputDescriptionTypeDef = TypedDict(
     "_RequiredKinesisStreamsInputDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalKinesisStreamsInputDescriptionTypeDef = TypedDict(
     "_OptionalKinesisStreamsInputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class KinesisStreamsInputDescriptionTypeDef(
     _RequiredKinesisStreamsInputDescriptionTypeDef, _OptionalKinesisStreamsInputDescriptionTypeDef
 ):
     pass
 
-
 _RequiredInputLambdaProcessorDescriptionTypeDef = TypedDict(
     "_RequiredInputLambdaProcessorDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalInputLambdaProcessorDescriptionTypeDef = TypedDict(
     "_OptionalInputLambdaProcessorDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class InputLambdaProcessorDescriptionTypeDef(
     _RequiredInputLambdaProcessorDescriptionTypeDef, _OptionalInputLambdaProcessorDescriptionTypeDef
 ):
     pass
 
-
 InputLambdaProcessorTypeDef = TypedDict(
     "InputLambdaProcessorTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
 InputLambdaProcessorUpdateTypeDef = TypedDict(
     "InputLambdaProcessorUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
+InputParallelismTypeDef = TypedDict(
+    "InputParallelismTypeDef",
+    {
+        "Count": int,
+    },
+    total=False,
+)
+
 InputParallelismUpdateTypeDef = TypedDict(
     "InputParallelismUpdateTypeDef",
     {
         "CountUpdate": int,
     },
 )
 
@@ -1066,19 +1134,17 @@
     "_OptionalRecordColumnTypeDef",
     {
         "Mapping": str,
     },
     total=False,
 )
 
-
 class RecordColumnTypeDef(_RequiredRecordColumnTypeDef, _OptionalRecordColumnTypeDef):
     pass
 
-
 KinesisFirehoseInputTypeDef = TypedDict(
     "KinesisFirehoseInputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1099,14 +1165,21 @@
 KinesisStreamsInputUpdateTypeDef = TypedDict(
     "KinesisStreamsInputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
+JSONMappingParametersOutputTypeDef = TypedDict(
+    "JSONMappingParametersOutputTypeDef",
+    {
+        "RecordRowPath": str,
+    },
+)
+
 JSONMappingParametersTypeDef = TypedDict(
     "JSONMappingParametersTypeDef",
     {
         "RecordRowPath": str,
     },
 )
 
@@ -1120,22 +1193,20 @@
     "_OptionalKinesisFirehoseOutputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class KinesisFirehoseOutputDescriptionTypeDef(
     _RequiredKinesisFirehoseOutputDescriptionTypeDef,
     _OptionalKinesisFirehoseOutputDescriptionTypeDef,
 ):
     pass
 
-
 KinesisFirehoseOutputTypeDef = TypedDict(
     "KinesisFirehoseOutputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1156,21 +1227,19 @@
     "_OptionalKinesisStreamsOutputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class KinesisStreamsOutputDescriptionTypeDef(
     _RequiredKinesisStreamsOutputDescriptionTypeDef, _OptionalKinesisStreamsOutputDescriptionTypeDef
 ):
     pass
 
-
 KinesisStreamsOutputTypeDef = TypedDict(
     "KinesisStreamsOutputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1191,21 +1260,19 @@
     "_OptionalLambdaOutputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
-
 class LambdaOutputDescriptionTypeDef(
     _RequiredLambdaOutputDescriptionTypeDef, _OptionalLambdaOutputDescriptionTypeDef
 ):
     pass
 
-
 LambdaOutputTypeDef = TypedDict(
     "LambdaOutputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1226,22 +1293,20 @@
     "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
     _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
     _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationSnapshotsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
@@ -1249,22 +1314,20 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationSnapshotsRequestRequestTypeDef(
     _RequiredListApplicationSnapshotsRequestRequestTypeDef,
     _OptionalListApplicationSnapshotsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -1272,22 +1335,20 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -1304,24 +1365,61 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
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
 
+_RequiredRecordColumnOutputTypeDef = TypedDict(
+    "_RequiredRecordColumnOutputTypeDef",
+    {
+        "Name": str,
+        "SqlType": str,
+    },
+)
+_OptionalRecordColumnOutputTypeDef = TypedDict(
+    "_OptionalRecordColumnOutputTypeDef",
+    {
+        "Mapping": str,
+    },
+    total=False,
+)
+
+class RecordColumnOutputTypeDef(
+    _RequiredRecordColumnOutputTypeDef, _OptionalRecordColumnOutputTypeDef
+):
+    pass
+
 _RequiredS3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredS3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -1329,22 +1427,20 @@
     "_OptionalS3ReferenceDataSourceDescriptionTypeDef",
     {
         "ReferenceRoleARN": str,
     },
     total=False,
 )
 
-
 class S3ReferenceDataSourceDescriptionTypeDef(
     _RequiredS3ReferenceDataSourceDescriptionTypeDef,
     _OptionalS3ReferenceDataSourceDescriptionTypeDef,
 ):
     pass
 
-
 S3ReferenceDataSourceTypeDef = TypedDict(
     "S3ReferenceDataSourceTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
     total=False,
@@ -1388,21 +1484,19 @@
     "_OptionalStopApplicationRequestRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
-
 class StopApplicationRequestRequestTypeDef(
     _RequiredStopApplicationRequestRequestTypeDef, _OptionalStopApplicationRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1441,22 +1535,20 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
-
 class AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef(
     _RequiredAddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     _OptionalAddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
 ):
     pass
 
-
 AddApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1485,22 +1577,20 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
-
 class AddApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredAddApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalAddApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 AddApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "AddApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1594,36 +1684,28 @@
         "TextContentUpdate": str,
         "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
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
 
 CustomArtifactConfigurationDescriptionTypeDef = TypedDict(
     "CustomArtifactConfigurationDescriptionTypeDef",
     {
         "ArtifactType": ArtifactTypeType,
-        "S3ContentLocationDescription": S3ContentLocationTypeDef,
-        "MavenReferenceDescription": MavenReferenceTypeDef,
+        "S3ContentLocationDescription": S3ContentLocationOutputTypeDef,
+        "MavenReferenceDescription": MavenReferenceOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCustomArtifactConfigurationTypeDef = TypedDict(
     "_RequiredCustomArtifactConfigurationTypeDef",
     {
@@ -1635,21 +1717,19 @@
     {
         "S3ContentLocation": S3ContentLocationTypeDef,
         "MavenReference": MavenReferenceTypeDef,
     },
     total=False,
 )
 
-
 class CustomArtifactConfigurationTypeDef(
     _RequiredCustomArtifactConfigurationTypeDef, _OptionalCustomArtifactConfigurationTypeDef
 ):
     pass
 
-
 DeployAsApplicationConfigurationDescriptionTypeDef = TypedDict(
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     {
         "S3ContentLocationDescription": S3ContentBaseLocationDescriptionTypeDef,
     },
 )
 
@@ -1696,27 +1776,27 @@
 EnvironmentPropertiesTypeDef = TypedDict(
     "EnvironmentPropertiesTypeDef",
     {
         "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
 )
 
-EnvironmentPropertyDescriptionsTypeDef = TypedDict(
-    "EnvironmentPropertyDescriptionsTypeDef",
+EnvironmentPropertyUpdatesTypeDef = TypedDict(
+    "EnvironmentPropertyUpdatesTypeDef",
     {
-        "PropertyGroupDescriptions": List[PropertyGroupTypeDef],
+        "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
-    total=False,
 )
 
-EnvironmentPropertyUpdatesTypeDef = TypedDict(
-    "EnvironmentPropertyUpdatesTypeDef",
+EnvironmentPropertyDescriptionsTypeDef = TypedDict(
+    "EnvironmentPropertyDescriptionsTypeDef",
     {
-        "PropertyGroups": Sequence[PropertyGroupTypeDef],
+        "PropertyGroupDescriptions": List[PropertyGroupOutputTypeDef],
     },
+    total=False,
 )
 
 FlinkApplicationConfigurationDescriptionTypeDef = TypedDict(
     "FlinkApplicationConfigurationDescriptionTypeDef",
     {
         "CheckpointConfigurationDescription": CheckpointConfigurationDescriptionTypeDef,
         "MonitoringConfigurationDescription": MonitoringConfigurationDescriptionTypeDef,
@@ -1745,16 +1825,16 @@
     },
     total=False,
 )
 
 RunConfigurationDescriptionTypeDef = TypedDict(
     "RunConfigurationDescriptionTypeDef",
     {
-        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationTypeDef,
-        "FlinkRunConfigurationDescription": FlinkRunConfigurationTypeDef,
+        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationOutputTypeDef,
+        "FlinkRunConfigurationDescription": FlinkRunConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 RunConfigurationUpdateTypeDef = TypedDict(
     "RunConfigurationUpdateTypeDef",
     {
@@ -1782,14 +1862,23 @@
 InputProcessingConfigurationUpdateTypeDef = TypedDict(
     "InputProcessingConfigurationUpdateTypeDef",
     {
         "InputLambdaProcessorUpdate": InputLambdaProcessorUpdateTypeDef,
     },
 )
 
+MappingParametersOutputTypeDef = TypedDict(
+    "MappingParametersOutputTypeDef",
+    {
+        "JSONMappingParameters": JSONMappingParametersOutputTypeDef,
+        "CSVMappingParameters": CSVMappingParametersOutputTypeDef,
+    },
+    total=False,
+)
+
 MappingParametersTypeDef = TypedDict(
     "MappingParametersTypeDef",
     {
         "JSONMappingParameters": JSONMappingParametersTypeDef,
         "CSVMappingParameters": CSVMappingParametersTypeDef,
     },
     total=False,
@@ -1799,15 +1888,15 @@
     "OutputDescriptionTypeDef",
     {
         "OutputId": str,
         "Name": str,
         "KinesisStreamsOutputDescription": KinesisStreamsOutputDescriptionTypeDef,
         "KinesisFirehoseOutputDescription": KinesisFirehoseOutputDescriptionTypeDef,
         "LambdaOutputDescription": LambdaOutputDescriptionTypeDef,
-        "DestinationSchema": DestinationSchemaTypeDef,
+        "DestinationSchema": DestinationSchemaOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
@@ -1821,19 +1910,17 @@
         "KinesisStreamsOutput": KinesisStreamsOutputTypeDef,
         "KinesisFirehoseOutput": KinesisFirehoseOutputTypeDef,
         "LambdaOutput": LambdaOutputTypeDef,
     },
     total=False,
 )
 
-
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-
 _RequiredOutputUpdateTypeDef = TypedDict(
     "_RequiredOutputUpdateTypeDef",
     {
         "OutputId": str,
     },
 )
 _OptionalOutputUpdateTypeDef = TypedDict(
@@ -1844,18 +1931,24 @@
         "KinesisFirehoseOutputUpdate": KinesisFirehoseOutputUpdateTypeDef,
         "LambdaOutputUpdate": LambdaOutputUpdateTypeDef,
         "DestinationSchemaUpdate": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
-
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
 )
@@ -1863,43 +1956,39 @@
     "_OptionalApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentDescription": CodeContentDescriptionTypeDef,
     },
     total=False,
 )
 
-
 class ApplicationCodeConfigurationDescriptionTypeDef(
     _RequiredApplicationCodeConfigurationDescriptionTypeDef,
     _OptionalApplicationCodeConfigurationDescriptionTypeDef,
 ):
     pass
 
-
 _RequiredApplicationCodeConfigurationTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
 )
 _OptionalApplicationCodeConfigurationTypeDef = TypedDict(
     "_OptionalApplicationCodeConfigurationTypeDef",
     {
         "CodeContent": CodeContentTypeDef,
     },
     total=False,
 )
 
-
 class ApplicationCodeConfigurationTypeDef(
     _RequiredApplicationCodeConfigurationTypeDef, _OptionalApplicationCodeConfigurationTypeDef
 ):
     pass
 
-
 ApplicationCodeConfigurationUpdateTypeDef = TypedDict(
     "ApplicationCodeConfigurationUpdateTypeDef",
     {
         "CodeContentTypeUpdate": CodeContentTypeType,
         "CodeContentUpdate": CodeContentUpdateTypeDef,
     },
     total=False,
@@ -1921,22 +2010,20 @@
         "CustomArtifactsConfigurationDescription": List[
             CustomArtifactConfigurationDescriptionTypeDef
         ],
     },
     total=False,
 )
 
-
 class ZeppelinApplicationConfigurationDescriptionTypeDef(
     _RequiredZeppelinApplicationConfigurationDescriptionTypeDef,
     _OptionalZeppelinApplicationConfigurationDescriptionTypeDef,
 ):
     pass
 
-
 ZeppelinApplicationConfigurationTypeDef = TypedDict(
     "ZeppelinApplicationConfigurationTypeDef",
     {
         "MonitoringConfiguration": ZeppelinMonitoringConfigurationTypeDef,
         "CatalogConfiguration": CatalogConfigurationTypeDef,
         "DeployAsApplicationConfiguration": DeployAsApplicationConfigurationTypeDef,
         "CustomArtifactsConfiguration": Sequence[CustomArtifactConfigurationTypeDef],
@@ -1999,21 +2086,38 @@
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
         "S3Configuration": S3ConfigurationTypeDef,
         "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DiscoverInputSchemaRequestRequestTypeDef(
     _RequiredDiscoverInputSchemaRequestRequestTypeDef,
     _OptionalDiscoverInputSchemaRequestRequestTypeDef,
 ):
     pass
 
+_RequiredRecordFormatOutputTypeDef = TypedDict(
+    "_RequiredRecordFormatOutputTypeDef",
+    {
+        "RecordFormatType": RecordFormatTypeType,
+    },
+)
+_OptionalRecordFormatOutputTypeDef = TypedDict(
+    "_OptionalRecordFormatOutputTypeDef",
+    {
+        "MappingParameters": MappingParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+class RecordFormatOutputTypeDef(
+    _RequiredRecordFormatOutputTypeDef, _OptionalRecordFormatOutputTypeDef
+):
+    pass
 
 _RequiredRecordFormatTypeDef = TypedDict(
     "_RequiredRecordFormatTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
@@ -2021,19 +2125,17 @@
     "_OptionalRecordFormatTypeDef",
     {
         "MappingParameters": MappingParametersTypeDef,
     },
     total=False,
 )
 
-
 class RecordFormatTypeDef(_RequiredRecordFormatTypeDef, _OptionalRecordFormatTypeDef):
     pass
 
-
 AddApplicationOutputResponseTypeDef = TypedDict(
     "AddApplicationOutputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2059,20 +2161,38 @@
     "_OptionalStartApplicationRequestRequestTypeDef",
     {
         "RunConfiguration": RunConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StartApplicationRequestRequestTypeDef(
     _RequiredStartApplicationRequestRequestTypeDef, _OptionalStartApplicationRequestRequestTypeDef
 ):
     pass
 
+_RequiredSourceSchemaOutputTypeDef = TypedDict(
+    "_RequiredSourceSchemaOutputTypeDef",
+    {
+        "RecordFormat": RecordFormatOutputTypeDef,
+        "RecordColumns": List[RecordColumnOutputTypeDef],
+    },
+)
+_OptionalSourceSchemaOutputTypeDef = TypedDict(
+    "_OptionalSourceSchemaOutputTypeDef",
+    {
+        "RecordEncoding": str,
+    },
+    total=False,
+)
+
+class SourceSchemaOutputTypeDef(
+    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
+):
+    pass
 
 InputSchemaUpdateTypeDef = TypedDict(
     "InputSchemaUpdateTypeDef",
     {
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
@@ -2091,47 +2211,21 @@
     "_OptionalSourceSchemaTypeDef",
     {
         "RecordEncoding": str,
     },
     total=False,
 )
 
-
 class SourceSchemaTypeDef(_RequiredSourceSchemaTypeDef, _OptionalSourceSchemaTypeDef):
     pass
 
-
-_RequiredInputUpdateTypeDef = TypedDict(
-    "_RequiredInputUpdateTypeDef",
-    {
-        "InputId": str,
-    },
-)
-_OptionalInputUpdateTypeDef = TypedDict(
-    "_OptionalInputUpdateTypeDef",
-    {
-        "NamePrefixUpdate": str,
-        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
-        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
-        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
-        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
-        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
-    },
-    total=False,
-)
-
-
-class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
-    pass
-
-
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2140,66 +2234,84 @@
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
-        "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
-    },
-    total=False,
-)
-
-_RequiredInputTypeDef = TypedDict(
-    "_RequiredInputTypeDef",
-    {
-        "NamePrefix": str,
-        "InputSchema": SourceSchemaTypeDef,
-    },
-)
-_OptionalInputTypeDef = TypedDict(
-    "_OptionalInputTypeDef",
-    {
-        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
-        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
-        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputParallelism": InputParallelismOutputTypeDef,
+        "InputStartingPositionConfiguration": InputStartingPositionConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
-class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
-    pass
-
-
 _RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
         "ReferenceId": str,
         "TableName": str,
         "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
     },
 )
 _OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
-        "ReferenceSchema": SourceSchemaTypeDef,
+        "ReferenceSchema": SourceSchemaOutputTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceDescriptionTypeDef(
     _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
 ):
     pass
 
+_RequiredInputUpdateTypeDef = TypedDict(
+    "_RequiredInputUpdateTypeDef",
+    {
+        "InputId": str,
+    },
+)
+_OptionalInputUpdateTypeDef = TypedDict(
+    "_OptionalInputUpdateTypeDef",
+    {
+        "NamePrefixUpdate": str,
+        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
+        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
+        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
+        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
+        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
+    },
+    total=False,
+)
+
+class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
+    pass
+
+_RequiredInputTypeDef = TypedDict(
+    "_RequiredInputTypeDef",
+    {
+        "NamePrefix": str,
+        "InputSchema": SourceSchemaTypeDef,
+    },
+)
+_OptionalInputTypeDef = TypedDict(
+    "_OptionalInputTypeDef",
+    {
+        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
+        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
+        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
+        "InputParallelism": InputParallelismTypeDef,
+    },
+    total=False,
+)
+
+class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
+    pass
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
@@ -2208,21 +2320,19 @@
     "_OptionalReferenceDataSourceTypeDef",
     {
         "S3ReferenceDataSource": S3ReferenceDataSourceTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceTypeDef(
     _RequiredReferenceDataSourceTypeDef, _OptionalReferenceDataSourceTypeDef
 ):
     pass
 
-
 _RequiredReferenceDataSourceUpdateTypeDef = TypedDict(
     "_RequiredReferenceDataSourceUpdateTypeDef",
     {
         "ReferenceId": str,
     },
 )
 _OptionalReferenceDataSourceUpdateTypeDef = TypedDict(
@@ -2231,40 +2341,29 @@
         "TableNameUpdate": str,
         "S3ReferenceDataSourceUpdate": S3ReferenceDataSourceUpdateTypeDef,
         "ReferenceSchemaUpdate": SourceSchemaTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
-
 AddApplicationInputResponseTypeDef = TypedDict(
     "AddApplicationInputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AddApplicationInputRequestRequestTypeDef = TypedDict(
-    "AddApplicationInputRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CurrentApplicationVersionId": int,
-        "Input": InputTypeDef,
-    },
-)
-
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2277,14 +2376,23 @@
         "InputDescriptions": List[InputDescriptionTypeDef],
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
     },
     total=False,
 )
 
+AddApplicationInputRequestRequestTypeDef = TypedDict(
+    "AddApplicationInputRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CurrentApplicationVersionId": int,
+        "Input": InputTypeDef,
+    },
+)
+
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
@@ -2384,21 +2492,19 @@
         "ConditionalToken": str,
         "ApplicationVersionRolledBackTo": int,
         "ApplicationMode": ApplicationModeType,
     },
     total=False,
 )
 
-
 class ApplicationDetailTypeDef(
     _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
 ):
     pass
 
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "RuntimeEnvironment": RuntimeEnvironmentType,
         "ServiceExecutionRole": str,
     },
@@ -2411,21 +2517,19 @@
         "CloudWatchLoggingOptions": Sequence[CloudWatchLoggingOptionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ApplicationMode": ApplicationModeType,
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
@@ -2437,21 +2541,19 @@
         "RunConfigurationUpdate": RunConfigurationUpdateTypeDef,
         "CloudWatchLoggingOptionUpdates": Sequence[CloudWatchLoggingOptionUpdateTypeDef],
         "ConditionalToken": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2/type_defs.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,28 +34,31 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationTypeDef",
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
+    "ApplicationRestoreConfigurationOutputTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
+    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
@@ -63,14 +66,16 @@
     "S3ApplicationCodeLocationDescriptionTypeDef",
     "S3ContentLocationTypeDef",
     "S3ContentLocationUpdateTypeDef",
     "CreateApplicationPresignedUrlRequestRequestTypeDef",
     "CreateApplicationPresignedUrlResponseTypeDef",
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
+    "MavenReferenceOutputTypeDef",
+    "S3ContentLocationOutputTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationOutputResponseTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
@@ -82,37 +87,43 @@
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
+    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
+    "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
+    "FlinkRunConfigurationOutputTypeDef",
     "FlinkRunConfigurationTypeDef",
-    "InputParallelismTypeDef",
+    "InputParallelismOutputTypeDef",
+    "InputStartingPositionConfigurationOutputTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
     "InputLambdaProcessorDescriptionTypeDef",
     "InputLambdaProcessorTypeDef",
     "InputLambdaProcessorUpdateTypeDef",
+    "InputParallelismTypeDef",
     "InputParallelismUpdateTypeDef",
     "RecordColumnTypeDef",
     "KinesisFirehoseInputTypeDef",
     "KinesisStreamsInputTypeDef",
     "KinesisFirehoseInputUpdateTypeDef",
     "KinesisStreamsInputUpdateTypeDef",
+    "JSONMappingParametersOutputTypeDef",
     "JSONMappingParametersTypeDef",
     "KinesisFirehoseOutputDescriptionTypeDef",
     "KinesisFirehoseOutputTypeDef",
     "KinesisFirehoseOutputUpdateTypeDef",
     "KinesisStreamsOutputDescriptionTypeDef",
     "KinesisStreamsOutputTypeDef",
     "KinesisStreamsOutputUpdateTypeDef",
@@ -121,15 +132,17 @@
     "LambdaOutputUpdateTypeDef",
     "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
     "ListApplicationSnapshotsRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
     "ResponseMetadataTypeDef",
     "RollbackApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -147,66 +160,69 @@
     "ListApplicationVersionsResponseTypeDef",
     "CatalogConfigurationDescriptionTypeDef",
     "CatalogConfigurationTypeDef",
     "CatalogConfigurationUpdateTypeDef",
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
-    "EnvironmentPropertyDescriptionsTypeDef",
     "EnvironmentPropertyUpdatesTypeDef",
+    "EnvironmentPropertyDescriptionsTypeDef",
     "FlinkApplicationConfigurationDescriptionTypeDef",
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
+    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ApplicationCodeConfigurationDescriptionTypeDef",
     "ApplicationCodeConfigurationTypeDef",
     "ApplicationCodeConfigurationUpdateTypeDef",
     "ZeppelinApplicationConfigurationDescriptionTypeDef",
     "ZeppelinApplicationConfigurationTypeDef",
     "ZeppelinApplicationConfigurationUpdateTypeDef",
     "RunConfigurationTypeDef",
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
+    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "SourceSchemaOutputTypeDef",
     "InputSchemaUpdateTypeDef",
     "SourceSchemaTypeDef",
-    "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "InputTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
+    "InputUpdateTypeDef",
+    "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
-    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
+    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "SqlApplicationConfigurationTypeDef",
     "SqlApplicationConfigurationUpdateTypeDef",
     "ApplicationConfigurationDescriptionTypeDef",
     "ApplicationConfigurationTypeDef",
     "ApplicationConfigurationUpdateTypeDef",
     "ApplicationDetailTypeDef",
@@ -237,20 +253,22 @@
     {
         "CloudWatchLoggingOptionId": str,
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
+
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
@@ -297,19 +315,21 @@
     {
         "SubnetIdUpdates": Sequence[str],
         "SecurityGroupIdUpdates": Sequence[str],
     },
     total=False,
 )
 
+
 class VpcConfigurationUpdateTypeDef(
     _RequiredVpcConfigurationUpdateTypeDef, _OptionalVpcConfigurationUpdateTypeDef
 ):
     pass
 
+
 ApplicationMaintenanceConfigurationDescriptionTypeDef = TypedDict(
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     {
         "ApplicationMaintenanceWindowStartTime": str,
         "ApplicationMaintenanceWindowEndTime": str,
     },
 )
@@ -317,33 +337,57 @@
 ApplicationMaintenanceConfigurationUpdateTypeDef = TypedDict(
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     {
         "ApplicationMaintenanceWindowStartTimeUpdate": str,
     },
 )
 
+_RequiredApplicationRestoreConfigurationOutputTypeDef = TypedDict(
+    "_RequiredApplicationRestoreConfigurationOutputTypeDef",
+    {
+        "ApplicationRestoreType": ApplicationRestoreTypeType,
+    },
+)
+_OptionalApplicationRestoreConfigurationOutputTypeDef = TypedDict(
+    "_OptionalApplicationRestoreConfigurationOutputTypeDef",
+    {
+        "SnapshotName": str,
+    },
+    total=False,
+)
+
+
+class ApplicationRestoreConfigurationOutputTypeDef(
+    _RequiredApplicationRestoreConfigurationOutputTypeDef,
+    _OptionalApplicationRestoreConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredApplicationRestoreConfigurationTypeDef = TypedDict(
     "_RequiredApplicationRestoreConfigurationTypeDef",
     {
         "ApplicationRestoreType": ApplicationRestoreTypeType,
     },
 )
 _OptionalApplicationRestoreConfigurationTypeDef = TypedDict(
     "_OptionalApplicationRestoreConfigurationTypeDef",
     {
         "SnapshotName": str,
     },
     total=False,
 )
 
+
 class ApplicationRestoreConfigurationTypeDef(
     _RequiredApplicationRestoreConfigurationTypeDef, _OptionalApplicationRestoreConfigurationTypeDef
 ):
     pass
 
+
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
         "ApplicationVersionId": int,
@@ -354,27 +398,37 @@
     "_OptionalApplicationSummaryTypeDef",
     {
         "ApplicationMode": ApplicationModeType,
     },
     total=False,
 )
 
+
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
+
 ApplicationVersionSummaryTypeDef = TypedDict(
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
+CSVMappingParametersOutputTypeDef = TypedDict(
+    "CSVMappingParametersOutputTypeDef",
+    {
+        "RecordRowDelimiter": str,
+        "RecordColumnDelimiter": str,
+    },
+)
+
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -423,19 +477,21 @@
         "CheckpointingEnabled": bool,
         "CheckpointInterval": int,
         "MinPauseBetweenCheckpoints": int,
     },
     total=False,
 )
 
+
 class CheckpointConfigurationTypeDef(
     _RequiredCheckpointConfigurationTypeDef, _OptionalCheckpointConfigurationTypeDef
 ):
     pass
 
+
 CheckpointConfigurationUpdateTypeDef = TypedDict(
     "CheckpointConfigurationUpdateTypeDef",
     {
         "ConfigurationTypeUpdate": ConfigurationTypeType,
         "CheckpointingEnabledUpdate": bool,
         "CheckpointIntervalUpdate": int,
         "MinPauseBetweenCheckpointsUpdate": int,
@@ -453,19 +509,21 @@
     "_OptionalCloudWatchLoggingOptionUpdateTypeDef",
     {
         "LogStreamARNUpdate": str,
     },
     total=False,
 )
 
+
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
+
 _RequiredS3ApplicationCodeLocationDescriptionTypeDef = TypedDict(
     "_RequiredS3ApplicationCodeLocationDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -473,20 +531,22 @@
     "_OptionalS3ApplicationCodeLocationDescriptionTypeDef",
     {
         "ObjectVersion": str,
     },
     total=False,
 )
 
+
 class S3ApplicationCodeLocationDescriptionTypeDef(
     _RequiredS3ApplicationCodeLocationDescriptionTypeDef,
     _OptionalS3ApplicationCodeLocationDescriptionTypeDef,
 ):
     pass
 
+
 _RequiredS3ContentLocationTypeDef = TypedDict(
     "_RequiredS3ContentLocationTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -494,19 +554,21 @@
     "_OptionalS3ContentLocationTypeDef",
     {
         "ObjectVersion": str,
     },
     total=False,
 )
 
+
 class S3ContentLocationTypeDef(
     _RequiredS3ContentLocationTypeDef, _OptionalS3ContentLocationTypeDef
 ):
     pass
 
+
 S3ContentLocationUpdateTypeDef = TypedDict(
     "S3ContentLocationUpdateTypeDef",
     {
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
         "ObjectVersionUpdate": str,
     },
@@ -524,20 +586,22 @@
     "_OptionalCreateApplicationPresignedUrlRequestRequestTypeDef",
     {
         "SessionExpirationDurationInSeconds": int,
     },
     total=False,
 )
 
+
 class CreateApplicationPresignedUrlRequestRequestTypeDef(
     _RequiredCreateApplicationPresignedUrlRequestRequestTypeDef,
     _OptionalCreateApplicationPresignedUrlRequestRequestTypeDef,
 ):
     pass
 
+
 CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
     "CreateApplicationPresignedUrlResponseTypeDef",
     {
         "AuthorizedUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -552,25 +616,58 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 CreateApplicationSnapshotRequestRequestTypeDef = TypedDict(
     "CreateApplicationSnapshotRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "SnapshotName": str,
     },
 )
 
+MavenReferenceOutputTypeDef = TypedDict(
+    "MavenReferenceOutputTypeDef",
+    {
+        "GroupId": str,
+        "ArtifactId": str,
+        "Version": str,
+    },
+)
+
+_RequiredS3ContentLocationOutputTypeDef = TypedDict(
+    "_RequiredS3ContentLocationOutputTypeDef",
+    {
+        "BucketARN": str,
+        "FileKey": str,
+    },
+)
+_OptionalS3ContentLocationOutputTypeDef = TypedDict(
+    "_OptionalS3ContentLocationOutputTypeDef",
+    {
+        "ObjectVersion": str,
+    },
+    total=False,
+)
+
+
+class S3ContentLocationOutputTypeDef(
+    _RequiredS3ContentLocationOutputTypeDef, _OptionalS3ContentLocationOutputTypeDef
+):
+    pass
+
+
 MavenReferenceTypeDef = TypedDict(
     "MavenReferenceTypeDef",
     {
         "GroupId": str,
         "ArtifactId": str,
         "Version": str,
     },
@@ -588,20 +685,22 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
+
 class DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef(
     _RequiredDeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     _OptionalDeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "InputId": str,
     },
@@ -681,20 +780,22 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
+
 class DeleteApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalDeleteApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "DeleteApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -710,39 +811,43 @@
     "_OptionalS3ContentBaseLocationDescriptionTypeDef",
     {
         "BasePath": str,
     },
     total=False,
 )
 
+
 class S3ContentBaseLocationDescriptionTypeDef(
     _RequiredS3ContentBaseLocationDescriptionTypeDef,
     _OptionalS3ContentBaseLocationDescriptionTypeDef,
 ):
     pass
 
+
 _RequiredS3ContentBaseLocationTypeDef = TypedDict(
     "_RequiredS3ContentBaseLocationTypeDef",
     {
         "BucketARN": str,
     },
 )
 _OptionalS3ContentBaseLocationTypeDef = TypedDict(
     "_OptionalS3ContentBaseLocationTypeDef",
     {
         "BasePath": str,
     },
     total=False,
 )
 
+
 class S3ContentBaseLocationTypeDef(
     _RequiredS3ContentBaseLocationTypeDef, _OptionalS3ContentBaseLocationTypeDef
 ):
     pass
 
+
 S3ContentBaseLocationUpdateTypeDef = TypedDict(
     "S3ContentBaseLocationUpdateTypeDef",
     {
         "BucketARNUpdate": str,
         "BasePathUpdate": str,
     },
     total=False,
@@ -758,20 +863,22 @@
     "_OptionalDescribeApplicationRequestRequestTypeDef",
     {
         "IncludeAdditionalDetails": bool,
     },
     total=False,
 )
 
+
 class DescribeApplicationRequestRequestTypeDef(
     _RequiredDescribeApplicationRequestRequestTypeDef,
     _OptionalDescribeApplicationRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeApplicationSnapshotRequestRequestTypeDef = TypedDict(
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "SnapshotName": str,
     },
 )
@@ -788,25 +895,34 @@
     "_OptionalSnapshotDetailsTypeDef",
     {
         "SnapshotCreationTimestamp": datetime,
     },
     total=False,
 )
 
+
 class SnapshotDetailsTypeDef(_RequiredSnapshotDetailsTypeDef, _OptionalSnapshotDetailsTypeDef):
     pass
 
+
 DescribeApplicationVersionRequestRequestTypeDef = TypedDict(
     "DescribeApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "ApplicationVersionId": int,
     },
 )
 
+DestinationSchemaOutputTypeDef = TypedDict(
+    "DestinationSchemaOutputTypeDef",
+    {
+        "RecordFormatType": RecordFormatTypeType,
+    },
+)
+
 DestinationSchemaTypeDef = TypedDict(
     "DestinationSchemaTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 
@@ -830,14 +946,22 @@
     "PropertyGroupTypeDef",
     {
         "PropertyGroupId": str,
         "PropertyMap": Mapping[str, str],
     },
 )
 
+PropertyGroupOutputTypeDef = TypedDict(
+    "PropertyGroupOutputTypeDef",
+    {
+        "PropertyGroupId": str,
+        "PropertyMap": Dict[str, str],
+    },
+)
+
 MonitoringConfigurationDescriptionTypeDef = TypedDict(
     "MonitoringConfigurationDescriptionTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
@@ -867,19 +991,21 @@
     {
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
     total=False,
 )
 
+
 class MonitoringConfigurationTypeDef(
     _RequiredMonitoringConfigurationTypeDef, _OptionalMonitoringConfigurationTypeDef
 ):
     pass
 
+
 _RequiredParallelismConfigurationTypeDef = TypedDict(
     "_RequiredParallelismConfigurationTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
     },
 )
 _OptionalParallelismConfigurationTypeDef = TypedDict(
@@ -888,19 +1014,21 @@
         "Parallelism": int,
         "ParallelismPerKPU": int,
         "AutoScalingEnabled": bool,
     },
     total=False,
 )
 
+
 class ParallelismConfigurationTypeDef(
     _RequiredParallelismConfigurationTypeDef, _OptionalParallelismConfigurationTypeDef
 ):
     pass
 
+
 MonitoringConfigurationUpdateTypeDef = TypedDict(
     "MonitoringConfigurationUpdateTypeDef",
     {
         "ConfigurationTypeUpdate": ConfigurationTypeType,
         "MetricsLevelUpdate": MetricsLevelType,
         "LogLevelUpdate": LogLevelType,
     },
@@ -914,101 +1042,131 @@
         "ParallelismUpdate": int,
         "ParallelismPerKPUUpdate": int,
         "AutoScalingEnabledUpdate": bool,
     },
     total=False,
 )
 
+FlinkRunConfigurationOutputTypeDef = TypedDict(
+    "FlinkRunConfigurationOutputTypeDef",
+    {
+        "AllowNonRestoredState": bool,
+    },
+    total=False,
+)
+
 FlinkRunConfigurationTypeDef = TypedDict(
     "FlinkRunConfigurationTypeDef",
     {
         "AllowNonRestoredState": bool,
     },
     total=False,
 )
 
-InputParallelismTypeDef = TypedDict(
-    "InputParallelismTypeDef",
+InputParallelismOutputTypeDef = TypedDict(
+    "InputParallelismOutputTypeDef",
     {
         "Count": int,
     },
     total=False,
 )
 
+InputStartingPositionConfigurationOutputTypeDef = TypedDict(
+    "InputStartingPositionConfigurationOutputTypeDef",
+    {
+        "InputStartingPosition": InputStartingPositionType,
+    },
+    total=False,
+)
+
 _RequiredKinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "_RequiredKinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalKinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "_OptionalKinesisFirehoseInputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class KinesisFirehoseInputDescriptionTypeDef(
     _RequiredKinesisFirehoseInputDescriptionTypeDef, _OptionalKinesisFirehoseInputDescriptionTypeDef
 ):
     pass
 
+
 _RequiredKinesisStreamsInputDescriptionTypeDef = TypedDict(
     "_RequiredKinesisStreamsInputDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalKinesisStreamsInputDescriptionTypeDef = TypedDict(
     "_OptionalKinesisStreamsInputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class KinesisStreamsInputDescriptionTypeDef(
     _RequiredKinesisStreamsInputDescriptionTypeDef, _OptionalKinesisStreamsInputDescriptionTypeDef
 ):
     pass
 
+
 _RequiredInputLambdaProcessorDescriptionTypeDef = TypedDict(
     "_RequiredInputLambdaProcessorDescriptionTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalInputLambdaProcessorDescriptionTypeDef = TypedDict(
     "_OptionalInputLambdaProcessorDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class InputLambdaProcessorDescriptionTypeDef(
     _RequiredInputLambdaProcessorDescriptionTypeDef, _OptionalInputLambdaProcessorDescriptionTypeDef
 ):
     pass
 
+
 InputLambdaProcessorTypeDef = TypedDict(
     "InputLambdaProcessorTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
 InputLambdaProcessorUpdateTypeDef = TypedDict(
     "InputLambdaProcessorUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
+InputParallelismTypeDef = TypedDict(
+    "InputParallelismTypeDef",
+    {
+        "Count": int,
+    },
+    total=False,
+)
+
 InputParallelismUpdateTypeDef = TypedDict(
     "InputParallelismUpdateTypeDef",
     {
         "CountUpdate": int,
     },
 )
 
@@ -1023,17 +1181,19 @@
     "_OptionalRecordColumnTypeDef",
     {
         "Mapping": str,
     },
     total=False,
 )
 
+
 class RecordColumnTypeDef(_RequiredRecordColumnTypeDef, _OptionalRecordColumnTypeDef):
     pass
 
+
 KinesisFirehoseInputTypeDef = TypedDict(
     "KinesisFirehoseInputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1054,14 +1214,21 @@
 KinesisStreamsInputUpdateTypeDef = TypedDict(
     "KinesisStreamsInputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
+JSONMappingParametersOutputTypeDef = TypedDict(
+    "JSONMappingParametersOutputTypeDef",
+    {
+        "RecordRowPath": str,
+    },
+)
+
 JSONMappingParametersTypeDef = TypedDict(
     "JSONMappingParametersTypeDef",
     {
         "RecordRowPath": str,
     },
 )
 
@@ -1075,20 +1242,22 @@
     "_OptionalKinesisFirehoseOutputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class KinesisFirehoseOutputDescriptionTypeDef(
     _RequiredKinesisFirehoseOutputDescriptionTypeDef,
     _OptionalKinesisFirehoseOutputDescriptionTypeDef,
 ):
     pass
 
+
 KinesisFirehoseOutputTypeDef = TypedDict(
     "KinesisFirehoseOutputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1109,19 +1278,21 @@
     "_OptionalKinesisStreamsOutputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class KinesisStreamsOutputDescriptionTypeDef(
     _RequiredKinesisStreamsOutputDescriptionTypeDef, _OptionalKinesisStreamsOutputDescriptionTypeDef
 ):
     pass
 
+
 KinesisStreamsOutputTypeDef = TypedDict(
     "KinesisStreamsOutputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1142,19 +1313,21 @@
     "_OptionalLambdaOutputDescriptionTypeDef",
     {
         "RoleARN": str,
     },
     total=False,
 )
 
+
 class LambdaOutputDescriptionTypeDef(
     _RequiredLambdaOutputDescriptionTypeDef, _OptionalLambdaOutputDescriptionTypeDef
 ):
     pass
 
+
 LambdaOutputTypeDef = TypedDict(
     "LambdaOutputTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1175,20 +1348,22 @@
     "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
     _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
     _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationSnapshotsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
@@ -1196,20 +1371,22 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationSnapshotsRequestRequestTypeDef(
     _RequiredListApplicationSnapshotsRequestRequestTypeDef,
     _OptionalListApplicationSnapshotsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -1217,20 +1394,22 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -1247,24 +1426,65 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
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
 
+_RequiredRecordColumnOutputTypeDef = TypedDict(
+    "_RequiredRecordColumnOutputTypeDef",
+    {
+        "Name": str,
+        "SqlType": str,
+    },
+)
+_OptionalRecordColumnOutputTypeDef = TypedDict(
+    "_OptionalRecordColumnOutputTypeDef",
+    {
+        "Mapping": str,
+    },
+    total=False,
+)
+
+
+class RecordColumnOutputTypeDef(
+    _RequiredRecordColumnOutputTypeDef, _OptionalRecordColumnOutputTypeDef
+):
+    pass
+
+
 _RequiredS3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredS3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -1272,20 +1492,22 @@
     "_OptionalS3ReferenceDataSourceDescriptionTypeDef",
     {
         "ReferenceRoleARN": str,
     },
     total=False,
 )
 
+
 class S3ReferenceDataSourceDescriptionTypeDef(
     _RequiredS3ReferenceDataSourceDescriptionTypeDef,
     _OptionalS3ReferenceDataSourceDescriptionTypeDef,
 ):
     pass
 
+
 S3ReferenceDataSourceTypeDef = TypedDict(
     "S3ReferenceDataSourceTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
     total=False,
@@ -1329,19 +1551,21 @@
     "_OptionalStopApplicationRequestRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
+
 class StopApplicationRequestRequestTypeDef(
     _RequiredStopApplicationRequestRequestTypeDef, _OptionalStopApplicationRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1380,20 +1604,22 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
+
 class AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef(
     _RequiredAddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     _OptionalAddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
 ):
     pass
 
+
 AddApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1422,20 +1648,22 @@
     {
         "CurrentApplicationVersionId": int,
         "ConditionalToken": str,
     },
     total=False,
 )
 
+
 class AddApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredAddApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalAddApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 AddApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "AddApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1529,36 +1757,28 @@
         "TextContentUpdate": str,
         "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
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
 
 CustomArtifactConfigurationDescriptionTypeDef = TypedDict(
     "CustomArtifactConfigurationDescriptionTypeDef",
     {
         "ArtifactType": ArtifactTypeType,
-        "S3ContentLocationDescription": S3ContentLocationTypeDef,
-        "MavenReferenceDescription": MavenReferenceTypeDef,
+        "S3ContentLocationDescription": S3ContentLocationOutputTypeDef,
+        "MavenReferenceDescription": MavenReferenceOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCustomArtifactConfigurationTypeDef = TypedDict(
     "_RequiredCustomArtifactConfigurationTypeDef",
     {
@@ -1570,19 +1790,21 @@
     {
         "S3ContentLocation": S3ContentLocationTypeDef,
         "MavenReference": MavenReferenceTypeDef,
     },
     total=False,
 )
 
+
 class CustomArtifactConfigurationTypeDef(
     _RequiredCustomArtifactConfigurationTypeDef, _OptionalCustomArtifactConfigurationTypeDef
 ):
     pass
 
+
 DeployAsApplicationConfigurationDescriptionTypeDef = TypedDict(
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     {
         "S3ContentLocationDescription": S3ContentBaseLocationDescriptionTypeDef,
     },
 )
 
@@ -1629,27 +1851,27 @@
 EnvironmentPropertiesTypeDef = TypedDict(
     "EnvironmentPropertiesTypeDef",
     {
         "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
 )
 
-EnvironmentPropertyDescriptionsTypeDef = TypedDict(
-    "EnvironmentPropertyDescriptionsTypeDef",
+EnvironmentPropertyUpdatesTypeDef = TypedDict(
+    "EnvironmentPropertyUpdatesTypeDef",
     {
-        "PropertyGroupDescriptions": List[PropertyGroupTypeDef],
+        "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
-    total=False,
 )
 
-EnvironmentPropertyUpdatesTypeDef = TypedDict(
-    "EnvironmentPropertyUpdatesTypeDef",
+EnvironmentPropertyDescriptionsTypeDef = TypedDict(
+    "EnvironmentPropertyDescriptionsTypeDef",
     {
-        "PropertyGroups": Sequence[PropertyGroupTypeDef],
+        "PropertyGroupDescriptions": List[PropertyGroupOutputTypeDef],
     },
+    total=False,
 )
 
 FlinkApplicationConfigurationDescriptionTypeDef = TypedDict(
     "FlinkApplicationConfigurationDescriptionTypeDef",
     {
         "CheckpointConfigurationDescription": CheckpointConfigurationDescriptionTypeDef,
         "MonitoringConfigurationDescription": MonitoringConfigurationDescriptionTypeDef,
@@ -1678,16 +1900,16 @@
     },
     total=False,
 )
 
 RunConfigurationDescriptionTypeDef = TypedDict(
     "RunConfigurationDescriptionTypeDef",
     {
-        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationTypeDef,
-        "FlinkRunConfigurationDescription": FlinkRunConfigurationTypeDef,
+        "ApplicationRestoreConfigurationDescription": ApplicationRestoreConfigurationOutputTypeDef,
+        "FlinkRunConfigurationDescription": FlinkRunConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 RunConfigurationUpdateTypeDef = TypedDict(
     "RunConfigurationUpdateTypeDef",
     {
@@ -1715,14 +1937,23 @@
 InputProcessingConfigurationUpdateTypeDef = TypedDict(
     "InputProcessingConfigurationUpdateTypeDef",
     {
         "InputLambdaProcessorUpdate": InputLambdaProcessorUpdateTypeDef,
     },
 )
 
+MappingParametersOutputTypeDef = TypedDict(
+    "MappingParametersOutputTypeDef",
+    {
+        "JSONMappingParameters": JSONMappingParametersOutputTypeDef,
+        "CSVMappingParameters": CSVMappingParametersOutputTypeDef,
+    },
+    total=False,
+)
+
 MappingParametersTypeDef = TypedDict(
     "MappingParametersTypeDef",
     {
         "JSONMappingParameters": JSONMappingParametersTypeDef,
         "CSVMappingParameters": CSVMappingParametersTypeDef,
     },
     total=False,
@@ -1732,15 +1963,15 @@
     "OutputDescriptionTypeDef",
     {
         "OutputId": str,
         "Name": str,
         "KinesisStreamsOutputDescription": KinesisStreamsOutputDescriptionTypeDef,
         "KinesisFirehoseOutputDescription": KinesisFirehoseOutputDescriptionTypeDef,
         "LambdaOutputDescription": LambdaOutputDescriptionTypeDef,
-        "DestinationSchema": DestinationSchemaTypeDef,
+        "DestinationSchema": DestinationSchemaOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
@@ -1754,17 +1985,19 @@
         "KinesisStreamsOutput": KinesisStreamsOutputTypeDef,
         "KinesisFirehoseOutput": KinesisFirehoseOutputTypeDef,
         "LambdaOutput": LambdaOutputTypeDef,
     },
     total=False,
 )
 
+
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
+
 _RequiredOutputUpdateTypeDef = TypedDict(
     "_RequiredOutputUpdateTypeDef",
     {
         "OutputId": str,
     },
 )
 _OptionalOutputUpdateTypeDef = TypedDict(
@@ -1775,56 +2008,70 @@
         "KinesisFirehoseOutputUpdate": KinesisFirehoseOutputUpdateTypeDef,
         "LambdaOutputUpdate": LambdaOutputUpdateTypeDef,
         "DestinationSchemaUpdate": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
+
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
 )
 _OptionalApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
     "_OptionalApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentDescription": CodeContentDescriptionTypeDef,
     },
     total=False,
 )
 
+
 class ApplicationCodeConfigurationDescriptionTypeDef(
     _RequiredApplicationCodeConfigurationDescriptionTypeDef,
     _OptionalApplicationCodeConfigurationDescriptionTypeDef,
 ):
     pass
 
+
 _RequiredApplicationCodeConfigurationTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
 )
 _OptionalApplicationCodeConfigurationTypeDef = TypedDict(
     "_OptionalApplicationCodeConfigurationTypeDef",
     {
         "CodeContent": CodeContentTypeDef,
     },
     total=False,
 )
 
+
 class ApplicationCodeConfigurationTypeDef(
     _RequiredApplicationCodeConfigurationTypeDef, _OptionalApplicationCodeConfigurationTypeDef
 ):
     pass
 
+
 ApplicationCodeConfigurationUpdateTypeDef = TypedDict(
     "ApplicationCodeConfigurationUpdateTypeDef",
     {
         "CodeContentTypeUpdate": CodeContentTypeType,
         "CodeContentUpdate": CodeContentUpdateTypeDef,
     },
     total=False,
@@ -1846,20 +2093,22 @@
         "CustomArtifactsConfigurationDescription": List[
             CustomArtifactConfigurationDescriptionTypeDef
         ],
     },
     total=False,
 )
 
+
 class ZeppelinApplicationConfigurationDescriptionTypeDef(
     _RequiredZeppelinApplicationConfigurationDescriptionTypeDef,
     _OptionalZeppelinApplicationConfigurationDescriptionTypeDef,
 ):
     pass
 
+
 ZeppelinApplicationConfigurationTypeDef = TypedDict(
     "ZeppelinApplicationConfigurationTypeDef",
     {
         "MonitoringConfiguration": ZeppelinMonitoringConfigurationTypeDef,
         "CatalogConfiguration": CatalogConfigurationTypeDef,
         "DeployAsApplicationConfiguration": DeployAsApplicationConfigurationTypeDef,
         "CustomArtifactsConfiguration": Sequence[CustomArtifactConfigurationTypeDef],
@@ -1922,37 +2171,62 @@
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
         "S3Configuration": S3ConfigurationTypeDef,
         "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DiscoverInputSchemaRequestRequestTypeDef(
     _RequiredDiscoverInputSchemaRequestRequestTypeDef,
     _OptionalDiscoverInputSchemaRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredRecordFormatOutputTypeDef = TypedDict(
+    "_RequiredRecordFormatOutputTypeDef",
+    {
+        "RecordFormatType": RecordFormatTypeType,
+    },
+)
+_OptionalRecordFormatOutputTypeDef = TypedDict(
+    "_OptionalRecordFormatOutputTypeDef",
+    {
+        "MappingParameters": MappingParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RecordFormatOutputTypeDef(
+    _RequiredRecordFormatOutputTypeDef, _OptionalRecordFormatOutputTypeDef
+):
+    pass
+
+
 _RequiredRecordFormatTypeDef = TypedDict(
     "_RequiredRecordFormatTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 _OptionalRecordFormatTypeDef = TypedDict(
     "_OptionalRecordFormatTypeDef",
     {
         "MappingParameters": MappingParametersTypeDef,
     },
     total=False,
 )
 
+
 class RecordFormatTypeDef(_RequiredRecordFormatTypeDef, _OptionalRecordFormatTypeDef):
     pass
 
+
 AddApplicationOutputResponseTypeDef = TypedDict(
     "AddApplicationOutputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1978,19 +2252,43 @@
     "_OptionalStartApplicationRequestRequestTypeDef",
     {
         "RunConfiguration": RunConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StartApplicationRequestRequestTypeDef(
     _RequiredStartApplicationRequestRequestTypeDef, _OptionalStartApplicationRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredSourceSchemaOutputTypeDef = TypedDict(
+    "_RequiredSourceSchemaOutputTypeDef",
+    {
+        "RecordFormat": RecordFormatOutputTypeDef,
+        "RecordColumns": List[RecordColumnOutputTypeDef],
+    },
+)
+_OptionalSourceSchemaOutputTypeDef = TypedDict(
+    "_OptionalSourceSchemaOutputTypeDef",
+    {
+        "RecordEncoding": str,
+    },
+    total=False,
+)
+
+
+class SourceSchemaOutputTypeDef(
+    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
+):
+    pass
+
+
 InputSchemaUpdateTypeDef = TypedDict(
     "InputSchemaUpdateTypeDef",
     {
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
@@ -2008,43 +2306,23 @@
     "_OptionalSourceSchemaTypeDef",
     {
         "RecordEncoding": str,
     },
     total=False,
 )
 
+
 class SourceSchemaTypeDef(_RequiredSourceSchemaTypeDef, _OptionalSourceSchemaTypeDef):
     pass
 
-_RequiredInputUpdateTypeDef = TypedDict(
-    "_RequiredInputUpdateTypeDef",
-    {
-        "InputId": str,
-    },
-)
-_OptionalInputUpdateTypeDef = TypedDict(
-    "_OptionalInputUpdateTypeDef",
-    {
-        "NamePrefixUpdate": str,
-        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
-        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
-        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
-        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
-        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
-    },
-    total=False,
-)
-
-class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
-    pass
 
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2053,21 +2331,68 @@
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
-        "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputParallelism": InputParallelismOutputTypeDef,
+        "InputStartingPositionConfiguration": InputStartingPositionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+    },
+)
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceSchema": SourceSchemaOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
+    pass
+
+
+_RequiredInputUpdateTypeDef = TypedDict(
+    "_RequiredInputUpdateTypeDef",
+    {
+        "InputId": str,
+    },
+)
+_OptionalInputUpdateTypeDef = TypedDict(
+    "_OptionalInputUpdateTypeDef",
+    {
+        "NamePrefixUpdate": str,
+        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
+        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
+        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
+        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
+        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
     },
     total=False,
 )
 
+
+class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
+    pass
+
+
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -2078,37 +2403,18 @@
         "KinesisStreamsInput": KinesisStreamsInputTypeDef,
         "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
     },
     total=False,
 )
 
+
 class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
-    },
-)
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceSchema": SourceSchemaTypeDef,
-    },
-    total=False,
-)
-
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
-    pass
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
@@ -2117,19 +2423,21 @@
     "_OptionalReferenceDataSourceTypeDef",
     {
         "S3ReferenceDataSource": S3ReferenceDataSourceTypeDef,
     },
     total=False,
 )
 
+
 class ReferenceDataSourceTypeDef(
     _RequiredReferenceDataSourceTypeDef, _OptionalReferenceDataSourceTypeDef
 ):
     pass
 
+
 _RequiredReferenceDataSourceUpdateTypeDef = TypedDict(
     "_RequiredReferenceDataSourceUpdateTypeDef",
     {
         "ReferenceId": str,
     },
 )
 _OptionalReferenceDataSourceUpdateTypeDef = TypedDict(
@@ -2138,38 +2446,31 @@
         "TableNameUpdate": str,
         "S3ReferenceDataSourceUpdate": S3ReferenceDataSourceUpdateTypeDef,
         "ReferenceSchemaUpdate": SourceSchemaTypeDef,
     },
     total=False,
 )
 
+
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
+
 AddApplicationInputResponseTypeDef = TypedDict(
     "AddApplicationInputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AddApplicationInputRequestRequestTypeDef = TypedDict(
-    "AddApplicationInputRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CurrentApplicationVersionId": int,
-        "Input": InputTypeDef,
-    },
-)
-
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2182,14 +2483,23 @@
         "InputDescriptions": List[InputDescriptionTypeDef],
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
     },
     total=False,
 )
 
+AddApplicationInputRequestRequestTypeDef = TypedDict(
+    "AddApplicationInputRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CurrentApplicationVersionId": int,
+        "Input": InputTypeDef,
+    },
+)
+
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
@@ -2289,19 +2599,21 @@
         "ConditionalToken": str,
         "ApplicationVersionRolledBackTo": int,
         "ApplicationMode": ApplicationModeType,
     },
     total=False,
 )
 
+
 class ApplicationDetailTypeDef(
     _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
 ):
     pass
 
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "RuntimeEnvironment": RuntimeEnvironmentType,
         "ServiceExecutionRole": str,
     },
@@ -2314,19 +2626,21 @@
         "CloudWatchLoggingOptions": Sequence[CloudWatchLoggingOptionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ApplicationMode": ApplicationModeType,
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
@@ -2338,19 +2652,21 @@
         "RunConfigurationUpdate": RunConfigurationUpdateTypeDef,
         "CloudWatchLoggingOptionUpdates": Sequence[CloudWatchLoggingOptionUpdateTypeDef],
         "ConditionalToken": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.12/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.0
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-kinesisanalyticsv2"></a>
 
 # mypy-boto3-kinesisanalyticsv2
 
 [![PyPI - mypy-boto3-kinesisanalyticsv2](https://img.shields.io/pypi/v/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisanalyticsv2?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisanalyticsv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalyticsv2)](https://pepy.tech/project/mypy-boto3-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalyticsV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[boto3.KinesisAnalyticsV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,17 +318,19 @@
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
+    ApplicationRestoreConfigurationOutputTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
@@ -368,14 +338,16 @@
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
     CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
+    MavenReferenceOutputTypeDef,
+    S3ContentLocationOutputTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
@@ -387,37 +359,43 @@
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
+    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
+    PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
+    FlinkRunConfigurationOutputTypeDef,
     FlinkRunConfigurationTypeDef,
-    InputParallelismTypeDef,
+    InputParallelismOutputTypeDef,
+    InputStartingPositionConfigurationOutputTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
     InputLambdaProcessorDescriptionTypeDef,
     InputLambdaProcessorTypeDef,
     InputLambdaProcessorUpdateTypeDef,
+    InputParallelismTypeDef,
     InputParallelismUpdateTypeDef,
     RecordColumnTypeDef,
     KinesisFirehoseInputTypeDef,
     KinesisStreamsInputTypeDef,
     KinesisFirehoseInputUpdateTypeDef,
     KinesisStreamsInputUpdateTypeDef,
+    JSONMappingParametersOutputTypeDef,
     JSONMappingParametersTypeDef,
     KinesisFirehoseOutputDescriptionTypeDef,
     KinesisFirehoseOutputTypeDef,
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
@@ -426,15 +404,17 @@
     LambdaOutputUpdateTypeDef,
     ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
     ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -452,66 +432,69 @@
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
     CatalogConfigurationTypeDef,
     CatalogConfigurationUpdateTypeDef,
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
-    EnvironmentPropertyDescriptionsTypeDef,
     EnvironmentPropertyUpdatesTypeDef,
+    EnvironmentPropertyDescriptionsTypeDef,
     FlinkApplicationConfigurationDescriptionTypeDef,
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
+    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
     AddApplicationInputProcessingConfigurationResponseTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
+    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
+    SourceSchemaOutputTypeDef,
     InputSchemaUpdateTypeDef,
     SourceSchemaTypeDef,
-    InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputUpdateTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
+    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     SqlApplicationConfigurationTypeDef,
     SqlApplicationConfigurationUpdateTypeDef,
     ApplicationConfigurationDescriptionTypeDef,
     ApplicationConfigurationTypeDef,
     ApplicationConfigurationUpdateTypeDef,
     ApplicationDetailTypeDef,
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt` & `mypy-boto3-kinesisanalyticsv2-1.28.12/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.0/setup.py` & `mypy-boto3-kinesisanalyticsv2-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisanalyticsv2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisAnalyticsV2 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.KinesisAnalyticsV2 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

