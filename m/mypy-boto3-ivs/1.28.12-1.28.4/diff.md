# Comparing `tmp/mypy-boto3-ivs-1.28.12.tar.gz` & `tmp/mypy-boto3-ivs-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-ivs-1.28.12.tar` & `mypy-boto3-ivs-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.504475 mypy-boto3-ivs-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-07-27 05:34:51.504475 mypy-boto3-ivs-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.484475 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-07-27 05:24:24.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-27 05:24:24.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-27 05:24:24.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-27 05:24:24.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-27 05:24:24.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28171 2023-07-27 05:24:24.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-27 05:24:24.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.504475 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-07-27 05:34:51.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:51.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:51.000000 mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.504475 mypy-boto3-ivs-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:24:23.000000 mypy-boto3-ivs-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.965310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26821 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/setup.py
```

### Comparing `mypy-boto3-ivs-1.28.12/LICENSE` & `mypy-boto3-ivs-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.12/PKG-INFO` & `mypy-boto3-ivs-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.12
-Summary: Type annotations for boto3.IVS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,14 +350,15 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
     BatchStartViewerSessionRevocationErrorTypeDef,
     BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     RenditionConfigurationTypeDef,
@@ -365,68 +366,67 @@
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
     S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
     RenditionConfigurationOutputTypeDef,
     ThumbnailConfigurationOutputTypeDef,
-    ResponseMetadataTypeDef,
     StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
     DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
     RecordingConfigurationSummaryTypeDef,
```

### Comparing `mypy-boto3-ivs-1.28.12/README.md` & `mypy-boto3-ivs-1.28.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,14 +318,15 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
     BatchStartViewerSessionRevocationErrorTypeDef,
     BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     RenditionConfigurationTypeDef,
@@ -333,68 +334,67 @@
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
     S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
     RenditionConfigurationOutputTypeDef,
     ThumbnailConfigurationOutputTypeDef,
-    ResponseMetadataTypeDef,
     StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
     DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
     RecordingConfigurationSummaryTypeDef,
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/__init__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/__init__.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/__main__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.IVS 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/client.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/client.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/literals.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -263,28 +262,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/literals.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -261,28 +260,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/paginator.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,98 +45,91 @@
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
     "ListStreamsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
         """
 
-
 class ListPlaybackKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlaybackKeyPairsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
         """
 
