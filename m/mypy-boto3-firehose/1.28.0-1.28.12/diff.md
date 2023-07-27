# Comparing `tmp/mypy-boto3-firehose-1.28.0.tar.gz` & `tmp/mypy-boto3-firehose-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-firehose-1.28.0.tar", last modified: Thu Jul  6 20:59:36 2023, max compression
+gzip compressed data, was "mypy-boto3-firehose-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
```

## Comparing `mypy-boto3-firehose-1.28.0.tar` & `mypy-boto3-firehose-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:36.686306 mypy-boto3-firehose-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-06 20:59:36.682306 mypy-boto3-firehose-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:36.670306 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45008 2023-07-06 20:41:06.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44959 2023-07-06 20:41:06.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:36.682306 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:36.686306 mypy-boto3-firehose-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:41:03.000000 mypy-boto3-firehose-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.012509 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-07-27 05:22:19.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54181 2023-07-27 05:22:18.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17545 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:41.000000 mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.016509 mypy-boto3-firehose-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:22:17.000000 mypy-boto3-firehose-1.28.12/setup.py
```

### Comparing `mypy-boto3-firehose-1.28.0/LICENSE` & `mypy-boto3-firehose-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.0/PKG-INFO` & `mypy-boto3-firehose-1.28.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.28.0
-Summary: Type annotations for boto3.Firehose 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Firehose 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,108 +319,141 @@
 ### Typed dictionaries
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
+    AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
+    AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
+    CloudWatchLoggingOptionsOutputTypeDef,
     VpcConfigurationDescriptionTypeDef,
+    AmazonopensearchserviceBufferingHintsOutputTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
+    AmazonopensearchserviceRetryOptionsOutputTypeDef,
+    BufferingHintsOutputTypeDef,
     BufferingHintsTypeDef,
+    CopyCommandOutputTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
     CreateDeliveryStreamOutputTypeDef,
+    SchemaConfigurationOutputTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
+    HiveJsonSerDeOutputTypeDef,
+    OpenXJsonSerDeOutputTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
+    RetryOptionsOutputTypeDef,
     RetryOptionsTypeDef,
+    ElasticsearchBufferingHintsOutputTypeDef,
     ElasticsearchBufferingHintsTypeDef,
     ElasticsearchRetryOptionsTypeDef,
+    ElasticsearchRetryOptionsOutputTypeDef,
+    KMSEncryptionConfigOutputTypeDef,
     KMSEncryptionConfigTypeDef,
+    HttpEndpointBufferingHintsOutputTypeDef,
     HttpEndpointBufferingHintsTypeDef,
+    HttpEndpointCommonAttributeOutputTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
+    HttpEndpointRetryOptionsOutputTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
     ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
+    TagOutputTypeDef,
+    OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
+    ParquetSerDeOutputTypeDef,
     ParquetSerDeTypeDef,
+    ProcessorParameterOutputTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
     PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
+    RedshiftRetryOptionsOutputTypeDef,
     ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
+    SplunkRetryOptionsOutputTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
-    ListTagsForDeliveryStreamOutputTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
+    DeserializerOutputTypeDef,
     DeserializerTypeDef,
+    DynamicPartitioningConfigurationOutputTypeDef,
     DynamicPartitioningConfigurationTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
+    HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
+    ListTagsForDeliveryStreamOutputTypeDef,
+    SerializerOutputTypeDef,
     SerializerTypeDef,
+    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
     PutRecordBatchOutputTypeDef,
+    InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
-    S3DestinationConfigurationTypeDef,
     S3DestinationDescriptionTypeDef,
+    S3DestinationConfigurationTypeDef,
     S3DestinationUpdateTypeDef,
+    OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
+    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
+    DataFormatConversionConfigurationOutputTypeDef,
     DataFormatConversionConfigurationTypeDef,
-    AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     AmazonOpenSearchServerlessDestinationDescriptionTypeDef,
+    AmazonopensearchserviceDestinationDescriptionTypeDef,
+    ElasticsearchDestinationDescriptionTypeDef,
+    HttpEndpointDestinationDescriptionTypeDef,
+    RedshiftDestinationDescriptionTypeDef,
+    SplunkDestinationDescriptionTypeDef,
+    AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     AmazonOpenSearchServerlessDestinationUpdateTypeDef,
     AmazonopensearchserviceDestinationConfigurationTypeDef,
-    AmazonopensearchserviceDestinationDescriptionTypeDef,
     AmazonopensearchserviceDestinationUpdateTypeDef,
     ElasticsearchDestinationConfigurationTypeDef,
-    ElasticsearchDestinationDescriptionTypeDef,
     ElasticsearchDestinationUpdateTypeDef,
     HttpEndpointDestinationConfigurationTypeDef,
-    HttpEndpointDestinationDescriptionTypeDef,
     HttpEndpointDestinationUpdateTypeDef,
     RedshiftDestinationConfigurationTypeDef,
-    RedshiftDestinationDescriptionTypeDef,
     RedshiftDestinationUpdateTypeDef,
     SplunkDestinationConfigurationTypeDef,
-    SplunkDestinationDescriptionTypeDef,
     SplunkDestinationUpdateTypeDef,
-    ExtendedS3DestinationConfigurationTypeDef,
     ExtendedS3DestinationDescriptionTypeDef,
+    ExtendedS3DestinationConfigurationTypeDef,
     ExtendedS3DestinationUpdateTypeDef,
-    CreateDeliveryStreamInputRequestTypeDef,
     DestinationDescriptionTypeDef,
+    CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
+def get_structure() -> AmazonOpenSearchServerlessBufferingHintsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.0/README.md` & `mypy-boto3-firehose-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,108 +287,141 @@
 ### Typed dictionaries
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
+    AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
+    AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
+    CloudWatchLoggingOptionsOutputTypeDef,
     VpcConfigurationDescriptionTypeDef,
+    AmazonopensearchserviceBufferingHintsOutputTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
+    AmazonopensearchserviceRetryOptionsOutputTypeDef,
+    BufferingHintsOutputTypeDef,
     BufferingHintsTypeDef,
+    CopyCommandOutputTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
     CreateDeliveryStreamOutputTypeDef,
+    SchemaConfigurationOutputTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
+    HiveJsonSerDeOutputTypeDef,
+    OpenXJsonSerDeOutputTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
+    RetryOptionsOutputTypeDef,
     RetryOptionsTypeDef,
+    ElasticsearchBufferingHintsOutputTypeDef,
     ElasticsearchBufferingHintsTypeDef,
     ElasticsearchRetryOptionsTypeDef,
+    ElasticsearchRetryOptionsOutputTypeDef,
+    KMSEncryptionConfigOutputTypeDef,
     KMSEncryptionConfigTypeDef,
+    HttpEndpointBufferingHintsOutputTypeDef,
     HttpEndpointBufferingHintsTypeDef,
+    HttpEndpointCommonAttributeOutputTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
+    HttpEndpointRetryOptionsOutputTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
     ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
+    TagOutputTypeDef,
+    OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
+    ParquetSerDeOutputTypeDef,
     ParquetSerDeTypeDef,
+    ProcessorParameterOutputTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
     PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
+    RedshiftRetryOptionsOutputTypeDef,
     ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
+    SplunkRetryOptionsOutputTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
-    ListTagsForDeliveryStreamOutputTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
+    DeserializerOutputTypeDef,
     DeserializerTypeDef,
+    DynamicPartitioningConfigurationOutputTypeDef,
     DynamicPartitioningConfigurationTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
+    HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
+    ListTagsForDeliveryStreamOutputTypeDef,
+    SerializerOutputTypeDef,
     SerializerTypeDef,
+    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
     PutRecordBatchOutputTypeDef,
+    InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
-    S3DestinationConfigurationTypeDef,
     S3DestinationDescriptionTypeDef,
+    S3DestinationConfigurationTypeDef,
     S3DestinationUpdateTypeDef,
+    OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
+    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
+    DataFormatConversionConfigurationOutputTypeDef,
     DataFormatConversionConfigurationTypeDef,
-    AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     AmazonOpenSearchServerlessDestinationDescriptionTypeDef,
+    AmazonopensearchserviceDestinationDescriptionTypeDef,
+    ElasticsearchDestinationDescriptionTypeDef,
+    HttpEndpointDestinationDescriptionTypeDef,
+    RedshiftDestinationDescriptionTypeDef,
+    SplunkDestinationDescriptionTypeDef,
+    AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     AmazonOpenSearchServerlessDestinationUpdateTypeDef,
     AmazonopensearchserviceDestinationConfigurationTypeDef,
-    AmazonopensearchserviceDestinationDescriptionTypeDef,
     AmazonopensearchserviceDestinationUpdateTypeDef,
     ElasticsearchDestinationConfigurationTypeDef,
-    ElasticsearchDestinationDescriptionTypeDef,
     ElasticsearchDestinationUpdateTypeDef,
     HttpEndpointDestinationConfigurationTypeDef,
-    HttpEndpointDestinationDescriptionTypeDef,
     HttpEndpointDestinationUpdateTypeDef,
     RedshiftDestinationConfigurationTypeDef,
-    RedshiftDestinationDescriptionTypeDef,
     RedshiftDestinationUpdateTypeDef,
     SplunkDestinationConfigurationTypeDef,
-    SplunkDestinationDescriptionTypeDef,
     SplunkDestinationUpdateTypeDef,
-    ExtendedS3DestinationConfigurationTypeDef,
     ExtendedS3DestinationDescriptionTypeDef,
+    ExtendedS3DestinationConfigurationTypeDef,
     ExtendedS3DestinationUpdateTypeDef,
-    CreateDeliveryStreamInputRequestTypeDef,
     DestinationDescriptionTypeDef,
