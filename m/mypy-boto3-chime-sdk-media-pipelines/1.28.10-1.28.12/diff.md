# Comparing `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.10.tar.gz` & `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10.tar` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57824 2023-07-24 19:47:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57781 2023-07-24 19:46:59.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 19:49:46.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:49:46.288631 mypy-boto3-chime-sdk-media-pipelines-1.28.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-24 19:46:58.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.876567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21021 2023-07-27 05:34:22.872567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.872567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63499 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63426 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.872567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21021 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.876567 mypy-boto3-chime-sdk-media-pipelines-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-27 05:18:15.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.12/setup.py
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/LICENSE` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.10
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,19 +368,19 @@
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     HorizontalLayoutConfigurationOutputTypeDef,
     PresenterOnlyConfigurationOutputTypeDef,
@@ -417,28 +417,28 @@
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     S3RecordingSinkRuntimeConfigurationOutputTypeDef,
     SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
     GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/README.md` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,19 +336,19 @@
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     HorizontalLayoutConfigurationOutputTypeDef,
     PresenterOnlyConfigurationOutputTypeDef,
@@ -385,28 +385,28 @@
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     S3RecordingSinkRuntimeConfigurationOutputTypeDef,
     SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
     GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/__main__.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10\nVersion:        "
-        " 1.28.10\nBuilder version: 7.15.1\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.10")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/client.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
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
@@ -324,14 +325,15 @@
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

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/literals.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,15 @@
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
@@ -322,14 +323,15 @@
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

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,19 +83,19 @@
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "ChannelDefinitionOutputTypeDef",
     "ChannelDefinitionTypeDef",
     "S3BucketSinkConfigurationOutputTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TimestampRangeOutputTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "HorizontalLayoutConfigurationOutputTypeDef",
     "PresenterOnlyConfigurationOutputTypeDef",
@@ -132,28 +132,28 @@
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
     "SentimentConfigurationOutputTypeDef",
     "SentimentConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationOutputTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkOutputTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FragmentSelectorOutputTypeDef",
     "FragmentSelectorTypeDef",
     "GridViewConfigurationOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
@@ -214,34 +214,48 @@
 )
 
 ActiveSpeakerOnlyConfigurationOutputTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationOutputTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
     },
+    total=False,
 )
 
 ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
     },
     total=False,
 )
 
-PostCallAnalyticsSettingsOutputTypeDef = TypedDict(
-    "PostCallAnalyticsSettingsOutputTypeDef",
+_RequiredPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
+    "_RequiredPostCallAnalyticsSettingsOutputTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
+    },
+)
+_OptionalPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
+    "_OptionalPostCallAnalyticsSettingsOutputTypeDef",
+    {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
+    total=False,
 )
 
+
+class PostCallAnalyticsSettingsOutputTypeDef(
+    _RequiredPostCallAnalyticsSettingsOutputTypeDef, _OptionalPostCallAnalyticsSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -278,14 +292,15 @@
         "FilterPartialResults": bool,
         "IdentifyLanguage": bool,
         "LanguageOptions": str,
         "PreferredLanguage": CallAnalyticsLanguageCodeType,
         "VocabularyNames": str,
         "VocabularyFilterNames": str,
     },
+    total=False,
 )
 
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
@@ -409,30 +424,58 @@
 AudioArtifactsConfigurationOutputTypeDef = TypedDict(
     "AudioArtifactsConfigurationOutputTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
-ContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "ContentArtifactsConfigurationOutputTypeDef",
+_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContentArtifactsConfigurationOutputTypeDef",
     {
         "State": ArtifactsStateType,
+    },
+)
+_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContentArtifactsConfigurationOutputTypeDef",
+    {
         "MuxType": Literal["ContentOnly"],
     },
+    total=False,
 )
 
-VideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "VideoArtifactsConfigurationOutputTypeDef",
+
+class ContentArtifactsConfigurationOutputTypeDef(
+    _RequiredContentArtifactsConfigurationOutputTypeDef,
+    _OptionalContentArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
+
+_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
     {
         "State": ArtifactsStateType,
+    },
+)
+_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
+    {
         "MuxType": Literal["VideoOnly"],
     },
+    total=False,
 )
 
