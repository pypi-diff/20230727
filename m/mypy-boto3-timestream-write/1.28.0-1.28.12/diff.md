# Comparing `tmp/mypy-boto3-timestream-write-1.28.0.tar.gz` & `tmp/mypy-boto3-timestream-write-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-write-1.28.0.tar", last modified: Thu Jul  6 21:00:47 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-write-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
```

## Comparing `mypy-boto3-timestream-write-1.28.0.tar` & `mypy-boto3-timestream-write-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.130451 mypy-boto3-timestream-write-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-06 21:00:47.130451 mypy-boto3-timestream-write-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.126450 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-06 20:57:14.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-06 20:57:14.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-06 20:57:14.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-06 20:57:14.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-06 20:57:14.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21308 2023-07-06 20:57:14.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.130451 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-06 21:00:46.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-06 21:00:46.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:46.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 21:00:46.000000 mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:47.130451 mypy-boto3-timestream-write-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-06 20:57:13.000000 mypy-boto3-timestream-write-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.685443 mypy-boto3-timestream-write-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-07-27 11:49:46.681443 mypy-boto3-timestream-write-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.681443 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29204 2023-07-27 11:48:02.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.681443 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 11:49:46.000000 mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.685443 mypy-boto3-timestream-write-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 11:48:01.000000 mypy-boto3-timestream-write-1.28.12/setup.py
```

### Comparing `mypy-boto3-timestream-write-1.28.0/LICENSE` & `mypy-boto3-timestream-write-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.0/PKG-INFO` & `mypy-boto3-timestream-write-1.28.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.0
-Summary: Type annotations for boto3.TimestreamWrite 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.TimestreamWrite 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,67 +309,86 @@
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
+    CsvConfigurationOutputTypeDef,
     CsvConfigurationTypeDef,
+    DataModelS3ConfigurationOutputTypeDef,
     DataModelS3ConfigurationTypeDef,
+    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
+    DataSourceS3ConfigurationOutputTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
+    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
+    ReportS3ConfigurationOutputTypeDef,
     ReportS3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
+    RetentionPropertiesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MagneticStoreRejectedDataLocationOutputTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
+    MixedMeasureMappingOutputTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
+    ReportConfigurationOutputTypeDef,
     ReportConfigurationTypeDef,
+    MagneticStoreWritePropertiesOutputTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
+    DataModelOutputTypeDef,
     DataModelTypeDef,
-    CreateTableRequestRequestTypeDef,
     TableTypeDef,
+    CreateTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
```

### Comparing `mypy-boto3-timestream-write-1.28.0/README.md` & `mypy-boto3-timestream-write-1.28.12/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,67 +277,86 @@
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
+    CsvConfigurationOutputTypeDef,
     CsvConfigurationTypeDef,
+    DataModelS3ConfigurationOutputTypeDef,
     DataModelS3ConfigurationTypeDef,
+    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
+    DataSourceS3ConfigurationOutputTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
+    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
+    ReportS3ConfigurationOutputTypeDef,
     ReportS3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
+    RetentionPropertiesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MagneticStoreRejectedDataLocationOutputTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
+    MixedMeasureMappingOutputTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
+    ReportConfigurationOutputTypeDef,
     ReportConfigurationTypeDef,
+    MagneticStoreWritePropertiesOutputTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
+    DataModelOutputTypeDef,
     DataModelTypeDef,
-    CreateTableRequestRequestTypeDef,
     TableTypeDef,