-
 class ListRecordingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecordingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
         """
 
-
 class ListStreamKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
     """
 
     def paginate(
-        self, *, channelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, channelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
         """
 
-
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/paginator.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,91 +45,98 @@
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
     "ListStreamsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
         """
 
+
 class ListPlaybackKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlaybackKeyPairsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
         """
 
+
 class ListRecordingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecordingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
         """
 
+
 class ListStreamKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
     """
 
     def paginate(
-        self, *, channelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, channelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
         """
 
+
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/type_defs.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
     "BatchStartViewerSessionRevocationErrorTypeDef",
     "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "RenditionConfigurationTypeDef",
@@ -51,68 +52,67 @@
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
     "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
     "StreamTypeDef",
     "GetStreamSessionRequestRequestTypeDef",
     "ImportPlaybackKeyPairRequestRequestTypeDef",
     "VideoConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     "PlaybackKeyPairSummaryTypeDef",
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
     "ListRecordingConfigurationsRequestRequestTypeDef",
-    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListStreamKeysRequestRequestTypeDef",
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutMetadataRequestRequestTypeDef",
     "RenditionConfigurationOutputTypeDef",
     "ThumbnailConfigurationOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
     "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
     "RecordingConfigurationSummaryTypeDef",
@@ -129,25 +129,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -164,15 +162,25 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -182,41 +190,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -245,15 +238,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -346,21 +338,14 @@
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -375,15 +360,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -410,15 +394,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -469,23 +452,22 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "filterByName": str,
-        "filterByRecordingConfigurationArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
@@ -493,22 +475,14 @@
         "filterByRecordingConfigurationArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaybackKeyPairsRequestRequestTypeDef = TypedDict(
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -517,56 +491,25 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
-)
-
-ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "channelArn": str,
-    },
-)
-_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
-    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
-    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStreamKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamKeysRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 _OptionalListStreamKeysRequestRequestTypeDef = TypedDict(
@@ -588,15 +531,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -622,15 +564,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -643,79 +584,47 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
 
 RenditionConfigurationOutputTypeDef = TypedDict(
     "RenditionConfigurationOutputTypeDef",
     {
         "renditionSelection": RenditionConfigurationRenditionSelectionType,
         "renditions": List[RenditionConfigurationRenditionType],
     },
-    total=False,
 )
 
 ThumbnailConfigurationOutputTypeDef = TypedDict(
     "ThumbnailConfigurationOutputTypeDef",
     {
         "recordingMode": RecordingModeType,
         "resolution": ThumbnailConfigurationResolutionType,
         "storage": List[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
@@ -747,15 +656,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -798,73 +706,88 @@
 
 
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamKeyResponseTypeDef = TypedDict(
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationResponseTypeDef",
     {
         "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
@@ -872,99 +795,145 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DestinationConfigurationOutputTypeDef = TypedDict(
     "DestinationConfigurationOutputTypeDef",
     {
         "s3": S3DestinationConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
 GetPlaybackKeyPairResponseTypeDef = TypedDict(
     "GetPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportPlaybackKeyPairResponseTypeDef = TypedDict(
     "ImportPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamResponseTypeDef = TypedDict(
     "GetStreamResponseTypeDef",
     {
         "stream": StreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
+)
+
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "filterByName": str,
+        "filterByRecordingConfigurationArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "channelArn": str,
+    },
+)
+_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
+    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
+    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
+):
+    pass
+
+
 ListPlaybackKeyPairsResponseTypeDef = TypedDict(
     "ListPlaybackKeyPairsResponseTypeDef",
     {
         "keyPairs": List[PlaybackKeyPairSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamKeysResponseTypeDef = TypedDict(
     "ListStreamKeysResponseTypeDef",
     {
         "nextToken": str,
         "streamKeys": List[StreamKeySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamSessionsResponseTypeDef = TypedDict(
     "ListStreamSessionsResponseTypeDef",
     {
         "nextToken": str,
         "streamSessions": List[StreamSessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsRequestListStreamsPaginateTypeDef",
     {
         "filterBy": StreamFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
@@ -976,69 +945,43 @@
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
         "arn": str,
         "destinationConfiguration": DestinationConfigurationOutputTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
         "name": str,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
         "destinationConfiguration": DestinationConfigurationOutputTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
-    {
         "name": str,
         "recordingReconnectWindowSeconds": int,
         "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
-):
-    pass
-
-
 _RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
     },
 )
 _OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
@@ -1062,48 +1005,47 @@
 
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecordingConfigurationResponseTypeDef = TypedDict(
     "CreateRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecordingConfigurationResponseTypeDef = TypedDict(
     "GetRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamSessionTypeDef = TypedDict(
     "StreamSessionTypeDef",
     {
         "channel": ChannelTypeDef,
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs/type_defs.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
     "BatchStartViewerSessionRevocationErrorTypeDef",
     "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "RenditionConfigurationTypeDef",
@@ -50,68 +51,67 @@
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
     "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
     "StreamTypeDef",
     "GetStreamSessionRequestRequestTypeDef",
     "ImportPlaybackKeyPairRequestRequestTypeDef",
     "VideoConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     "PlaybackKeyPairSummaryTypeDef",
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
     "ListRecordingConfigurationsRequestRequestTypeDef",
-    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListStreamKeysRequestRequestTypeDef",
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutMetadataRequestRequestTypeDef",
     "RenditionConfigurationOutputTypeDef",
     "ThumbnailConfigurationOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
     "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
     "RecordingConfigurationSummaryTypeDef",
@@ -128,25 +128,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -163,15 +161,25 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -181,39 +189,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -240,15 +235,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -339,21 +333,14 @@
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -368,15 +355,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -403,15 +389,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -458,23 +443,22 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "filterByName": str,
-        "filterByRecordingConfigurationArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
@@ -482,22 +466,14 @@
         "filterByRecordingConfigurationArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaybackKeyPairsRequestRequestTypeDef = TypedDict(
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -506,54 +482,25 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
-)
-
-ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "channelArn": str,
-    },
-)
-_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
-    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
-    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
-):
-    pass
-
 _RequiredListStreamKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamKeysRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 _OptionalListStreamKeysRequestRequestTypeDef = TypedDict(
@@ -573,15 +520,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -605,15 +551,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -626,79 +571,47 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
 
 RenditionConfigurationOutputTypeDef = TypedDict(
     "RenditionConfigurationOutputTypeDef",
     {
         "renditionSelection": RenditionConfigurationRenditionSelectionType,
         "renditions": List[RenditionConfigurationRenditionType],
     },
-    total=False,
 )
 
 ThumbnailConfigurationOutputTypeDef = TypedDict(
     "ThumbnailConfigurationOutputTypeDef",
     {
         "recordingMode": RecordingModeType,
         "resolution": ThumbnailConfigurationResolutionType,
         "storage": List[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
@@ -728,15 +641,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -777,73 +689,88 @@
     pass
 
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamKeyResponseTypeDef = TypedDict(
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationResponseTypeDef",
     {
         "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
@@ -851,99 +778,143 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DestinationConfigurationOutputTypeDef = TypedDict(
     "DestinationConfigurationOutputTypeDef",
     {
         "s3": S3DestinationConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
 GetPlaybackKeyPairResponseTypeDef = TypedDict(
     "GetPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportPlaybackKeyPairResponseTypeDef = TypedDict(
     "ImportPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamResponseTypeDef = TypedDict(
     "GetStreamResponseTypeDef",
     {
         "stream": StreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
+)
+
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "filterByName": str,
+        "filterByRecordingConfigurationArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "channelArn": str,
+    },
+)
+_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
+    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
+    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
+):
+    pass
+
 ListPlaybackKeyPairsResponseTypeDef = TypedDict(
     "ListPlaybackKeyPairsResponseTypeDef",
     {
         "keyPairs": List[PlaybackKeyPairSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamKeysResponseTypeDef = TypedDict(
     "ListStreamKeysResponseTypeDef",
     {
         "nextToken": str,
         "streamKeys": List[StreamKeySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamSessionsResponseTypeDef = TypedDict(
     "ListStreamSessionsResponseTypeDef",
     {
         "nextToken": str,
         "streamSessions": List[StreamSessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsRequestListStreamsPaginateTypeDef",
     {
         "filterBy": StreamFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
@@ -955,65 +926,43 @@
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
         "arn": str,
         "destinationConfiguration": DestinationConfigurationOutputTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
         "name": str,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
         "destinationConfiguration": DestinationConfigurationOutputTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
-    {
         "name": str,
         "recordingReconnectWindowSeconds": int,
         "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
-):
-    pass
-
 _RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
     },
 )
 _OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
@@ -1035,48 +984,47 @@
     pass
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecordingConfigurationResponseTypeDef = TypedDict(
     "CreateRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecordingConfigurationResponseTypeDef = TypedDict(
     "GetRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamSessionTypeDef = TypedDict(
     "StreamSessionTypeDef",
     {
         "channel": ChannelTypeDef,
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.12
-Summary: Type annotations for boto3.IVS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,14 +350,15 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
     BatchStartViewerSessionRevocationErrorTypeDef,
     BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
     RenditionConfigurationTypeDef,
@@ -365,68 +366,67 @@
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
     S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
     RenditionConfigurationOutputTypeDef,
     ThumbnailConfigurationOutputTypeDef,
-    ResponseMetadataTypeDef,
     StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
     DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
     RecordingConfigurationSummaryTypeDef,
```

### Comparing `mypy-boto3-ivs-1.28.12/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.12/setup.py` & `mypy-boto3-ivs-1.28.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.28.12",
+    version="1.28.4",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IVS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