+
+class VideoArtifactsConfigurationOutputTypeDef(
+    _RequiredVideoArtifactsConfigurationOutputTypeDef,
+    _OptionalVideoArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
+
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -474,22 +517,35 @@
 
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
 
-ChannelDefinitionOutputTypeDef = TypedDict(
-    "ChannelDefinitionOutputTypeDef",
+_RequiredChannelDefinitionOutputTypeDef = TypedDict(
+    "_RequiredChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
+    },
+)
+_OptionalChannelDefinitionOutputTypeDef = TypedDict(
+    "_OptionalChannelDefinitionOutputTypeDef",
+    {
         "ParticipantRole": ParticipantRoleType,
     },
+    total=False,
 )
 
+
+class ChannelDefinitionOutputTypeDef(
+    _RequiredChannelDefinitionOutputTypeDef, _OptionalChannelDefinitionOutputTypeDef
+):
+    pass
+
+
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
@@ -525,25 +581,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
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
-
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -565,14 +610,21 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimestampRangeOutputTypeDef = TypedDict(
     "TimestampRangeOutputTypeDef",
     {
         "StartTimestamp": datetime,
         "EndTimestamp": datetime,
     },
 )
@@ -610,41 +662,45 @@
     "HorizontalLayoutConfigurationOutputTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": HorizontalTilePositionType,
         "TileCount": int,
         "TileAspectRatio": str,
     },
+    total=False,
 )
 
 PresenterOnlyConfigurationOutputTypeDef = TypedDict(
     "PresenterOnlyConfigurationOutputTypeDef",
     {
         "PresenterPosition": PresenterPositionType,
     },
+    total=False,
 )
 
 VerticalLayoutConfigurationOutputTypeDef = TypedDict(
     "VerticalLayoutConfigurationOutputTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": VerticalTilePositionType,
         "TileCount": int,
         "TileAspectRatio": str,
     },
+    total=False,
 )
 
 VideoAttributeOutputTypeDef = TypedDict(
     "VideoAttributeOutputTypeDef",
     {
         "CornerRadius": int,
         "BorderColor": BorderColorType,
         "HighlightColor": HighlightColorType,
         "BorderThickness": int,
     },
+    total=False,
 )
 
 HorizontalLayoutConfigurationTypeDef = TypedDict(
     "HorizontalLayoutConfigurationTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": HorizontalTilePositionType,
@@ -694,23 +750,36 @@
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
-KeywordMatchConfigurationOutputTypeDef = TypedDict(
-    "KeywordMatchConfigurationOutputTypeDef",
+_RequiredKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKeywordMatchConfigurationOutputTypeDef",
     {
         "RuleName": str,
         "Keywords": List[str],
+    },
+)
+_OptionalKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKeywordMatchConfigurationOutputTypeDef",
+    {
         "Negate": bool,
     },
+    total=False,
 )
 
+
+class KeywordMatchConfigurationOutputTypeDef(
+    _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -730,14 +799,15 @@
 
 
 KinesisDataStreamSinkConfigurationOutputTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
@@ -745,14 +815,15 @@
 )
 
 RecordingStreamConfigurationOutputTypeDef = TypedDict(
     "RecordingStreamConfigurationOutputTypeDef",
     {
         "StreamArn": str,
     },
+    total=False,
 )
 
 RecordingStreamConfigurationTypeDef = TypedDict(
     "RecordingStreamConfigurationTypeDef",
     {
         "StreamArn": str,
     },
@@ -760,14 +831,15 @@
 )
 
 LambdaFunctionSinkConfigurationOutputTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 LambdaFunctionSinkConfigurationTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
@@ -785,14 +857,15 @@
 
 MediaCapturePipelineSummaryTypeDef = TypedDict(
     "MediaCapturePipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
+    total=False,
 )
 
 ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -803,14 +876,15 @@
 MediaInsightsPipelineConfigurationSummaryTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationId": str,
         "MediaInsightsPipelineConfigurationArn": str,
     },
