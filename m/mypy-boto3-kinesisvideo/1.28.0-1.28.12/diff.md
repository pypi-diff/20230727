# Comparing `tmp/mypy-boto3-kinesisvideo-1.28.0.tar.gz` & `tmp/mypy-boto3-kinesisvideo-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.0.tar", last modified: Thu Jul  6 20:59:55 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.12.tar", last modified: Thu Jul 27 05:34:54 2023, max compression
```

## Comparing `mypy-boto3-kinesisvideo-1.28.0.tar` & `mypy-boto3-kinesisvideo-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.898346 mypy-boto3-kinesisvideo-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-07-06 20:59:55.898346 mypy-boto3-kinesisvideo-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.878346 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-07-06 20:44:56.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-06 20:44:58.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-06 20:44:58.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-06 20:44:56.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-06 20:44:56.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28642 2023-07-06 20:44:58.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28603 2023-07-06 20:44:58.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:55.898346 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-07-06 20:59:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:55.000000 mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:55.898346 mypy-boto3-kinesisvideo-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:44:55.000000 mypy-boto3-kinesisvideo-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33223 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33176 2023-07-27 05:24:48.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:54.000000 mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:54.836464 mypy-boto3-kinesisvideo-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:24:47.000000 mypy-boto3-kinesisvideo-1.28.12/setup.py
```

### Comparing `mypy-boto3-kinesisvideo-1.28.0/LICENSE` & `mypy-boto3-kinesisvideo-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.0
-Summary: Type annotations for boto3.KinesisVideo 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KinesisVideo 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kinesisvideo"></a>
 
 # mypy-boto3-kinesisvideo
 
 [![PyPI - mypy-boto3-kinesisvideo](https://img.shields.io/pypi/v/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,96 +353,109 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
-    SingleMasterConfigurationTypeDef,
+    SingleMasterConfigurationOutputTypeDef,
     ChannelNameConditionTypeDef,
+    SingleMasterConfigurationTypeDef,
     TagTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamInputRequestTypeDef,
     CreateStreamOutputTypeDef,
     DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
+    LocalSizeConfigOutputTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
     DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationTypeDef,
+    MediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     LastRecorderStatusTypeDef,
     LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
     GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
+    ImageGenerationDestinationConfigOutputTypeDef,
     ImageGenerationDestinationConfigTypeDef,
     ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
+    MediaSourceConfigOutputTypeDef,
     MediaSourceConfigTypeDef,
+    MediaStorageConfigurationTypeDef,
+    NotificationDestinationConfigOutputTypeDef,
     NotificationDestinationConfigTypeDef,
     PaginatorConfigTypeDef,
+    ScheduleConfigOutputTypeDef,
     ScheduleConfigTypeDef,
     ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
-    UpdateSignalingChannelInputRequestTypeDef,
     ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
+    UpdateSignalingChannelInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    DeletionConfigOutputTypeDef,
     DeletionConfigTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
+    RecorderConfigOutputTypeDef,
+    UploaderConfigOutputTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
+    EdgeConfigOutputTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
-    StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
+    StartEdgeConfigurationUpdateInputRequestTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_structure() -> SingleMasterConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.0/README.md` & `mypy-boto3-kinesisvideo-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kinesisvideo"></a>
 
 # mypy-boto3-kinesisvideo
 
 [![PyPI - mypy-boto3-kinesisvideo](https://img.shields.io/pypi/v/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,96 +321,109 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
-    SingleMasterConfigurationTypeDef,
+    SingleMasterConfigurationOutputTypeDef,
     ChannelNameConditionTypeDef,
+    SingleMasterConfigurationTypeDef,
     TagTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamInputRequestTypeDef,
     CreateStreamOutputTypeDef,
     DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
+    LocalSizeConfigOutputTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
     DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationTypeDef,
+    MediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     LastRecorderStatusTypeDef,
     LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
     GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
+    ImageGenerationDestinationConfigOutputTypeDef,
     ImageGenerationDestinationConfigTypeDef,
     ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
+    MediaSourceConfigOutputTypeDef,
     MediaSourceConfigTypeDef,
+    MediaStorageConfigurationTypeDef,
+    NotificationDestinationConfigOutputTypeDef,
     NotificationDestinationConfigTypeDef,
     PaginatorConfigTypeDef,
+    ScheduleConfigOutputTypeDef,
     ScheduleConfigTypeDef,
     ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
-    UpdateSignalingChannelInputRequestTypeDef,
     ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
+    UpdateSignalingChannelInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    DeletionConfigOutputTypeDef,
     DeletionConfigTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
+    RecorderConfigOutputTypeDef,
+    UploaderConfigOutputTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
+    EdgeConfigOutputTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
-    StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
+    StartEdgeConfigurationUpdateInputRequestTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_structure() -> SingleMasterConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/__init__.py` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/__init__.pyi` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/__main__.py` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideo 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.KinesisVideo 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/client.py` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/client.pyi` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/literals.py` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
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
@@ -289,26 +290,28 @@
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

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/literals.pyi` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
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
@@ -287,26 +288,28 @@
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

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/paginator.py` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/paginator.pyi` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/type_defs.py` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesisvideo service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
+    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationOutputTypeDef
 
-    data: SingleMasterConfigurationTypeDef = {...}
+    data: SingleMasterConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -38,98 +38,110 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "SingleMasterConfigurationTypeDef",
+    "SingleMasterConfigurationOutputTypeDef",
     "ChannelNameConditionTypeDef",
+    "SingleMasterConfigurationTypeDef",
     "TagTypeDef",
     "CreateSignalingChannelOutputTypeDef",
     "CreateStreamInputRequestTypeDef",
     "CreateStreamOutputTypeDef",
     "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
+    "LocalSizeConfigOutputTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
     "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
-    "MediaStorageConfigurationTypeDef",
+    "MediaStorageConfigurationOutputTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "LastRecorderStatusTypeDef",
     "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
     "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
+    "ImageGenerationDestinationConfigOutputTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
     "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
+    "MediaSourceConfigOutputTypeDef",
     "MediaSourceConfigTypeDef",
+    "MediaStorageConfigurationTypeDef",
+    "NotificationDestinationConfigOutputTypeDef",
     "NotificationDestinationConfigTypeDef",
     "PaginatorConfigTypeDef",
+    "ScheduleConfigOutputTypeDef",
     "ScheduleConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
-    "UpdateSignalingChannelInputRequestTypeDef",
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListSignalingChannelsInputRequestTypeDef",
+    "UpdateSignalingChannelInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "DeletionConfigOutputTypeDef",
     "DeletionConfigTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
+    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
+    "RecorderConfigOutputTypeDef",
+    "UploaderConfigOutputTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
+    "EdgeConfigOutputTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
-    "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
+    "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
-SingleMasterConfigurationTypeDef = TypedDict(
-    "SingleMasterConfigurationTypeDef",
+SingleMasterConfigurationOutputTypeDef = TypedDict(
+    "SingleMasterConfigurationOutputTypeDef",
     {
         "MessageTtlSeconds": int,
     },
     total=False,
 )
 
 ChannelNameConditionTypeDef = TypedDict(
@@ -137,14 +149,22 @@
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
 )
 
+SingleMasterConfigurationTypeDef = TypedDict(
+    "SingleMasterConfigurationTypeDef",
+    {
+        "MessageTtlSeconds": int,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -171,21 +191,19 @@
         "KmsKeyId": str,
         "DataRetentionInHours": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
-
 CreateStreamOutputTypeDef = TypedDict(
     "CreateStreamOutputTypeDef",
     {
         "StreamARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -209,42 +227,47 @@
     "_OptionalDeleteSignalingChannelInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class DeleteSignalingChannelInputRequestTypeDef(
     _RequiredDeleteSignalingChannelInputRequestTypeDef,
     _OptionalDeleteSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalDeleteStreamInputRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class DeleteStreamInputRequestTypeDef(
     _RequiredDeleteStreamInputRequestTypeDef, _OptionalDeleteStreamInputRequestTypeDef
 ):
     pass
 
+LocalSizeConfigOutputTypeDef = TypedDict(
+    "LocalSizeConfigOutputTypeDef",
+    {
+        "MaxLocalMediaSizeInMB": int,
+        "StrategyOnFullSize": StrategyOnFullSizeType,
+    },
+    total=False,
+)
 
 LocalSizeConfigTypeDef = TypedDict(
     "LocalSizeConfigTypeDef",
     {
         "MaxLocalMediaSizeInMB": int,
         "StrategyOnFullSize": StrategyOnFullSizeType,
     },
@@ -304,35 +327,33 @@
     {
         "ChannelName": str,
         "ChannelARN": str,
     },
     total=False,
 )
 
-_RequiredMediaStorageConfigurationTypeDef = TypedDict(
-    "_RequiredMediaStorageConfigurationTypeDef",
+_RequiredMediaStorageConfigurationOutputTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationOutputTypeDef",
     {
         "Status": MediaStorageConfigurationStatusType,
     },
 )
-_OptionalMediaStorageConfigurationTypeDef = TypedDict(
-    "_OptionalMediaStorageConfigurationTypeDef",
+_OptionalMediaStorageConfigurationOutputTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationOutputTypeDef",
     {
         "StreamARN": str,
     },
     total=False,
 )
 
-
-class MediaStorageConfigurationTypeDef(
-    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
+class MediaStorageConfigurationOutputTypeDef(
+    _RequiredMediaStorageConfigurationOutputTypeDef, _OptionalMediaStorageConfigurationOutputTypeDef
 ):
     pass
 
-
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -405,21 +426,19 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
-
 GetDataEndpointOutputTypeDef = TypedDict(
     "GetDataEndpointOutputTypeDef",
     {
         "DataEndpoint": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -438,14 +457,22 @@
     {
         "Protocol": ChannelProtocolType,
         "ResourceEndpoint": str,
     },
     total=False,
 )
 
+ImageGenerationDestinationConfigOutputTypeDef = TypedDict(
+    "ImageGenerationDestinationConfigOutputTypeDef",
+    {
+        "Uri": str,
+        "DestinationRegion": str,
+    },
+)
+
 ImageGenerationDestinationConfigTypeDef = TypedDict(
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
@@ -460,22 +487,20 @@
     "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
     _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
     "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
     {
         "HubDeviceArn": str,
     },
 )
 _OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
@@ -483,22 +508,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEdgeAgentConfigurationsInputRequestTypeDef(
     _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
     _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
 ):
     pass
 
-
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -514,21 +537,19 @@
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "NextToken": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -549,22 +570,56 @@
     {
         "NextToken": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MediaSourceConfigOutputTypeDef = TypedDict(
+    "MediaSourceConfigOutputTypeDef",
+    {
+        "MediaUriSecretArn": str,
+        "MediaUriType": MediaUriTypeType,
+    },
+)
+
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
 
+_RequiredMediaStorageConfigurationTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationTypeDef",
+    {
+        "Status": MediaStorageConfigurationStatusType,
+    },
+)
+_OptionalMediaStorageConfigurationTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationTypeDef",
+    {
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+class MediaStorageConfigurationTypeDef(
+    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
+):
+    pass
+
+NotificationDestinationConfigOutputTypeDef = TypedDict(
+    "NotificationDestinationConfigOutputTypeDef",
+    {
+        "Uri": str,
+    },
+)
+
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
     },
 )
 
@@ -574,14 +629,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ScheduleConfigOutputTypeDef = TypedDict(
+    "ScheduleConfigOutputTypeDef",
+    {
+        "ScheduleExpression": str,
+        "DurationInSeconds": int,
+    },
+)
+
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
     },
 )
@@ -608,21 +671,19 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-
 class TagStreamInputRequestTypeDef(
     _RequiredTagStreamInputRequestTypeDef, _OptionalTagStreamInputRequestTypeDef
 ):
     pass
 
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeyList": Sequence[str],
     },
 )
@@ -638,21 +699,19 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-
 class UntagStreamInputRequestTypeDef(
     _RequiredUntagStreamInputRequestTypeDef, _OptionalUntagStreamInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDataRetentionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRetentionInputRequestTypeDef",
     {
         "CurrentVersion": str,
         "Operation": UpdateDataRetentionOperationType,
         "DataRetentionChangeInHours": int,
     },
@@ -662,21 +721,19 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class UpdateDataRetentionInputRequestTypeDef(
     _RequiredUpdateDataRetentionInputRequestTypeDef, _OptionalUpdateDataRetentionInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStreamInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
 )
 _OptionalUpdateStreamInputRequestTypeDef = TypedDict(
@@ -686,35 +743,52 @@
         "StreamARN": str,
         "DeviceName": str,
         "MediaType": str,
     },
     total=False,
 )
 
-
 class UpdateStreamInputRequestTypeDef(
     _RequiredUpdateStreamInputRequestTypeDef, _OptionalUpdateStreamInputRequestTypeDef
 ):
     pass
 
-
 ChannelInfoTypeDef = TypedDict(
     "ChannelInfoTypeDef",
     {
         "ChannelName": str,
         "ChannelARN": str,
         "ChannelType": ChannelTypeType,
         "ChannelStatus": StatusType,
         "CreationTime": datetime,
-        "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
+        "SingleMasterConfiguration": SingleMasterConfigurationOutputTypeDef,
         "Version": str,
     },
     total=False,
 )
 
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListSignalingChannelsInputRequestTypeDef = TypedDict(
+    "ListSignalingChannelsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
         "CurrentVersion": str,
     },
 )
@@ -722,41 +796,20 @@
     "_OptionalUpdateSignalingChannelInputRequestTypeDef",
     {
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSignalingChannelsInputRequestTypeDef = TypedDict(
-    "ListSignalingChannelsInputRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredCreateSignalingChannelInputRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalCreateSignalingChannelInputRequestTypeDef = TypedDict(
@@ -765,30 +818,38 @@
         "ChannelType": ChannelTypeType,
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSignalingChannelInputRequestTypeDef(
     _RequiredCreateSignalingChannelInputRequestTypeDef,
     _OptionalCreateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DeletionConfigOutputTypeDef = TypedDict(
+    "DeletionConfigOutputTypeDef",
+    {
+        "EdgeRetentionInHours": int,
+        "LocalSizeConfig": LocalSizeConfigOutputTypeDef,
+        "DeleteAfterUpload": bool,
+    },
+    total=False,
+)
+
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
@@ -803,27 +864,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
-        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+        "MediaStorageConfiguration": MediaStorageConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
-    {
-        "ChannelARN": str,
-        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-    },
-)
-
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -856,57 +909,79 @@
     "_OptionalGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "SingleMasterChannelEndpointConfiguration": SingleMasterChannelEndpointConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class GetSignalingChannelEndpointInputRequestTypeDef(
     _RequiredGetSignalingChannelEndpointInputRequestTypeDef,
     _OptionalGetSignalingChannelEndpointInputRequestTypeDef,
 ):
     pass
 
-
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredImageGenerationConfigurationOutputTypeDef",
+    {
+        "Status": ConfigurationStatusType,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "DestinationConfig": ImageGenerationDestinationConfigOutputTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalImageGenerationConfigurationOutputTypeDef",
+    {
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+    },
+    total=False,
+)
+
+class ImageGenerationConfigurationOutputTypeDef(
+    _RequiredImageGenerationConfigurationOutputTypeDef,
+    _OptionalImageGenerationConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
-
 class ImageGenerationConfigurationTypeDef(
     _RequiredImageGenerationConfigurationTypeDef, _OptionalImageGenerationConfigurationTypeDef
 ):
     pass
 
-
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -918,41 +993,81 @@
         "MaxResults": int,
         "NextToken": str,
         "StreamNameCondition": StreamNameConditionTypeDef,
     },
     total=False,
 )
 
+UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelARN": str,
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+    },
+)
+
+NotificationConfigurationOutputTypeDef = TypedDict(
+    "NotificationConfigurationOutputTypeDef",
+    {
+        "Status": ConfigurationStatusType,
+        "DestinationConfig": NotificationDestinationConfigOutputTypeDef,
+    },
+)
+
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "DestinationConfig": NotificationDestinationConfigTypeDef,
     },
 )
 
+_RequiredRecorderConfigOutputTypeDef = TypedDict(
+    "_RequiredRecorderConfigOutputTypeDef",
+    {
+        "MediaSourceConfig": MediaSourceConfigOutputTypeDef,
+    },
+)
+_OptionalRecorderConfigOutputTypeDef = TypedDict(
+    "_OptionalRecorderConfigOutputTypeDef",
+    {
+        "ScheduleConfig": ScheduleConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class RecorderConfigOutputTypeDef(
+    _RequiredRecorderConfigOutputTypeDef, _OptionalRecorderConfigOutputTypeDef
+):
+    pass
+
+UploaderConfigOutputTypeDef = TypedDict(
+    "UploaderConfigOutputTypeDef",
+    {
+        "ScheduleConfig": ScheduleConfigOutputTypeDef,
+    },
+)
+
 _RequiredRecorderConfigTypeDef = TypedDict(
     "_RequiredRecorderConfigTypeDef",
     {
         "MediaSourceConfig": MediaSourceConfigTypeDef,
     },
 )
 _OptionalRecorderConfigTypeDef = TypedDict(
     "_OptionalRecorderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
     total=False,
 )
 
-
 class RecorderConfigTypeDef(_RequiredRecorderConfigTypeDef, _OptionalRecorderConfigTypeDef):
     pass
 
-
 UploaderConfigTypeDef = TypedDict(
     "UploaderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
 )
 
@@ -972,15 +1087,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
+        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
@@ -990,29 +1105,48 @@
     },
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredEdgeConfigOutputTypeDef = TypedDict(
+    "_RequiredEdgeConfigOutputTypeDef",
+    {
+        "HubDeviceArn": str,
+        "RecorderConfig": RecorderConfigOutputTypeDef,
+    },
+)
+_OptionalEdgeConfigOutputTypeDef = TypedDict(
+    "_OptionalEdgeConfigOutputTypeDef",
+    {
+        "UploaderConfig": UploaderConfigOutputTypeDef,
+        "DeletionConfig": DeletionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class EdgeConfigOutputTypeDef(_RequiredEdgeConfigOutputTypeDef, _OptionalEdgeConfigOutputTypeDef):
+    pass
+
 _RequiredEdgeConfigTypeDef = TypedDict(
     "_RequiredEdgeConfigTypeDef",
     {
         "HubDeviceArn": str,
         "RecorderConfig": RecorderConfigTypeDef,
     },
 )
@@ -1021,48 +1155,60 @@
     {
         "UploaderConfig": UploaderConfigTypeDef,
         "DeletionConfig": DeletionConfigTypeDef,
     },
     total=False,
 )
 
-
 class EdgeConfigTypeDef(_RequiredEdgeConfigTypeDef, _OptionalEdgeConfigTypeDef):
     pass
 
-
 DescribeEdgeConfigurationOutputTypeDef = TypedDict(
     "DescribeEdgeConfigurationOutputTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigTypeDef,
+        "EdgeConfig": EdgeConfigOutputTypeDef,
         "EdgeAgentStatus": EdgeAgentStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigTypeDef,
+        "EdgeConfig": EdgeConfigOutputTypeDef,
     },
     total=False,
 )
 
+StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
+    "StartEdgeConfigurationUpdateOutputTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -1070,36 +1216,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class StartEdgeConfigurationUpdateInputRequestTypeDef(
     _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef,
     _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef,
 ):
     pass
 
-
-StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
-    "StartEdgeConfigurationUpdateOutputTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "SyncStatus": SyncStatusType,
-        "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsOutputTypeDef",
     {
         "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo/type_defs.pyi` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesisvideo service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
+    from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationOutputTypeDef
 
-    data: SingleMasterConfigurationTypeDef = {...}
+    data: SingleMasterConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -38,97 +38,111 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "SingleMasterConfigurationTypeDef",
+    "SingleMasterConfigurationOutputTypeDef",
     "ChannelNameConditionTypeDef",
+    "SingleMasterConfigurationTypeDef",
     "TagTypeDef",
     "CreateSignalingChannelOutputTypeDef",
     "CreateStreamInputRequestTypeDef",
     "CreateStreamOutputTypeDef",
     "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
+    "LocalSizeConfigOutputTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
     "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
-    "MediaStorageConfigurationTypeDef",
+    "MediaStorageConfigurationOutputTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "LastRecorderStatusTypeDef",
     "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
     "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
+    "ImageGenerationDestinationConfigOutputTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
     "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
+    "MediaSourceConfigOutputTypeDef",
     "MediaSourceConfigTypeDef",
+    "MediaStorageConfigurationTypeDef",
+    "NotificationDestinationConfigOutputTypeDef",
     "NotificationDestinationConfigTypeDef",
     "PaginatorConfigTypeDef",
+    "ScheduleConfigOutputTypeDef",
     "ScheduleConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
-    "UpdateSignalingChannelInputRequestTypeDef",
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListSignalingChannelsInputRequestTypeDef",
+    "UpdateSignalingChannelInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "DeletionConfigOutputTypeDef",
     "DeletionConfigTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
+    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
+    "RecorderConfigOutputTypeDef",
+    "UploaderConfigOutputTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
+    "EdgeConfigOutputTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
-    "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
+    "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
-SingleMasterConfigurationTypeDef = TypedDict(
-    "SingleMasterConfigurationTypeDef",
+SingleMasterConfigurationOutputTypeDef = TypedDict(
+    "SingleMasterConfigurationOutputTypeDef",
     {
         "MessageTtlSeconds": int,
     },
     total=False,
 )
 
 ChannelNameConditionTypeDef = TypedDict(
@@ -136,14 +150,22 @@
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
 )
 
+SingleMasterConfigurationTypeDef = TypedDict(
+    "SingleMasterConfigurationTypeDef",
+    {
+        "MessageTtlSeconds": int,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -170,19 +192,21 @@
         "KmsKeyId": str,
         "DataRetentionInHours": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
+
 CreateStreamOutputTypeDef = TypedDict(
     "CreateStreamOutputTypeDef",
     {
         "StreamARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -206,39 +230,52 @@
     "_OptionalDeleteSignalingChannelInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class DeleteSignalingChannelInputRequestTypeDef(
     _RequiredDeleteSignalingChannelInputRequestTypeDef,
     _OptionalDeleteSignalingChannelInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalDeleteStreamInputRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class DeleteStreamInputRequestTypeDef(
     _RequiredDeleteStreamInputRequestTypeDef, _OptionalDeleteStreamInputRequestTypeDef
 ):
     pass
 
+
+LocalSizeConfigOutputTypeDef = TypedDict(
+    "LocalSizeConfigOutputTypeDef",
+    {
+        "MaxLocalMediaSizeInMB": int,
+        "StrategyOnFullSize": StrategyOnFullSizeType,
+    },
+    total=False,
+)
+
 LocalSizeConfigTypeDef = TypedDict(
     "LocalSizeConfigTypeDef",
     {
         "MaxLocalMediaSizeInMB": int,
         "StrategyOnFullSize": StrategyOnFullSizeType,
     },
     total=False,
@@ -297,33 +334,35 @@
     {
         "ChannelName": str,
         "ChannelARN": str,
     },
     total=False,
 )
 
-_RequiredMediaStorageConfigurationTypeDef = TypedDict(
-    "_RequiredMediaStorageConfigurationTypeDef",
+_RequiredMediaStorageConfigurationOutputTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationOutputTypeDef",
     {
         "Status": MediaStorageConfigurationStatusType,
     },
 )
-_OptionalMediaStorageConfigurationTypeDef = TypedDict(
-    "_OptionalMediaStorageConfigurationTypeDef",
+_OptionalMediaStorageConfigurationOutputTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationOutputTypeDef",
     {
         "StreamARN": str,
     },
     total=False,
 )
 
-class MediaStorageConfigurationTypeDef(
-    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
+
+class MediaStorageConfigurationOutputTypeDef(
+    _RequiredMediaStorageConfigurationOutputTypeDef, _OptionalMediaStorageConfigurationOutputTypeDef
 ):
     pass
 
+
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -396,19 +435,21 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
+
 GetDataEndpointOutputTypeDef = TypedDict(
     "GetDataEndpointOutputTypeDef",
     {
         "DataEndpoint": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -427,14 +468,22 @@
     {
         "Protocol": ChannelProtocolType,
         "ResourceEndpoint": str,
     },
     total=False,
 )
 
+ImageGenerationDestinationConfigOutputTypeDef = TypedDict(
+    "ImageGenerationDestinationConfigOutputTypeDef",
+    {
+        "Uri": str,
+        "DestinationRegion": str,
+    },
+)
+
 ImageGenerationDestinationConfigTypeDef = TypedDict(
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
@@ -449,20 +498,22 @@
     "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
     _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
     "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
     {
         "HubDeviceArn": str,
     },
 )
 _OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
@@ -470,20 +521,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEdgeAgentConfigurationsInputRequestTypeDef(
     _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
     _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
 ):
     pass
 
+
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -499,19 +552,21 @@
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "NextToken": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -532,22 +587,58 @@
     {
         "NextToken": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MediaSourceConfigOutputTypeDef = TypedDict(
+    "MediaSourceConfigOutputTypeDef",
+    {
+        "MediaUriSecretArn": str,
+        "MediaUriType": MediaUriTypeType,
+    },
+)
+
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
 
+_RequiredMediaStorageConfigurationTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationTypeDef",
+    {
+        "Status": MediaStorageConfigurationStatusType,
+    },
+)
+_OptionalMediaStorageConfigurationTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationTypeDef",
+    {
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+
+class MediaStorageConfigurationTypeDef(
+    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
+):
+    pass
+
+
+NotificationDestinationConfigOutputTypeDef = TypedDict(
+    "NotificationDestinationConfigOutputTypeDef",
+    {
+        "Uri": str,
+    },
+)
+
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
     },
 )
 
@@ -557,14 +648,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ScheduleConfigOutputTypeDef = TypedDict(
+    "ScheduleConfigOutputTypeDef",
+    {
+        "ScheduleExpression": str,
+        "DurationInSeconds": int,
+    },
+)
+
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
     },
 )
@@ -591,19 +690,21 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
+
 class TagStreamInputRequestTypeDef(
     _RequiredTagStreamInputRequestTypeDef, _OptionalTagStreamInputRequestTypeDef
 ):
     pass
 
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeyList": Sequence[str],
     },
 )
@@ -619,19 +720,21 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
+
 class UntagStreamInputRequestTypeDef(
     _RequiredUntagStreamInputRequestTypeDef, _OptionalUntagStreamInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDataRetentionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRetentionInputRequestTypeDef",
     {
         "CurrentVersion": str,
         "Operation": UpdateDataRetentionOperationType,
         "DataRetentionChangeInHours": int,
     },
@@ -641,19 +744,21 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class UpdateDataRetentionInputRequestTypeDef(
     _RequiredUpdateDataRetentionInputRequestTypeDef, _OptionalUpdateDataRetentionInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStreamInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
 )
 _OptionalUpdateStreamInputRequestTypeDef = TypedDict(
@@ -663,33 +768,54 @@
         "StreamARN": str,
         "DeviceName": str,
         "MediaType": str,
     },
     total=False,
 )
 
+
 class UpdateStreamInputRequestTypeDef(
     _RequiredUpdateStreamInputRequestTypeDef, _OptionalUpdateStreamInputRequestTypeDef
 ):
     pass
 
+
 ChannelInfoTypeDef = TypedDict(
     "ChannelInfoTypeDef",
     {
         "ChannelName": str,
         "ChannelARN": str,
         "ChannelType": ChannelTypeType,
         "ChannelStatus": StatusType,
         "CreationTime": datetime,
-        "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
+        "SingleMasterConfiguration": SingleMasterConfigurationOutputTypeDef,
         "Version": str,
     },
     total=False,
 )
 
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListSignalingChannelsInputRequestTypeDef = TypedDict(
+    "ListSignalingChannelsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
         "CurrentVersion": str,
     },
 )
@@ -697,38 +823,21 @@
     "_OptionalUpdateSignalingChannelInputRequestTypeDef",
     {
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSignalingChannelsInputRequestTypeDef = TypedDict(
-    "ListSignalingChannelsInputRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredCreateSignalingChannelInputRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
@@ -738,28 +847,40 @@
         "ChannelType": ChannelTypeType,
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSignalingChannelInputRequestTypeDef(
     _RequiredCreateSignalingChannelInputRequestTypeDef,
     _OptionalCreateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DeletionConfigOutputTypeDef = TypedDict(
+    "DeletionConfigOutputTypeDef",
+    {
+        "EdgeRetentionInHours": int,
+        "LocalSizeConfig": LocalSizeConfigOutputTypeDef,
+        "DeleteAfterUpload": bool,
+    },
+    total=False,
+)
+
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
@@ -774,27 +895,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
-        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+        "MediaStorageConfiguration": MediaStorageConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
-    "UpdateMediaStorageConfigurationInputRequestTypeDef",
-    {
-        "ChannelARN": str,
-        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-    },
-)
-
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -827,53 +940,85 @@
     "_OptionalGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "SingleMasterChannelEndpointConfiguration": SingleMasterChannelEndpointConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class GetSignalingChannelEndpointInputRequestTypeDef(
     _RequiredGetSignalingChannelEndpointInputRequestTypeDef,
     _OptionalGetSignalingChannelEndpointInputRequestTypeDef,
 ):
     pass
 
+
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredImageGenerationConfigurationOutputTypeDef",
+    {
+        "Status": ConfigurationStatusType,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "DestinationConfig": ImageGenerationDestinationConfigOutputTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalImageGenerationConfigurationOutputTypeDef",
+    {
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+    },
+    total=False,
+)
+
+
+class ImageGenerationConfigurationOutputTypeDef(
+    _RequiredImageGenerationConfigurationOutputTypeDef,
+    _OptionalImageGenerationConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
+
 class ImageGenerationConfigurationTypeDef(
     _RequiredImageGenerationConfigurationTypeDef, _OptionalImageGenerationConfigurationTypeDef
 ):
     pass
 
+
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -885,39 +1030,85 @@
         "MaxResults": int,
         "NextToken": str,
         "StreamNameCondition": StreamNameConditionTypeDef,
     },
     total=False,
 )
 
+UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelARN": str,
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+    },
+)
+
+NotificationConfigurationOutputTypeDef = TypedDict(
+    "NotificationConfigurationOutputTypeDef",
+    {
+        "Status": ConfigurationStatusType,
+        "DestinationConfig": NotificationDestinationConfigOutputTypeDef,
+    },
+)
+
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "DestinationConfig": NotificationDestinationConfigTypeDef,
     },
 )
 