+    CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
+def get_structure() -> AmazonOpenSearchServerlessBufferingHintsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__main__.py` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Firehose 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Firehose 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose\nOther"
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

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.py` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.pyi` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.py` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,15 @@
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
@@ -313,26 +314,28 @@
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

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.pyi` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,15 @@
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
@@ -311,26 +312,28 @@
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

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.py` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for firehose service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsTypeDef
+    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsOutputTypeDef
 
-    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = {...}
+    data: AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -50,106 +50,148 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     "AmazonOpenSearchServerlessRetryOptionsTypeDef",
     "CloudWatchLoggingOptionsTypeDef",
     "VpcConfigurationTypeDef",
+    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
+    "CloudWatchLoggingOptionsOutputTypeDef",
     "VpcConfigurationDescriptionTypeDef",
+    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
+    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
+    "BufferingHintsOutputTypeDef",
     "BufferingHintsTypeDef",
+    "CopyCommandOutputTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDeliveryStreamOutputTypeDef",
+    "SchemaConfigurationOutputTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
+    "HiveJsonSerDeOutputTypeDef",
+    "OpenXJsonSerDeOutputTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
+    "RetryOptionsOutputTypeDef",
     "RetryOptionsTypeDef",
+    "ElasticsearchBufferingHintsOutputTypeDef",
     "ElasticsearchBufferingHintsTypeDef",
     "ElasticsearchRetryOptionsTypeDef",
+    "ElasticsearchRetryOptionsOutputTypeDef",
+    "KMSEncryptionConfigOutputTypeDef",
     "KMSEncryptionConfigTypeDef",
+    "HttpEndpointBufferingHintsOutputTypeDef",
     "HttpEndpointBufferingHintsTypeDef",
+    "HttpEndpointCommonAttributeOutputTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
+    "HttpEndpointRetryOptionsOutputTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
     "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
+    "TagOutputTypeDef",
+    "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
+    "ParquetSerDeOutputTypeDef",
     "ParquetSerDeTypeDef",
+    "ProcessorParameterOutputTypeDef",
     "ProcessorParameterTypeDef",
     "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
     "PutRecordOutputTypeDef",
     "RedshiftRetryOptionsTypeDef",
+    "RedshiftRetryOptionsOutputTypeDef",
     "ResponseMetadataTypeDef",
     "SplunkRetryOptionsTypeDef",
+    "SplunkRetryOptionsOutputTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
-    "ListTagsForDeliveryStreamOutputTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
+    "DeserializerOutputTypeDef",
     "DeserializerTypeDef",
+    "DynamicPartitioningConfigurationOutputTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
+    "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    "SerializerOutputTypeDef",
     "SerializerTypeDef",
+    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
     "PutRecordBatchOutputTypeDef",
+    "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
-    "S3DestinationConfigurationTypeDef",
     "S3DestinationDescriptionTypeDef",
+    "S3DestinationConfigurationTypeDef",
     "S3DestinationUpdateTypeDef",
+    "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
+    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
+    "DataFormatConversionConfigurationOutputTypeDef",
     "DataFormatConversionConfigurationTypeDef",
-    "AmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
+    "ElasticsearchDestinationDescriptionTypeDef",
+    "HttpEndpointDestinationDescriptionTypeDef",
+    "RedshiftDestinationDescriptionTypeDef",
+    "SplunkDestinationDescriptionTypeDef",
+    "AmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     "AmazonopensearchserviceDestinationConfigurationTypeDef",
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     "ElasticsearchDestinationConfigurationTypeDef",
-    "ElasticsearchDestinationDescriptionTypeDef",
     "ElasticsearchDestinationUpdateTypeDef",
     "HttpEndpointDestinationConfigurationTypeDef",
-    "HttpEndpointDestinationDescriptionTypeDef",
     "HttpEndpointDestinationUpdateTypeDef",
     "RedshiftDestinationConfigurationTypeDef",
-    "RedshiftDestinationDescriptionTypeDef",
     "RedshiftDestinationUpdateTypeDef",
     "SplunkDestinationConfigurationTypeDef",
-    "SplunkDestinationDescriptionTypeDef",
     "SplunkDestinationUpdateTypeDef",
-    "ExtendedS3DestinationConfigurationTypeDef",
     "ExtendedS3DestinationDescriptionTypeDef",
+    "ExtendedS3DestinationConfigurationTypeDef",
     "ExtendedS3DestinationUpdateTypeDef",
-    "CreateDeliveryStreamInputRequestTypeDef",
     "DestinationDescriptionTypeDef",
+    "CreateDeliveryStreamInputRequestTypeDef",
     "UpdateDestinationInputRequestTypeDef",
     "DeliveryStreamDescriptionTypeDef",
     "DescribeDeliveryStreamOutputTypeDef",
 )
 
+AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
+    {
+        "IntervalInSeconds": int,
+        "SizeInMBs": int,
+    },
+    total=False,
+)
+
 AmazonOpenSearchServerlessBufferingHintsTypeDef = TypedDict(
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -178,24 +220,51 @@
     {
         "SubnetIds": Sequence[str],
         "RoleARN": str,
         "SecurityGroupIds": Sequence[str],
     },
 )
 
+AmazonOpenSearchServerlessRetryOptionsOutputTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
+CloudWatchLoggingOptionsOutputTypeDef = TypedDict(
+    "CloudWatchLoggingOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "LogGroupName": str,
+        "LogStreamName": str,
+    },
+    total=False,
+)
+
 VpcConfigurationDescriptionTypeDef = TypedDict(
     "VpcConfigurationDescriptionTypeDef",
     {
         "SubnetIds": List[str],
         "RoleARN": str,
         "SecurityGroupIds": List[str],
         "VpcId": str,
     },
 )
 