+    total=False,
 )
 
 ListMediaPipelinesRequestRequestTypeDef = TypedDict(
     "ListMediaPipelinesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -820,14 +894,15 @@
 
 MediaPipelineSummaryTypeDef = TypedDict(
     "MediaPipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
+    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
@@ -837,23 +912,37 @@
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-LiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
-    "LiveConnectorRTMPConfigurationOutputTypeDef",
+_RequiredLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLiveConnectorRTMPConfigurationOutputTypeDef",
     {
         "Url": str,
+    },
+)
+_OptionalLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLiveConnectorRTMPConfigurationOutputTypeDef",
+    {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
+    total=False,
 )
 
+
+class LiveConnectorRTMPConfigurationOutputTypeDef(
+    _RequiredLiveConnectorRTMPConfigurationOutputTypeDef,
+    _OptionalLiveConnectorRTMPConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredLiveConnectorRTMPConfigurationTypeDef = TypedDict(
     "_RequiredLiveConnectorRTMPConfigurationTypeDef",
     {
         "Url": str,
     },
 )
 _OptionalLiveConnectorRTMPConfigurationTypeDef = TypedDict(
@@ -874,36 +963,40 @@
 
 S3RecordingSinkConfigurationOutputTypeDef = TypedDict(
     "S3RecordingSinkConfigurationOutputTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
+    total=False,
 )
 
 SnsTopicSinkConfigurationOutputTypeDef = TypedDict(
     "SnsTopicSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 SqsQueueSinkConfigurationOutputTypeDef = TypedDict(
     "SqsQueueSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 VoiceAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
     "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
     {
         "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
         "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
     },
+    total=False,
 )
 
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
@@ -958,20 +1051,32 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
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
 SelectedVideoStreamsOutputTypeDef = TypedDict(
     "SelectedVideoStreamsOutputTypeDef",
     {
         "AttendeeIds": List[str],
         "ExternalUserIds": List[str],
     },
+    total=False,
 )
 
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
@@ -991,33 +1096,47 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
-AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
+    },
+)
+_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsOutputTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
+    total=False,
 )
 
+
+class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
+    _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+    _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -1069,22 +1188,35 @@
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
-StreamChannelDefinitionOutputTypeDef = TypedDict(
-    "StreamChannelDefinitionOutputTypeDef",
+_RequiredStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_RequiredStreamChannelDefinitionOutputTypeDef",
     {
         "NumberOfChannels": int,
+    },
+)
+_OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_OptionalStreamChannelDefinitionOutputTypeDef",
+    {
         "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
+    total=False,
 )
 
+
+class StreamChannelDefinitionOutputTypeDef(
+    _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
+):
+    pass
+
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
@@ -1122,21 +1254,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 FragmentSelectorOutputTypeDef = TypedDict(
     "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
@@ -1145,27 +1270,40 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
-GridViewConfigurationOutputTypeDef = TypedDict(
-    "GridViewConfigurationOutputTypeDef",
+_RequiredGridViewConfigurationOutputTypeDef = TypedDict(
+    "_RequiredGridViewConfigurationOutputTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
+    },
+)
+_OptionalGridViewConfigurationOutputTypeDef = TypedDict(
+    "_OptionalGridViewConfigurationOutputTypeDef",
+    {
         "PresenterOnlyConfiguration": PresenterOnlyConfigurationOutputTypeDef,
         "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationOutputTypeDef,
         "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationOutputTypeDef,
         "VerticalLayoutConfiguration": VerticalLayoutConfigurationOutputTypeDef,
         "VideoAttribute": VideoAttributeOutputTypeDef,
         "CanvasOrientation": CanvasOrientationType,
     },
+    total=False,
 )
 
+
+class GridViewConfigurationOutputTypeDef(
+    _RequiredGridViewConfigurationOutputTypeDef, _OptionalGridViewConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -1189,43 +1327,43 @@
 
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LiveConnectorSinkConfigurationOutputTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationOutputTypeDef",
     {
         "SinkType": Literal["RTMP"],
@@ -1237,24 +1375,37 @@
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
-RealTimeAlertRuleOutputTypeDef = TypedDict(
-    "RealTimeAlertRuleOutputTypeDef",
+_RequiredRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_RequiredRealTimeAlertRuleOutputTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
+    },
+)
+_OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_OptionalRealTimeAlertRuleOutputTypeDef",
+    {
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
         "SentimentConfiguration": SentimentConfigurationOutputTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+
+class RealTimeAlertRuleOutputTypeDef(
+    _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -1275,43 +1426,58 @@
 
 
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
     },
+    total=False,
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
-MediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
+_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
+    },
+)
+_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
         "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
             AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
         ),
         "AmazonTranscribeProcessorConfiguration": (
             AmazonTranscribeProcessorConfigurationOutputTypeDef
         ),
         "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationOutputTypeDef,
         "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationOutputTypeDef,
         "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationOutputTypeDef,
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationOutputTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationOutputTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+
+class MediaInsightsPipelineConfigurationElementOutputTypeDef(
+    _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
+    _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
+):
+    pass
+
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -1349,22 +1515,35 @@
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
-StreamConfigurationOutputTypeDef = TypedDict(
-    "StreamConfigurationOutputTypeDef",
+_RequiredStreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamConfigurationOutputTypeDef",
     {
         "StreamArn": str,
-        "FragmentNumber": str,
         "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
     },
 )