+    CreateTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
```

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/__main__.py` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamWrite 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.TimestreamWrite 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
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

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/client.py` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/client.pyi` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/literals.py` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
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
@@ -251,26 +252,28 @@
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

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/literals.pyi` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
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
@@ -249,26 +250,28 @@
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

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/type_defs.py` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -31,71 +31,89 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
-    "CreateBatchLoadTaskResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
+    "CsvConfigurationOutputTypeDef",
     "CsvConfigurationTypeDef",
+    "DataModelS3ConfigurationOutputTypeDef",
     "DataModelS3ConfigurationTypeDef",
+    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
+    "DataSourceS3ConfigurationOutputTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
+    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
+    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
+    "ReportS3ConfigurationOutputTypeDef",
     "ReportS3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
+    "RetentionPropertiesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
+    "CreateBatchLoadTaskResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
+    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MagneticStoreRejectedDataLocationOutputTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
+    "ReportConfigurationOutputTypeDef",
     "ReportConfigurationTypeDef",
+    "MagneticStoreWritePropertiesOutputTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
+    "DataModelOutputTypeDef",
     "DataModelTypeDef",
-    "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
+    "CreateTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
+    "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
@@ -125,19 +143,22 @@
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
     },
     total=False,
 )
 
-CreateBatchLoadTaskResponseTypeDef = TypedDict(
-    "CreateBatchLoadTaskResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "TaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -162,65 +183,112 @@
     "RetentionPropertiesTypeDef",
     {
         "MemoryStoreRetentionPeriodInHours": int,
         "MagneticStoreRetentionPeriodInDays": int,
     },
 )
 
+CsvConfigurationOutputTypeDef = TypedDict(
+    "CsvConfigurationOutputTypeDef",
+    {
+        "ColumnSeparator": str,
+        "EscapeChar": str,
+        "QuoteChar": str,
+        "NullValue": str,
+        "TrimWhiteSpace": bool,
+    },
+    total=False,
+)
+
 CsvConfigurationTypeDef = TypedDict(
     "CsvConfigurationTypeDef",
     {
         "ColumnSeparator": str,
         "EscapeChar": str,
         "QuoteChar": str,
         "NullValue": str,
         "TrimWhiteSpace": bool,
     },
     total=False,
 )
 
+DataModelS3ConfigurationOutputTypeDef = TypedDict(
+    "DataModelS3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKey": str,
+    },
+    total=False,
+)
+
 DataModelS3ConfigurationTypeDef = TypedDict(
     "DataModelS3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
+DimensionMappingOutputTypeDef = TypedDict(
+    "DimensionMappingOutputTypeDef",
+    {
+        "SourceColumn": str,
+        "DestinationColumn": str,
+    },
+    total=False,
+)
+
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "SourceColumn": str,
         "DestinationColumn": str,
     },
     total=False,
 )
 
+_RequiredDataSourceS3ConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDataSourceS3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+    },
+)
+_OptionalDataSourceS3ConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDataSourceS3ConfigurationOutputTypeDef",
+    {
+        "ObjectKeyPrefix": str,
+    },
+    total=False,
+)
+
+class DataSourceS3ConfigurationOutputTypeDef(
+    _RequiredDataSourceS3ConfigurationOutputTypeDef, _OptionalDataSourceS3ConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredDataSourceS3ConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalDataSourceS3ConfigurationTypeDef = TypedDict(
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
-
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
-
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -273,26 +341,17 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
-
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -321,14 +380,33 @@
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
+S3ConfigurationOutputTypeDef = TypedDict(
+    "S3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKeyPrefix": str,
+        "EncryptionOption": S3EncryptionOptionType,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
 S3ConfigurationTypeDef = TypedDict(
     "S3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
@@ -341,14 +419,35 @@
     {
         "Name": str,
         "Value": str,
         "Type": MeasureValueTypeType,
     },
 )
 
+_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
+    {
+        "SourceColumn": str,
+    },
+)
+_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
+    {
+        "TargetMultiMeasureAttributeName": str,
+        "MeasureValueType": ScalarMeasureValueTypeType,
+    },
+    total=False,
+)
+
+class MultiMeasureAttributeMappingOutputTypeDef(
+    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
+    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
+):
+    pass
+
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
     },
 )
 _OptionalMultiMeasureAttributeMappingTypeDef = TypedDict(
@@ -356,20 +455,38 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
-
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
+_RequiredPartitionKeyOutputTypeDef = TypedDict(
+    "_RequiredPartitionKeyOutputTypeDef",
+    {
+        "Type": PartitionKeyTypeType,
+    },
+)
+_OptionalPartitionKeyOutputTypeDef = TypedDict(
+    "_OptionalPartitionKeyOutputTypeDef",
+    {
+        "Name": str,
+        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
+    },
+    total=False,
+)
+
+class PartitionKeyOutputTypeDef(
+    _RequiredPartitionKeyOutputTypeDef, _OptionalPartitionKeyOutputTypeDef
+):
+    pass
 
 _RequiredPartitionKeyTypeDef = TypedDict(
     "_RequiredPartitionKeyTypeDef",
     {
         "Type": PartitionKeyTypeType,
     },
 )
@@ -378,29 +495,48 @@
     {
         "Name": str,
         "EnforcementInRecord": PartitionKeyEnforcementLevelType,
     },
     total=False,
 )
 
-
 class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
     pass
 
-
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
     total=False,
 )
 
+_RequiredReportS3ConfigurationOutputTypeDef = TypedDict(
+    "_RequiredReportS3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+    },
+)
+_OptionalReportS3ConfigurationOutputTypeDef = TypedDict(
+    "_OptionalReportS3ConfigurationOutputTypeDef",
+    {
+        "ObjectKeyPrefix": str,
+        "EncryptionOption": S3EncryptionOptionType,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class ReportS3ConfigurationOutputTypeDef(
+    _RequiredReportS3ConfigurationOutputTypeDef, _OptionalReportS3ConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredReportS3ConfigurationTypeDef = TypedDict(
     "_RequiredReportS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalReportS3ConfigurationTypeDef = TypedDict(
@@ -409,36 +545,31 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
+    "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "TaskId": str,
     },
 )
 
-ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
-    "ResumeBatchLoadTaskRequestRequestTypeDef",
+RetentionPropertiesOutputTypeDef = TypedDict(
+    "RetentionPropertiesOutputTypeDef",
     {
-        "TaskId": str,
+        "MemoryStoreRetentionPeriodInHours": int,
+        "MagneticStoreRetentionPeriodInDays": int,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -450,20 +581,35 @@
     "UpdateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "KmsKeyId": str,
     },
 )
 
+CreateBatchLoadTaskResponseTypeDef = TypedDict(
+    "CreateBatchLoadTaskResponseTypeDef",
+    {
+        "TaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListBatchLoadTasksResponseTypeDef = TypedDict(
     "ListBatchLoadTasksResponseTypeDef",
     {
         "NextToken": str,
         "BatchLoadTasks": List[BatchLoadTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -474,70 +620,80 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
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
 
 CreateDatabaseResponseTypeDef = TypedDict(
     "CreateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatabaseResponseTypeDef = TypedDict(
     "DescribeDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesResponseTypeDef = TypedDict(
     "ListDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDatabaseResponseTypeDef = TypedDict(
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDataSourceConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigurationOutputTypeDef",
+    {
+        "DataSourceS3Configuration": DataSourceS3ConfigurationOutputTypeDef,
+        "DataFormat": Literal["CSV"],
+    },
+)
+_OptionalDataSourceConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigurationOutputTypeDef",
+    {
+        "CsvConfiguration": CsvConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+class DataSourceConfigurationOutputTypeDef(
+    _RequiredDataSourceConfigurationOutputTypeDef, _OptionalDataSourceConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
         "DataFormat": Literal["CSV"],
     },
 )
@@ -545,29 +701,43 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
-
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MagneticStoreRejectedDataLocationOutputTypeDef = TypedDict(
+    "MagneticStoreRejectedDataLocationOutputTypeDef",
+    {
+        "S3Configuration": S3ConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
@@ -583,14 +753,55 @@
         "TimeUnit": TimeUnitType,
         "Version": int,
         "MeasureValues": Sequence[MeasureValueTypeDef],
     },
     total=False,
 )
 
+_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_RequiredMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+    },
+)
+_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_OptionalMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureName": str,
+        "SourceColumn": str,
+        "TargetMeasureName": str,
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+class MixedMeasureMappingOutputTypeDef(
+    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
+):
+    pass
+
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -600,87 +811,117 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
-
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
+    {
+        "CompositePartitionKey": List[PartitionKeyOutputTypeDef],
+    },
+    total=False,
+)
 
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
     },
     total=False,
 )
 
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReportConfigurationOutputTypeDef = TypedDict(
+    "ReportConfigurationOutputTypeDef",
+    {
+        "ReportS3Configuration": ReportS3ConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
+    "_RequiredMagneticStoreWritePropertiesOutputTypeDef",
+    {
+        "EnableMagneticStoreWrites": bool,
+    },
+)
+_OptionalMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
+    "_OptionalMagneticStoreWritePropertiesOutputTypeDef",
+    {
+        "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationOutputTypeDef,
+    },
+    total=False,
+)
+
+class MagneticStoreWritePropertiesOutputTypeDef(
+    _RequiredMagneticStoreWritePropertiesOutputTypeDef,
+    _OptionalMagneticStoreWritePropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_RequiredMagneticStoreWritePropertiesTypeDef",
     {
         "EnableMagneticStoreWrites": bool,
     },
 )
 _OptionalMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
-
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
-
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -689,20 +930,39 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
-
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
+_RequiredDataModelOutputTypeDef = TypedDict(
+    "_RequiredDataModelOutputTypeDef",
+    {
+        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+    },
+)
+_OptionalDataModelOutputTypeDef = TypedDict(
+    "_OptionalDataModelOutputTypeDef",
+    {
+        "TimeColumn": str,
+        "TimeUnit": TimeUnitType,
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
+    pass
 
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
@@ -714,18 +974,32 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
+TableTypeDef = TypedDict(
+    "TableTypeDef",
+    {
+        "Arn": str,
+        "TableName": str,
+        "DatabaseName": str,
+        "TableStatus": TableStatusType,
+        "RetentionProperties": RetentionPropertiesOutputTypeDef,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+    total=False,
+)
 
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
@@ -737,37 +1011,19 @@
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
-
-TableTypeDef = TypedDict(
-    "TableTypeDef",
-    {
-        "Arn": str,
-        "TableName": str,
-        "DatabaseName": str,
-        "TableStatus": TableStatusType,
-        "RetentionProperties": RetentionPropertiesTypeDef,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -777,72 +1033,79 @@
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+DataModelConfigurationOutputTypeDef = TypedDict(
+    "DataModelConfigurationOutputTypeDef",
+    {
+        "DataModel": DataModelOutputTypeDef,
+        "DataModelS3Configuration": DataModelS3ConfigurationOutputTypeDef,
+    },
+    total=False,
+)
 
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
 )
 
 CreateTableResponseTypeDef = TypedDict(
     "CreateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "Tables": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableResponseTypeDef = TypedDict(
     "UpdateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
-        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
+        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
-        "ReportConfiguration": ReportConfigurationTypeDef,
-        "DataModelConfiguration": DataModelConfigurationTypeDef,
+        "ReportConfiguration": ReportConfigurationOutputTypeDef,
+        "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
@@ -865,22 +1128,20 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
-
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write/type_defs.pyi` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,70 +31,90 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
-    "CreateBatchLoadTaskResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
+    "CsvConfigurationOutputTypeDef",
     "CsvConfigurationTypeDef",
