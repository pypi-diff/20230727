# Comparing `tmp/mypy-boto3-elastictranscoder-1.28.0.tar.gz` & `tmp/mypy-boto3-elastictranscoder-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elastictranscoder-1.28.0.tar", last modified: Thu Jul  6 20:59:31 2023, max compression
+gzip compressed data, was "mypy-boto3-elastictranscoder-1.28.12.tar", last modified: Thu Jul 27 05:34:39 2023, max compression
```

## Comparing `mypy-boto3-elastictranscoder-1.28.0.tar` & `mypy-boto3-elastictranscoder-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:31.630295 mypy-boto3-elastictranscoder-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-07-06 20:59:31.630295 mypy-boto3-elastictranscoder-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:31.614295 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22871 2023-07-06 20:40:26.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22852 2023-07-06 20:40:25.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:31.630295 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-07-06 20:59:31.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 20:59:31.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:31.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:31.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:31.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:31.000000 mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:31.630295 mypy-boto3-elastictranscoder-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-06 20:40:23.000000 mypy-boto3-elastictranscoder-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.104519 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29436 2023-07-27 05:21:52.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:38.000000 mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:39.120519 mypy-boto3-elastictranscoder-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:21:51.000000 mypy-boto3-elastictranscoder-1.28.12/setup.py
```

### Comparing `mypy-boto3-elastictranscoder-1.28.0/LICENSE` & `mypy-boto3-elastictranscoder-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/PKG-INFO` & `mypy-boto3-elastictranscoder-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticTranscoder 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticTranscoder 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elastictranscoder"></a>
 
 # mypy-boto3-elastictranscoder
 
 [![PyPI - mypy-boto3-elastictranscoder](https://img.shields.io/pypi/v/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastictranscoder?color=blue)](https://pypistats.org/packages/mypy-boto3-elastictranscoder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,88 +358,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
+    AudioCodecOptionsOutputTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
+    TimeSpanOutputTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
+    DetectedPropertiesOutputTypeDef,
     DetectedPropertiesTypeDef,
+    HlsContentProtectionOutputTypeDef,
     TimingTypeDef,
     ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
     ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    NotificationsOutputTypeDef,
     PaginatorConfigTypeDef,
+    PermissionOutputTypeDef,
     PermissionTypeDef,
+    PlayReadyDrmOutputTypeDef,
+    ThumbnailsOutputTypeDef,
+    PresetWatermarkOutputTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
     TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
+    ArtworkOutputTypeDef,
+    CaptionFormatOutputTypeDef,
+    CaptionSourceOutputTypeDef,
+    JobWatermarkOutputTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
+    AudioParametersOutputTypeDef,
     AudioParametersTypeDef,
+    ClipOutputTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
-    PlaylistTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
+    PlaylistTypeDef,
+    VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
+    JobAlbumArtOutputTypeDef,
+    CaptionsOutputTypeDef,
+    InputCaptionsOutputTypeDef,
     JobAlbumArtTypeDef,
     CaptionsTypeDef,
     InputCaptionsTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
-    CreateJobOutputTypeDef,
+    CreatePresetRequestRequestTypeDef,
     JobOutputTypeDef,
+    JobInputOutputTypeDef,
+    CreateJobOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
+    CreateJobRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_structure() -> EncryptionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.0/README.md` & `mypy-boto3-elastictranscoder-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elastictranscoder"></a>
 
 # mypy-boto3-elastictranscoder
 
 [![PyPI - mypy-boto3-elastictranscoder](https://img.shields.io/pypi/v/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastictranscoder?color=blue)](https://pypistats.org/packages/mypy-boto3-elastictranscoder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,88 +326,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
+    AudioCodecOptionsOutputTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
+    TimeSpanOutputTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
+    DetectedPropertiesOutputTypeDef,
     DetectedPropertiesTypeDef,
+    HlsContentProtectionOutputTypeDef,
     TimingTypeDef,
     ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
     ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    NotificationsOutputTypeDef,
     PaginatorConfigTypeDef,
+    PermissionOutputTypeDef,
     PermissionTypeDef,
+    PlayReadyDrmOutputTypeDef,
+    ThumbnailsOutputTypeDef,
+    PresetWatermarkOutputTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
     TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
+    ArtworkOutputTypeDef,
+    CaptionFormatOutputTypeDef,
+    CaptionSourceOutputTypeDef,
+    JobWatermarkOutputTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
+    AudioParametersOutputTypeDef,
     AudioParametersTypeDef,
+    ClipOutputTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
-    PlaylistTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
+    PlaylistTypeDef,
+    VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
+    JobAlbumArtOutputTypeDef,
+    CaptionsOutputTypeDef,
+    InputCaptionsOutputTypeDef,
     JobAlbumArtTypeDef,
     CaptionsTypeDef,
     InputCaptionsTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
-    CreateJobOutputTypeDef,
+    CreatePresetRequestRequestTypeDef,
     JobOutputTypeDef,
+    JobInputOutputTypeDef,
+    CreateJobOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
+    CreateJobRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_structure() -> EncryptionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/__init__.py` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/__init__.pyi` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/__main__.py` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticTranscoder 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ElasticTranscoder 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/client.py` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/client.pyi` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/literals.py` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
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
@@ -241,26 +242,28 @@
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

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/literals.pyi` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
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
@@ -239,26 +240,28 @@
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

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/paginator.py` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/paginator.pyi` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/type_defs.py` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,112 +2,156 @@
 Type annotations for elastictranscoder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elastictranscoder.type_defs import EncryptionTypeDef
+    from mypy_boto3_elastictranscoder.type_defs import EncryptionOutputTypeDef
 
-    data: EncryptionTypeDef = {...}
+    data: EncryptionOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
+    "AudioCodecOptionsOutputTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
+    "TimeSpanOutputTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
+    "DetectedPropertiesOutputTypeDef",
     "DetectedPropertiesTypeDef",
+    "HlsContentProtectionOutputTypeDef",
     "TimingTypeDef",
     "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
     "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
+    "NotificationsOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "PermissionOutputTypeDef",
     "PermissionTypeDef",
+    "PlayReadyDrmOutputTypeDef",
+    "ThumbnailsOutputTypeDef",
+    "PresetWatermarkOutputTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
     "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
+    "ArtworkOutputTypeDef",
+    "CaptionFormatOutputTypeDef",
+    "CaptionSourceOutputTypeDef",
+    "JobWatermarkOutputTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
+    "AudioParametersOutputTypeDef",
     "AudioParametersTypeDef",
+    "ClipOutputTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
-    "PlaylistTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
+    "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
+    "PlaylistTypeDef",
+    "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
+    "JobAlbumArtOutputTypeDef",
+    "CaptionsOutputTypeDef",
+    "InputCaptionsOutputTypeDef",
     "JobAlbumArtTypeDef",
     "CaptionsTypeDef",
     "InputCaptionsTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "CreatePresetRequestRequestTypeDef",
     "PresetTypeDef",
-    "CreateJobOutputTypeDef",
+    "CreatePresetRequestRequestTypeDef",
     "JobOutputTypeDef",
+    "JobInputOutputTypeDef",
+    "CreateJobOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
 )
 
+EncryptionOutputTypeDef = TypedDict(
+    "EncryptionOutputTypeDef",
+    {
+        "Mode": str,
+        "Key": str,
+        "KeyMd5": str,
+        "InitializationVector": str,
+    },
+    total=False,
+)
+
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
         "KeyMd5": str,
         "InitializationVector": str,
     },
     total=False,
 )
 
+AudioCodecOptionsOutputTypeDef = TypedDict(
+    "AudioCodecOptionsOutputTypeDef",
+    {
+        "Profile": str,
+        "BitDepth": str,
+        "BitOrder": str,
+        "Signed": str,
+    },
+    total=False,
+)
+
 AudioCodecOptionsTypeDef = TypedDict(
     "AudioCodecOptionsTypeDef",
     {
         "Profile": str,
         "BitDepth": str,
         "BitOrder": str,
         "Signed": str,
@@ -118,14 +162,23 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+TimeSpanOutputTypeDef = TypedDict(
+    "TimeSpanOutputTypeDef",
+    {
+        "StartTime": str,
+        "Duration": str,
+    },
+    total=False,
+)
+
 TimeSpanTypeDef = TypedDict(
     "TimeSpanTypeDef",
     {
         "StartTime": str,
         "Duration": str,
     },
     total=False,
@@ -202,26 +255,51 @@
 DeletePresetRequestRequestTypeDef = TypedDict(
     "DeletePresetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DetectedPropertiesOutputTypeDef = TypedDict(
+    "DetectedPropertiesOutputTypeDef",
+    {
+        "Width": int,
+        "Height": int,
+        "FrameRate": str,
+        "FileSize": int,
+        "DurationMillis": int,
+    },
+    total=False,
+)
+
 DetectedPropertiesTypeDef = TypedDict(
     "DetectedPropertiesTypeDef",
     {
         "Width": int,
         "Height": int,
         "FrameRate": str,
         "FileSize": int,
         "DurationMillis": int,
     },
     total=False,
 )
 
+HlsContentProtectionOutputTypeDef = TypedDict(
+    "HlsContentProtectionOutputTypeDef",
+    {
+        "Method": str,
+        "Key": str,
+        "KeyMd5": str,
+        "InitializationVector": str,
+        "LicenseAcquisitionUrl": str,
+        "KeyStoragePolicy": str,
+    },
+    total=False,
+)
+
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
@@ -351,34 +429,100 @@
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
+NotificationsOutputTypeDef = TypedDict(
+    "NotificationsOutputTypeDef",
+    {
+        "Progressing": str,
+        "Completed": str,
+        "Warning": str,
+        "Error": str,
+    },
+    total=False,
+)
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
 
+PermissionOutputTypeDef = TypedDict(
+    "PermissionOutputTypeDef",
+    {
+        "GranteeType": str,
+        "Grantee": str,
+        "Access": List[str],
+    },
+    total=False,
+)
+
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
     total=False,
 )
 
+PlayReadyDrmOutputTypeDef = TypedDict(
+    "PlayReadyDrmOutputTypeDef",
+    {
+        "Format": str,
+        "Key": str,
+        "KeyMd5": str,
+        "KeyId": str,
+        "InitializationVector": str,
+        "LicenseAcquisitionUrl": str,
+    },
+    total=False,
+)
+
+ThumbnailsOutputTypeDef = TypedDict(
+    "ThumbnailsOutputTypeDef",
+    {
+        "Format": str,
+        "Interval": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+    },
+    total=False,
+)
+
+PresetWatermarkOutputTypeDef = TypedDict(
+    "PresetWatermarkOutputTypeDef",
+    {
+        "Id": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "SizingPolicy": str,
+        "HorizontalAlign": str,
+        "HorizontalOffset": str,
+        "VerticalAlign": str,
+        "VerticalOffset": str,
+        "Opacity": str,
+        "Target": str,
+    },
+    total=False,
+)
+
 PresetWatermarkTypeDef = TypedDict(
     "PresetWatermarkTypeDef",
     {
         "Id": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -456,14 +600,60 @@
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
 
+ArtworkOutputTypeDef = TypedDict(
+    "ArtworkOutputTypeDef",
+    {
+        "InputKey": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+        "AlbumArtFormat": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+CaptionFormatOutputTypeDef = TypedDict(
+    "CaptionFormatOutputTypeDef",
+    {
+        "Format": str,
+        "Pattern": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+CaptionSourceOutputTypeDef = TypedDict(
+    "CaptionSourceOutputTypeDef",
+    {
+        "Key": str,
+        "Language": str,
+        "TimeOffset": str,
+        "Label": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+JobWatermarkOutputTypeDef = TypedDict(
+    "JobWatermarkOutputTypeDef",
+    {
+        "PresetWatermarkId": str,
+        "InputKey": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
 ArtworkTypeDef = TypedDict(
     "ArtworkTypeDef",
     {
         "InputKey": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -502,27 +692,48 @@
         "PresetWatermarkId": str,
         "InputKey": str,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
+AudioParametersOutputTypeDef = TypedDict(
+    "AudioParametersOutputTypeDef",
+    {
+        "Codec": str,
+        "SampleRate": str,
+        "BitRate": str,
+        "Channels": str,
+        "AudioPackingMode": str,
+        "CodecOptions": AudioCodecOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 AudioParametersTypeDef = TypedDict(
     "AudioParametersTypeDef",
     {
         "Codec": str,
         "SampleRate": str,
         "BitRate": str,
         "Channels": str,
         "AudioPackingMode": str,
         "CodecOptions": AudioCodecOptionsTypeDef,
     },
     total=False,
 )
 
+ClipOutputTypeDef = TypedDict(
+    "ClipOutputTypeDef",
+    {
+        "TimeSpan": TimeSpanOutputTypeDef,
+    },
+    total=False,
+)
+
 ClipTypeDef = TypedDict(
     "ClipTypeDef",
     {
         "TimeSpan": TimeSpanTypeDef,
     },
     total=False,
 )
@@ -535,46 +746,78 @@
         "OutputKeys": Sequence[str],
         "HlsContentProtection": HlsContentProtectionTypeDef,
         "PlayReadyDrm": PlayReadyDrmTypeDef,
     },
     total=False,
 )
 
-PlaylistTypeDef = TypedDict(
-    "PlaylistTypeDef",
-    {
-        "Name": str,
-        "Format": str,
-        "OutputKeys": List[str],
-        "HlsContentProtection": HlsContentProtectionTypeDef,
-        "PlayReadyDrm": PlayReadyDrmTypeDef,
-        "Status": str,
-        "StatusDetail": str,
-    },
-    total=False,
-)
-
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
+PipelineOutputConfigOutputTypeDef = TypedDict(
+    "PipelineOutputConfigOutputTypeDef",
+    {
+        "Bucket": str,
+        "StorageClass": str,
+        "Permissions": List[PermissionOutputTypeDef],
+    },
+    total=False,
+)
+
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
+PlaylistTypeDef = TypedDict(
+    "PlaylistTypeDef",
+    {
+        "Name": str,
+        "Format": str,
+        "OutputKeys": List[str],
+        "HlsContentProtection": HlsContentProtectionOutputTypeDef,
+        "PlayReadyDrm": PlayReadyDrmOutputTypeDef,
+        "Status": str,
+        "StatusDetail": str,
+    },
+    total=False,
+)
+
+VideoParametersOutputTypeDef = TypedDict(
+    "VideoParametersOutputTypeDef",
+    {
+        "Codec": str,
+        "CodecOptions": Dict[str, str],
+        "KeyframesMaxDist": str,
+        "FixedGOP": str,
+        "BitRate": str,
+        "FrameRate": str,
+        "MaxFrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "DisplayAspectRatio": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+        "Watermarks": List[PresetWatermarkOutputTypeDef],
+    },
+    total=False,
+)
+
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
         "Codec": str,
         "CodecOptions": Mapping[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -610,14 +853,42 @@
 
 class ReadJobRequestJobCompleteWaitTypeDef(
     _RequiredReadJobRequestJobCompleteWaitTypeDef, _OptionalReadJobRequestJobCompleteWaitTypeDef
 ):
     pass
 
 
+JobAlbumArtOutputTypeDef = TypedDict(
+    "JobAlbumArtOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "Artwork": List[ArtworkOutputTypeDef],
+    },
+    total=False,
+)
+
+CaptionsOutputTypeDef = TypedDict(
+    "CaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceOutputTypeDef],
+        "CaptionFormats": List[CaptionFormatOutputTypeDef],
+    },
+    total=False,
+)
+
+InputCaptionsOutputTypeDef = TypedDict(
+    "InputCaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceOutputTypeDef],
+    },
+    total=False,
+)
+
 JobAlbumArtTypeDef = TypedDict(
     "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
         "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
@@ -638,14 +909,32 @@
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
     },
     total=False,
 )
 
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Status": str,
+        "InputBucket": str,
+        "OutputBucket": str,
+        "Role": str,
+        "AwsKmsKeyArn": str,
+        "Notifications": NotificationsOutputTypeDef,
+        "ContentConfig": PipelineOutputConfigOutputTypeDef,
+        "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "Name": str,
         "InputBucket": str,
         "Role": str,
     },
@@ -665,32 +954,14 @@
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Status": str,
-        "InputBucket": str,
-        "OutputBucket": str,
-        "Role": str,
-        "AwsKmsKeyArn": str,
-        "Notifications": NotificationsTypeDef,
-        "ContentConfig": PipelineOutputConfigTypeDef,
-        "ThumbnailConfig": PipelineOutputConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -710,14 +981,30 @@
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Container": str,
+        "Audio": AudioParametersOutputTypeDef,
+        "Video": VideoParametersOutputTypeDef,
+        "Thumbnails": ThumbnailsOutputTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Container": str,
     },
 )
@@ -735,72 +1022,73 @@
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
 
-PresetTypeDef = TypedDict(
-    "PresetTypeDef",
+JobOutputTypeDef = TypedDict(
+    "JobOutputTypeDef",
     {
         "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Container": str,
-        "Audio": AudioParametersTypeDef,
-        "Video": VideoParametersTypeDef,
-        "Thumbnails": ThumbnailsTypeDef,
-        "Type": str,
+        "Key": str,
+        "ThumbnailPattern": str,
+        "ThumbnailEncryption": EncryptionOutputTypeDef,
+        "Rotate": str,
+        "PresetId": str,
+        "SegmentDuration": str,
+        "Status": str,
+        "StatusDetail": str,
+        "Duration": int,
+        "Width": int,
+        "Height": int,
+        "FrameRate": str,
+        "FileSize": int,
+        "DurationMillis": int,
+        "Watermarks": List[JobWatermarkOutputTypeDef],
+        "AlbumArt": JobAlbumArtOutputTypeDef,
+        "Composition": List[ClipOutputTypeDef],
+        "Captions": CaptionsOutputTypeDef,
+        "Encryption": EncryptionOutputTypeDef,
+        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
-CreateJobOutputTypeDef = TypedDict(
-    "CreateJobOutputTypeDef",
+JobInputOutputTypeDef = TypedDict(
+    "JobInputOutputTypeDef",
     {
         "Key": str,
-        "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionTypeDef,
-        "Rotate": str,
-        "PresetId": str,
-        "SegmentDuration": str,
-        "Watermarks": Sequence[JobWatermarkTypeDef],
-        "AlbumArt": JobAlbumArtTypeDef,
-        "Composition": Sequence[ClipTypeDef],
-        "Captions": CaptionsTypeDef,
-        "Encryption": EncryptionTypeDef,
+        "FrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "Interlaced": str,
+        "Container": str,
+        "Encryption": EncryptionOutputTypeDef,
+        "TimeSpan": TimeSpanOutputTypeDef,
+        "InputCaptions": InputCaptionsOutputTypeDef,
+        "DetectedProperties": DetectedPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-JobOutputTypeDef = TypedDict(
-    "JobOutputTypeDef",
+CreateJobOutputTypeDef = TypedDict(
+    "CreateJobOutputTypeDef",
     {
-        "Id": str,
         "Key": str,
         "ThumbnailPattern": str,
         "ThumbnailEncryption": EncryptionTypeDef,
         "Rotate": str,
         "PresetId": str,
         "SegmentDuration": str,
-        "Status": str,
-        "StatusDetail": str,
-        "Duration": int,
-        "Width": int,
-        "Height": int,
-        "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-        "Watermarks": List[JobWatermarkTypeDef],
+        "Watermarks": Sequence[JobWatermarkTypeDef],
         "AlbumArt": JobAlbumArtTypeDef,
-        "Composition": List[ClipTypeDef],
+        "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
-        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
@@ -892,14 +1180,33 @@
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "PipelineId": str,
+        "Input": JobInputOutputTypeDef,
+        "Inputs": List[JobInputOutputTypeDef],
+        "Output": JobOutputTypeDef,
+        "Outputs": List[JobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": List[PlaylistTypeDef],
+        "Status": str,
+        "UserMetadata": Dict[str, str],
+        "Timing": TimingTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalCreateJobRequestRequestTypeDef = TypedDict(
@@ -919,33 +1226,14 @@
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
 
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "PipelineId": str,
-        "Input": JobInputTypeDef,
-        "Inputs": List[JobInputTypeDef],
-        "Output": JobOutputTypeDef,
-        "Outputs": List[JobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": List[PlaylistTypeDef],
-        "Status": str,
-        "UserMetadata": Dict[str, str],
-        "Timing": TimingTypeDef,
-    },
-    total=False,
-)
-
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/type_defs.pyi` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/type_defs.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,111 +2,155 @@
 Type annotations for elastictranscoder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elastictranscoder.type_defs import EncryptionTypeDef
+    from mypy_boto3_elastictranscoder.type_defs import EncryptionOutputTypeDef
 
-    data: EncryptionTypeDef = {...}
+    data: EncryptionOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
+    "AudioCodecOptionsOutputTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
+    "TimeSpanOutputTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
+    "DetectedPropertiesOutputTypeDef",
     "DetectedPropertiesTypeDef",
+    "HlsContentProtectionOutputTypeDef",
     "TimingTypeDef",
     "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
     "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
+    "NotificationsOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "PermissionOutputTypeDef",
     "PermissionTypeDef",
+    "PlayReadyDrmOutputTypeDef",
+    "ThumbnailsOutputTypeDef",
+    "PresetWatermarkOutputTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
     "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
+    "ArtworkOutputTypeDef",
+    "CaptionFormatOutputTypeDef",
+    "CaptionSourceOutputTypeDef",
+    "JobWatermarkOutputTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
+    "AudioParametersOutputTypeDef",
     "AudioParametersTypeDef",
+    "ClipOutputTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
-    "PlaylistTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
+    "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
+    "PlaylistTypeDef",
+    "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
+    "JobAlbumArtOutputTypeDef",
+    "CaptionsOutputTypeDef",
+    "InputCaptionsOutputTypeDef",
     "JobAlbumArtTypeDef",
     "CaptionsTypeDef",
     "InputCaptionsTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "CreatePresetRequestRequestTypeDef",
     "PresetTypeDef",
-    "CreateJobOutputTypeDef",
+    "CreatePresetRequestRequestTypeDef",
     "JobOutputTypeDef",
+    "JobInputOutputTypeDef",
+    "CreateJobOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
 )
 
+EncryptionOutputTypeDef = TypedDict(
+    "EncryptionOutputTypeDef",
+    {
+        "Mode": str,
+        "Key": str,
+        "KeyMd5": str,
+        "InitializationVector": str,
+    },
+    total=False,
+)
+
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
         "KeyMd5": str,
         "InitializationVector": str,
     },
     total=False,
 )
 
+AudioCodecOptionsOutputTypeDef = TypedDict(
+    "AudioCodecOptionsOutputTypeDef",
+    {
+        "Profile": str,
+        "BitDepth": str,
+        "BitOrder": str,
+        "Signed": str,
+    },
+    total=False,
+)
+
 AudioCodecOptionsTypeDef = TypedDict(
     "AudioCodecOptionsTypeDef",
     {
         "Profile": str,
         "BitDepth": str,
         "BitOrder": str,
         "Signed": str,
@@ -117,14 +161,23 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+TimeSpanOutputTypeDef = TypedDict(
+    "TimeSpanOutputTypeDef",
+    {
+        "StartTime": str,
+        "Duration": str,
+    },
+    total=False,
+)
+
 TimeSpanTypeDef = TypedDict(
     "TimeSpanTypeDef",
     {
         "StartTime": str,
         "Duration": str,
     },
     total=False,
@@ -201,26 +254,51 @@
 DeletePresetRequestRequestTypeDef = TypedDict(
     "DeletePresetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DetectedPropertiesOutputTypeDef = TypedDict(
+    "DetectedPropertiesOutputTypeDef",
+    {
+        "Width": int,
+        "Height": int,
+        "FrameRate": str,
+        "FileSize": int,
+        "DurationMillis": int,
+    },
+    total=False,
+)
+
 DetectedPropertiesTypeDef = TypedDict(
     "DetectedPropertiesTypeDef",
     {
         "Width": int,
         "Height": int,
         "FrameRate": str,
         "FileSize": int,
         "DurationMillis": int,
     },
     total=False,
 )
 
+HlsContentProtectionOutputTypeDef = TypedDict(
+    "HlsContentProtectionOutputTypeDef",
+    {
+        "Method": str,
+        "Key": str,
+        "KeyMd5": str,
+        "InitializationVector": str,
+        "LicenseAcquisitionUrl": str,
+        "KeyStoragePolicy": str,
+    },
+    total=False,
+)
+
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
@@ -342,34 +420,100 @@
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
+NotificationsOutputTypeDef = TypedDict(
+    "NotificationsOutputTypeDef",
+    {
+        "Progressing": str,
+        "Completed": str,
+        "Warning": str,
+        "Error": str,
+    },
+    total=False,
+)
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
 
+PermissionOutputTypeDef = TypedDict(
+    "PermissionOutputTypeDef",
+    {
+        "GranteeType": str,
+        "Grantee": str,
+        "Access": List[str],
+    },
+    total=False,
+)
+
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
     total=False,
 )
 
+PlayReadyDrmOutputTypeDef = TypedDict(
+    "PlayReadyDrmOutputTypeDef",
+    {
+        "Format": str,
+        "Key": str,
+        "KeyMd5": str,
+        "KeyId": str,
+        "InitializationVector": str,
+        "LicenseAcquisitionUrl": str,
+    },
+    total=False,
+)
+
+ThumbnailsOutputTypeDef = TypedDict(
+    "ThumbnailsOutputTypeDef",
+    {
+        "Format": str,
+        "Interval": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+    },
+    total=False,
+)
+
+PresetWatermarkOutputTypeDef = TypedDict(
+    "PresetWatermarkOutputTypeDef",
+    {
+        "Id": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "SizingPolicy": str,
+        "HorizontalAlign": str,
+        "HorizontalOffset": str,
+        "VerticalAlign": str,
+        "VerticalOffset": str,
+        "Opacity": str,
+        "Target": str,
+    },
+    total=False,
+)
+
 PresetWatermarkTypeDef = TypedDict(
     "PresetWatermarkTypeDef",
     {
         "Id": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -447,14 +591,60 @@
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
 
+ArtworkOutputTypeDef = TypedDict(
+    "ArtworkOutputTypeDef",
+    {
+        "InputKey": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+        "AlbumArtFormat": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+CaptionFormatOutputTypeDef = TypedDict(
+    "CaptionFormatOutputTypeDef",
+    {
+        "Format": str,
+        "Pattern": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+CaptionSourceOutputTypeDef = TypedDict(
+    "CaptionSourceOutputTypeDef",
+    {
+        "Key": str,
+        "Language": str,
+        "TimeOffset": str,
+        "Label": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+JobWatermarkOutputTypeDef = TypedDict(
+    "JobWatermarkOutputTypeDef",
+    {
+        "PresetWatermarkId": str,
+        "InputKey": str,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
 ArtworkTypeDef = TypedDict(
     "ArtworkTypeDef",
     {
         "InputKey": str,
         "MaxWidth": str,
         "MaxHeight": str,
         "SizingPolicy": str,
@@ -493,27 +683,48 @@
         "PresetWatermarkId": str,
         "InputKey": str,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
+AudioParametersOutputTypeDef = TypedDict(
+    "AudioParametersOutputTypeDef",
+    {
+        "Codec": str,
+        "SampleRate": str,
+        "BitRate": str,
+        "Channels": str,
+        "AudioPackingMode": str,
+        "CodecOptions": AudioCodecOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 AudioParametersTypeDef = TypedDict(
     "AudioParametersTypeDef",
     {
         "Codec": str,
         "SampleRate": str,
         "BitRate": str,
         "Channels": str,
         "AudioPackingMode": str,
         "CodecOptions": AudioCodecOptionsTypeDef,
     },
     total=False,
 )
 
+ClipOutputTypeDef = TypedDict(
+    "ClipOutputTypeDef",
+    {
+        "TimeSpan": TimeSpanOutputTypeDef,
+    },
+    total=False,
+)
+
 ClipTypeDef = TypedDict(
     "ClipTypeDef",
     {
         "TimeSpan": TimeSpanTypeDef,
     },
     total=False,
 )
@@ -526,46 +737,78 @@
         "OutputKeys": Sequence[str],
         "HlsContentProtection": HlsContentProtectionTypeDef,
         "PlayReadyDrm": PlayReadyDrmTypeDef,
     },
     total=False,
 )
 
-PlaylistTypeDef = TypedDict(
-    "PlaylistTypeDef",
-    {
-        "Name": str,
-        "Format": str,
-        "OutputKeys": List[str],
-        "HlsContentProtection": HlsContentProtectionTypeDef,
-        "PlayReadyDrm": PlayReadyDrmTypeDef,
-        "Status": str,
-        "StatusDetail": str,
-    },
-    total=False,
-)
-
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
+PipelineOutputConfigOutputTypeDef = TypedDict(
+    "PipelineOutputConfigOutputTypeDef",
+    {
+        "Bucket": str,
+        "StorageClass": str,
+        "Permissions": List[PermissionOutputTypeDef],
+    },
+    total=False,
+)
+
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
+PlaylistTypeDef = TypedDict(
+    "PlaylistTypeDef",
+    {
+        "Name": str,
+        "Format": str,
+        "OutputKeys": List[str],
+        "HlsContentProtection": HlsContentProtectionOutputTypeDef,
+        "PlayReadyDrm": PlayReadyDrmOutputTypeDef,
+        "Status": str,
+        "StatusDetail": str,
+    },
+    total=False,
+)
+
+VideoParametersOutputTypeDef = TypedDict(
+    "VideoParametersOutputTypeDef",
+    {
+        "Codec": str,
+        "CodecOptions": Dict[str, str],
+        "KeyframesMaxDist": str,
+        "FixedGOP": str,
+        "BitRate": str,
+        "FrameRate": str,
+        "MaxFrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "DisplayAspectRatio": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+        "Watermarks": List[PresetWatermarkOutputTypeDef],
+    },
+    total=False,
+)
+
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
         "Codec": str,
         "CodecOptions": Mapping[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -599,14 +842,42 @@
 )
 
 class ReadJobRequestJobCompleteWaitTypeDef(
     _RequiredReadJobRequestJobCompleteWaitTypeDef, _OptionalReadJobRequestJobCompleteWaitTypeDef
 ):
     pass
 
+JobAlbumArtOutputTypeDef = TypedDict(
+    "JobAlbumArtOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "Artwork": List[ArtworkOutputTypeDef],
+    },
+    total=False,
+)
+
+CaptionsOutputTypeDef = TypedDict(
+    "CaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceOutputTypeDef],
+        "CaptionFormats": List[CaptionFormatOutputTypeDef],
+    },
+    total=False,
+)
+
+InputCaptionsOutputTypeDef = TypedDict(
+    "InputCaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceOutputTypeDef],
+    },
+    total=False,
+)
+
 JobAlbumArtTypeDef = TypedDict(
     "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
         "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
@@ -627,14 +898,32 @@
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
     },
     total=False,
 )
 
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Status": str,
+        "InputBucket": str,
+        "OutputBucket": str,
+        "Role": str,
+        "AwsKmsKeyArn": str,
+        "Notifications": NotificationsOutputTypeDef,
+        "ContentConfig": PipelineOutputConfigOutputTypeDef,
+        "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "Name": str,
         "InputBucket": str,
         "Role": str,
     },
@@ -652,32 +941,14 @@
 )
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Status": str,
-        "InputBucket": str,
-        "OutputBucket": str,
-        "Role": str,
-        "AwsKmsKeyArn": str,
-        "Notifications": NotificationsTypeDef,
-        "ContentConfig": PipelineOutputConfigTypeDef,
-        "ThumbnailConfig": PipelineOutputConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -695,14 +966,30 @@
 )
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Container": str,
+        "Audio": AudioParametersOutputTypeDef,
+        "Video": VideoParametersOutputTypeDef,
+        "Thumbnails": ThumbnailsOutputTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Container": str,
     },
 )
@@ -718,72 +1005,73 @@
 )
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
-PresetTypeDef = TypedDict(
-    "PresetTypeDef",
+JobOutputTypeDef = TypedDict(
+    "JobOutputTypeDef",
     {
         "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Container": str,
-        "Audio": AudioParametersTypeDef,
-        "Video": VideoParametersTypeDef,
-        "Thumbnails": ThumbnailsTypeDef,
-        "Type": str,
+        "Key": str,
+        "ThumbnailPattern": str,
+        "ThumbnailEncryption": EncryptionOutputTypeDef,
+        "Rotate": str,
+        "PresetId": str,
+        "SegmentDuration": str,
+        "Status": str,
+        "StatusDetail": str,
+        "Duration": int,
+        "Width": int,
+        "Height": int,
+        "FrameRate": str,
+        "FileSize": int,
+        "DurationMillis": int,
+        "Watermarks": List[JobWatermarkOutputTypeDef],
+        "AlbumArt": JobAlbumArtOutputTypeDef,
+        "Composition": List[ClipOutputTypeDef],
+        "Captions": CaptionsOutputTypeDef,
+        "Encryption": EncryptionOutputTypeDef,
+        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
-CreateJobOutputTypeDef = TypedDict(
-    "CreateJobOutputTypeDef",
+JobInputOutputTypeDef = TypedDict(
+    "JobInputOutputTypeDef",
     {
         "Key": str,
-        "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionTypeDef,
-        "Rotate": str,
-        "PresetId": str,
-        "SegmentDuration": str,
-        "Watermarks": Sequence[JobWatermarkTypeDef],
-        "AlbumArt": JobAlbumArtTypeDef,
-        "Composition": Sequence[ClipTypeDef],
-        "Captions": CaptionsTypeDef,
-        "Encryption": EncryptionTypeDef,
+        "FrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "Interlaced": str,
+        "Container": str,
+        "Encryption": EncryptionOutputTypeDef,
+        "TimeSpan": TimeSpanOutputTypeDef,
+        "InputCaptions": InputCaptionsOutputTypeDef,
+        "DetectedProperties": DetectedPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-JobOutputTypeDef = TypedDict(
-    "JobOutputTypeDef",
+CreateJobOutputTypeDef = TypedDict(
+    "CreateJobOutputTypeDef",
     {
-        "Id": str,
         "Key": str,
         "ThumbnailPattern": str,
         "ThumbnailEncryption": EncryptionTypeDef,
         "Rotate": str,
         "PresetId": str,
         "SegmentDuration": str,
-        "Status": str,
-        "StatusDetail": str,
-        "Duration": int,
-        "Width": int,
-        "Height": int,
-        "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-        "Watermarks": List[JobWatermarkTypeDef],
+        "Watermarks": Sequence[JobWatermarkTypeDef],
         "AlbumArt": JobAlbumArtTypeDef,
-        "Composition": List[ClipTypeDef],
+        "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
-        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
@@ -875,14 +1163,33 @@
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "PipelineId": str,
+        "Input": JobInputOutputTypeDef,
+        "Inputs": List[JobInputOutputTypeDef],
+        "Output": JobOutputTypeDef,
+        "Outputs": List[JobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": List[PlaylistTypeDef],
+        "Status": str,
+        "UserMetadata": Dict[str, str],
+        "Timing": TimingTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalCreateJobRequestRequestTypeDef = TypedDict(
@@ -900,33 +1207,14 @@
 )
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "PipelineId": str,
-        "Input": JobInputTypeDef,
-        "Inputs": List[JobInputTypeDef],
-        "Output": JobOutputTypeDef,
-        "Outputs": List[JobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": List[PlaylistTypeDef],
-        "Status": str,
-        "UserMetadata": Dict[str, str],
-        "Timing": TimingTypeDef,
-    },
-    total=False,
-)
-
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/waiter.py` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder/waiter.pyi` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/PKG-INFO` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastictranscoder
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticTranscoder 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticTranscoder 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elastictranscoder"></a>
 
 # mypy-boto3-elastictranscoder
 
 [![PyPI - mypy-boto3-elastictranscoder](https://img.shields.io/pypi/v/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastictranscoder.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastictranscoder?color=blue)](https://pypistats.org/packages/mypy-boto3-elastictranscoder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastictranscoder)](https://pepy.tech/project/mypy-boto3-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticTranscoder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[boto3.ElasticTranscoder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [mypy-boto3-elastictranscoder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,88 +358,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_elastictranscoder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elastictranscoder.type_defs import (
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
+    AudioCodecOptionsOutputTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
+    TimeSpanOutputTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
+    DetectedPropertiesOutputTypeDef,
     DetectedPropertiesTypeDef,
+    HlsContentProtectionOutputTypeDef,
     TimingTypeDef,
     ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
     ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
     ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    NotificationsOutputTypeDef,
     PaginatorConfigTypeDef,
+    PermissionOutputTypeDef,
     PermissionTypeDef,
+    PlayReadyDrmOutputTypeDef,
+    ThumbnailsOutputTypeDef,
+    PresetWatermarkOutputTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
     TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
+    ArtworkOutputTypeDef,
+    CaptionFormatOutputTypeDef,
+    CaptionSourceOutputTypeDef,
+    JobWatermarkOutputTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
+    AudioParametersOutputTypeDef,
     AudioParametersTypeDef,
+    ClipOutputTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
-    PlaylistTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
+    PlaylistTypeDef,
+    VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
+    JobAlbumArtOutputTypeDef,
+    CaptionsOutputTypeDef,
+    InputCaptionsOutputTypeDef,
     JobAlbumArtTypeDef,
     CaptionsTypeDef,
     InputCaptionsTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
-    CreateJobOutputTypeDef,
+    CreatePresetRequestRequestTypeDef,
     JobOutputTypeDef,
+    JobInputOutputTypeDef,
+    CreateJobOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
+    CreateJobRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_structure() -> EncryptionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elastictranscoder-1.28.0/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt` & `mypy-boto3-elastictranscoder-1.28.12/mypy_boto3_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastictranscoder-1.28.0/setup.py` & `mypy-boto3-elastictranscoder-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elastictranscoder",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticTranscoder 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ElasticTranscoder 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