+_OptionalStreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamConfigurationOutputTypeDef",
+    {
+        "FragmentNumber": str,
+    },
+    total=False,
+)
+
+
+class StreamConfigurationOutputTypeDef(
+    _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
+):
+    pass
+
 
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
@@ -1396,23 +1575,37 @@
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
 
-CompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "CompositedVideoArtifactsConfigurationOutputTypeDef",
+_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
+    },
+)
+_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef",
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
-        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+
+class CompositedVideoArtifactsConfigurationOutputTypeDef(
+    _RequiredCompositedVideoArtifactsConfigurationOutputTypeDef,
+    _OptionalCompositedVideoArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1434,14 +1627,15 @@
 
 RealTimeAlertConfigurationOutputTypeDef = TypedDict(
     "RealTimeAlertConfigurationOutputTypeDef",
     {
         "Disabled": bool,
         "Rules": List[RealTimeAlertRuleOutputTypeDef],
     },
+    total=False,
 )
 
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
@@ -1479,34 +1673,61 @@
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
 )
 
-ArtifactsConfigurationOutputTypeDef = TypedDict(
-    "ArtifactsConfigurationOutputTypeDef",
+_RequiredArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredArtifactsConfigurationOutputTypeDef",
     {
         "Audio": AudioArtifactsConfigurationOutputTypeDef,
         "Video": VideoArtifactsConfigurationOutputTypeDef,
         "Content": ContentArtifactsConfigurationOutputTypeDef,
+    },
+)
+_OptionalArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalArtifactsConfigurationOutputTypeDef",
+    {
         "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
-ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+
+class ArtifactsConfigurationOutputTypeDef(
+    _RequiredArtifactsConfigurationOutputTypeDef, _OptionalArtifactsConfigurationOutputTypeDef
+):
+    pass
+
+
+_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
+    },
+)
+_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
         "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+
+class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
+    _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+    _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredArtifactsConfigurationTypeDef",
     {
         "Audio": AudioArtifactsConfigurationTypeDef,
         "Video": VideoArtifactsConfigurationTypeDef,
         "Content": ContentArtifactsConfigurationTypeDef,
     },
@@ -1558,14 +1779,15 @@
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
         "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
         "MediaInsightsPipelineConfigurationId": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
@@ -1645,14 +1867,15 @@
         "MediaInsightsRuntimeMetadata": Dict[str, str],
         "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
             KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
         ),
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationOutputTypeDef,
         "CreatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationArn": str,
     },
@@ -1684,14 +1907,15 @@
 
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationOutputTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
@@ -1719,45 +1943,46 @@
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceOutputTypeDef],
         "Sinks": List[ConcatenationSinkOutputTypeDef],
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
@@ -1780,15 +2005,15 @@
     pass
 
 
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
@@ -1798,27 +2023,29 @@
         "Status": MediaPipelineStatusType,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationOutputTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
@@ -1868,52 +2095,53 @@
     pass
 
 
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
+    total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -82,19 +82,19 @@
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "ChannelDefinitionOutputTypeDef",
     "ChannelDefinitionTypeDef",
     "S3BucketSinkConfigurationOutputTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TimestampRangeOutputTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "HorizontalLayoutConfigurationOutputTypeDef",
     "PresenterOnlyConfigurationOutputTypeDef",