+    "DataModelS3ConfigurationOutputTypeDef",
     "DataModelS3ConfigurationTypeDef",
+    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
+    "DataSourceS3ConfigurationOutputTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
+    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
+    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
+    "ReportS3ConfigurationOutputTypeDef",
     "ReportS3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
+    "RetentionPropertiesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
+    "CreateBatchLoadTaskResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
+    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MagneticStoreRejectedDataLocationOutputTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
+    "ReportConfigurationOutputTypeDef",
     "ReportConfigurationTypeDef",
+    "MagneticStoreWritePropertiesOutputTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
+    "DataModelOutputTypeDef",
     "DataModelTypeDef",
-    "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
+    "CreateTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
+    "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
@@ -124,19 +144,22 @@
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
     },
     total=False,
 )
 
-CreateBatchLoadTaskResponseTypeDef = TypedDict(
-    "CreateBatchLoadTaskResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "TaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -161,63 +184,116 @@
     "RetentionPropertiesTypeDef",
     {
         "MemoryStoreRetentionPeriodInHours": int,
         "MagneticStoreRetentionPeriodInDays": int,
     },
 )
 
+CsvConfigurationOutputTypeDef = TypedDict(
+    "CsvConfigurationOutputTypeDef",
+    {
+        "ColumnSeparator": str,
+        "EscapeChar": str,
+        "QuoteChar": str,
+        "NullValue": str,
+        "TrimWhiteSpace": bool,
+    },
+    total=False,
+)
+
 CsvConfigurationTypeDef = TypedDict(
     "CsvConfigurationTypeDef",
     {
         "ColumnSeparator": str,
         "EscapeChar": str,
         "QuoteChar": str,
         "NullValue": str,
         "TrimWhiteSpace": bool,
     },
     total=False,
 )
 
