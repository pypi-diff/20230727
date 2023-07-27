# Comparing `tmp/mypy-boto3-kinesisanalytics-1.28.0.tar.gz` & `tmp/mypy-boto3-kinesisanalytics-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisanalytics-1.28.0.tar", last modified: Thu Jul  6 20:59:55 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisanalytics-1.28.12.tar", last modified: Thu Jul 27 05:34:54 2023, max compression
```

## Comparing `mypy-boto3-kinesisanalytics-1.28.0.tar` & `mypy-boto3-kinesisanalytics-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.518345 mypy-boto3-kinesisanalytics-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-07-06 20:59:55.510346 mypy-boto3-kinesisanalytics-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.506345 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-06 20:44:50.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-06 20:44:50.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-07-06 20:44:51.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-07-06 20:44:51.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.510346 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:59:55.000000 mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:55.518345 mypy-boto3-kinesisanalytics-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:44:48.000000 mypy-boto3-kinesisanalytics-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.012466 mypy-boto3-kinesisanalytics-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-07-27 05:34:54.004466 mypy-boto3-kinesisanalytics-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.996466 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29122 2023-07-27 05:24:44.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.004466 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:53.000000 mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:54.012466 mypy-boto3-kinesisanalytics-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:24:43.000000 mypy-boto3-kinesisanalytics-1.28.12/setup.py
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/LICENSE` & `mypy-boto3-kinesisanalytics-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/PKG-INFO` & `mypy-boto3-kinesisanalytics-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalytics
-Version: 1.28.0
-Summary: Type annotations for boto3.KinesisAnalytics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KinesisAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kinesisanalytics"></a>
 
 # mypy-boto3-kinesisanalytics
 
 [![PyPI - mypy-boto3-kinesisanalytics](https://img.shields.io/pypi/v/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,85 +304,95 @@
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
+    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
+    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
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
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
     ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
+    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
+    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
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
+    ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ApplicationDetailTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/README.md` & `mypy-boto3-kinesisanalytics-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kinesisanalytics"></a>
 
 # mypy-boto3-kinesisanalytics
 
 [![PyPI - mypy-boto3-kinesisanalytics](https://img.shields.io/pypi/v/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,85 +272,95 @@
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
+    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
+    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
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
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
     ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
+    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
+    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
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
+    ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ApplicationDetailTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/__main__.py` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisAnalytics 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.KinesisAnalytics 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics\nOther"
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

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/client.py` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/client.pyi` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/literals.py` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
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
@@ -235,26 +236,28 @@
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

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/literals.pyi` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
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
@@ -233,26 +234,28 @@
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

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/type_defs.py` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,85 +24,95 @@
 
 
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ApplicationSummaryTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
+    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
+    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
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
     "LambdaOutputDescriptionTypeDef",
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
     "ResponseMetadataTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
+    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
+    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
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
+    "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ApplicationDetailTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "ApplicationUpdateTypeDef",
     "DescribeApplicationResponseTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
 )
 
 CloudWatchLoggingOptionTypeDef = TypedDict(
@@ -163,14 +173,22 @@
 
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
 
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
@@ -241,14 +259,21 @@
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
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
 
@@ -265,22 +290,30 @@
     {
         "RoleARN": str,
         "BucketARN": str,
         "FileKey": str,
     },
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
 KinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "KinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
     total=False,
@@ -317,14 +350,22 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
     total=False,
 )
@@ -379,14 +420,21 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
 
@@ -480,14 +528,55 @@
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
 S3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "S3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
         "ReferenceRoleARN": str,
     },
@@ -560,22 +649,14 @@
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "HasMoreApplications": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
@@ -606,14 +687,23 @@
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
@@ -623,15 +713,15 @@
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
@@ -673,14 +763,22 @@
 )
 
 
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "InputConfigurations": Sequence[InputConfigurationTypeDef],
     },
 )
@@ -703,14 +801,35 @@
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
         "S3Configuration": S3ConfigurationTypeDef,
         "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
     },
     total=False,
 )
 
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
@@ -731,14 +850,36 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Output": OutputTypeDef,
     },
 )
 
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
@@ -761,42 +902,18 @@
 )
 
 
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
 
@@ -805,64 +922,88 @@
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
     },
     total=False,
 )
 