@@ -131,28 +131,28 @@
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "S3RecordingSinkRuntimeConfigurationOutputTypeDef",
     "SentimentConfigurationOutputTypeDef",
     "SentimentConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationOutputTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkOutputTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FragmentSelectorOutputTypeDef",
     "FragmentSelectorTypeDef",
     "GridViewConfigurationOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
@@ -213,34 +213,46 @@
 )
 
 ActiveSpeakerOnlyConfigurationOutputTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationOutputTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
     },
+    total=False,
 )
 
 ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
     "ActiveSpeakerOnlyConfigurationTypeDef",
     {
         "ActiveSpeakerPosition": ActiveSpeakerPositionType,
     },
     total=False,
 )
 
-PostCallAnalyticsSettingsOutputTypeDef = TypedDict(
-    "PostCallAnalyticsSettingsOutputTypeDef",
+_RequiredPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
+    "_RequiredPostCallAnalyticsSettingsOutputTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
+    },
+)
+_OptionalPostCallAnalyticsSettingsOutputTypeDef = TypedDict(
+    "_OptionalPostCallAnalyticsSettingsOutputTypeDef",
+    {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
+    total=False,
 )
 
+class PostCallAnalyticsSettingsOutputTypeDef(
+    _RequiredPostCallAnalyticsSettingsOutputTypeDef, _OptionalPostCallAnalyticsSettingsOutputTypeDef
+):
+    pass
+
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -275,14 +287,15 @@
         "FilterPartialResults": bool,
         "IdentifyLanguage": bool,
         "LanguageOptions": str,
         "PreferredLanguage": CallAnalyticsLanguageCodeType,
         "VocabularyNames": str,
         "VocabularyFilterNames": str,
     },
+    total=False,
 )
 
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
@@ -406,30 +419,54 @@
 AudioArtifactsConfigurationOutputTypeDef = TypedDict(
     "AudioArtifactsConfigurationOutputTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
-ContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "ContentArtifactsConfigurationOutputTypeDef",
+_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContentArtifactsConfigurationOutputTypeDef",
     {
         "State": ArtifactsStateType,
+    },
+)
+_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContentArtifactsConfigurationOutputTypeDef",
+    {
         "MuxType": Literal["ContentOnly"],
     },
+    total=False,
 )
 
-VideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "VideoArtifactsConfigurationOutputTypeDef",
+class ContentArtifactsConfigurationOutputTypeDef(
+    _RequiredContentArtifactsConfigurationOutputTypeDef,
+    _OptionalContentArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
     {
         "State": ArtifactsStateType,
+    },
+)
+_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
+    {
         "MuxType": Literal["VideoOnly"],
     },
+    total=False,
 )
 
+class VideoArtifactsConfigurationOutputTypeDef(
+    _RequiredVideoArtifactsConfigurationOutputTypeDef,
+    _OptionalVideoArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -467,22 +504,33 @@
 )
 
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
-ChannelDefinitionOutputTypeDef = TypedDict(
-    "ChannelDefinitionOutputTypeDef",
+_RequiredChannelDefinitionOutputTypeDef = TypedDict(
+    "_RequiredChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
+    },
+)
+_OptionalChannelDefinitionOutputTypeDef = TypedDict(
+    "_OptionalChannelDefinitionOutputTypeDef",
+    {
         "ParticipantRole": ParticipantRoleType,
     },
+    total=False,
 )
 
+class ChannelDefinitionOutputTypeDef(
+    _RequiredChannelDefinitionOutputTypeDef, _OptionalChannelDefinitionOutputTypeDef
+):
+    pass
+
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
@@ -516,25 +564,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
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
-
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -556,14 +593,21 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimestampRangeOutputTypeDef = TypedDict(
     "TimestampRangeOutputTypeDef",
     {
         "StartTimestamp": datetime,
         "EndTimestamp": datetime,
     },
 )
@@ -601,41 +645,45 @@
     "HorizontalLayoutConfigurationOutputTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": HorizontalTilePositionType,
         "TileCount": int,
         "TileAspectRatio": str,
     },