+DataModelS3ConfigurationOutputTypeDef = TypedDict(
+    "DataModelS3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKey": str,
+    },
+    total=False,
+)
+
 DataModelS3ConfigurationTypeDef = TypedDict(
     "DataModelS3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
+DimensionMappingOutputTypeDef = TypedDict(
+    "DimensionMappingOutputTypeDef",
+    {
+        "SourceColumn": str,
+        "DestinationColumn": str,
+    },
+    total=False,
+)
+
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "SourceColumn": str,
         "DestinationColumn": str,
     },
     total=False,
 )
 
+_RequiredDataSourceS3ConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDataSourceS3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+    },
+)
+_OptionalDataSourceS3ConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDataSourceS3ConfigurationOutputTypeDef",
+    {
+        "ObjectKeyPrefix": str,
+    },
+    total=False,
+)
+
+
+class DataSourceS3ConfigurationOutputTypeDef(
+    _RequiredDataSourceS3ConfigurationOutputTypeDef, _OptionalDataSourceS3ConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredDataSourceS3ConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalDataSourceS3ConfigurationTypeDef = TypedDict(
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
+
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
+
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -270,23 +346,18 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
+
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
@@ -316,14 +387,33 @@
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
+S3ConfigurationOutputTypeDef = TypedDict(
+    "S3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKeyPrefix": str,
+        "EncryptionOption": S3EncryptionOptionType,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
 S3ConfigurationTypeDef = TypedDict(
     "S3ConfigurationTypeDef",
     {
         "BucketName": str,
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
@@ -336,14 +426,37 @@
     {
         "Name": str,
         "Value": str,
         "Type": MeasureValueTypeType,
     },
 )
 
+_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
+    {
+        "SourceColumn": str,
+    },
+)
+_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
+    {
+        "TargetMultiMeasureAttributeName": str,
+        "MeasureValueType": ScalarMeasureValueTypeType,
+    },
+    total=False,
+)
+
+
+class MultiMeasureAttributeMappingOutputTypeDef(
+    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
+    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
+):
+    pass
+
+
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
     },
 )
 _OptionalMultiMeasureAttributeMappingTypeDef = TypedDict(
@@ -351,19 +464,43 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
+
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
+
+_RequiredPartitionKeyOutputTypeDef = TypedDict(
+    "_RequiredPartitionKeyOutputTypeDef",
+    {
+        "Type": PartitionKeyTypeType,
+    },
+)
+_OptionalPartitionKeyOutputTypeDef = TypedDict(
+    "_OptionalPartitionKeyOutputTypeDef",
+    {
+        "Name": str,
+        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
+    },
+    total=False,
+)
+
+
+class PartitionKeyOutputTypeDef(
+    _RequiredPartitionKeyOutputTypeDef, _OptionalPartitionKeyOutputTypeDef
+):
+    pass
+
+
 _RequiredPartitionKeyTypeDef = TypedDict(
     "_RequiredPartitionKeyTypeDef",
     {
         "Type": PartitionKeyTypeType,
     },
 )
 _OptionalPartitionKeyTypeDef = TypedDict(
@@ -371,27 +508,52 @@
     {
         "Name": str,
         "EnforcementInRecord": PartitionKeyEnforcementLevelType,
     },
     total=False,
 )
 
+
 class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
     pass
 
+
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
     total=False,
 )
 