-_RequiredInputTypeDef = TypedDict(
-    "_RequiredInputTypeDef",
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
-        "NamePrefix": str,
-        "InputSchema": SourceSchemaTypeDef,
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
     },
 )
-_OptionalInputTypeDef = TypedDict(
-    "_OptionalInputTypeDef",
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
-        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
-        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
-        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
+        "ReferenceSchema": SourceSchemaOutputTypeDef,
     },
     total=False,
 )
 
 
-class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
     pass
 
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
+_RequiredInputUpdateTypeDef = TypedDict(
+    "_RequiredInputUpdateTypeDef",
     {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+        "InputId": str,
     },
 )
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
+_OptionalInputUpdateTypeDef = TypedDict(
+    "_OptionalInputUpdateTypeDef",
     {
-        "ReferenceSchema": SourceSchemaTypeDef,
+        "NamePrefixUpdate": str,
+        "InputProcessingConfigurationUpdate": InputProcessingConfigurationUpdateTypeDef,
+        "KinesisStreamsInputUpdate": KinesisStreamsInputUpdateTypeDef,
+        "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
+        "InputSchemaUpdate": InputSchemaUpdateTypeDef,
+        "InputParallelismUpdate": InputParallelismUpdateTypeDef,
     },
     total=False,
 )
 
 
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
+class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
+    pass
+
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
+
+class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
@@ -903,14 +1044,45 @@
 
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
 
+_RequiredApplicationDetailTypeDef = TypedDict(
+    "_RequiredApplicationDetailTypeDef",
+    {
+        "ApplicationName": str,
+        "ApplicationARN": str,
+        "ApplicationStatus": ApplicationStatusType,
+        "ApplicationVersionId": int,
+    },
+)
+_OptionalApplicationDetailTypeDef = TypedDict(
+    "_OptionalApplicationDetailTypeDef",
+    {
+        "ApplicationDescription": str,
+        "CreateTimestamp": datetime,
+        "LastUpdateTimestamp": datetime,
+        "InputDescriptions": List[InputDescriptionTypeDef],
+        "OutputDescriptions": List[OutputDescriptionTypeDef],
+        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
+        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
+        "ApplicationCode": str,
+    },
+    total=False,
+)
+
+
+class ApplicationDetailTypeDef(
+    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
+):
+    pass
+
+
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
     },