+_RequiredRecorderConfigOutputTypeDef = TypedDict(
+    "_RequiredRecorderConfigOutputTypeDef",
+    {
+        "MediaSourceConfig": MediaSourceConfigOutputTypeDef,
+    },
+)
+_OptionalRecorderConfigOutputTypeDef = TypedDict(
+    "_OptionalRecorderConfigOutputTypeDef",
+    {
+        "ScheduleConfig": ScheduleConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RecorderConfigOutputTypeDef(
+    _RequiredRecorderConfigOutputTypeDef, _OptionalRecorderConfigOutputTypeDef
+):
+    pass
+
+
+UploaderConfigOutputTypeDef = TypedDict(
+    "UploaderConfigOutputTypeDef",
+    {
+        "ScheduleConfig": ScheduleConfigOutputTypeDef,
+    },
+)
+
 _RequiredRecorderConfigTypeDef = TypedDict(
     "_RequiredRecorderConfigTypeDef",
     {
         "MediaSourceConfig": MediaSourceConfigTypeDef,
     },
 )
 _OptionalRecorderConfigTypeDef = TypedDict(
     "_OptionalRecorderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
     total=False,
 )
 
+
 class RecorderConfigTypeDef(_RequiredRecorderConfigTypeDef, _OptionalRecorderConfigTypeDef):
     pass
 
+
 UploaderConfigTypeDef = TypedDict(
     "UploaderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
 )
 
@@ -937,15 +1128,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
+        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
@@ -955,29 +1146,50 @@
     },
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredEdgeConfigOutputTypeDef = TypedDict(
+    "_RequiredEdgeConfigOutputTypeDef",
+    {
+        "HubDeviceArn": str,
+        "RecorderConfig": RecorderConfigOutputTypeDef,
+    },
+)
+_OptionalEdgeConfigOutputTypeDef = TypedDict(
+    "_OptionalEdgeConfigOutputTypeDef",
+    {
+        "UploaderConfig": UploaderConfigOutputTypeDef,
+        "DeletionConfig": DeletionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EdgeConfigOutputTypeDef(_RequiredEdgeConfigOutputTypeDef, _OptionalEdgeConfigOutputTypeDef):
+    pass
+
+
 _RequiredEdgeConfigTypeDef = TypedDict(
     "_RequiredEdgeConfigTypeDef",
     {
         "HubDeviceArn": str,
         "RecorderConfig": RecorderConfigTypeDef,
     },
 )
@@ -986,46 +1198,62 @@
     {
         "UploaderConfig": UploaderConfigTypeDef,
         "DeletionConfig": DeletionConfigTypeDef,
     },
     total=False,
 )
 
+
 class EdgeConfigTypeDef(_RequiredEdgeConfigTypeDef, _OptionalEdgeConfigTypeDef):
     pass
 
+
 DescribeEdgeConfigurationOutputTypeDef = TypedDict(
     "DescribeEdgeConfigurationOutputTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigTypeDef,
+        "EdgeConfig": EdgeConfigOutputTypeDef,
         "EdgeAgentStatus": EdgeAgentStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigTypeDef,
+        "EdgeConfig": EdgeConfigOutputTypeDef,
     },
     total=False,
 )
 
+StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
+    "StartEdgeConfigurationUpdateOutputTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -1033,33 +1261,21 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class StartEdgeConfigurationUpdateInputRequestTypeDef(
     _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef,
     _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef,
 ):
     pass
 
-StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
-    "StartEdgeConfigurationUpdateOutputTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-        "SyncStatus": SyncStatusType,
-        "FailedStatusDetails": str,
-        "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
     "ListEdgeAgentConfigurationsOutputTypeDef",
     {
         "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
```

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.0
-Summary: Type annotations for boto3.KinesisVideo 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KinesisVideo 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kinesisvideo"></a>
 
 # mypy-boto3-kinesisvideo
 
 [![PyPI - mypy-boto3-kinesisvideo](https://img.shields.io/pypi/v/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesisvideo)](https://pepy.tech/project/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,96 +353,109 @@
 ### Typed dictionaries
 
 `mypy_boto3_kinesisvideo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
-    SingleMasterConfigurationTypeDef,
+    SingleMasterConfigurationOutputTypeDef,
     ChannelNameConditionTypeDef,
+    SingleMasterConfigurationTypeDef,
     TagTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamInputRequestTypeDef,
     CreateStreamOutputTypeDef,
     DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
+    LocalSizeConfigOutputTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
     DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationTypeDef,
+    MediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     LastRecorderStatusTypeDef,
     LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
     GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
+    ImageGenerationDestinationConfigOutputTypeDef,
     ImageGenerationDestinationConfigTypeDef,
     ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
+    MediaSourceConfigOutputTypeDef,
     MediaSourceConfigTypeDef,
+    MediaStorageConfigurationTypeDef,
+    NotificationDestinationConfigOutputTypeDef,
     NotificationDestinationConfigTypeDef,
     PaginatorConfigTypeDef,
+    ScheduleConfigOutputTypeDef,
     ScheduleConfigTypeDef,
     ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
-    UpdateSignalingChannelInputRequestTypeDef,
     ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
+    UpdateSignalingChannelInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    DeletionConfigOutputTypeDef,
     DeletionConfigTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
+    RecorderConfigOutputTypeDef,
+    UploaderConfigOutputTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
+    EdgeConfigOutputTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     ListEdgeAgentConfigurationsEdgeConfigTypeDef,
-    StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
+    StartEdgeConfigurationUpdateInputRequestTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_structure() -> SingleMasterConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kinesisvideo-1.28.0/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt` & `mypy-boto3-kinesisvideo-1.28.12/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.0/setup.py` & `mypy-boto3-kinesisvideo-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisvideo",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideo 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.KinesisVideo 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