+_RequiredReportS3ConfigurationOutputTypeDef = TypedDict(
+    "_RequiredReportS3ConfigurationOutputTypeDef",
+    {
+        "BucketName": str,
+    },
+)
+_OptionalReportS3ConfigurationOutputTypeDef = TypedDict(
+    "_OptionalReportS3ConfigurationOutputTypeDef",
+    {
+        "ObjectKeyPrefix": str,
+        "EncryptionOption": S3EncryptionOptionType,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class ReportS3ConfigurationOutputTypeDef(
+    _RequiredReportS3ConfigurationOutputTypeDef, _OptionalReportS3ConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredReportS3ConfigurationTypeDef = TypedDict(
     "_RequiredReportS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalReportS3ConfigurationTypeDef = TypedDict(
@@ -400,37 +562,36 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
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
 
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
+RetentionPropertiesOutputTypeDef = TypedDict(
+    "RetentionPropertiesOutputTypeDef",
+    {
+        "MemoryStoreRetentionPeriodInHours": int,
+        "MagneticStoreRetentionPeriodInDays": int,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -439,20 +600,35 @@
     "UpdateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "KmsKeyId": str,
     },
 )
 
+CreateBatchLoadTaskResponseTypeDef = TypedDict(
+    "CreateBatchLoadTaskResponseTypeDef",
+    {
+        "TaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListBatchLoadTasksResponseTypeDef = TypedDict(
     "ListBatchLoadTasksResponseTypeDef",
     {
         "NextToken": str,
         "BatchLoadTasks": List[BatchLoadTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -463,68 +639,84 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateDatabaseResponseTypeDef = TypedDict(
     "CreateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatabaseResponseTypeDef = TypedDict(
     "DescribeDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesResponseTypeDef = TypedDict(
     "ListDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDatabaseResponseTypeDef = TypedDict(
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDataSourceConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigurationOutputTypeDef",
+    {
+        "DataSourceS3Configuration": DataSourceS3ConfigurationOutputTypeDef,
+        "DataFormat": Literal["CSV"],
+    },
+)
+_OptionalDataSourceConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigurationOutputTypeDef",
+    {
+        "CsvConfiguration": CsvConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+
+class DataSourceConfigurationOutputTypeDef(
+    _RequiredDataSourceConfigurationOutputTypeDef, _OptionalDataSourceConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
         "DataFormat": Literal["CSV"],
     },
 )
@@ -532,25 +724,43 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MagneticStoreRejectedDataLocationOutputTypeDef = TypedDict(
+    "MagneticStoreRejectedDataLocationOutputTypeDef",
+    {
+        "S3Configuration": S3ConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
@@ -568,14 +778,59 @@
         "TimeUnit": TimeUnitType,
         "Version": int,
         "MeasureValues": Sequence[MeasureValueTypeDef],
     },
     total=False,
 )
 
+_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_RequiredMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+    },
+)
+_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_OptionalMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureName": str,
+        "SourceColumn": str,
+        "TargetMeasureName": str,
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class MixedMeasureMappingOutputTypeDef(
+    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
+):
+    pass
+
+
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
+
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -585,81 +840,125 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
+    {
+        "CompositePartitionKey": List[PartitionKeyOutputTypeDef],
+    },
+    total=False,
+)
+
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
     },
     total=False,
 )
 
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReportConfigurationOutputTypeDef = TypedDict(
+    "ReportConfigurationOutputTypeDef",
+    {
+        "ReportS3Configuration": ReportS3ConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
+    "_RequiredMagneticStoreWritePropertiesOutputTypeDef",
+    {
+        "EnableMagneticStoreWrites": bool,
+    },
+)
+_OptionalMagneticStoreWritePropertiesOutputTypeDef = TypedDict(
+    "_OptionalMagneticStoreWritePropertiesOutputTypeDef",
+    {
+        "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class MagneticStoreWritePropertiesOutputTypeDef(
+    _RequiredMagneticStoreWritePropertiesOutputTypeDef,
+    _OptionalMagneticStoreWritePropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_RequiredMagneticStoreWritePropertiesTypeDef",
     {
         "EnableMagneticStoreWrites": bool,
     },
 )
 _OptionalMagneticStoreWritePropertiesTypeDef = TypedDict(
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
+
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
+
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -668,19 +967,44 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
+
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredDataModelOutputTypeDef = TypedDict(
+    "_RequiredDataModelOutputTypeDef",
+    {
+        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+    },
+)
+_OptionalDataModelOutputTypeDef = TypedDict(
+    "_OptionalDataModelOutputTypeDef",
+    {
+        "TimeColumn": str,
+        "TimeUnit": TimeUnitType,
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+
+class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
+    pass
+
+
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -691,17 +1015,35 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
+
+TableTypeDef = TypedDict(
+    "TableTypeDef",
+    {
+        "Arn": str,
+        "TableName": str,
+        "DatabaseName": str,
+        "TableStatus": TableStatusType,
+        "RetentionProperties": RetentionPropertiesOutputTypeDef,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesOutputTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -712,34 +1054,20 @@
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
-TableTypeDef = TypedDict(
-    "TableTypeDef",
-    {
-        "Arn": str,
-        "TableName": str,
-        "DatabaseName": str,
-        "TableStatus": TableStatusType,
-        "RetentionProperties": RetentionPropertiesTypeDef,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
-    },
-    total=False,
-)
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
@@ -750,70 +1078,81 @@
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+
+DataModelConfigurationOutputTypeDef = TypedDict(
+    "DataModelConfigurationOutputTypeDef",
+    {
+        "DataModel": DataModelOutputTypeDef,
+        "DataModelS3Configuration": DataModelS3ConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
 )
 
 CreateTableResponseTypeDef = TypedDict(
     "CreateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "Tables": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableResponseTypeDef = TypedDict(
     "UpdateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
-        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
+        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
-        "ReportConfiguration": ReportConfigurationTypeDef,
-        "DataModelConfiguration": DataModelConfigurationTypeDef,
+        "ReportConfiguration": ReportConfigurationOutputTypeDef,
+        "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
@@ -836,20 +1175,22 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
+
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/PKG-INFO` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.0
-Summary: Type annotations for boto3.TimestreamWrite 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.TimestreamWrite 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-write)](https://pepy.tech/project/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,67 +309,86 @@
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
+    CsvConfigurationOutputTypeDef,
     CsvConfigurationTypeDef,
+    DataModelS3ConfigurationOutputTypeDef,
     DataModelS3ConfigurationTypeDef,
+    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
+    DataSourceS3ConfigurationOutputTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
+    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
+    ReportS3ConfigurationOutputTypeDef,
     ReportS3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
+    RetentionPropertiesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MagneticStoreRejectedDataLocationOutputTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
+    MixedMeasureMappingOutputTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
+    ReportConfigurationOutputTypeDef,
     ReportConfigurationTypeDef,
+    MagneticStoreWritePropertiesOutputTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
+    DataModelOutputTypeDef,
     DataModelTypeDef,
-    CreateTableRequestRequestTypeDef,
     TableTypeDef,
+    CreateTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
```

### Comparing `mypy-boto3-timestream-write-1.28.0/mypy_boto3_timestream_write.egg-info/SOURCES.txt` & `mypy-boto3-timestream-write-1.28.12/mypy_boto3_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.0/setup.py` & `mypy-boto3-timestream-write-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-write",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamWrite 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.TimestreamWrite 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