@@ -938,45 +1110,14 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredApplicationDetailTypeDef = TypedDict(
-    "_RequiredApplicationDetailTypeDef",
-    {
-        "ApplicationName": str,
-        "ApplicationARN": str,
-        "ApplicationStatus": ApplicationStatusType,
-        "ApplicationVersionId": int,
-    },
-)
-_OptionalApplicationDetailTypeDef = TypedDict(
-    "_OptionalApplicationDetailTypeDef",
-    {
-        "ApplicationDescription": str,
-        "CreateTimestamp": datetime,
-        "LastUpdateTimestamp": datetime,
-        "InputDescriptions": List[InputDescriptionTypeDef],
-        "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ApplicationCode": str,
-    },
-    total=False,
-)
-
-
-class ApplicationDetailTypeDef(
-    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
-):
-    pass
-
-
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics/type_defs.pyi` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -23,85 +23,95 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ApplicationSummaryTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
+    "CSVMappingParametersOutputTypeDef",
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
+    "DestinationSchemaOutputTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
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
     "LambdaOutputDescriptionTypeDef",
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "RecordColumnOutputTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
     "ResponseMetadataTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
+    "MappingParametersOutputTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
+    "RecordFormatOutputTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
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
+    "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ApplicationDetailTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "ApplicationUpdateTypeDef",
     "DescribeApplicationResponseTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
 )
 
 CloudWatchLoggingOptionTypeDef = TypedDict(
@@ -158,14 +168,22 @@
 )
 
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
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
@@ -234,14 +252,21 @@
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
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
 
@@ -258,22 +283,30 @@
     {
         "RoleARN": str,
         "BucketARN": str,
         "FileKey": str,
     },
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
 KinesisFirehoseInputDescriptionTypeDef = TypedDict(
     "KinesisFirehoseInputDescriptionTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
     total=False,
@@ -310,14 +343,22 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
     total=False,
 )
@@ -370,14 +411,21 @@
     {
         "ResourceARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
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
 
@@ -471,14 +519,51 @@
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
 S3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "S3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
         "ReferenceRoleARN": str,
     },
@@ -551,22 +636,14 @@
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "HasMoreApplications": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
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
@@ -597,14 +674,23 @@
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
@@ -614,15 +700,15 @@
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
@@ -660,14 +746,22 @@
     },
     total=False,
 )
 
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "InputConfigurations": Sequence[InputConfigurationTypeDef],
     },
 )
@@ -690,14 +784,33 @@
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
         "S3Configuration": S3ConfigurationTypeDef,
         "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
     },
     total=False,
 )
 
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
+
 _RequiredRecordFormatTypeDef = TypedDict(
     "_RequiredRecordFormatTypeDef",
     {
         "RecordFormatType": RecordFormatTypeType,
     },
 )
 _OptionalRecordFormatTypeDef = TypedDict(
@@ -716,14 +829,34 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Output": OutputTypeDef,
     },
 )
 
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
+
 InputSchemaUpdateTypeDef = TypedDict(
     "InputSchemaUpdateTypeDef",
     {
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
@@ -744,40 +877,18 @@
     },
     total=False,
 )
 
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
 
@@ -786,21 +897,64 @@
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
     },
     total=False,
 )
 
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
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
+    pass
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
+    },
+    total=False,
+)
+
+class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
+    pass
+
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -814,35 +968,14 @@
     },
     total=False,
 )
 
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
-
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
 )
@@ -876,14 +1009,43 @@
 )
 
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
+_RequiredApplicationDetailTypeDef = TypedDict(
+    "_RequiredApplicationDetailTypeDef",
+    {
+        "ApplicationName": str,
+        "ApplicationARN": str,
+        "ApplicationStatus": ApplicationStatusType,
+        "ApplicationVersionId": int,
+    },
+)
+_OptionalApplicationDetailTypeDef = TypedDict(
+    "_OptionalApplicationDetailTypeDef",
+    {
+        "ApplicationDescription": str,
+        "CreateTimestamp": datetime,
+        "LastUpdateTimestamp": datetime,
+        "InputDescriptions": List[InputDescriptionTypeDef],
+        "OutputDescriptions": List[OutputDescriptionTypeDef],
+        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
+        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
+        "ApplicationCode": str,
+    },
+    total=False,
+)
+
+class ApplicationDetailTypeDef(
+    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
+):
+    pass
+
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
     },
@@ -909,43 +1071,14 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-_RequiredApplicationDetailTypeDef = TypedDict(
-    "_RequiredApplicationDetailTypeDef",
-    {
-        "ApplicationName": str,
-        "ApplicationARN": str,
-        "ApplicationStatus": ApplicationStatusType,
-        "ApplicationVersionId": int,
-    },
-)
-_OptionalApplicationDetailTypeDef = TypedDict(
-    "_OptionalApplicationDetailTypeDef",
-    {
-        "ApplicationDescription": str,
-        "CreateTimestamp": datetime,
-        "LastUpdateTimestamp": datetime,
-        "InputDescriptions": List[InputDescriptionTypeDef],
-        "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ApplicationCode": str,
-    },
-    total=False,
-)
-
-class ApplicationDetailTypeDef(
-    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
-):
-    pass
-
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalytics
-Version: 1.28.0
-Summary: Type annotations for boto3.KinesisAnalytics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KinesisAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kinesisanalytics"></a>
 
 # mypy-boto3-kinesisanalytics
 
 [![PyPI - mypy-boto3-kinesisanalytics](https://img.shields.io/pypi/v/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisanalytics?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisanalytics)](https://pepy.tech/project/mypy-boto3-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisAnalytics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[boto3.KinesisAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [mypy-boto3-kinesisanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,85 +304,95 @@
 
 ```python
 from mypy_boto3_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
+    CSVMappingParametersOutputTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
+    DestinationSchemaOutputTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
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
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    RecordColumnOutputTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
     ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
+    MappingParametersOutputTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
+    RecordFormatOutputTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
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
+    ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ApplicationDetailTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt` & `mypy-boto3-kinesisanalytics-1.28.12/mypy_boto3_kinesisanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalytics-1.28.0/setup.py` & `mypy-boto3-kinesisanalytics-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisanalytics",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kinesisanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisAnalytics 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.KinesisAnalytics 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