+    total=False,
 )
 
 PresenterOnlyConfigurationOutputTypeDef = TypedDict(
     "PresenterOnlyConfigurationOutputTypeDef",
     {
         "PresenterPosition": PresenterPositionType,
     },
+    total=False,
 )
 
 VerticalLayoutConfigurationOutputTypeDef = TypedDict(
     "VerticalLayoutConfigurationOutputTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": VerticalTilePositionType,
         "TileCount": int,
         "TileAspectRatio": str,
     },
+    total=False,
 )
 
 VideoAttributeOutputTypeDef = TypedDict(
     "VideoAttributeOutputTypeDef",
     {
         "CornerRadius": int,
         "BorderColor": BorderColorType,
         "HighlightColor": HighlightColorType,
         "BorderThickness": int,
     },
+    total=False,
 )
 
 HorizontalLayoutConfigurationTypeDef = TypedDict(
     "HorizontalLayoutConfigurationTypeDef",
     {
         "TileOrder": TileOrderType,
         "TilePosition": HorizontalTilePositionType,
@@ -685,23 +733,34 @@
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
-KeywordMatchConfigurationOutputTypeDef = TypedDict(
-    "KeywordMatchConfigurationOutputTypeDef",
+_RequiredKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKeywordMatchConfigurationOutputTypeDef",
     {
         "RuleName": str,
         "Keywords": List[str],
+    },
+)
+_OptionalKeywordMatchConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKeywordMatchConfigurationOutputTypeDef",
+    {
         "Negate": bool,
     },
+    total=False,
 )
 
+class KeywordMatchConfigurationOutputTypeDef(
+    _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -719,14 +778,15 @@
     pass
 
 KinesisDataStreamSinkConfigurationOutputTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
@@ -734,14 +794,15 @@
 )
 
 RecordingStreamConfigurationOutputTypeDef = TypedDict(
     "RecordingStreamConfigurationOutputTypeDef",
     {
         "StreamArn": str,
     },
+    total=False,
 )
 
 RecordingStreamConfigurationTypeDef = TypedDict(
     "RecordingStreamConfigurationTypeDef",
     {
         "StreamArn": str,
     },
@@ -749,14 +810,15 @@
 )
 
 LambdaFunctionSinkConfigurationOutputTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 LambdaFunctionSinkConfigurationTypeDef = TypedDict(
     "LambdaFunctionSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
@@ -774,14 +836,15 @@
 
 MediaCapturePipelineSummaryTypeDef = TypedDict(
     "MediaCapturePipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
+    total=False,
 )
 
 ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -792,14 +855,15 @@
 MediaInsightsPipelineConfigurationSummaryTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationSummaryTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationId": str,
         "MediaInsightsPipelineConfigurationArn": str,
     },
+    total=False,
 )
 
 ListMediaPipelinesRequestRequestTypeDef = TypedDict(
     "ListMediaPipelinesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -809,14 +873,15 @@
 
 MediaPipelineSummaryTypeDef = TypedDict(
     "MediaPipelineSummaryTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
     },
+    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
@@ -826,23 +891,35 @@
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-LiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
-    "LiveConnectorRTMPConfigurationOutputTypeDef",
+_RequiredLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLiveConnectorRTMPConfigurationOutputTypeDef",
     {
         "Url": str,
+    },
+)
+_OptionalLiveConnectorRTMPConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLiveConnectorRTMPConfigurationOutputTypeDef",
+    {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
+    total=False,
 )
 