+AmazonopensearchserviceBufferingHintsOutputTypeDef = TypedDict(
+    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
+    {
+        "IntervalInSeconds": int,
+        "SizeInMBs": int,
+    },
+    total=False,
+)
+
 AmazonopensearchserviceBufferingHintsTypeDef = TypedDict(
     "AmazonopensearchserviceBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -205,23 +274,62 @@
     "AmazonopensearchserviceRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+AmazonopensearchserviceRetryOptionsOutputTypeDef = TypedDict(
+    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
+BufferingHintsOutputTypeDef = TypedDict(
+    "BufferingHintsOutputTypeDef",
+    {
+        "SizeInMBs": int,
+        "IntervalInSeconds": int,
+    },
+    total=False,
+)
+
 BufferingHintsTypeDef = TypedDict(
     "BufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
+_RequiredCopyCommandOutputTypeDef = TypedDict(
+    "_RequiredCopyCommandOutputTypeDef",
+    {
+        "DataTableName": str,
+    },
+)
+_OptionalCopyCommandOutputTypeDef = TypedDict(
+    "_OptionalCopyCommandOutputTypeDef",
+    {
+        "DataTableColumns": str,
+        "CopyOptions": str,
+    },
+    total=False,
+)
+
+
+class CopyCommandOutputTypeDef(
+    _RequiredCopyCommandOutputTypeDef, _OptionalCopyCommandOutputTypeDef
+):
+    pass
+
+
 _RequiredCopyCommandTypeDef = TypedDict(
     "_RequiredCopyCommandTypeDef",
     {
         "DataTableName": str,
     },
 )
 _OptionalCopyCommandTypeDef = TypedDict(
@@ -291,14 +399,27 @@
     "CreateDeliveryStreamOutputTypeDef",
     {
         "DeliveryStreamARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchemaConfigurationOutputTypeDef = TypedDict(
+    "SchemaConfigurationOutputTypeDef",
+    {
+        "RoleARN": str,
+        "CatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Region": str,
+        "VersionId": str,
+    },
+    total=False,
+)
+
 SchemaConfigurationTypeDef = TypedDict(
     "SchemaConfigurationTypeDef",
     {
         "RoleARN": str,
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
@@ -357,14 +478,32 @@
 class DescribeDeliveryStreamInputRequestTypeDef(
     _RequiredDescribeDeliveryStreamInputRequestTypeDef,
     _OptionalDescribeDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
 
+HiveJsonSerDeOutputTypeDef = TypedDict(
+    "HiveJsonSerDeOutputTypeDef",
+    {
+        "TimestampFormats": List[str],
+    },
+    total=False,
+)
+
+OpenXJsonSerDeOutputTypeDef = TypedDict(
+    "OpenXJsonSerDeOutputTypeDef",
+    {
+        "ConvertDotsInJsonKeysToUnderscores": bool,
+        "CaseInsensitive": bool,
+        "ColumnToJsonKeyMappings": Dict[str, str],
+    },
+    total=False,
+)
+
 HiveJsonSerDeTypeDef = TypedDict(
     "HiveJsonSerDeTypeDef",
     {
         "TimestampFormats": Sequence[str],
     },
     total=False,
 )
@@ -375,22 +514,39 @@
         "ConvertDotsInJsonKeysToUnderscores": bool,
         "CaseInsensitive": bool,
         "ColumnToJsonKeyMappings": Mapping[str, str],
     },
     total=False,
 )
 
+RetryOptionsOutputTypeDef = TypedDict(
+    "RetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
 RetryOptionsTypeDef = TypedDict(
     "RetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+ElasticsearchBufferingHintsOutputTypeDef = TypedDict(
+    "ElasticsearchBufferingHintsOutputTypeDef",
+    {
+        "IntervalInSeconds": int,
+        "SizeInMBs": int,
+    },
+    total=False,
+)
+
 ElasticsearchBufferingHintsTypeDef = TypedDict(
     "ElasticsearchBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -400,30 +556,62 @@
     "ElasticsearchRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+ElasticsearchRetryOptionsOutputTypeDef = TypedDict(
+    "ElasticsearchRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
+KMSEncryptionConfigOutputTypeDef = TypedDict(
+    "KMSEncryptionConfigOutputTypeDef",
+    {
+        "AWSKMSKeyARN": str,
+    },
+)
+
 KMSEncryptionConfigTypeDef = TypedDict(
     "KMSEncryptionConfigTypeDef",
     {
         "AWSKMSKeyARN": str,
     },
 )
 
+HttpEndpointBufferingHintsOutputTypeDef = TypedDict(
+    "HttpEndpointBufferingHintsOutputTypeDef",
+    {
+        "SizeInMBs": int,
+        "IntervalInSeconds": int,
+    },
+    total=False,
+)
+
 HttpEndpointBufferingHintsTypeDef = TypedDict(
     "HttpEndpointBufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
+HttpEndpointCommonAttributeOutputTypeDef = TypedDict(
+    "HttpEndpointCommonAttributeOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeValue": str,
+    },
+)
+
 HttpEndpointCommonAttributeTypeDef = TypedDict(
     "HttpEndpointCommonAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
 )
@@ -463,14 +651,22 @@
     "HttpEndpointRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+HttpEndpointRetryOptionsOutputTypeDef = TypedDict(
+    "HttpEndpointRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
 KinesisStreamSourceDescriptionTypeDef = TypedDict(
     "KinesisStreamSourceDescriptionTypeDef",
     {
         "KinesisStreamARN": str,
         "RoleARN": str,
         "DeliveryStartTimestamp": datetime,
     },
@@ -515,14 +711,50 @@
 class ListTagsForDeliveryStreamInputRequestTypeDef(
     _RequiredListTagsForDeliveryStreamInputRequestTypeDef,
     _OptionalListTagsForDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
 
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
+OrcSerDeOutputTypeDef = TypedDict(
+    "OrcSerDeOutputTypeDef",
+    {
+        "StripeSizeBytes": int,
+        "BlockSizeBytes": int,
+        "RowIndexStride": int,
+        "EnablePadding": bool,
+        "PaddingTolerance": float,
+        "Compression": OrcCompressionType,
+        "BloomFilterColumns": List[str],
+        "BloomFilterFalsePositiveProbability": float,
+        "DictionaryKeyThreshold": float,
+        "FormatVersion": OrcFormatVersionType,
+    },
+    total=False,
+)
+
 OrcSerDeTypeDef = TypedDict(
     "OrcSerDeTypeDef",
     {
         "StripeSizeBytes": int,
         "BlockSizeBytes": int,
         "RowIndexStride": int,
         "EnablePadding": bool,
@@ -532,27 +764,48 @@
         "BloomFilterFalsePositiveProbability": float,
         "DictionaryKeyThreshold": float,
         "FormatVersion": OrcFormatVersionType,
     },
     total=False,
 )
 
+ParquetSerDeOutputTypeDef = TypedDict(
+    "ParquetSerDeOutputTypeDef",
+    {
+        "BlockSizeBytes": int,
+        "PageSizeBytes": int,
+        "Compression": ParquetCompressionType,
+        "EnableDictionaryCompression": bool,
+        "MaxPaddingBytes": int,
+        "WriterVersion": ParquetWriterVersionType,
+    },
+    total=False,
+)
+
 ParquetSerDeTypeDef = TypedDict(
     "ParquetSerDeTypeDef",
     {
         "BlockSizeBytes": int,
         "PageSizeBytes": int,
         "Compression": ParquetCompressionType,
         "EnableDictionaryCompression": bool,
         "MaxPaddingBytes": int,
         "WriterVersion": ParquetWriterVersionType,
     },
     total=False,
 )
 
+ProcessorParameterOutputTypeDef = TypedDict(
+    "ProcessorParameterOutputTypeDef",
+    {
+        "ParameterName": ProcessorParameterNameType,
+        "ParameterValue": str,
+    },
+)
+
 ProcessorParameterTypeDef = TypedDict(
     "ProcessorParameterTypeDef",
     {
         "ParameterName": ProcessorParameterNameType,
         "ParameterValue": str,
     },
 )
@@ -587,14 +840,22 @@
     "RedshiftRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+RedshiftRetryOptionsOutputTypeDef = TypedDict(
+    "RedshiftRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
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
@@ -606,14 +867,22 @@
     "SplunkRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+SplunkRetryOptionsOutputTypeDef = TypedDict(
+    "SplunkRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
 StopDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 
@@ -645,23 +914,14 @@
 class StartDeliveryStreamEncryptionInputRequestTypeDef(
     _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef,
     _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
 
-ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
-    "ListTagsForDeliveryStreamOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "HasMoreTags": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagDeliveryStreamInputRequestTypeDef = TypedDict(
     "TagDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -673,41 +933,77 @@
         "KeyType": KeyTypeType,
         "Status": DeliveryStreamEncryptionStatusType,
         "FailureDescription": FailureDescriptionTypeDef,
     },
     total=False,
 )
 
+DeserializerOutputTypeDef = TypedDict(
+    "DeserializerOutputTypeDef",
+    {
+        "OpenXJsonSerDe": OpenXJsonSerDeOutputTypeDef,
+        "HiveJsonSerDe": HiveJsonSerDeOutputTypeDef,
+    },
+    total=False,
+)
+
 DeserializerTypeDef = TypedDict(
     "DeserializerTypeDef",
     {
         "OpenXJsonSerDe": OpenXJsonSerDeTypeDef,
         "HiveJsonSerDe": HiveJsonSerDeTypeDef,
     },
     total=False,
 )
 
+DynamicPartitioningConfigurationOutputTypeDef = TypedDict(
+    "DynamicPartitioningConfigurationOutputTypeDef",
+    {
+        "RetryOptions": RetryOptionsOutputTypeDef,
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 DynamicPartitioningConfigurationTypeDef = TypedDict(
     "DynamicPartitioningConfigurationTypeDef",
     {
         "RetryOptions": RetryOptionsTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "NoEncryptionConfig": Literal["NoEncryption"],
+        "KMSEncryptionConfig": KMSEncryptionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "NoEncryptionConfig": Literal["NoEncryption"],
         "KMSEncryptionConfig": KMSEncryptionConfigTypeDef,
     },
     total=False,
 )
 
+HttpEndpointRequestConfigurationOutputTypeDef = TypedDict(
+    "HttpEndpointRequestConfigurationOutputTypeDef",
+    {
+        "ContentEncoding": ContentEncodingType,
+        "CommonAttributes": List[HttpEndpointCommonAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
 HttpEndpointRequestConfigurationTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationTypeDef",
     {
         "ContentEncoding": ContentEncodingType,
         "CommonAttributes": Sequence[HttpEndpointCommonAttributeTypeDef],
     },
     total=False,
@@ -717,23 +1013,60 @@
     "SourceDescriptionTypeDef",
     {
         "KinesisStreamSourceDescription": KinesisStreamSourceDescriptionTypeDef,
     },
     total=False,
 )
 
+ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "HasMoreTags": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SerializerOutputTypeDef = TypedDict(
+    "SerializerOutputTypeDef",
+    {
+        "ParquetSerDe": ParquetSerDeOutputTypeDef,
+        "OrcSerDe": OrcSerDeOutputTypeDef,
+    },
+    total=False,
+)
+
 SerializerTypeDef = TypedDict(
     "SerializerTypeDef",
     {
         "ParquetSerDe": ParquetSerDeTypeDef,
         "OrcSerDe": OrcSerDeTypeDef,
     },
     total=False,
 )
 
+_RequiredProcessorOutputTypeDef = TypedDict(
+    "_RequiredProcessorOutputTypeDef",
+    {
+        "Type": ProcessorTypeType,
+    },
+)
+_OptionalProcessorOutputTypeDef = TypedDict(
+    "_OptionalProcessorOutputTypeDef",
+    {
+        "Parameters": List[ProcessorParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ProcessorOutputTypeDef(_RequiredProcessorOutputTypeDef, _OptionalProcessorOutputTypeDef):
+    pass
+
+
 _RequiredProcessorTypeDef = TypedDict(
     "_RequiredProcessorTypeDef",
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorTypeDef = TypedDict(
@@ -771,72 +1104,80 @@
         "FailedPutCount": int,
         "Encrypted": bool,
         "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InputFormatConfigurationOutputTypeDef = TypedDict(
+    "InputFormatConfigurationOutputTypeDef",
+    {
+        "Deserializer": DeserializerOutputTypeDef,
+    },
+    total=False,
+)
+
 InputFormatConfigurationTypeDef = TypedDict(
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
     },
     total=False,
 )
 
-_RequiredS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredS3DestinationConfigurationTypeDef",
+_RequiredS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsOutputTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
-_OptionalS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalS3DestinationConfigurationTypeDef",
+_OptionalS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
     },
     total=False,
 )
 
 
-class S3DestinationConfigurationTypeDef(
-    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
+class S3DestinationDescriptionTypeDef(
+    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
 ):
     pass
 
 
-_RequiredS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredS3DestinationDescriptionTypeDef",
+_RequiredS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalS3DestinationDescriptionTypeDef",
+_OptionalS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
 
-class S3DestinationDescriptionTypeDef(
-    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
+class S3DestinationConfigurationTypeDef(
+    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
 
 S3DestinationUpdateTypeDef = TypedDict(
     "S3DestinationUpdateTypeDef",
     {
@@ -848,42 +1189,188 @@
         "CompressionFormat": CompressionFormatType,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
+OutputFormatConfigurationOutputTypeDef = TypedDict(
+    "OutputFormatConfigurationOutputTypeDef",
+    {
+        "Serializer": SerializerOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputFormatConfigurationTypeDef = TypedDict(
     "OutputFormatConfigurationTypeDef",
     {
         "Serializer": SerializerTypeDef,
     },
     total=False,
 )
 
+ProcessingConfigurationOutputTypeDef = TypedDict(
+    "ProcessingConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Processors": List[ProcessorOutputTypeDef],
+    },
+    total=False,
+)
+
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "Enabled": bool,
         "Processors": Sequence[ProcessorTypeDef],
     },
     total=False,
 )
 
+DataFormatConversionConfigurationOutputTypeDef = TypedDict(
+    "DataFormatConversionConfigurationOutputTypeDef",
+    {
+        "SchemaConfiguration": SchemaConfigurationOutputTypeDef,
+        "InputFormatConfiguration": InputFormatConfigurationOutputTypeDef,
+        "OutputFormatConfiguration": OutputFormatConfigurationOutputTypeDef,
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 DataFormatConversionConfigurationTypeDef = TypedDict(
     "DataFormatConversionConfigurationTypeDef",
     {
         "SchemaConfiguration": SchemaConfigurationTypeDef,
         "InputFormatConfiguration": InputFormatConfigurationTypeDef,
         "OutputFormatConfiguration": OutputFormatConfigurationTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
+AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "CollectionEndpoint": str,
+        "IndexName": str,
+        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
+        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
+        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
+        "BufferingHints": AmazonopensearchserviceBufferingHintsOutputTypeDef,
+        "RetryOptions": AmazonopensearchserviceRetryOptionsOutputTypeDef,
+        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+ElasticsearchDestinationDescriptionTypeDef = TypedDict(
+    "ElasticsearchDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
+        "BufferingHints": ElasticsearchBufferingHintsOutputTypeDef,
+        "RetryOptions": ElasticsearchRetryOptionsOutputTypeDef,
+        "S3BackupMode": ElasticsearchS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+HttpEndpointDestinationDescriptionTypeDef = TypedDict(
+    "HttpEndpointDestinationDescriptionTypeDef",
+    {
+        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
+        "BufferingHints": HttpEndpointBufferingHintsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "RequestConfiguration": HttpEndpointRequestConfigurationOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "RoleARN": str,
+        "RetryOptions": HttpEndpointRetryOptionsOutputTypeDef,
+        "S3BackupMode": HttpEndpointS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredRedshiftDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "ClusterJDBCURL": str,
+        "CopyCommand": CopyCommandOutputTypeDef,
+        "Username": str,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+)
+_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalRedshiftDestinationDescriptionTypeDef",
+    {
+        "RetryOptions": RedshiftRetryOptionsOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "S3BackupMode": RedshiftS3BackupModeType,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RedshiftDestinationDescriptionTypeDef(
+    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
+):
+    pass
+
+
+SplunkDestinationDescriptionTypeDef = TypedDict(
+    "SplunkDestinationDescriptionTypeDef",
+    {
+        "HECEndpoint": str,
+        "HECEndpointType": HECEndpointTypeType,
+        "HECToken": str,
+        "HECAcknowledgmentTimeoutInSeconds": int,
+        "RetryOptions": SplunkRetryOptionsOutputTypeDef,
+        "S3BackupMode": SplunkS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef = TypedDict(
     "_RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "IndexName": str,
         "S3Configuration": S3DestinationConfigurationTypeDef,
     },
@@ -906,31 +1393,14 @@
 class AmazonOpenSearchServerlessDestinationConfigurationTypeDef(
     _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     _OptionalAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
 ):
     pass
 
 
-AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "CollectionEndpoint": str,
-        "IndexName": str,
-        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
-        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
-        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 AmazonOpenSearchServerlessDestinationUpdateTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
         "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
@@ -971,34 +1441,14 @@
 class AmazonopensearchserviceDestinationConfigurationTypeDef(
     _RequiredAmazonopensearchserviceDestinationConfigurationTypeDef,
     _OptionalAmazonopensearchserviceDestinationConfigurationTypeDef,
 ):
     pass
 
 
-AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
-        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
-        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
-        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 AmazonopensearchserviceDestinationUpdateTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1042,34 +1492,14 @@
 class ElasticsearchDestinationConfigurationTypeDef(
     _RequiredElasticsearchDestinationConfigurationTypeDef,
     _OptionalElasticsearchDestinationConfigurationTypeDef,
 ):
     pass
 
 
-ElasticsearchDestinationDescriptionTypeDef = TypedDict(
-    "ElasticsearchDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
-        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
-        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
-        "S3BackupMode": ElasticsearchS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 ElasticsearchDestinationUpdateTypeDef = TypedDict(
     "ElasticsearchDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1109,30 +1539,14 @@
 class HttpEndpointDestinationConfigurationTypeDef(
     _RequiredHttpEndpointDestinationConfigurationTypeDef,
     _OptionalHttpEndpointDestinationConfigurationTypeDef,
 ):
     pass
 
 
-HttpEndpointDestinationDescriptionTypeDef = TypedDict(
-    "HttpEndpointDestinationDescriptionTypeDef",
-    {
-        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
-        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "RoleARN": str,
-        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
-        "S3BackupMode": HttpEndpointS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 HttpEndpointDestinationUpdateTypeDef = TypedDict(
     "HttpEndpointDestinationUpdateTypeDef",
     {
         "EndpointConfiguration": HttpEndpointConfigurationTypeDef,
         "BufferingHints": HttpEndpointBufferingHintsTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
@@ -1172,43 +1586,14 @@
 class RedshiftDestinationConfigurationTypeDef(
     _RequiredRedshiftDestinationConfigurationTypeDef,
     _OptionalRedshiftDestinationConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredRedshiftDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "ClusterJDBCURL": str,
-        "CopyCommand": CopyCommandTypeDef,
-        "Username": str,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-)
-_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalRedshiftDestinationDescriptionTypeDef",
-    {
-        "RetryOptions": RedshiftRetryOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "S3BackupMode": RedshiftS3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class RedshiftDestinationDescriptionTypeDef(
-    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
-):
-    pass
-
-
 RedshiftDestinationUpdateTypeDef = TypedDict(
     "RedshiftDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
         "CopyCommand": CopyCommandTypeDef,
         "Username": str,
@@ -1247,30 +1632,14 @@
 
 class SplunkDestinationConfigurationTypeDef(
     _RequiredSplunkDestinationConfigurationTypeDef, _OptionalSplunkDestinationConfigurationTypeDef
 ):
     pass
 
 
-SplunkDestinationDescriptionTypeDef = TypedDict(
-    "SplunkDestinationDescriptionTypeDef",
-    {
-        "HECEndpoint": str,
-        "HECEndpointType": HECEndpointTypeType,
-        "HECToken": str,
-        "HECAcknowledgmentTimeoutInSeconds": int,
-        "RetryOptions": SplunkRetryOptionsTypeDef,
-        "S3BackupMode": SplunkS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
 SplunkDestinationUpdateTypeDef = TypedDict(
     "SplunkDestinationUpdateTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
@@ -1279,76 +1648,76 @@
         "S3Update": S3DestinationUpdateTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationConfigurationTypeDef",
+_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsOutputTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
-_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationConfigurationTypeDef",
+_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
-        "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
-        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "DataFormatConversionConfiguration": DataFormatConversionConfigurationOutputTypeDef,
+        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
-class ExtendedS3DestinationConfigurationTypeDef(
-    _RequiredExtendedS3DestinationConfigurationTypeDef,
-    _OptionalExtendedS3DestinationConfigurationTypeDef,
+class ExtendedS3DestinationDescriptionTypeDef(
+    _RequiredExtendedS3DestinationDescriptionTypeDef,
+    _OptionalExtendedS3DestinationDescriptionTypeDef,
 ):
     pass
 
 
-_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationDescriptionTypeDef",
+_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationDescriptionTypeDef",
+_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class ExtendedS3DestinationDescriptionTypeDef(
-    _RequiredExtendedS3DestinationDescriptionTypeDef,
-    _OptionalExtendedS3DestinationDescriptionTypeDef,
+class ExtendedS3DestinationConfigurationTypeDef(
+    _RequiredExtendedS3DestinationConfigurationTypeDef,
+    _OptionalExtendedS3DestinationConfigurationTypeDef,
 ):
     pass
 
 
 ExtendedS3DestinationUpdateTypeDef = TypedDict(
     "ExtendedS3DestinationUpdateTypeDef",
     {
@@ -1365,14 +1734,46 @@
         "S3BackupUpdate": S3DestinationUpdateTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredDestinationDescriptionTypeDef",
+    {
+        "DestinationId": str,
+    },
+)
+_OptionalDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalDestinationDescriptionTypeDef",
+    {
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
+        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
+        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
+        "AmazonopensearchserviceDestinationDescription": (
+            AmazonopensearchserviceDestinationDescriptionTypeDef
+        ),
+        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
+        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
+        "AmazonOpenSearchServerlessDestinationDescription": (
+            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
+        ),
+    },
+    total=False,
+)
+
+
+class DestinationDescriptionTypeDef(
+    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
+):
+    pass
+
+
 _RequiredCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -1404,46 +1805,14 @@
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
     _OptionalCreateDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredDestinationDescriptionTypeDef",
-    {
-        "DestinationId": str,
-    },
-)
-_OptionalDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalDestinationDescriptionTypeDef",
-    {
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
-        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
-        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
-        "AmazonopensearchserviceDestinationDescription": (
-            AmazonopensearchserviceDestinationDescriptionTypeDef
-        ),
-        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
-        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
-        "AmazonOpenSearchServerlessDestinationDescription": (
-            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
-        ),
-    },
-    total=False,
-)
-
-
-class DestinationDescriptionTypeDef(
-    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
-):
-    pass
-
-
 _RequiredUpdateDestinationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "CurrentDeliveryStreamVersionId": str,
         "DestinationId": str,
     },
```

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.pyi` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for firehose service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsTypeDef
+    from mypy_boto3_firehose.type_defs import AmazonOpenSearchServerlessBufferingHintsOutputTypeDef
 
-    data: AmazonOpenSearchServerlessBufferingHintsTypeDef = {...}
+    data: AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -49,106 +49,148 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     "AmazonOpenSearchServerlessRetryOptionsTypeDef",
     "CloudWatchLoggingOptionsTypeDef",
     "VpcConfigurationTypeDef",
+    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
+    "CloudWatchLoggingOptionsOutputTypeDef",
     "VpcConfigurationDescriptionTypeDef",
+    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
     "AmazonopensearchserviceBufferingHintsTypeDef",
     "AmazonopensearchserviceRetryOptionsTypeDef",
+    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
+    "BufferingHintsOutputTypeDef",
     "BufferingHintsTypeDef",
+    "CopyCommandOutputTypeDef",
     "CopyCommandTypeDef",
     "DeliveryStreamEncryptionConfigurationInputTypeDef",
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDeliveryStreamOutputTypeDef",
+    "SchemaConfigurationOutputTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
+    "HiveJsonSerDeOutputTypeDef",
+    "OpenXJsonSerDeOutputTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
+    "RetryOptionsOutputTypeDef",
     "RetryOptionsTypeDef",
+    "ElasticsearchBufferingHintsOutputTypeDef",
     "ElasticsearchBufferingHintsTypeDef",
     "ElasticsearchRetryOptionsTypeDef",
+    "ElasticsearchRetryOptionsOutputTypeDef",
+    "KMSEncryptionConfigOutputTypeDef",
     "KMSEncryptionConfigTypeDef",
+    "HttpEndpointBufferingHintsOutputTypeDef",
     "HttpEndpointBufferingHintsTypeDef",
+    "HttpEndpointCommonAttributeOutputTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
+    "HttpEndpointRetryOptionsOutputTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
     "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
+    "TagOutputTypeDef",
+    "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
+    "ParquetSerDeOutputTypeDef",
     "ParquetSerDeTypeDef",
+    "ProcessorParameterOutputTypeDef",
     "ProcessorParameterTypeDef",
     "RecordTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
     "PutRecordOutputTypeDef",
     "RedshiftRetryOptionsTypeDef",
+    "RedshiftRetryOptionsOutputTypeDef",
     "ResponseMetadataTypeDef",
     "SplunkRetryOptionsTypeDef",
+    "SplunkRetryOptionsOutputTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     "UntagDeliveryStreamInputRequestTypeDef",
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
-    "ListTagsForDeliveryStreamOutputTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
+    "DeserializerOutputTypeDef",
     "DeserializerTypeDef",
+    "DynamicPartitioningConfigurationOutputTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
+    "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    "SerializerOutputTypeDef",
     "SerializerTypeDef",
+    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
     "PutRecordBatchOutputTypeDef",
+    "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
-    "S3DestinationConfigurationTypeDef",
     "S3DestinationDescriptionTypeDef",
+    "S3DestinationConfigurationTypeDef",
     "S3DestinationUpdateTypeDef",
+    "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
+    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
+    "DataFormatConversionConfigurationOutputTypeDef",
     "DataFormatConversionConfigurationTypeDef",
-    "AmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
+    "ElasticsearchDestinationDescriptionTypeDef",
+    "HttpEndpointDestinationDescriptionTypeDef",
+    "RedshiftDestinationDescriptionTypeDef",
+    "SplunkDestinationDescriptionTypeDef",
+    "AmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     "AmazonopensearchserviceDestinationConfigurationTypeDef",
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     "ElasticsearchDestinationConfigurationTypeDef",
-    "ElasticsearchDestinationDescriptionTypeDef",
     "ElasticsearchDestinationUpdateTypeDef",
     "HttpEndpointDestinationConfigurationTypeDef",
-    "HttpEndpointDestinationDescriptionTypeDef",
     "HttpEndpointDestinationUpdateTypeDef",
     "RedshiftDestinationConfigurationTypeDef",
-    "RedshiftDestinationDescriptionTypeDef",
     "RedshiftDestinationUpdateTypeDef",
     "SplunkDestinationConfigurationTypeDef",
-    "SplunkDestinationDescriptionTypeDef",
     "SplunkDestinationUpdateTypeDef",
-    "ExtendedS3DestinationConfigurationTypeDef",
     "ExtendedS3DestinationDescriptionTypeDef",
+    "ExtendedS3DestinationConfigurationTypeDef",
     "ExtendedS3DestinationUpdateTypeDef",
-    "CreateDeliveryStreamInputRequestTypeDef",
     "DestinationDescriptionTypeDef",
+    "CreateDeliveryStreamInputRequestTypeDef",
     "UpdateDestinationInputRequestTypeDef",
     "DeliveryStreamDescriptionTypeDef",
     "DescribeDeliveryStreamOutputTypeDef",
 )
 
+AmazonOpenSearchServerlessBufferingHintsOutputTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessBufferingHintsOutputTypeDef",
+    {
+        "IntervalInSeconds": int,
+        "SizeInMBs": int,
+    },
+    total=False,
+)
+
 AmazonOpenSearchServerlessBufferingHintsTypeDef = TypedDict(
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -177,24 +219,51 @@
     {
         "SubnetIds": Sequence[str],
         "RoleARN": str,
         "SecurityGroupIds": Sequence[str],
     },
 )
 
+AmazonOpenSearchServerlessRetryOptionsOutputTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
+CloudWatchLoggingOptionsOutputTypeDef = TypedDict(
+    "CloudWatchLoggingOptionsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "LogGroupName": str,
+        "LogStreamName": str,
+    },
+    total=False,
+)
+
 VpcConfigurationDescriptionTypeDef = TypedDict(
     "VpcConfigurationDescriptionTypeDef",
     {
         "SubnetIds": List[str],
         "RoleARN": str,
         "SecurityGroupIds": List[str],
         "VpcId": str,
     },
 )
 
+AmazonopensearchserviceBufferingHintsOutputTypeDef = TypedDict(
+    "AmazonopensearchserviceBufferingHintsOutputTypeDef",
+    {
+        "IntervalInSeconds": int,
+        "SizeInMBs": int,
+    },
+    total=False,
+)
+
 AmazonopensearchserviceBufferingHintsTypeDef = TypedDict(
     "AmazonopensearchserviceBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -204,23 +273,60 @@
     "AmazonopensearchserviceRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+AmazonopensearchserviceRetryOptionsOutputTypeDef = TypedDict(
+    "AmazonopensearchserviceRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
+BufferingHintsOutputTypeDef = TypedDict(
+    "BufferingHintsOutputTypeDef",
+    {
+        "SizeInMBs": int,
+        "IntervalInSeconds": int,
+    },
+    total=False,
+)
+
 BufferingHintsTypeDef = TypedDict(
     "BufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
+_RequiredCopyCommandOutputTypeDef = TypedDict(
+    "_RequiredCopyCommandOutputTypeDef",
+    {
+        "DataTableName": str,
+    },
+)
+_OptionalCopyCommandOutputTypeDef = TypedDict(
+    "_OptionalCopyCommandOutputTypeDef",
+    {
+        "DataTableColumns": str,
+        "CopyOptions": str,
+    },
+    total=False,
+)
+
+class CopyCommandOutputTypeDef(
+    _RequiredCopyCommandOutputTypeDef, _OptionalCopyCommandOutputTypeDef
+):
+    pass
+
 _RequiredCopyCommandTypeDef = TypedDict(
     "_RequiredCopyCommandTypeDef",
     {
         "DataTableName": str,
     },
 )
 _OptionalCopyCommandTypeDef = TypedDict(
@@ -284,14 +390,27 @@
     "CreateDeliveryStreamOutputTypeDef",
     {
         "DeliveryStreamARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchemaConfigurationOutputTypeDef = TypedDict(
+    "SchemaConfigurationOutputTypeDef",
+    {
+        "RoleARN": str,
+        "CatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Region": str,
+        "VersionId": str,
+    },
+    total=False,
+)
+
 SchemaConfigurationTypeDef = TypedDict(
     "SchemaConfigurationTypeDef",
     {
         "RoleARN": str,
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
@@ -346,14 +465,32 @@
 
 class DescribeDeliveryStreamInputRequestTypeDef(
     _RequiredDescribeDeliveryStreamInputRequestTypeDef,
     _OptionalDescribeDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
+HiveJsonSerDeOutputTypeDef = TypedDict(
+    "HiveJsonSerDeOutputTypeDef",
+    {
+        "TimestampFormats": List[str],
+    },
+    total=False,
+)
+
+OpenXJsonSerDeOutputTypeDef = TypedDict(
+    "OpenXJsonSerDeOutputTypeDef",
+    {
+        "ConvertDotsInJsonKeysToUnderscores": bool,
+        "CaseInsensitive": bool,
+        "ColumnToJsonKeyMappings": Dict[str, str],
+    },
+    total=False,
+)
+
 HiveJsonSerDeTypeDef = TypedDict(
     "HiveJsonSerDeTypeDef",
     {
         "TimestampFormats": Sequence[str],
     },
     total=False,
 )
@@ -364,22 +501,39 @@
         "ConvertDotsInJsonKeysToUnderscores": bool,
         "CaseInsensitive": bool,
         "ColumnToJsonKeyMappings": Mapping[str, str],
     },
     total=False,
 )
 
+RetryOptionsOutputTypeDef = TypedDict(
+    "RetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
 RetryOptionsTypeDef = TypedDict(
     "RetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+ElasticsearchBufferingHintsOutputTypeDef = TypedDict(
+    "ElasticsearchBufferingHintsOutputTypeDef",
+    {
+        "IntervalInSeconds": int,
+        "SizeInMBs": int,
+    },
+    total=False,
+)
+
 ElasticsearchBufferingHintsTypeDef = TypedDict(
     "ElasticsearchBufferingHintsTypeDef",
     {
         "IntervalInSeconds": int,
         "SizeInMBs": int,
     },
     total=False,
@@ -389,30 +543,62 @@
     "ElasticsearchRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+ElasticsearchRetryOptionsOutputTypeDef = TypedDict(
+    "ElasticsearchRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
+KMSEncryptionConfigOutputTypeDef = TypedDict(
+    "KMSEncryptionConfigOutputTypeDef",
+    {
+        "AWSKMSKeyARN": str,
+    },
+)
+
 KMSEncryptionConfigTypeDef = TypedDict(
     "KMSEncryptionConfigTypeDef",
     {
         "AWSKMSKeyARN": str,
     },
 )
 
+HttpEndpointBufferingHintsOutputTypeDef = TypedDict(
+    "HttpEndpointBufferingHintsOutputTypeDef",
+    {
+        "SizeInMBs": int,
+        "IntervalInSeconds": int,
+    },
+    total=False,
+)
+
 HttpEndpointBufferingHintsTypeDef = TypedDict(
     "HttpEndpointBufferingHintsTypeDef",
     {
         "SizeInMBs": int,
         "IntervalInSeconds": int,
     },
     total=False,
 )
 
+HttpEndpointCommonAttributeOutputTypeDef = TypedDict(
+    "HttpEndpointCommonAttributeOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeValue": str,
+    },
+)
+
 HttpEndpointCommonAttributeTypeDef = TypedDict(
     "HttpEndpointCommonAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
 )
@@ -450,14 +636,22 @@
     "HttpEndpointRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+HttpEndpointRetryOptionsOutputTypeDef = TypedDict(
+    "HttpEndpointRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
 KinesisStreamSourceDescriptionTypeDef = TypedDict(
     "KinesisStreamSourceDescriptionTypeDef",
     {
         "KinesisStreamARN": str,
         "RoleARN": str,
         "DeliveryStartTimestamp": datetime,
     },
@@ -500,14 +694,48 @@
 
 class ListTagsForDeliveryStreamInputRequestTypeDef(
     _RequiredListTagsForDeliveryStreamInputRequestTypeDef,
     _OptionalListTagsForDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
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
+OrcSerDeOutputTypeDef = TypedDict(
+    "OrcSerDeOutputTypeDef",
+    {
+        "StripeSizeBytes": int,
+        "BlockSizeBytes": int,
+        "RowIndexStride": int,
+        "EnablePadding": bool,
+        "PaddingTolerance": float,
+        "Compression": OrcCompressionType,
+        "BloomFilterColumns": List[str],
+        "BloomFilterFalsePositiveProbability": float,
+        "DictionaryKeyThreshold": float,
+        "FormatVersion": OrcFormatVersionType,
+    },
+    total=False,
+)
+
 OrcSerDeTypeDef = TypedDict(
     "OrcSerDeTypeDef",
     {
         "StripeSizeBytes": int,
         "BlockSizeBytes": int,
         "RowIndexStride": int,
         "EnablePadding": bool,
@@ -517,27 +745,48 @@
         "BloomFilterFalsePositiveProbability": float,
         "DictionaryKeyThreshold": float,
         "FormatVersion": OrcFormatVersionType,
     },
     total=False,
 )
 
+ParquetSerDeOutputTypeDef = TypedDict(
+    "ParquetSerDeOutputTypeDef",
+    {
+        "BlockSizeBytes": int,
+        "PageSizeBytes": int,
+        "Compression": ParquetCompressionType,
+        "EnableDictionaryCompression": bool,
+        "MaxPaddingBytes": int,
+        "WriterVersion": ParquetWriterVersionType,
+    },
+    total=False,
+)
+
 ParquetSerDeTypeDef = TypedDict(
     "ParquetSerDeTypeDef",
     {
         "BlockSizeBytes": int,
         "PageSizeBytes": int,
         "Compression": ParquetCompressionType,
         "EnableDictionaryCompression": bool,
         "MaxPaddingBytes": int,
         "WriterVersion": ParquetWriterVersionType,
     },
     total=False,
 )
 
+ProcessorParameterOutputTypeDef = TypedDict(
+    "ProcessorParameterOutputTypeDef",
+    {
+        "ParameterName": ProcessorParameterNameType,
+        "ParameterValue": str,
+    },
+)
+
 ProcessorParameterTypeDef = TypedDict(
     "ProcessorParameterTypeDef",
     {
         "ParameterName": ProcessorParameterNameType,
         "ParameterValue": str,
     },
 )
@@ -572,14 +821,22 @@
     "RedshiftRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+RedshiftRetryOptionsOutputTypeDef = TypedDict(
+    "RedshiftRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
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
@@ -591,14 +848,22 @@
     "SplunkRetryOptionsTypeDef",
     {
         "DurationInSeconds": int,
     },
     total=False,
 )
 
+SplunkRetryOptionsOutputTypeDef = TypedDict(
+    "SplunkRetryOptionsOutputTypeDef",
+    {
+        "DurationInSeconds": int,
+    },
+    total=False,
+)
+
 StopDeliveryStreamEncryptionInputRequestTypeDef = TypedDict(
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 
@@ -628,23 +893,14 @@
 
 class StartDeliveryStreamEncryptionInputRequestTypeDef(
     _RequiredStartDeliveryStreamEncryptionInputRequestTypeDef,
     _OptionalStartDeliveryStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
-ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
-    "ListTagsForDeliveryStreamOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "HasMoreTags": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagDeliveryStreamInputRequestTypeDef = TypedDict(
     "TagDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -656,41 +912,77 @@
         "KeyType": KeyTypeType,
         "Status": DeliveryStreamEncryptionStatusType,
         "FailureDescription": FailureDescriptionTypeDef,
     },
     total=False,
 )
 
+DeserializerOutputTypeDef = TypedDict(
+    "DeserializerOutputTypeDef",
+    {
+        "OpenXJsonSerDe": OpenXJsonSerDeOutputTypeDef,
+        "HiveJsonSerDe": HiveJsonSerDeOutputTypeDef,
+    },
+    total=False,
+)
+
 DeserializerTypeDef = TypedDict(
     "DeserializerTypeDef",
     {
         "OpenXJsonSerDe": OpenXJsonSerDeTypeDef,
         "HiveJsonSerDe": HiveJsonSerDeTypeDef,
     },
     total=False,
 )
 
+DynamicPartitioningConfigurationOutputTypeDef = TypedDict(
+    "DynamicPartitioningConfigurationOutputTypeDef",
+    {
+        "RetryOptions": RetryOptionsOutputTypeDef,
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 DynamicPartitioningConfigurationTypeDef = TypedDict(
     "DynamicPartitioningConfigurationTypeDef",
     {
         "RetryOptions": RetryOptionsTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "NoEncryptionConfig": Literal["NoEncryption"],
+        "KMSEncryptionConfig": KMSEncryptionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "NoEncryptionConfig": Literal["NoEncryption"],
         "KMSEncryptionConfig": KMSEncryptionConfigTypeDef,
     },
     total=False,
 )
 
+HttpEndpointRequestConfigurationOutputTypeDef = TypedDict(
+    "HttpEndpointRequestConfigurationOutputTypeDef",
+    {
+        "ContentEncoding": ContentEncodingType,
+        "CommonAttributes": List[HttpEndpointCommonAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
 HttpEndpointRequestConfigurationTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationTypeDef",
     {
         "ContentEncoding": ContentEncodingType,
         "CommonAttributes": Sequence[HttpEndpointCommonAttributeTypeDef],
     },
     total=False,
@@ -700,23 +992,58 @@
     "SourceDescriptionTypeDef",
     {
         "KinesisStreamSourceDescription": KinesisStreamSourceDescriptionTypeDef,
     },
     total=False,
 )
 
+ListTagsForDeliveryStreamOutputTypeDef = TypedDict(
+    "ListTagsForDeliveryStreamOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "HasMoreTags": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SerializerOutputTypeDef = TypedDict(
+    "SerializerOutputTypeDef",
+    {
+        "ParquetSerDe": ParquetSerDeOutputTypeDef,
+        "OrcSerDe": OrcSerDeOutputTypeDef,
+    },
+    total=False,
+)
+
 SerializerTypeDef = TypedDict(
     "SerializerTypeDef",
     {
         "ParquetSerDe": ParquetSerDeTypeDef,
         "OrcSerDe": OrcSerDeTypeDef,
     },
     total=False,
 )
 
+_RequiredProcessorOutputTypeDef = TypedDict(
+    "_RequiredProcessorOutputTypeDef",
+    {
+        "Type": ProcessorTypeType,
+    },
+)
+_OptionalProcessorOutputTypeDef = TypedDict(
+    "_OptionalProcessorOutputTypeDef",
+    {
+        "Parameters": List[ProcessorParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class ProcessorOutputTypeDef(_RequiredProcessorOutputTypeDef, _OptionalProcessorOutputTypeDef):
+    pass
+
 _RequiredProcessorTypeDef = TypedDict(
     "_RequiredProcessorTypeDef",
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorTypeDef = TypedDict(
@@ -752,69 +1079,77 @@
         "FailedPutCount": int,
         "Encrypted": bool,
         "RequestResponses": List[PutRecordBatchResponseEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InputFormatConfigurationOutputTypeDef = TypedDict(
+    "InputFormatConfigurationOutputTypeDef",
+    {
+        "Deserializer": DeserializerOutputTypeDef,
+    },
+    total=False,
+)
+
 InputFormatConfigurationTypeDef = TypedDict(
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
     },
     total=False,
 )
 
-_RequiredS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredS3DestinationConfigurationTypeDef",
+_RequiredS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsOutputTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
-_OptionalS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalS3DestinationConfigurationTypeDef",
+_OptionalS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
     },
     total=False,
 )
 
-class S3DestinationConfigurationTypeDef(
-    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
+class S3DestinationDescriptionTypeDef(
+    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
 ):
     pass
 
-_RequiredS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredS3DestinationDescriptionTypeDef",
+_RequiredS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalS3DestinationDescriptionTypeDef",
+_OptionalS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-class S3DestinationDescriptionTypeDef(
-    _RequiredS3DestinationDescriptionTypeDef, _OptionalS3DestinationDescriptionTypeDef
+class S3DestinationConfigurationTypeDef(
+    _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
 S3DestinationUpdateTypeDef = TypedDict(
     "S3DestinationUpdateTypeDef",
     {
         "RoleARN": str,
@@ -825,42 +1160,186 @@
         "CompressionFormat": CompressionFormatType,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
+OutputFormatConfigurationOutputTypeDef = TypedDict(
+    "OutputFormatConfigurationOutputTypeDef",
+    {
+        "Serializer": SerializerOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputFormatConfigurationTypeDef = TypedDict(
     "OutputFormatConfigurationTypeDef",
     {
         "Serializer": SerializerTypeDef,
     },
     total=False,
 )
 
+ProcessingConfigurationOutputTypeDef = TypedDict(
+    "ProcessingConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Processors": List[ProcessorOutputTypeDef],
+    },
+    total=False,
+)
+
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "Enabled": bool,
         "Processors": Sequence[ProcessorTypeDef],
     },
     total=False,
 )
 
+DataFormatConversionConfigurationOutputTypeDef = TypedDict(
+    "DataFormatConversionConfigurationOutputTypeDef",
+    {
+        "SchemaConfiguration": SchemaConfigurationOutputTypeDef,
+        "InputFormatConfiguration": InputFormatConfigurationOutputTypeDef,
+        "OutputFormatConfiguration": OutputFormatConfigurationOutputTypeDef,
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 DataFormatConversionConfigurationTypeDef = TypedDict(
     "DataFormatConversionConfigurationTypeDef",
     {
         "SchemaConfiguration": SchemaConfigurationTypeDef,
         "InputFormatConfiguration": InputFormatConfigurationTypeDef,
         "OutputFormatConfiguration": OutputFormatConfigurationTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
+AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "CollectionEndpoint": str,
+        "IndexName": str,
+        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
+        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
+        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
+        "BufferingHints": AmazonopensearchserviceBufferingHintsOutputTypeDef,
+        "RetryOptions": AmazonopensearchserviceRetryOptionsOutputTypeDef,
+        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+ElasticsearchDestinationDescriptionTypeDef = TypedDict(
+    "ElasticsearchDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
+        "BufferingHints": ElasticsearchBufferingHintsOutputTypeDef,
+        "RetryOptions": ElasticsearchRetryOptionsOutputTypeDef,
+        "S3BackupMode": ElasticsearchS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+HttpEndpointDestinationDescriptionTypeDef = TypedDict(
+    "HttpEndpointDestinationDescriptionTypeDef",
+    {
+        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
+        "BufferingHints": HttpEndpointBufferingHintsOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "RequestConfiguration": HttpEndpointRequestConfigurationOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "RoleARN": str,
+        "RetryOptions": HttpEndpointRetryOptionsOutputTypeDef,
+        "S3BackupMode": HttpEndpointS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+    total=False,
+)
+
+_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredRedshiftDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "ClusterJDBCURL": str,
+        "CopyCommand": CopyCommandOutputTypeDef,
+        "Username": str,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+)
+_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalRedshiftDestinationDescriptionTypeDef",
+    {
+        "RetryOptions": RedshiftRetryOptionsOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "S3BackupMode": RedshiftS3BackupModeType,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class RedshiftDestinationDescriptionTypeDef(
+    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
+):
+    pass
+
+SplunkDestinationDescriptionTypeDef = TypedDict(
+    "SplunkDestinationDescriptionTypeDef",
+    {
+        "HECEndpoint": str,
+        "HECEndpointType": HECEndpointTypeType,
+        "HECToken": str,
+        "HECAcknowledgmentTimeoutInSeconds": int,
+        "RetryOptions": SplunkRetryOptionsOutputTypeDef,
+        "S3BackupMode": SplunkS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef = TypedDict(
     "_RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "IndexName": str,
         "S3Configuration": S3DestinationConfigurationTypeDef,
     },
@@ -881,31 +1360,14 @@
 
 class AmazonOpenSearchServerlessDestinationConfigurationTypeDef(
     _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     _OptionalAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
 ):
     pass
 
-AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "CollectionEndpoint": str,
-        "IndexName": str,
-        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
-        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
-        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 AmazonOpenSearchServerlessDestinationUpdateTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
         "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
@@ -944,34 +1406,14 @@
 
 class AmazonopensearchserviceDestinationConfigurationTypeDef(
     _RequiredAmazonopensearchserviceDestinationConfigurationTypeDef,
     _OptionalAmazonopensearchserviceDestinationConfigurationTypeDef,
 ):
     pass
 
-AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
-        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
-        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
-        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 AmazonopensearchserviceDestinationUpdateTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1013,34 +1455,14 @@
 
 class ElasticsearchDestinationConfigurationTypeDef(
     _RequiredElasticsearchDestinationConfigurationTypeDef,
     _OptionalElasticsearchDestinationConfigurationTypeDef,
 ):
     pass
 
-ElasticsearchDestinationDescriptionTypeDef = TypedDict(
-    "ElasticsearchDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
-        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
-        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
-        "S3BackupMode": ElasticsearchS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 ElasticsearchDestinationUpdateTypeDef = TypedDict(
     "ElasticsearchDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1078,30 +1500,14 @@
 
 class HttpEndpointDestinationConfigurationTypeDef(
     _RequiredHttpEndpointDestinationConfigurationTypeDef,
     _OptionalHttpEndpointDestinationConfigurationTypeDef,
 ):
     pass
 
-HttpEndpointDestinationDescriptionTypeDef = TypedDict(
-    "HttpEndpointDestinationDescriptionTypeDef",
-    {
-        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
-        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "RoleARN": str,
-        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
-        "S3BackupMode": HttpEndpointS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-    total=False,
-)
-
 HttpEndpointDestinationUpdateTypeDef = TypedDict(
     "HttpEndpointDestinationUpdateTypeDef",
     {
         "EndpointConfiguration": HttpEndpointConfigurationTypeDef,
         "BufferingHints": HttpEndpointBufferingHintsTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
@@ -1139,41 +1545,14 @@
 
 class RedshiftDestinationConfigurationTypeDef(
     _RequiredRedshiftDestinationConfigurationTypeDef,
     _OptionalRedshiftDestinationConfigurationTypeDef,
 ):
     pass
 
-_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredRedshiftDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "ClusterJDBCURL": str,
-        "CopyCommand": CopyCommandTypeDef,
-        "Username": str,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-)
-_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalRedshiftDestinationDescriptionTypeDef",
-    {
-        "RetryOptions": RedshiftRetryOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "S3BackupMode": RedshiftS3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
-class RedshiftDestinationDescriptionTypeDef(
-    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
-):
-    pass
-
 RedshiftDestinationUpdateTypeDef = TypedDict(
     "RedshiftDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
         "CopyCommand": CopyCommandTypeDef,
         "Username": str,
@@ -1210,30 +1589,14 @@
 )
 
 class SplunkDestinationConfigurationTypeDef(
     _RequiredSplunkDestinationConfigurationTypeDef, _OptionalSplunkDestinationConfigurationTypeDef
 ):
     pass
 
-SplunkDestinationDescriptionTypeDef = TypedDict(
-    "SplunkDestinationDescriptionTypeDef",
-    {
-        "HECEndpoint": str,
-        "HECEndpointType": HECEndpointTypeType,
-        "HECToken": str,
-        "HECAcknowledgmentTimeoutInSeconds": int,
-        "RetryOptions": SplunkRetryOptionsTypeDef,
-        "S3BackupMode": SplunkS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
 SplunkDestinationUpdateTypeDef = TypedDict(
     "SplunkDestinationUpdateTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
@@ -1242,73 +1605,73 @@
         "S3Update": S3DestinationUpdateTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationConfigurationTypeDef",
+_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsOutputTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
-_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationConfigurationTypeDef",
+_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
-        "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
-        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "DataFormatConversionConfiguration": DataFormatConversionConfigurationOutputTypeDef,
+        "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class ExtendedS3DestinationConfigurationTypeDef(
-    _RequiredExtendedS3DestinationConfigurationTypeDef,
-    _OptionalExtendedS3DestinationConfigurationTypeDef,
+class ExtendedS3DestinationDescriptionTypeDef(
+    _RequiredExtendedS3DestinationDescriptionTypeDef,
+    _OptionalExtendedS3DestinationDescriptionTypeDef,
 ):
     pass
 
-_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationDescriptionTypeDef",
+_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationDescriptionTypeDef",
+_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
-class ExtendedS3DestinationDescriptionTypeDef(
-    _RequiredExtendedS3DestinationDescriptionTypeDef,
-    _OptionalExtendedS3DestinationDescriptionTypeDef,
+class ExtendedS3DestinationConfigurationTypeDef(
+    _RequiredExtendedS3DestinationConfigurationTypeDef,
+    _OptionalExtendedS3DestinationConfigurationTypeDef,
 ):
     pass
 
 ExtendedS3DestinationUpdateTypeDef = TypedDict(
     "ExtendedS3DestinationUpdateTypeDef",
     {
         "RoleARN": str,
@@ -1324,14 +1687,44 @@
         "S3BackupUpdate": S3DestinationUpdateTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredDestinationDescriptionTypeDef",
+    {
+        "DestinationId": str,
+    },
+)
+_OptionalDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalDestinationDescriptionTypeDef",
+    {
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
+        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
+        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
+        "AmazonopensearchserviceDestinationDescription": (
+            AmazonopensearchserviceDestinationDescriptionTypeDef
+        ),
+        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
+        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
+        "AmazonOpenSearchServerlessDestinationDescription": (
+            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
+        ),
+    },
+    total=False,
+)
+
+class DestinationDescriptionTypeDef(
+    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
+):
+    pass
+
 _RequiredCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -1361,44 +1754,14 @@
 
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
     _OptionalCreateDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
-_RequiredDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredDestinationDescriptionTypeDef",
-    {
-        "DestinationId": str,
-    },
-)
-_OptionalDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalDestinationDescriptionTypeDef",
-    {
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
-        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
-        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
-        "AmazonopensearchserviceDestinationDescription": (
-            AmazonopensearchserviceDestinationDescriptionTypeDef
-        ),
-        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
-        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
-        "AmazonOpenSearchServerlessDestinationDescription": (
-            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
-        ),
-    },
-    total=False,
-)
-
-class DestinationDescriptionTypeDef(
-    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
-):
-    pass
-
 _RequiredUpdateDestinationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "CurrentDeliveryStreamVersionId": str,
         "DestinationId": str,
     },
```

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/PKG-INFO` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.28.0
-Summary: Type annotations for boto3.Firehose 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Firehose 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-firehose"></a>
 
 # mypy-boto3-firehose
 
 [![PyPI - mypy-boto3-firehose](https://img.shields.io/pypi/v/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-firehose)](https://pepy.tech/project/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
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
 [mypy-boto3-firehose docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,108 +319,141 @@
 ### Typed dictionaries
 
 `mypy_boto3_firehose.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_firehose.type_defs import (
+    AmazonOpenSearchServerlessBufferingHintsOutputTypeDef,
     AmazonOpenSearchServerlessBufferingHintsTypeDef,
     AmazonOpenSearchServerlessRetryOptionsTypeDef,
     CloudWatchLoggingOptionsTypeDef,
     VpcConfigurationTypeDef,
+    AmazonOpenSearchServerlessRetryOptionsOutputTypeDef,
+    CloudWatchLoggingOptionsOutputTypeDef,
     VpcConfigurationDescriptionTypeDef,
+    AmazonopensearchserviceBufferingHintsOutputTypeDef,
     AmazonopensearchserviceBufferingHintsTypeDef,
     AmazonopensearchserviceRetryOptionsTypeDef,
+    AmazonopensearchserviceRetryOptionsOutputTypeDef,
+    BufferingHintsOutputTypeDef,
     BufferingHintsTypeDef,
+    CopyCommandOutputTypeDef,
     CopyCommandTypeDef,
     DeliveryStreamEncryptionConfigurationInputTypeDef,
     KinesisStreamSourceConfigurationTypeDef,
     TagTypeDef,
     CreateDeliveryStreamOutputTypeDef,
+    SchemaConfigurationOutputTypeDef,
     SchemaConfigurationTypeDef,
     DeleteDeliveryStreamInputRequestTypeDef,
     FailureDescriptionTypeDef,
     DescribeDeliveryStreamInputRequestTypeDef,
+    HiveJsonSerDeOutputTypeDef,
+    OpenXJsonSerDeOutputTypeDef,
     HiveJsonSerDeTypeDef,
     OpenXJsonSerDeTypeDef,
+    RetryOptionsOutputTypeDef,
     RetryOptionsTypeDef,
+    ElasticsearchBufferingHintsOutputTypeDef,
     ElasticsearchBufferingHintsTypeDef,
     ElasticsearchRetryOptionsTypeDef,
+    ElasticsearchRetryOptionsOutputTypeDef,
+    KMSEncryptionConfigOutputTypeDef,
     KMSEncryptionConfigTypeDef,
+    HttpEndpointBufferingHintsOutputTypeDef,
     HttpEndpointBufferingHintsTypeDef,
+    HttpEndpointCommonAttributeOutputTypeDef,
     HttpEndpointCommonAttributeTypeDef,
     HttpEndpointConfigurationTypeDef,
     HttpEndpointDescriptionTypeDef,
     HttpEndpointRetryOptionsTypeDef,
+    HttpEndpointRetryOptionsOutputTypeDef,
     KinesisStreamSourceDescriptionTypeDef,
     ListDeliveryStreamsInputRequestTypeDef,
     ListDeliveryStreamsOutputTypeDef,
     ListTagsForDeliveryStreamInputRequestTypeDef,
+    TagOutputTypeDef,
+    OrcSerDeOutputTypeDef,
     OrcSerDeTypeDef,
+    ParquetSerDeOutputTypeDef,
     ParquetSerDeTypeDef,
+    ProcessorParameterOutputTypeDef,
     ProcessorParameterTypeDef,
     RecordTypeDef,
     PutRecordBatchResponseEntryTypeDef,
     PutRecordOutputTypeDef,
     RedshiftRetryOptionsTypeDef,
+    RedshiftRetryOptionsOutputTypeDef,
     ResponseMetadataTypeDef,
     SplunkRetryOptionsTypeDef,
+    SplunkRetryOptionsOutputTypeDef,
     StopDeliveryStreamEncryptionInputRequestTypeDef,
     UntagDeliveryStreamInputRequestTypeDef,
     StartDeliveryStreamEncryptionInputRequestTypeDef,
-    ListTagsForDeliveryStreamOutputTypeDef,
     TagDeliveryStreamInputRequestTypeDef,
     DeliveryStreamEncryptionConfigurationTypeDef,
+    DeserializerOutputTypeDef,
     DeserializerTypeDef,
+    DynamicPartitioningConfigurationOutputTypeDef,
     DynamicPartitioningConfigurationTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
+    HttpEndpointRequestConfigurationOutputTypeDef,
     HttpEndpointRequestConfigurationTypeDef,
     SourceDescriptionTypeDef,
+    ListTagsForDeliveryStreamOutputTypeDef,
+    SerializerOutputTypeDef,
     SerializerTypeDef,
+    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     PutRecordBatchInputRequestTypeDef,
     PutRecordInputRequestTypeDef,
     PutRecordBatchOutputTypeDef,
+    InputFormatConfigurationOutputTypeDef,
     InputFormatConfigurationTypeDef,
-    S3DestinationConfigurationTypeDef,
     S3DestinationDescriptionTypeDef,
+    S3DestinationConfigurationTypeDef,
     S3DestinationUpdateTypeDef,
+    OutputFormatConfigurationOutputTypeDef,
     OutputFormatConfigurationTypeDef,
+    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
+    DataFormatConversionConfigurationOutputTypeDef,
     DataFormatConversionConfigurationTypeDef,
-    AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     AmazonOpenSearchServerlessDestinationDescriptionTypeDef,
+    AmazonopensearchserviceDestinationDescriptionTypeDef,
+    ElasticsearchDestinationDescriptionTypeDef,
+    HttpEndpointDestinationDescriptionTypeDef,
+    RedshiftDestinationDescriptionTypeDef,
+    SplunkDestinationDescriptionTypeDef,
+    AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     AmazonOpenSearchServerlessDestinationUpdateTypeDef,
     AmazonopensearchserviceDestinationConfigurationTypeDef,
-    AmazonopensearchserviceDestinationDescriptionTypeDef,
     AmazonopensearchserviceDestinationUpdateTypeDef,
     ElasticsearchDestinationConfigurationTypeDef,
-    ElasticsearchDestinationDescriptionTypeDef,
     ElasticsearchDestinationUpdateTypeDef,
     HttpEndpointDestinationConfigurationTypeDef,
-    HttpEndpointDestinationDescriptionTypeDef,
     HttpEndpointDestinationUpdateTypeDef,
     RedshiftDestinationConfigurationTypeDef,
-    RedshiftDestinationDescriptionTypeDef,
     RedshiftDestinationUpdateTypeDef,
     SplunkDestinationConfigurationTypeDef,
-    SplunkDestinationDescriptionTypeDef,
     SplunkDestinationUpdateTypeDef,
-    ExtendedS3DestinationConfigurationTypeDef,
     ExtendedS3DestinationDescriptionTypeDef,
+    ExtendedS3DestinationConfigurationTypeDef,
     ExtendedS3DestinationUpdateTypeDef,
-    CreateDeliveryStreamInputRequestTypeDef,
     DestinationDescriptionTypeDef,
+    CreateDeliveryStreamInputRequestTypeDef,
     UpdateDestinationInputRequestTypeDef,
     DeliveryStreamDescriptionTypeDef,
     DescribeDeliveryStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
+def get_structure() -> AmazonOpenSearchServerlessBufferingHintsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/SOURCES.txt` & `mypy-boto3-firehose-1.28.12/mypy_boto3_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.28.0/setup.py` & `mypy-boto3-firehose-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-firehose",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Firehose 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Firehose 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