+class LiveConnectorRTMPConfigurationOutputTypeDef(
+    _RequiredLiveConnectorRTMPConfigurationOutputTypeDef,
+    _OptionalLiveConnectorRTMPConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredLiveConnectorRTMPConfigurationTypeDef = TypedDict(
     "_RequiredLiveConnectorRTMPConfigurationTypeDef",
     {
         "Url": str,
     },
 )
 _OptionalLiveConnectorRTMPConfigurationTypeDef = TypedDict(
@@ -861,36 +938,40 @@
 
 S3RecordingSinkConfigurationOutputTypeDef = TypedDict(
     "S3RecordingSinkConfigurationOutputTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
+    total=False,
 )
 
 SnsTopicSinkConfigurationOutputTypeDef = TypedDict(
     "SnsTopicSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 SqsQueueSinkConfigurationOutputTypeDef = TypedDict(
     "SqsQueueSinkConfigurationOutputTypeDef",
     {
         "InsightsTarget": str,
     },
+    total=False,
 )
 
 VoiceAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
     "VoiceAnalyticsProcessorConfigurationOutputTypeDef",
     {
         "SpeakerSearchStatus": VoiceAnalyticsConfigurationStatusType,
         "VoiceToneAnalysisStatus": VoiceAnalyticsConfigurationStatusType,
     },
+    total=False,
 )
 
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
@@ -945,20 +1026,32 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
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
 SelectedVideoStreamsOutputTypeDef = TypedDict(
     "SelectedVideoStreamsOutputTypeDef",
     {
         "AttendeeIds": List[str],
         "ExternalUserIds": List[str],
     },
+    total=False,
 )
 
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
@@ -978,33 +1071,45 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
-AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
+    },
+)
+_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
+    {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsOutputTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
+    total=False,
 )
 
+class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
+    _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+    _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -1054,22 +1159,33 @@
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
-StreamChannelDefinitionOutputTypeDef = TypedDict(
-    "StreamChannelDefinitionOutputTypeDef",
+_RequiredStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_RequiredStreamChannelDefinitionOutputTypeDef",
     {
         "NumberOfChannels": int,
+    },
+)
+_OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
+    "_OptionalStreamChannelDefinitionOutputTypeDef",
+    {
         "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
+    total=False,
 )
 
+class StreamChannelDefinitionOutputTypeDef(
+    _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
+):
+    pass
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
@@ -1105,21 +1221,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 FragmentSelectorOutputTypeDef = TypedDict(
     "FragmentSelectorOutputTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeOutputTypeDef,
     },
 )
@@ -1128,27 +1237,38 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
-GridViewConfigurationOutputTypeDef = TypedDict(
-    "GridViewConfigurationOutputTypeDef",
+_RequiredGridViewConfigurationOutputTypeDef = TypedDict(
+    "_RequiredGridViewConfigurationOutputTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
+    },
+)
+_OptionalGridViewConfigurationOutputTypeDef = TypedDict(
+    "_OptionalGridViewConfigurationOutputTypeDef",
+    {
         "PresenterOnlyConfiguration": PresenterOnlyConfigurationOutputTypeDef,
         "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationOutputTypeDef,
         "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationOutputTypeDef,
         "VerticalLayoutConfiguration": VerticalLayoutConfigurationOutputTypeDef,
         "VideoAttribute": VideoAttributeOutputTypeDef,
         "CanvasOrientation": CanvasOrientationType,
     },
+    total=False,
 )
 
+class GridViewConfigurationOutputTypeDef(
+    _RequiredGridViewConfigurationOutputTypeDef, _OptionalGridViewConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -1170,43 +1290,43 @@
     pass
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LiveConnectorSinkConfigurationOutputTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationOutputTypeDef",
     {
         "SinkType": Literal["RTMP"],
@@ -1218,24 +1338,35 @@
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
-RealTimeAlertRuleOutputTypeDef = TypedDict(
-    "RealTimeAlertRuleOutputTypeDef",
+_RequiredRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_RequiredRealTimeAlertRuleOutputTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
+    },
+)
+_OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
+    "_OptionalRealTimeAlertRuleOutputTypeDef",
+    {
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
         "SentimentConfiguration": SentimentConfigurationOutputTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+class RealTimeAlertRuleOutputTypeDef(
+    _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
+):
+    pass
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -1254,43 +1385,56 @@
     pass
 
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
     },
+    total=False,
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
-MediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
+_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
+    },
+)
+_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
+    "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
+    {
         "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
             AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
         ),
         "AmazonTranscribeProcessorConfiguration": (
             AmazonTranscribeProcessorConfigurationOutputTypeDef
         ),
         "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationOutputTypeDef,
         "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationOutputTypeDef,
         "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationOutputTypeDef,
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationOutputTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationOutputTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+class MediaInsightsPipelineConfigurationElementOutputTypeDef(
+    _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
+    _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
+):
+    pass
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -1326,22 +1470,33 @@
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
-StreamConfigurationOutputTypeDef = TypedDict(
-    "StreamConfigurationOutputTypeDef",
+_RequiredStreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamConfigurationOutputTypeDef",
     {
         "StreamArn": str,
-        "FragmentNumber": str,
         "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
     },
 )
+_OptionalStreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamConfigurationOutputTypeDef",
+    {
+        "FragmentNumber": str,
+    },
+    total=False,
+)
+
+class StreamConfigurationOutputTypeDef(
+    _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
@@ -1371,23 +1526,35 @@
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
 
-CompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "CompositedVideoArtifactsConfigurationOutputTypeDef",
+_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCompositedVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
+    },
+)
+_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCompositedVideoArtifactsConfigurationOutputTypeDef",
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
-        "GridViewConfiguration": GridViewConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+class CompositedVideoArtifactsConfigurationOutputTypeDef(
+    _RequiredCompositedVideoArtifactsConfigurationOutputTypeDef,
+    _OptionalCompositedVideoArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1407,14 +1574,15 @@
 
 RealTimeAlertConfigurationOutputTypeDef = TypedDict(
     "RealTimeAlertConfigurationOutputTypeDef",
     {
         "Disabled": bool,
         "Rules": List[RealTimeAlertRuleOutputTypeDef],
     },
+    total=False,
 )
 
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
@@ -1452,34 +1620,57 @@
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
 )
 
-ArtifactsConfigurationOutputTypeDef = TypedDict(
-    "ArtifactsConfigurationOutputTypeDef",
+_RequiredArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredArtifactsConfigurationOutputTypeDef",
     {
         "Audio": AudioArtifactsConfigurationOutputTypeDef,
         "Video": VideoArtifactsConfigurationOutputTypeDef,
         "Content": ContentArtifactsConfigurationOutputTypeDef,
+    },
+)
+_OptionalArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalArtifactsConfigurationOutputTypeDef",
+    {
         "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
-ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+class ArtifactsConfigurationOutputTypeDef(
+    _RequiredArtifactsConfigurationOutputTypeDef, _OptionalArtifactsConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
+    },
+)
+_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
+    {
         "CompositedVideo": CompositedVideoArtifactsConfigurationOutputTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
+class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
+    _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+    _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredArtifactsConfigurationTypeDef",
     {
         "Audio": AudioArtifactsConfigurationTypeDef,
         "Video": VideoArtifactsConfigurationTypeDef,
         "Content": ContentArtifactsConfigurationTypeDef,
     },
@@ -1527,14 +1718,15 @@
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
         "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
         "MediaInsightsPipelineConfigurationId": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
@@ -1610,14 +1802,15 @@
         "MediaInsightsRuntimeMetadata": Dict[str, str],
         "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
             KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
         ),
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationOutputTypeDef,
         "CreatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationArn": str,
     },
@@ -1647,14 +1840,15 @@
 
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationOutputTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
@@ -1682,45 +1876,46 @@
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceOutputTypeDef],
         "Sinks": List[ConcatenationSinkOutputTypeDef],
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
@@ -1741,15 +1936,15 @@
 ):
     pass
 
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
@@ -1759,27 +1954,29 @@
         "Status": MediaPipelineStatusType,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationOutputTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
@@ -1825,52 +2022,53 @@
 ):
     pass
 
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
+    total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.10
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-media-pipelines)](https://pepy.tech/project/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,19 +368,19 @@
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionOutputTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationOutputTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     TimestampRangeOutputTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     HorizontalLayoutConfigurationOutputTypeDef,
     PresenterOnlyConfigurationOutputTypeDef,
@@ -417,28 +417,28 @@
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     S3RecordingSinkRuntimeConfigurationOutputTypeDef,
     SentimentConfigurationOutputTypeDef,
     SentimentConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationOutputTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionOutputTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkOutputTypeDef,
     ConcatenationSinkTypeDef,
     TagResourceRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     FragmentSelectorOutputTypeDef,
     FragmentSelectorTypeDef,
     GridViewConfigurationOutputTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.10/setup.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.12/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-media-pipelines",
-    version="1.28.10",
+    version="1.28.12",
     packages=["mypy_boto3_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.10 service generated with"
-        " mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

