# Comparing `tmp/mypy-boto3-mediaconvert-1.28.12.tar.gz` & `tmp/mypy-boto3-mediaconvert-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconvert-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconvert-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-mediaconvert-1.28.12.tar` & `mypy-boto3-mediaconvert-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.352444 mypy-boto3-mediaconvert-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    39090 2023-07-27 05:35:00.348444 mypy-boto3-mediaconvert-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37583 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.340444 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55606 2023-07-27 05:26:04.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55604 2023-07-27 05:26:04.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   175093 2023-07-27 05:26:09.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   175068 2023-07-27 05:26:06.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.348444 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    39090 2023-07-27 05:35:00.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:35:00.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:00.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:35:00.000000 mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.352444 mypy-boto3-mediaconvert-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:26:03.000000 mypy-boto3-mediaconvert-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.227903 mypy-boto3-mediaconvert-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    39103 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37598 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55551 2023-07-21 20:32:30.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55549 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   171396 2023-07-21 20:32:34.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171379 2023-07-21 20:32:31.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    39103 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.227903 mypy-boto3-mediaconvert-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-21 20:32:27.000000 mypy-boto3-mediaconvert-1.28.9/setup.py
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/LICENSE` & `mypy-boto3-mediaconvert-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.12/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaConvert 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.9
+Summary: Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -852,27 +852,28 @@
     MpdSettingsOutputTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
@@ -927,21 +928,17 @@
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateOutputTypeDef,
     MotionImageInsertionOffsetOutputTypeDef,
@@ -958,20 +955,18 @@
     NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsOutputTypeDef,
     NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
     PolicyTypeDef,
     ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
@@ -1016,14 +1011,19 @@
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsOutputTypeDef,
     HlsEncryptionSettingsOutputTypeDef,
     MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyResponseTypeDef,
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/README.md` & `mypy-boto3-mediaconvert-1.28.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -820,27 +820,28 @@
     MpdSettingsOutputTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
@@ -895,21 +896,17 @@
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateOutputTypeDef,
     MotionImageInsertionOffsetOutputTypeDef,
@@ -926,20 +923,18 @@
     NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsOutputTypeDef,
     NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
     PolicyTypeDef,
     ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
@@ -984,14 +979,19 @@
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsOutputTypeDef,
     HlsEncryptionSettingsOutputTypeDef,
     MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyResponseTypeDef,
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/__init__.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/__init__.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/__main__.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConvert 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MediaConvert 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/client.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/client.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/literals.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1413,15 +1413,14 @@
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
@@ -1500,15 +1499,14 @@
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
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/literals.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1411,15 +1411,14 @@
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
@@ -1498,15 +1497,14 @@
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
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/paginator.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 
@@ -93,15 +93,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -113,15 +113,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobspaginator)
         """
 
 
@@ -133,15 +133,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listpresetspaginator)
         """
 
 
@@ -152,13 +152,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/paginator.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 class ListJobTemplatesPaginator(Paginator):
@@ -89,15 +89,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -108,15 +108,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobspaginator)
         """
 
 class ListPresetsPaginator(Paginator):
@@ -127,15 +127,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listpresetspaginator)
         """
 
 class ListQueuesPaginator(Paginator):
@@ -145,13 +145,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/type_defs.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -537,27 +537,28 @@
     "MpdSettingsOutputTypeDef",
     "F4vSettingsTypeDef",
     "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
     "HopDestinationTypeDef",
+    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
     "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerOutputTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
     "DolbyVisionLevel6MetadataOutputTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
     "DvbNitSettingsOutputTypeDef",
     "DvbNitSettingsTypeDef",
@@ -612,21 +613,17 @@
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamOutputTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateOutputTypeDef",
     "MotionImageInsertionOffsetOutputTypeDef",
@@ -643,20 +640,18 @@
     "NoiseReducerFilterSettingsOutputTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsOutputTypeDef",
     "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyTypeDef",
     "ProresSettingsOutputTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationAccessControlOutputTypeDef",
     "S3DestinationAccessControlTypeDef",
     "S3EncryptionSettingsOutputTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimecodeBurninOutputTypeDef",
     "TimecodeBurninTypeDef",
@@ -701,14 +696,19 @@
     "UpdateQueueRequestRequestTypeDef",
     "DashIsoEncryptionSettingsOutputTypeDef",
     "HlsEncryptionSettingsOutputTypeDef",
     "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DolbyVisionOutputTypeDef",
     "DolbyVisionTypeDef",
     "EsamSettingsOutputTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyResponseTypeDef",
@@ -826,15 +826,14 @@
         "CodingMode": AacCodingModeType,
         "RateControlMode": AacRateControlModeType,
         "RawFormat": AacRawFormatType,
         "SampleRate": int,
         "Specification": AacSpecificationType,
         "VbrQuality": AacVbrQualityType,
     },
-    total=False,
 )
 
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
         "Bitrate": int,
@@ -859,15 +858,14 @@
         "DynamicRangeCompressionLine": Ac3DynamicRangeCompressionLineType,
         "DynamicRangeCompressionProfile": Ac3DynamicRangeCompressionProfileType,
         "DynamicRangeCompressionRf": Ac3DynamicRangeCompressionRfType,
         "LfeFilter": Ac3LfeFilterType,
         "MetadataControl": Ac3MetadataControlType,
         "SampleRate": int,
     },
-    total=False,
 )
 
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Ac3BitstreamModeType,
@@ -899,15 +897,14 @@
 
 AdvancedInputFilterSettingsOutputTypeDef = TypedDict(
     "AdvancedInputFilterSettingsOutputTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
     },
-    total=False,
 )
 
 AdvancedInputFilterSettingsTypeDef = TypedDict(
     "AdvancedInputFilterSettingsTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
@@ -918,15 +915,14 @@
 AiffSettingsOutputTypeDef = TypedDict(
     "AiffSettingsOutputTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
-    total=False,
 )
 
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
@@ -938,15 +934,14 @@
 AllowedRenditionSizeOutputTypeDef = TypedDict(
     "AllowedRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
         "Width": int,
     },
-    total=False,
 )
 
 AllowedRenditionSizeTypeDef = TypedDict(
     "AllowedRenditionSizeTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
@@ -958,15 +953,14 @@
 AncillarySourceSettingsOutputTypeDef = TypedDict(
     "AncillarySourceSettingsOutputTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
         "TerminateCaptions": AncillaryTerminateCaptionsType,
     },
-    total=False,
 )
 
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
@@ -983,15 +977,14 @@
 )
 
 AudioChannelTaggingSettingsOutputTypeDef = TypedDict(
     "AudioChannelTaggingSettingsOutputTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
-    total=False,
 )
 
 AudioChannelTaggingSettingsTypeDef = TypedDict(
     "AudioChannelTaggingSettingsTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
@@ -1015,15 +1008,14 @@
         "LtRtSurroundMixLevel": float,
         "MeteringMode": Eac3AtmosMeteringModeType,
         "SampleRate": int,
         "SpeechThreshold": int,
         "StereoDownmix": Eac3AtmosStereoDownmixType,
         "SurroundExMode": Eac3AtmosSurroundExModeType,
     },
-    total=False,
 )
 
 Eac3SettingsOutputTypeDef = TypedDict(
     "Eac3SettingsOutputTypeDef",
     {
         "AttenuationControl": Eac3AttenuationControlType,
         "Bitrate": int,
@@ -1043,68 +1035,62 @@
         "PassthroughControl": Eac3PassthroughControlType,
         "PhaseControl": Eac3PhaseControlType,
         "SampleRate": int,
         "StereoDownmix": Eac3StereoDownmixType,
         "SurroundExMode": Eac3SurroundExModeType,
         "SurroundMode": Eac3SurroundModeType,
     },
-    total=False,
 )
 
 Mp2SettingsOutputTypeDef = TypedDict(
     "Mp2SettingsOutputTypeDef",
     {
         "Bitrate": int,
         "Channels": int,
         "SampleRate": int,
     },
-    total=False,
 )
 
 Mp3SettingsOutputTypeDef = TypedDict(
     "Mp3SettingsOutputTypeDef",
     {
         "Bitrate": int,
         "Channels": int,
         "RateControlMode": Mp3RateControlModeType,
         "SampleRate": int,
         "VbrQuality": int,
     },
-    total=False,
 )
 
 OpusSettingsOutputTypeDef = TypedDict(
     "OpusSettingsOutputTypeDef",
     {
         "Bitrate": int,
         "Channels": int,
         "SampleRate": int,
     },
-    total=False,
 )
 
 VorbisSettingsOutputTypeDef = TypedDict(
     "VorbisSettingsOutputTypeDef",
     {
         "Channels": int,
         "SampleRate": int,
         "VbrQuality": int,
     },
-    total=False,
 )
 
 WavSettingsOutputTypeDef = TypedDict(
     "WavSettingsOutputTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "Format": WavFormatType,
         "SampleRate": int,
     },
-    total=False,
 )
 
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Literal["COMPLETE_MAIN"],
@@ -1215,15 +1201,14 @@
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
         "CorrectionGateLevel": int,
         "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
-    total=False,
 )
 
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
@@ -1237,15 +1222,14 @@
 )
 
 AudioSelectorGroupOutputTypeDef = TypedDict(
     "AudioSelectorGroupOutputTypeDef",
     {
         "AudioSelectorNames": List[str],
     },
-    total=False,
 )
 
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
@@ -1255,15 +1239,14 @@
 HlsRenditionGroupSettingsOutputTypeDef = TypedDict(
     "HlsRenditionGroupSettingsOutputTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
-    total=False,
 )
 
 HlsRenditionGroupSettingsTypeDef = TypedDict(
     "HlsRenditionGroupSettingsTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
@@ -1274,33 +1257,30 @@
 
 ForceIncludeRenditionSizeOutputTypeDef = TypedDict(
     "ForceIncludeRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Width": int,
     },
-    total=False,
 )
 
 MinBottomRenditionSizeOutputTypeDef = TypedDict(
     "MinBottomRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Width": int,
     },
-    total=False,
 )
 
 MinTopRenditionSizeOutputTypeDef = TypedDict(
     "MinTopRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Width": int,
     },
-    total=False,
 )
 
 ForceIncludeRenditionSizeTypeDef = TypedDict(
     "ForceIncludeRenditionSizeTypeDef",
     {
         "Height": int,
         "Width": int,
@@ -1328,15 +1308,14 @@
 
 Av1QvbrSettingsOutputTypeDef = TypedDict(
     "Av1QvbrSettingsOutputTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
-    total=False,
 )
 
 Av1QvbrSettingsTypeDef = TypedDict(
     "Av1QvbrSettingsTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
@@ -1345,15 +1324,14 @@
 )
 
 AvailBlankingOutputTypeDef = TypedDict(
     "AvailBlankingOutputTypeDef",
     {
         "AvailBlankingImage": str,
     },
-    total=False,
 )
 
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": str,
     },
@@ -1361,15 +1339,14 @@
 )
 
 AvcIntraUhdSettingsOutputTypeDef = TypedDict(
     "AvcIntraUhdSettingsOutputTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
-    total=False,
 )
 
 AvcIntraUhdSettingsTypeDef = TypedDict(
     "AvcIntraUhdSettingsTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
@@ -1378,15 +1355,14 @@
 
 BandwidthReductionFilterOutputTypeDef = TypedDict(
     "BandwidthReductionFilterOutputTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
     },
-    total=False,
 )
 
 BandwidthReductionFilterTypeDef = TypedDict(
     "BandwidthReductionFilterTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
@@ -1415,15 +1391,14 @@
         "ShadowXOffset": int,
         "ShadowYOffset": int,
         "StylePassthrough": BurnInSubtitleStylePassthroughType,
         "TeletextSpacing": BurninSubtitleTeletextSpacingType,
         "XPosition": int,
         "YPosition": int,
     },
-    total=False,
 )
 
 BurninDestinationSettingsTypeDef = TypedDict(
     "BurninDestinationSettingsTypeDef",
     {
         "Alignment": BurninSubtitleAlignmentType,
         "ApplyFontColor": BurninSubtitleApplyFontColorType,
@@ -1484,75 +1459,67 @@
         "StylePassthrough": DvbSubtitleStylePassthroughType,
         "SubtitlingType": DvbSubtitlingTypeType,
         "TeletextSpacing": DvbSubtitleTeletextSpacingType,
         "Width": int,
         "XPosition": int,
         "YPosition": int,
     },
-    total=False,
 )
 
 EmbeddedDestinationSettingsOutputTypeDef = TypedDict(
     "EmbeddedDestinationSettingsOutputTypeDef",
     {
         "Destination608ChannelNumber": int,
         "Destination708ServiceNumber": int,
     },
-    total=False,
 )
 
 ImscDestinationSettingsOutputTypeDef = TypedDict(
     "ImscDestinationSettingsOutputTypeDef",
     {
         "Accessibility": ImscAccessibilitySubsType,
         "StylePassthrough": ImscStylePassthroughType,
     },
-    total=False,
 )
 
 SccDestinationSettingsOutputTypeDef = TypedDict(
     "SccDestinationSettingsOutputTypeDef",
     {
         "Framerate": SccDestinationFramerateType,
     },
-    total=False,
 )
 
 SrtDestinationSettingsOutputTypeDef = TypedDict(
     "SrtDestinationSettingsOutputTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
-    total=False,
 )
 
 TeletextDestinationSettingsOutputTypeDef = TypedDict(
     "TeletextDestinationSettingsOutputTypeDef",
     {
         "PageNumber": str,
         "PageTypes": List[TeletextPageTypeType],
     },
-    total=False,
 )
 
 TtmlDestinationSettingsOutputTypeDef = TypedDict(
     "TtmlDestinationSettingsOutputTypeDef",
     {
         "StylePassthrough": TtmlStylePassthroughType,
     },
-    total=False,
 )
 
 WebvttDestinationSettingsOutputTypeDef = TypedDict(
     "WebvttDestinationSettingsOutputTypeDef",
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
-    total=False,
 )
 
 DvbSubDestinationSettingsTypeDef = TypedDict(
     "DvbSubDestinationSettingsTypeDef",
     {
         "Alignment": DvbSubtitleAlignmentType,
         "ApplyFontColor": DvbSubtitleApplyFontColorType,
@@ -1647,15 +1614,14 @@
 
 CaptionSourceFramerateOutputTypeDef = TypedDict(
     "CaptionSourceFramerateOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
-    total=False,
 )
 
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -1664,52 +1630,47 @@
 )
 
 DvbSubSourceSettingsOutputTypeDef = TypedDict(
     "DvbSubSourceSettingsOutputTypeDef",
     {
         "Pid": int,
     },
-    total=False,
 )
 
 EmbeddedSourceSettingsOutputTypeDef = TypedDict(
     "EmbeddedSourceSettingsOutputTypeDef",
     {
         "Convert608To708": EmbeddedConvert608To708Type,
         "Source608ChannelNumber": int,
         "Source608TrackNumber": int,
         "TerminateCaptions": EmbeddedTerminateCaptionsType,
     },
-    total=False,
 )
 
 TeletextSourceSettingsOutputTypeDef = TypedDict(
     "TeletextSourceSettingsOutputTypeDef",
     {
         "PageNumber": str,
     },
-    total=False,
 )
 
 TrackSourceSettingsOutputTypeDef = TypedDict(
     "TrackSourceSettingsOutputTypeDef",
     {
         "TrackNumber": int,
     },
-    total=False,
 )
 
 WebvttHlsSourceSettingsOutputTypeDef = TypedDict(
     "WebvttHlsSourceSettingsOutputTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
-    total=False,
 )
 
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "Pid": int,
     },
@@ -1755,15 +1716,14 @@
 
 OutputChannelMappingOutputTypeDef = TypedDict(
     "OutputChannelMappingOutputTypeDef",
     {
         "InputChannels": List[int],
         "InputChannelsFineTune": List[float],
     },
-    total=False,
 )
 
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
@@ -1775,15 +1735,14 @@
     "ClipLimitsOutputTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
-    total=False,
 )
 
 ClipLimitsTypeDef = TypedDict(
     "ClipLimitsTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
@@ -1795,15 +1754,14 @@
 
 CmafAdditionalManifestOutputTypeDef = TypedDict(
     "CmafAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -1816,26 +1774,24 @@
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": List[str],
         "HlsSignaledSystemIds": List[str],
         "ResourceId": str,
         "Url": str,
     },
-    total=False,
 )
 
 StaticKeyProviderOutputTypeDef = TypedDict(
     "StaticKeyProviderOutputTypeDef",
     {
         "KeyFormat": str,
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderCmafTypeDef = TypedDict(
     "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": Sequence[str],
@@ -1863,15 +1819,14 @@
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
-    total=False,
 )
 
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
@@ -1897,15 +1852,14 @@
         "Scte35Esam": CmfcScte35EsamType,
         "Scte35Source": CmfcScte35SourceType,
         "TimedMetadata": CmfcTimedMetadataType,
         "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
-    total=False,
 )
 
 CmfcSettingsTypeDef = TypedDict(
     "CmfcSettingsTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "AudioGroupId": str,
@@ -1937,15 +1891,14 @@
         "MaxLuminance": int,
         "MinLuminance": int,
         "RedPrimaryX": int,
         "RedPrimaryY": int,
         "WhitePointX": int,
         "WhitePointY": int,
     },
-    total=False,
 )
 
 Hdr10MetadataTypeDef = TypedDict(
     "Hdr10MetadataTypeDef",
     {
         "BluePrimaryX": int,
         "BluePrimaryY": int,
@@ -1964,15 +1917,14 @@
 )
 
 F4vSettingsOutputTypeDef = TypedDict(
     "F4vSettingsOutputTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
-    total=False,
 )
 
 M3u8SettingsOutputTypeDef = TypedDict(
     "M3u8SettingsOutputTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
@@ -1990,40 +1942,37 @@
         "Scte35Pid": int,
         "Scte35Source": M3u8Scte35SourceType,
         "TimedMetadata": TimedMetadataType,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
 MovSettingsOutputTypeDef = TypedDict(
     "MovSettingsOutputTypeDef",
     {
         "ClapAtom": MovClapAtomType,
         "CslgAtom": MovCslgAtomType,
         "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
         "PaddingControl": MovPaddingControlType,
         "Reference": MovReferenceType,
     },
-    total=False,
 )
 
 Mp4SettingsOutputTypeDef = TypedDict(
     "Mp4SettingsOutputTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "CslgAtom": Mp4CslgAtomType,
         "CttsVersion": int,
         "FreeSpaceBox": Mp4FreeSpaceBoxType,
         "MoovPlacement": Mp4MoovPlacementType,
         "Mp4MajorBrand": str,
     },
-    total=False,
 )
 
 MpdSettingsOutputTypeDef = TypedDict(
     "MpdSettingsOutputTypeDef",
     {
         "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
         "AudioDuration": MpdAudioDurationType,
@@ -2033,15 +1982,14 @@
         "Scte35Esam": MpdScte35EsamType,
         "Scte35Source": MpdScte35SourceType,
         "TimedMetadata": MpdTimedMetadataType,
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
-    total=False,
 )
 
 F4vSettingsTypeDef = TypedDict(
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
@@ -2123,14 +2071,25 @@
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
     total=False,
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
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
@@ -2138,15 +2097,14 @@
 
 DashAdditionalManifestOutputTypeDef = TypedDict(
     "DashAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -2158,15 +2116,14 @@
     "SpekeKeyProviderOutputTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": List[str],
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
@@ -2182,15 +2139,14 @@
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
-    total=False,
 )
 
 DashIsoImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
@@ -2205,15 +2161,14 @@
 DeinterlacerOutputTypeDef = TypedDict(
     "DeinterlacerOutputTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
         "Mode": DeinterlacerModeType,
     },
-    total=False,
 )
 
 DeinterlacerTypeDef = TypedDict(
     "DeinterlacerTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
@@ -2239,19 +2194,20 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -2263,15 +2219,14 @@
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Url": str,
     },
-    total=False,
 )
 
 DisassociateCertificateRequestRequestTypeDef = TypedDict(
     "DisassociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
@@ -2279,15 +2234,14 @@
 
 DolbyVisionLevel6MetadataOutputTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataOutputTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
-    total=False,
 )
 
 DolbyVisionLevel6MetadataTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
@@ -2298,15 +2252,14 @@
 DvbNitSettingsOutputTypeDef = TypedDict(
     "DvbNitSettingsOutputTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
         "NitInterval": int,
     },
-    total=False,
 )
 
 DvbNitSettingsTypeDef = TypedDict(
     "DvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
@@ -2319,15 +2272,14 @@
     "DvbSdtSettingsOutputTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
-    total=False,
 )
 
 DvbSdtSettingsTypeDef = TypedDict(
     "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
@@ -2338,15 +2290,14 @@
 )
 
 DvbTdtSettingsOutputTypeDef = TypedDict(
     "DvbTdtSettingsOutputTypeDef",
     {
         "TdtInterval": int,
     },
-    total=False,
 )
 
 DvbTdtSettingsTypeDef = TypedDict(
     "DvbTdtSettingsTypeDef",
     {
         "TdtInterval": int,
     },
@@ -2354,15 +2305,14 @@
 )
 
 EsamManifestConfirmConditionNotificationOutputTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationOutputTypeDef",
     {
         "MccXml": str,
     },
-    total=False,
 )
 
 EsamManifestConfirmConditionNotificationTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationTypeDef",
     {
         "MccXml": str,
     },
@@ -2370,15 +2320,14 @@
 )
 
 EsamSignalProcessingNotificationOutputTypeDef = TypedDict(
     "EsamSignalProcessingNotificationOutputTypeDef",
     {
         "SccXml": str,
     },
-    total=False,
 )
 
 EsamSignalProcessingNotificationTypeDef = TypedDict(
     "EsamSignalProcessingNotificationTypeDef",
     {
         "SccXml": str,
     },
@@ -2387,15 +2336,14 @@
 
 ExtendedDataServicesOutputTypeDef = TypedDict(
     "ExtendedDataServicesOutputTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
     },
-    total=False,
 )
 
 ExtendedDataServicesTypeDef = TypedDict(
     "ExtendedDataServicesTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
@@ -2407,15 +2355,14 @@
     "FrameCaptureSettingsOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "MaxCaptures": int,
         "Quality": int,
     },
-    total=False,
 )
 
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2442,15 +2389,14 @@
 PolicyOutputTypeDef = TypedDict(
     "PolicyOutputTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
         "S3Inputs": InputPolicyType,
     },
-    total=False,
 )
 
 GetPresetRequestRequestTypeDef = TypedDict(
     "GetPresetRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -2466,15 +2412,14 @@
 H264QvbrSettingsOutputTypeDef = TypedDict(
     "H264QvbrSettingsOutputTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
-    total=False,
 )
 
 H264QvbrSettingsTypeDef = TypedDict(
     "H264QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
@@ -2486,15 +2431,14 @@
 H265QvbrSettingsOutputTypeDef = TypedDict(
     "H265QvbrSettingsOutputTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
-    total=False,
 )
 
 H265QvbrSettingsTypeDef = TypedDict(
     "H265QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
@@ -2505,15 +2449,14 @@
 
 Hdr10PlusOutputTypeDef = TypedDict(
     "Hdr10PlusOutputTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
-    total=False,
 )
 
 Hdr10PlusTypeDef = TypedDict(
     "Hdr10PlusTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
@@ -2523,15 +2466,14 @@
 
 HlsAdditionalManifestOutputTypeDef = TypedDict(
     "HlsAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -2543,15 +2485,14 @@
     "HlsCaptionLanguageMappingOutputTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 HlsCaptionLanguageMappingTypeDef = TypedDict(
     "HlsCaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
@@ -2567,15 +2508,14 @@
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
-    total=False,
 )
 
 HlsImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "HlsImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
@@ -2594,34 +2534,31 @@
         "AudioOnlyContainer": HlsAudioOnlyContainerType,
         "AudioRenditionSets": str,
         "AudioTrackType": HlsAudioTrackTypeType,
         "DescriptiveVideoServiceFlag": HlsDescriptiveVideoServiceFlagType,
         "IFrameOnlyManifest": HlsIFrameOnlyManifestType,
         "SegmentModifier": str,
     },
-    total=False,
 )
 
 HopDestinationOutputTypeDef = TypedDict(
     "HopDestinationOutputTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
-    total=False,
 )
 
 Id3InsertionOutputTypeDef = TypedDict(
     "Id3InsertionOutputTypeDef",
     {
         "Id3": str,
         "Timecode": str,
     },
-    total=False,
 )
 
 Id3InsertionTypeDef = TypedDict(
     "Id3InsertionTypeDef",
     {
         "Id3": str,
         "Timecode": str,
@@ -2640,15 +2577,14 @@
         "ImageX": int,
         "ImageY": int,
         "Layer": int,
         "Opacity": int,
         "StartTime": str,
         "Width": int,
     },
-    total=False,
 )
 
 InsertableImageTypeDef = TypedDict(
     "InsertableImageTypeDef",
     {
         "Duration": int,
         "FadeIn": int,
@@ -2667,15 +2603,14 @@
 
 InputClippingOutputTypeDef = TypedDict(
     "InputClippingOutputTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
     },
-    total=False,
 )
 
 InputClippingTypeDef = TypedDict(
     "InputClippingTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
@@ -2687,15 +2622,14 @@
     "InputDecryptionSettingsOutputTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
-    total=False,
 )
 
 InputDecryptionSettingsTypeDef = TypedDict(
     "InputDecryptionSettingsTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
@@ -2706,26 +2640,24 @@
 )
 
 InputVideoGeneratorOutputTypeDef = TypedDict(
     "InputVideoGeneratorOutputTypeDef",
     {
         "Duration": int,
     },
-    total=False,
 )
 
 RectangleOutputTypeDef = TypedDict(
     "RectangleOutputTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
-    total=False,
 )
 
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
@@ -2745,15 +2677,14 @@
 
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
-    total=False,
 )
 
 KantarWatermarkSettingsOutputTypeDef = TypedDict(
     "KantarWatermarkSettingsOutputTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -2765,24 +2696,22 @@
         "Metadata3": str,
         "Metadata4": str,
         "Metadata5": str,
         "Metadata6": str,
         "Metadata7": str,
         "Metadata8": str,
     },
-    total=False,
 )
 
 NielsenConfigurationOutputTypeDef = TypedDict(
     "NielsenConfigurationOutputTypeDef",
     {
         "BreakoutCode": int,
         "DistributorId": str,
     },
-    total=False,
 )
 
 NielsenNonLinearWatermarkSettingsOutputTypeDef = TypedDict(
     "NielsenNonLinearWatermarkSettingsOutputTypeDef",
     {
         "ActiveWatermarkProcess": NielsenActiveWatermarkProcessTypeType,
         "AdiFilename": str,
@@ -2792,26 +2721,24 @@
         "EpisodeId": str,
         "MetadataDestination": str,
         "SourceId": int,
         "SourceWatermarkStatus": NielsenSourceWatermarkStatusTypeType,
         "TicServerUrl": str,
         "UniqueTicPerAudioTrack": NielsenUniqueTicPerAudioTrackTypeType,
     },
-    total=False,
 )
 
 TimecodeConfigOutputTypeDef = TypedDict(
     "TimecodeConfigOutputTypeDef",
     {
         "Anchor": str,
         "Source": TimecodeSourceType,
         "Start": str,
         "TimestampOffset": str,
     },
-    total=False,
 )
 
 KantarWatermarkSettingsTypeDef = TypedDict(
     "KantarWatermarkSettingsTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -2871,114 +2798,69 @@
 QueueTransitionTypeDef = TypedDict(
     "QueueTransitionTypeDef",
     {
         "DestinationQueue": str,
         "SourceQueue": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
-    total=False,
 )
 
 WarningGroupTypeDef = TypedDict(
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
     },
 )
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -2995,23 +2877,21 @@
 
 ResourceTagsTypeDef = TypedDict(
     "ResourceTagsTypeDef",
     {
         "Arn": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 M2tsScte35EsamOutputTypeDef = TypedDict(
     "M2tsScte35EsamOutputTypeDef",
     {
         "Scte35EsamPid": int,
     },
-    total=False,
 )
 
 M2tsScte35EsamTypeDef = TypedDict(
     "M2tsScte35EsamTypeDef",
     {
         "Scte35EsamPid": int,
     },
@@ -3020,24 +2900,22 @@
 
 MotionImageInsertionFramerateOutputTypeDef = TypedDict(
     "MotionImageInsertionFramerateOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
-    total=False,
 )
 
 MotionImageInsertionOffsetOutputTypeDef = TypedDict(
     "MotionImageInsertionOffsetOutputTypeDef",
     {
         "ImageX": int,
         "ImageY": int,
     },
-    total=False,
 )
 
 MotionImageInsertionFramerateTypeDef = TypedDict(
     "MotionImageInsertionFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -3087,15 +2965,14 @@
         "SlowPal": Mpeg2SlowPalType,
         "Softness": int,
         "SpatialAdaptiveQuantization": Mpeg2SpatialAdaptiveQuantizationType,
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
-    total=False,
 )
 
 Mpeg2SettingsTypeDef = TypedDict(
     "Mpeg2SettingsTypeDef",
     {
         "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
         "Bitrate": int,
@@ -3136,15 +3013,14 @@
 
 MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
     "MsSmoothAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -3154,15 +3030,14 @@
 
 MxfXavcProfileSettingsOutputTypeDef = TypedDict(
     "MxfXavcProfileSettingsOutputTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
     },
-    total=False,
 )
 
 MxfXavcProfileSettingsTypeDef = TypedDict(
     "MxfXavcProfileSettingsTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
@@ -3174,15 +3049,14 @@
     "NexGuardFileMarkerSettingsOutputTypeDef",
     {
         "License": str,
         "Payload": int,
         "Preset": str,
         "Strength": WatermarkingStrengthType,
     },
-    total=False,
 )
 
 NexGuardFileMarkerSettingsTypeDef = TypedDict(
     "NexGuardFileMarkerSettingsTypeDef",
     {
         "License": str,
         "Payload": int,
@@ -3193,15 +3067,14 @@
 )
 
 NoiseReducerFilterSettingsOutputTypeDef = TypedDict(
     "NoiseReducerFilterSettingsOutputTypeDef",
     {
         "Strength": int,
     },
-    total=False,
 )
 
 NoiseReducerFilterSettingsTypeDef = TypedDict(
     "NoiseReducerFilterSettingsTypeDef",
     {
         "Strength": int,
     },
@@ -3211,27 +3084,25 @@
 NoiseReducerSpatialFilterSettingsOutputTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsOutputTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
         "Strength": int,
     },
-    total=False,
 )
 
 NoiseReducerTemporalFilterSettingsOutputTypeDef = TypedDict(
     "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     {
         "AggressiveMode": int,
         "PostTemporalSharpening": NoiseFilterPostTemporalSharpeningType,
         "PostTemporalSharpeningStrength": NoiseFilterPostTemporalSharpeningStrengthType,
         "Speed": int,
         "Strength": int,
     },
-    total=False,
 )
 
 NoiseReducerSpatialFilterSettingsTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
@@ -3254,25 +3125,14 @@
 
 VideoDetailTypeDef = TypedDict(
     "VideoDetailTypeDef",
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
-    total=False,
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
 )
 
 PolicyTypeDef = TypedDict(
     "PolicyTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
@@ -3294,15 +3154,14 @@
         "ParControl": ProresParControlType,
         "ParDenominator": int,
         "ParNumerator": int,
         "ScanTypeConversionMode": ProresScanTypeConversionModeType,
         "SlowPal": ProresSlowPalType,
         "Telecine": ProresTelecineType,
     },
-    total=False,
 )
 
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
@@ -3327,34 +3186,21 @@
         "Commitment": Literal["ONE_YEAR"],
         "ExpiresAt": datetime,
         "PurchasedAt": datetime,
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
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
 
 S3DestinationAccessControlOutputTypeDef = TypedDict(
     "S3DestinationAccessControlOutputTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
-    total=False,
 )
 
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
@@ -3364,15 +3210,14 @@
 S3EncryptionSettingsOutputTypeDef = TypedDict(
     "S3EncryptionSettingsOutputTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
         "KmsKeyArn": str,
     },
-    total=False,
 )
 
 S3EncryptionSettingsTypeDef = TypedDict(
     "S3EncryptionSettingsTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
@@ -3392,15 +3237,14 @@
 TimecodeBurninOutputTypeDef = TypedDict(
     "TimecodeBurninOutputTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
         "Prefix": str,
     },
-    total=False,
 )
 
 TimecodeBurninTypeDef = TypedDict(
     "TimecodeBurninTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
@@ -3439,15 +3283,14 @@
         "FramerateNumerator": int,
         "InterlaceMode": Vc3InterlaceModeType,
         "ScanTypeConversionMode": Vc3ScanTypeConversionModeType,
         "SlowPal": Vc3SlowPalType,
         "Telecine": Vc3TelecineType,
         "Vc3Class": Vc3ClassType,
     },
-    total=False,
 )
 
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
@@ -3475,15 +3318,14 @@
         "MaxBitrate": int,
         "ParControl": Vp8ParControlType,
         "ParDenominator": int,
         "ParNumerator": int,
         "QualityTuningLevel": Vp8QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
-    total=False,
 )
 
 Vp9SettingsOutputTypeDef = TypedDict(
     "Vp9SettingsOutputTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp9FramerateControlType,
@@ -3495,15 +3337,14 @@
         "MaxBitrate": int,
         "ParControl": Vp9ParControlType,
         "ParDenominator": int,
         "ParNumerator": int,
         "QualityTuningLevel": Vp9QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
-    total=False,
 )
 
 Vp8SettingsTypeDef = TypedDict(
     "Vp8SettingsTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp8FramerateControlType,
@@ -3543,15 +3384,14 @@
 )
 
 Xavc4kIntraCbgProfileSettingsOutputTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
-    total=False,
 )
 
 Xavc4kIntraCbgProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
@@ -3559,15 +3399,14 @@
 )
 
 Xavc4kIntraVbrProfileSettingsOutputTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
-    total=False,
 )
 
 Xavc4kIntraVbrProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
@@ -3582,15 +3421,14 @@
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
         "GopClosedCadence": int,
         "HrdBufferSize": int,
         "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
         "Slices": int,
     },
-    total=False,
 )
 
 Xavc4kProfileSettingsTypeDef = TypedDict(
     "Xavc4kProfileSettingsTypeDef",
     {
         "BitrateClass": Xavc4kProfileBitrateClassType,
         "CodecProfile": Xavc4kProfileCodecProfileType,
@@ -3605,15 +3443,14 @@
 )
 
 XavcHdIntraCbgProfileSettingsOutputTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsOutputTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
-    total=False,
 )
 
 XavcHdIntraCbgProfileSettingsTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
@@ -3629,15 +3466,14 @@
         "GopClosedCadence": int,
         "HrdBufferSize": int,
         "InterlaceMode": XavcInterlaceModeType,
         "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
         "Slices": int,
         "Telecine": XavcHdProfileTelecineType,
     },
-    total=False,
 )
 
 XavcHdProfileSettingsTypeDef = TypedDict(
     "XavcHdProfileSettingsTypeDef",
     {
         "BitrateClass": XavcHdProfileBitrateClassType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
@@ -3663,15 +3499,14 @@
         "Eac3Settings": Eac3SettingsOutputTypeDef,
         "Mp2Settings": Mp2SettingsOutputTypeDef,
         "Mp3Settings": Mp3SettingsOutputTypeDef,
         "OpusSettings": OpusSettingsOutputTypeDef,
         "VorbisSettings": VorbisSettingsOutputTypeDef,
         "WavSettings": WavSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
@@ -3693,15 +3528,14 @@
     {
         "AllowedRenditions": List[AllowedRenditionSizeOutputTypeDef],
         "ForceIncludeRenditions": List[ForceIncludeRenditionSizeOutputTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeOutputTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeOutputTypeDef,
         "Type": RuleTypeType,
     },
-    total=False,
 )
 
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
@@ -3725,15 +3559,14 @@
         "MaxBitrate": int,
         "NumberBFramesBetweenReferenceFrames": int,
         "QvbrSettings": Av1QvbrSettingsOutputTypeDef,
         "RateControlMode": Literal["QVBR"],
         "Slices": int,
         "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
     },
-    total=False,
 )
 
 Av1SettingsTypeDef = TypedDict(
     "Av1SettingsTypeDef",
     {
         "AdaptiveQuantization": Av1AdaptiveQuantizationType,
         "BitDepth": Av1BitDepthType,
@@ -3762,15 +3595,14 @@
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "InterlaceMode": AvcIntraInterlaceModeType,
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
-    total=False,
 )
 
 AvcIntraSettingsTypeDef = TypedDict(
     "AvcIntraSettingsTypeDef",
     {
         "AvcIntraClass": AvcIntraClassType,
         "AvcIntraUhdSettings": AvcIntraUhdSettingsTypeDef,
@@ -3796,15 +3628,14 @@
         "ImscDestinationSettings": ImscDestinationSettingsOutputTypeDef,
         "SccDestinationSettings": SccDestinationSettingsOutputTypeDef,
         "SrtDestinationSettings": SrtDestinationSettingsOutputTypeDef,
         "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
         "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
         "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
@@ -3826,15 +3657,14 @@
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateOutputTypeDef,
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
-    total=False,
 )
 
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
@@ -3847,15 +3677,14 @@
 )
 
 ChannelMappingOutputTypeDef = TypedDict(
     "ChannelMappingOutputTypeDef",
     {
         "OutputChannels": List[OutputChannelMappingOutputTypeDef],
     },
-    total=False,
 )
 
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
@@ -3868,15 +3697,14 @@
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
         "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
-    total=False,
 )
 
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
@@ -3898,15 +3726,14 @@
         "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
         "HdrToSdrToneMapper": HDRToSDRToneMapperType,
         "Hue": int,
         "SampleRangeConversion": SampleRangeConversionType,
         "Saturation": int,
         "SdrReferenceWhiteLevel": int,
     },
-    total=False,
 )
 
 VideoSelectorOutputTypeDef = TypedDict(
     "VideoSelectorOutputTypeDef",
     {
         "AlphaBehavior": AlphaBehaviorType,
         "ColorSpace": ColorSpaceType,
@@ -3915,15 +3742,14 @@
         "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
         "PadVideo": PadVideoType,
         "Pid": int,
         "ProgramNumber": int,
         "Rotate": InputRotateType,
         "SampleRange": InputSampleRangeType,
     },
-    total=False,
 )
 
 ColorCorrectorTypeDef = TypedDict(
     "ColorCorrectorTypeDef",
     {
         "Brightness": int,
         "ClipLimits": ClipLimitsTypeDef,
@@ -4006,37 +3832,34 @@
 
 DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
     "DashIsoEncryptionSettingsOutputTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 HlsEncryptionSettingsOutputTypeDef = TypedDict(
     "HlsEncryptionSettingsOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": HlsEncryptionTypeType,
         "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
         "OfflineEncrypted": HlsOfflineEncryptedType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
         "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": HlsKeyProviderTypeType,
     },
-    total=False,
 )
 
 MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
     "MsSmoothEncryptionSettingsOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -4062,32 +3885,83 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    {
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DolbyVisionOutputTypeDef = TypedDict(
     "DolbyVisionOutputTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataOutputTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
         "Mapping": DolbyVisionMappingType,
         "Profile": DolbyVisionProfileType,
     },
-    total=False,
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
@@ -4102,15 +3976,14 @@
     {
         "ManifestConfirmConditionNotification": (
             EsamManifestConfirmConditionNotificationOutputTypeDef
         ),
         "ResponseSignalPreroll": int,
         "SignalProcessingNotification": EsamSignalProcessingNotificationOutputTypeDef,
     },
-    total=False,
 )
 
 EsamSettingsTypeDef = TypedDict(
     "EsamSettingsTypeDef",
     {
         "ManifestConfirmConditionNotification": EsamManifestConfirmConditionNotificationTypeDef,
         "ResponseSignalPreroll": int,
@@ -4119,23 +3992,23 @@
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 H264SettingsOutputTypeDef = TypedDict(
     "H264SettingsOutputTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -4177,15 +4050,14 @@
         "Softness": int,
         "SpatialAdaptiveQuantization": H264SpatialAdaptiveQuantizationType,
         "Syntax": H264SyntaxType,
         "Telecine": H264TelecineType,
         "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
         "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
-    total=False,
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
@@ -4275,15 +4147,14 @@
         "Telecine": H265TelecineType,
         "TemporalAdaptiveQuantization": H265TemporalAdaptiveQuantizationType,
         "TemporalIds": H265TemporalIdsType,
         "Tiles": H265TilesType,
         "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
         "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
     },
-    total=False,
 )
 
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
@@ -4332,23 +4203,21 @@
 )
 
 OutputSettingsOutputTypeDef = TypedDict(
     "OutputSettingsOutputTypeDef",
     {
         "HlsSettings": HlsSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 TimedMetadataInsertionOutputTypeDef = TypedDict(
     "TimedMetadataInsertionOutputTypeDef",
     {
         "Id3Insertions": List[Id3InsertionOutputTypeDef],
     },
-    total=False,
 )
 
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
@@ -4357,15 +4226,14 @@
 
 ImageInserterOutputTypeDef = TypedDict(
     "ImageInserterOutputTypeDef",
     {
         "InsertableImages": List[InsertableImageOutputTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
-    total=False,
 )
 
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
@@ -4373,15 +4241,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 M2tsSettingsOutputTypeDef = TypedDict(
     "M2tsSettingsOutputTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
@@ -4420,15 +4288,14 @@
         "SegmentationMarkers": M2tsSegmentationMarkersType,
         "SegmentationStyle": M2tsSegmentationStyleType,
         "SegmentationTime": float,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
@@ -4479,15 +4346,14 @@
         "Framerate": MotionImageInsertionFramerateOutputTypeDef,
         "Input": str,
         "InsertionMode": MotionImageInsertionModeType,
         "Offset": MotionImageInsertionOffsetOutputTypeDef,
         "Playback": MotionImagePlaybackType,
         "StartTime": str,
     },
-    total=False,
 )
 
 MotionImageInserterTypeDef = TypedDict(
     "MotionImageInserterTypeDef",
     {
         "Framerate": MotionImageInsertionFramerateTypeDef,
         "Input": str,
@@ -4502,15 +4368,14 @@
 MxfSettingsOutputTypeDef = TypedDict(
     "MxfSettingsOutputTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
         "XavcProfileSettings": MxfXavcProfileSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 MxfSettingsTypeDef = TypedDict(
     "MxfSettingsTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
@@ -4520,15 +4385,14 @@
 )
 
 PartnerWatermarkingOutputTypeDef = TypedDict(
     "PartnerWatermarkingOutputTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 PartnerWatermarkingTypeDef = TypedDict(
     "PartnerWatermarkingTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsTypeDef,
     },
@@ -4539,15 +4403,14 @@
     "NoiseReducerOutputTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsOutputTypeDef,
         "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsOutputTypeDef,
         "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 NoiseReducerTypeDef = TypedDict(
     "NoiseReducerTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsTypeDef,
@@ -4559,59 +4422,46 @@
 
 OutputDetailTypeDef = TypedDict(
     "OutputDetailTypeDef",
     {
         "DurationInMs": int,
         "VideoDetails": VideoDetailTypeDef,
     },
-    total=False,
 )
 
 PutPolicyRequestRequestTypeDef = TypedDict(
     "PutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 
-_RequiredQueueTypeDef = TypedDict(
-    "_RequiredQueueTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalQueueTypeDef = TypedDict(
-    "_OptionalQueueTypeDef",
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
         "PricingPlan": PricingPlanType,
         "ProgressingJobsCount": int,
         "ReservationPlan": ReservationPlanTypeDef,
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
-    total=False,
 )
 
-
-class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
-    pass
-
-
 S3DestinationSettingsOutputTypeDef = TypedDict(
     "S3DestinationSettingsOutputTypeDef",
     {
         "AccessControl": S3DestinationAccessControlOutputTypeDef,
         "Encryption": S3EncryptionSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
@@ -4635,15 +4485,14 @@
         "TemporalAdaptiveQuantization": XavcTemporalAdaptiveQuantizationType,
         "Xavc4kIntraCbgProfileSettings": Xavc4kIntraCbgProfileSettingsOutputTypeDef,
         "Xavc4kIntraVbrProfileSettings": Xavc4kIntraVbrProfileSettingsOutputTypeDef,
         "Xavc4kProfileSettings": Xavc4kProfileSettingsOutputTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsOutputTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 XavcSettingsTypeDef = TypedDict(
     "XavcSettingsTypeDef",
     {
         "AdaptiveQuantization": XavcAdaptiveQuantizationType,
         "EntropyEncoding": XavcEntropyEncodingType,
@@ -4669,15 +4518,14 @@
     "AutomatedAbrSettingsOutputTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": List[AutomatedAbrRuleOutputTypeDef],
     },
-    total=False,
 )
 
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
@@ -4692,26 +4540,24 @@
     {
         "CaptionSelectorName": str,
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 CaptionDescriptionPresetOutputTypeDef = TypedDict(
     "CaptionDescriptionPresetOutputTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
@@ -4729,15 +4575,14 @@
         "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
         "FileSourceSettings": FileSourceSettingsOutputTypeDef,
         "SourceType": CaptionSourceTypeType,
         "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
         "TrackSourceSettings": TrackSourceSettingsOutputTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionSourceSettingsTypeDef = TypedDict(
     "CaptionSourceSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
@@ -4754,15 +4599,14 @@
 RemixSettingsOutputTypeDef = TypedDict(
     "RemixSettingsOutputTypeDef",
     {
         "ChannelMapping": ChannelMappingOutputTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
-    total=False,
 )
 
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
@@ -4780,15 +4624,14 @@
         "M2tsSettings": M2tsSettingsOutputTypeDef,
         "M3u8Settings": M3u8SettingsOutputTypeDef,
         "MovSettings": MovSettingsOutputTypeDef,
         "Mp4Settings": Mp4SettingsOutputTypeDef,
         "MpdSettings": MpdSettingsOutputTypeDef,
         "MxfSettings": MxfSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
@@ -4811,15 +4654,14 @@
         "DolbyVision": DolbyVisionOutputTypeDef,
         "Hdr10Plus": Hdr10PlusOutputTypeDef,
         "ImageInserter": ImageInserterOutputTypeDef,
         "NoiseReducer": NoiseReducerOutputTypeDef,
         "PartnerWatermarking": PartnerWatermarkingOutputTypeDef,
         "TimecodeBurnin": TimecodeBurninOutputTypeDef,
     },
-    total=False,
 )
 
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
@@ -4834,56 +4676,54 @@
 )
 
 OutputGroupDetailTypeDef = TypedDict(
     "OutputGroupDetailTypeDef",
     {
         "OutputDetails": List[OutputDetailTypeDef],
     },
-    total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DestinationSettingsOutputTypeDef = TypedDict(
     "DestinationSettingsOutputTypeDef",
     {
         "S3Settings": S3DestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
     },
@@ -4902,15 +4742,14 @@
         "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
         "ProresSettings": ProresSettingsOutputTypeDef,
         "Vc3Settings": Vc3SettingsOutputTypeDef,
         "Vp8Settings": Vp8SettingsOutputTypeDef,
         "Vp9Settings": Vp9SettingsOutputTypeDef,
         "XavcSettings": XavcSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "Av1Settings": Av1SettingsTypeDef,
         "AvcIntraSettings": AvcIntraSettingsTypeDef,
@@ -4929,15 +4768,14 @@
 )
 
 AutomatedEncodingSettingsOutputTypeDef = TypedDict(
     "AutomatedEncodingSettingsOutputTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
@@ -4947,15 +4785,14 @@
 CaptionSelectorOutputTypeDef = TypedDict(
     "CaptionSelectorOutputTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
@@ -4975,15 +4812,14 @@
         "CodecSettings": AudioCodecSettingsOutputTypeDef,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageCodeControl": AudioLanguageCodeControlType,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "StreamName": str,
     },
-    total=False,
 )
 
 AudioSelectorOutputTypeDef = TypedDict(
     "AudioSelectorOutputTypeDef",
     {
         "AudioDurationCorrection": AudioDurationCorrectionType,
         "CustomLanguageCode": str,
@@ -4994,15 +4830,14 @@
         "Offset": int,
         "Pids": List[int],
         "ProgramSelection": int,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": List[int],
     },
-    total=False,
 )
 
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
@@ -5065,15 +4900,14 @@
         "StreamInfResolution": CmafStreamInfResolutionType,
         "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
         "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
-    total=False,
 )
 
 DashIsoGroupSettingsOutputTypeDef = TypedDict(
     "DashIsoGroupSettingsOutputTypeDef",
     {
         "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
@@ -5093,24 +4927,22 @@
         "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
         "SegmentControl": DashIsoSegmentControlType,
         "SegmentLength": int,
         "SegmentLengthControl": DashIsoSegmentLengthControlType,
         "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
         "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
     },
-    total=False,
 )
 
 FileGroupSettingsOutputTypeDef = TypedDict(
     "FileGroupSettingsOutputTypeDef",
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 HlsGroupSettingsOutputTypeDef = TypedDict(
     "HlsGroupSettingsOutputTypeDef",
     {
         "AdMarkers": List[HlsAdMarkersType],
         "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
@@ -5141,30 +4973,28 @@
         "SegmentsPerSubdirectory": int,
         "StreamInfResolution": HlsStreamInfResolutionType,
         "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
-    total=False,
 )
 
 MsSmoothGroupSettingsOutputTypeDef = TypedDict(
     "MsSmoothGroupSettingsOutputTypeDef",
     {
         "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsOutputTypeDef,
         "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
-    total=False,
 )
 
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
@@ -5303,15 +5133,14 @@
         "RespondToAfd": RespondToAfdType,
         "ScalingBehavior": ScalingBehaviorType,
         "Sharpness": int,
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
         "Width": int,
     },
-    total=False,
 )
 
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
@@ -5356,15 +5185,14 @@
         "PsiControl": InputPsiControlType,
         "SupplementalImps": List[str],
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorOutputTypeDef,
         "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateOutputTypeDef = TypedDict(
     "InputTemplateOutputTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
@@ -5383,15 +5211,14 @@
         "Position": RectangleOutputTypeDef,
         "ProgramNumber": int,
         "PsiControl": InputPsiControlType,
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
         "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
@@ -5454,15 +5281,14 @@
         "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
         "FileGroupSettings": FileGroupSettingsOutputTypeDef,
         "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
         "Type": OutputGroupTypeType,
     },
-    total=False,
 )
 
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
@@ -5482,26 +5308,24 @@
         "ContainerSettings": ContainerSettingsOutputTypeDef,
         "Extension": str,
         "NameModifier": str,
         "OutputSettings": OutputSettingsOutputTypeDef,
         "Preset": str,
         "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsOutputTypeDef = TypedDict(
     "PresetSettingsOutputTypeDef",
     {
         "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
         "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
         "ContainerSettings": ContainerSettingsOutputTypeDef,
         "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsTypeDef = TypedDict(
     "PresetSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
@@ -5516,54 +5340,42 @@
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
         "Outputs": List[OutputTypeDef],
     },
-    total=False,
 )
 
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
     total=False,
 )
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsOutputTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
     {
         "Arn": str,
         "Category": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
         "Type": TypeType,
     },
-    total=False,
 )
 
-
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
-
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": PresetSettingsTypeDef,
     },
 )
@@ -5619,15 +5431,14 @@
         "MotionImageInserter": MotionImageInserterOutputTypeDef,
         "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
         "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
         "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobTemplateSettingsOutputTypeDef = TypedDict(
     "JobTemplateSettingsOutputTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingOutputTypeDef,
@@ -5638,15 +5449,14 @@
         "MotionImageInserter": MotionImageInserterOutputTypeDef,
         "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
         "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
         "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
@@ -5683,52 +5493,45 @@
     total=False,
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPresetResponseTypeDef = TypedDict(
     "GetPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "NextToken": str,
         "Presets": List[PresetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePresetResponseTypeDef = TypedDict(
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsOutputTypeDef,
-    },
-)
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+JobTypeDef = TypedDict(
+    "JobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
         "ClientRequestToken": str,
         "CreatedAt": datetime,
@@ -5741,59 +5544,44 @@
         "JobTemplate": str,
         "Messages": JobMessagesTypeDef,
         "OutputGroupDetails": List[OutputGroupDetailTypeDef],
         "Priority": int,
         "Queue": str,
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
+        "Role": str,
+        "Settings": JobSettingsOutputTypeDef,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
-    total=False,
 )
 
-
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
-    {
-        "Name": str,
-        "Settings": JobTemplateSettingsOutputTypeDef,
-    },
-)
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+JobTemplateTypeDef = TypedDict(
+    "JobTemplateTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "Arn": str,
         "Category": str,
         "CreatedAt": datetime,
         "Description": str,
         "HopDestinations": List[HopDestinationOutputTypeDef],
         "LastUpdated": datetime,
+        "Name": str,
         "Priority": int,
         "Queue": str,
+        "Settings": JobTemplateSettingsOutputTypeDef,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Type": TypeType,
     },
-    total=False,
 )
 
-
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
-    pass
-
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Role": str,
         "Settings": JobSettingsTypeDef,
     },
 )
@@ -5879,60 +5667,60 @@
     pass
 
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert/type_defs.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -536,27 +536,28 @@
     "MpdSettingsOutputTypeDef",
     "F4vSettingsTypeDef",
     "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
     "HopDestinationTypeDef",
+    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
     "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
     "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerOutputTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
     "DolbyVisionLevel6MetadataOutputTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
     "DvbNitSettingsOutputTypeDef",
     "DvbNitSettingsTypeDef",
@@ -611,21 +612,17 @@
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamOutputTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateOutputTypeDef",
     "MotionImageInsertionOffsetOutputTypeDef",
@@ -642,20 +639,18 @@
     "NoiseReducerFilterSettingsOutputTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsOutputTypeDef",
     "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyTypeDef",
     "ProresSettingsOutputTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationAccessControlOutputTypeDef",
     "S3DestinationAccessControlTypeDef",
     "S3EncryptionSettingsOutputTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimecodeBurninOutputTypeDef",
     "TimecodeBurninTypeDef",
@@ -700,14 +695,19 @@
     "UpdateQueueRequestRequestTypeDef",
     "DashIsoEncryptionSettingsOutputTypeDef",
     "HlsEncryptionSettingsOutputTypeDef",
     "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DolbyVisionOutputTypeDef",
     "DolbyVisionTypeDef",
     "EsamSettingsOutputTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyResponseTypeDef",
@@ -825,15 +825,14 @@
         "CodingMode": AacCodingModeType,
         "RateControlMode": AacRateControlModeType,
         "RawFormat": AacRawFormatType,
         "SampleRate": int,
         "Specification": AacSpecificationType,
         "VbrQuality": AacVbrQualityType,
     },
-    total=False,
 )
 
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
         "Bitrate": int,
@@ -858,15 +857,14 @@
         "DynamicRangeCompressionLine": Ac3DynamicRangeCompressionLineType,
         "DynamicRangeCompressionProfile": Ac3DynamicRangeCompressionProfileType,
         "DynamicRangeCompressionRf": Ac3DynamicRangeCompressionRfType,
         "LfeFilter": Ac3LfeFilterType,
         "MetadataControl": Ac3MetadataControlType,
         "SampleRate": int,
     },
-    total=False,
 )
 
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Ac3BitstreamModeType,
@@ -898,15 +896,14 @@
 
 AdvancedInputFilterSettingsOutputTypeDef = TypedDict(
     "AdvancedInputFilterSettingsOutputTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
     },
-    total=False,
 )
 
 AdvancedInputFilterSettingsTypeDef = TypedDict(
     "AdvancedInputFilterSettingsTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
@@ -917,15 +914,14 @@
 AiffSettingsOutputTypeDef = TypedDict(
     "AiffSettingsOutputTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
-    total=False,
 )
 
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
@@ -937,15 +933,14 @@
 AllowedRenditionSizeOutputTypeDef = TypedDict(
     "AllowedRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
         "Width": int,
     },
-    total=False,
 )
 
 AllowedRenditionSizeTypeDef = TypedDict(
     "AllowedRenditionSizeTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
@@ -957,15 +952,14 @@
 AncillarySourceSettingsOutputTypeDef = TypedDict(
     "AncillarySourceSettingsOutputTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
         "TerminateCaptions": AncillaryTerminateCaptionsType,
     },
-    total=False,
 )
 
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
@@ -982,15 +976,14 @@
 )
 
 AudioChannelTaggingSettingsOutputTypeDef = TypedDict(
     "AudioChannelTaggingSettingsOutputTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
-    total=False,
 )
 
 AudioChannelTaggingSettingsTypeDef = TypedDict(
     "AudioChannelTaggingSettingsTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
@@ -1014,15 +1007,14 @@
         "LtRtSurroundMixLevel": float,
         "MeteringMode": Eac3AtmosMeteringModeType,
         "SampleRate": int,
         "SpeechThreshold": int,
         "StereoDownmix": Eac3AtmosStereoDownmixType,
         "SurroundExMode": Eac3AtmosSurroundExModeType,
     },
-    total=False,
 )
 
 Eac3SettingsOutputTypeDef = TypedDict(
     "Eac3SettingsOutputTypeDef",
     {
         "AttenuationControl": Eac3AttenuationControlType,
         "Bitrate": int,
@@ -1042,68 +1034,62 @@
         "PassthroughControl": Eac3PassthroughControlType,
         "PhaseControl": Eac3PhaseControlType,
         "SampleRate": int,
         "StereoDownmix": Eac3StereoDownmixType,
         "SurroundExMode": Eac3SurroundExModeType,
         "SurroundMode": Eac3SurroundModeType,
     },
-    total=False,
 )
 
 Mp2SettingsOutputTypeDef = TypedDict(
     "Mp2SettingsOutputTypeDef",
     {
         "Bitrate": int,
         "Channels": int,
         "SampleRate": int,
     },
-    total=False,
 )
 
 Mp3SettingsOutputTypeDef = TypedDict(
     "Mp3SettingsOutputTypeDef",
     {
         "Bitrate": int,
         "Channels": int,
         "RateControlMode": Mp3RateControlModeType,
         "SampleRate": int,
         "VbrQuality": int,
     },
-    total=False,
 )
 
 OpusSettingsOutputTypeDef = TypedDict(
     "OpusSettingsOutputTypeDef",
     {
         "Bitrate": int,
         "Channels": int,
         "SampleRate": int,
     },
-    total=False,
 )
 
 VorbisSettingsOutputTypeDef = TypedDict(
     "VorbisSettingsOutputTypeDef",
     {
         "Channels": int,
         "SampleRate": int,
         "VbrQuality": int,
     },
-    total=False,
 )
 
 WavSettingsOutputTypeDef = TypedDict(
     "WavSettingsOutputTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "Format": WavFormatType,
         "SampleRate": int,
     },
-    total=False,
 )
 
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Literal["COMPLETE_MAIN"],
@@ -1214,15 +1200,14 @@
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
         "CorrectionGateLevel": int,
         "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
-    total=False,
 )
 
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
@@ -1236,15 +1221,14 @@
 )
 
 AudioSelectorGroupOutputTypeDef = TypedDict(
     "AudioSelectorGroupOutputTypeDef",
     {
         "AudioSelectorNames": List[str],
     },
-    total=False,
 )
 
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
@@ -1254,15 +1238,14 @@
 HlsRenditionGroupSettingsOutputTypeDef = TypedDict(
     "HlsRenditionGroupSettingsOutputTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
-    total=False,
 )
 
 HlsRenditionGroupSettingsTypeDef = TypedDict(
     "HlsRenditionGroupSettingsTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
@@ -1273,33 +1256,30 @@
 
 ForceIncludeRenditionSizeOutputTypeDef = TypedDict(
     "ForceIncludeRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Width": int,
     },
-    total=False,
 )
 
 MinBottomRenditionSizeOutputTypeDef = TypedDict(
     "MinBottomRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Width": int,
     },
-    total=False,
 )
 
 MinTopRenditionSizeOutputTypeDef = TypedDict(
     "MinTopRenditionSizeOutputTypeDef",
     {
         "Height": int,
         "Width": int,
     },
-    total=False,
 )
 
 ForceIncludeRenditionSizeTypeDef = TypedDict(
     "ForceIncludeRenditionSizeTypeDef",
     {
         "Height": int,
         "Width": int,
@@ -1327,15 +1307,14 @@
 
 Av1QvbrSettingsOutputTypeDef = TypedDict(
     "Av1QvbrSettingsOutputTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
-    total=False,
 )
 
 Av1QvbrSettingsTypeDef = TypedDict(
     "Av1QvbrSettingsTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
@@ -1344,15 +1323,14 @@
 )
 
 AvailBlankingOutputTypeDef = TypedDict(
     "AvailBlankingOutputTypeDef",
     {
         "AvailBlankingImage": str,
     },
-    total=False,
 )
 
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": str,
     },
@@ -1360,15 +1338,14 @@
 )
 
 AvcIntraUhdSettingsOutputTypeDef = TypedDict(
     "AvcIntraUhdSettingsOutputTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
-    total=False,
 )
 
 AvcIntraUhdSettingsTypeDef = TypedDict(
     "AvcIntraUhdSettingsTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
@@ -1377,15 +1354,14 @@
 
 BandwidthReductionFilterOutputTypeDef = TypedDict(
     "BandwidthReductionFilterOutputTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
     },
-    total=False,
 )
 
 BandwidthReductionFilterTypeDef = TypedDict(
     "BandwidthReductionFilterTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
@@ -1414,15 +1390,14 @@
         "ShadowXOffset": int,
         "ShadowYOffset": int,
         "StylePassthrough": BurnInSubtitleStylePassthroughType,
         "TeletextSpacing": BurninSubtitleTeletextSpacingType,
         "XPosition": int,
         "YPosition": int,
     },
-    total=False,
 )
 
 BurninDestinationSettingsTypeDef = TypedDict(
     "BurninDestinationSettingsTypeDef",
     {
         "Alignment": BurninSubtitleAlignmentType,
         "ApplyFontColor": BurninSubtitleApplyFontColorType,
@@ -1483,75 +1458,67 @@
         "StylePassthrough": DvbSubtitleStylePassthroughType,
         "SubtitlingType": DvbSubtitlingTypeType,
         "TeletextSpacing": DvbSubtitleTeletextSpacingType,
         "Width": int,
         "XPosition": int,
         "YPosition": int,
     },
-    total=False,
 )
 
 EmbeddedDestinationSettingsOutputTypeDef = TypedDict(
     "EmbeddedDestinationSettingsOutputTypeDef",
     {
         "Destination608ChannelNumber": int,
         "Destination708ServiceNumber": int,
     },
-    total=False,
 )
 
 ImscDestinationSettingsOutputTypeDef = TypedDict(
     "ImscDestinationSettingsOutputTypeDef",
     {
         "Accessibility": ImscAccessibilitySubsType,
         "StylePassthrough": ImscStylePassthroughType,
     },
-    total=False,
 )
 
 SccDestinationSettingsOutputTypeDef = TypedDict(
     "SccDestinationSettingsOutputTypeDef",
     {
         "Framerate": SccDestinationFramerateType,
     },
-    total=False,
 )
 
 SrtDestinationSettingsOutputTypeDef = TypedDict(
     "SrtDestinationSettingsOutputTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
-    total=False,
 )
 
 TeletextDestinationSettingsOutputTypeDef = TypedDict(
     "TeletextDestinationSettingsOutputTypeDef",
     {
         "PageNumber": str,
         "PageTypes": List[TeletextPageTypeType],
     },
-    total=False,
 )
 
 TtmlDestinationSettingsOutputTypeDef = TypedDict(
     "TtmlDestinationSettingsOutputTypeDef",
     {
         "StylePassthrough": TtmlStylePassthroughType,
     },
-    total=False,
 )
 
 WebvttDestinationSettingsOutputTypeDef = TypedDict(
     "WebvttDestinationSettingsOutputTypeDef",
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
-    total=False,
 )
 
 DvbSubDestinationSettingsTypeDef = TypedDict(
     "DvbSubDestinationSettingsTypeDef",
     {
         "Alignment": DvbSubtitleAlignmentType,
         "ApplyFontColor": DvbSubtitleApplyFontColorType,
@@ -1646,15 +1613,14 @@
 
 CaptionSourceFramerateOutputTypeDef = TypedDict(
     "CaptionSourceFramerateOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
-    total=False,
 )
 
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -1663,52 +1629,47 @@
 )
 
 DvbSubSourceSettingsOutputTypeDef = TypedDict(
     "DvbSubSourceSettingsOutputTypeDef",
     {
         "Pid": int,
     },
-    total=False,
 )
 
 EmbeddedSourceSettingsOutputTypeDef = TypedDict(
     "EmbeddedSourceSettingsOutputTypeDef",
     {
         "Convert608To708": EmbeddedConvert608To708Type,
         "Source608ChannelNumber": int,
         "Source608TrackNumber": int,
         "TerminateCaptions": EmbeddedTerminateCaptionsType,
     },
-    total=False,
 )
 
 TeletextSourceSettingsOutputTypeDef = TypedDict(
     "TeletextSourceSettingsOutputTypeDef",
     {
         "PageNumber": str,
     },
-    total=False,
 )
 
 TrackSourceSettingsOutputTypeDef = TypedDict(
     "TrackSourceSettingsOutputTypeDef",
     {
         "TrackNumber": int,
     },
-    total=False,
 )
 
 WebvttHlsSourceSettingsOutputTypeDef = TypedDict(
     "WebvttHlsSourceSettingsOutputTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
-    total=False,
 )
 
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "Pid": int,
     },
@@ -1754,15 +1715,14 @@
 
 OutputChannelMappingOutputTypeDef = TypedDict(
     "OutputChannelMappingOutputTypeDef",
     {
         "InputChannels": List[int],
         "InputChannelsFineTune": List[float],
     },
-    total=False,
 )
 
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
@@ -1774,15 +1734,14 @@
     "ClipLimitsOutputTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
-    total=False,
 )
 
 ClipLimitsTypeDef = TypedDict(
     "ClipLimitsTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
@@ -1794,15 +1753,14 @@
 
 CmafAdditionalManifestOutputTypeDef = TypedDict(
     "CmafAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -1815,26 +1773,24 @@
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": List[str],
         "HlsSignaledSystemIds": List[str],
         "ResourceId": str,
         "Url": str,
     },
-    total=False,
 )
 
 StaticKeyProviderOutputTypeDef = TypedDict(
     "StaticKeyProviderOutputTypeDef",
     {
         "KeyFormat": str,
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderCmafTypeDef = TypedDict(
     "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": Sequence[str],
@@ -1862,15 +1818,14 @@
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
-    total=False,
 )
 
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
@@ -1896,15 +1851,14 @@
         "Scte35Esam": CmfcScte35EsamType,
         "Scte35Source": CmfcScte35SourceType,
         "TimedMetadata": CmfcTimedMetadataType,
         "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
-    total=False,
 )
 
 CmfcSettingsTypeDef = TypedDict(
     "CmfcSettingsTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "AudioGroupId": str,
@@ -1936,15 +1890,14 @@
         "MaxLuminance": int,
         "MinLuminance": int,
         "RedPrimaryX": int,
         "RedPrimaryY": int,
         "WhitePointX": int,
         "WhitePointY": int,
     },
-    total=False,
 )
 
 Hdr10MetadataTypeDef = TypedDict(
     "Hdr10MetadataTypeDef",
     {
         "BluePrimaryX": int,
         "BluePrimaryY": int,
@@ -1963,15 +1916,14 @@
 )
 
 F4vSettingsOutputTypeDef = TypedDict(
     "F4vSettingsOutputTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
-    total=False,
 )
 
 M3u8SettingsOutputTypeDef = TypedDict(
     "M3u8SettingsOutputTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
@@ -1989,40 +1941,37 @@
         "Scte35Pid": int,
         "Scte35Source": M3u8Scte35SourceType,
         "TimedMetadata": TimedMetadataType,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
 MovSettingsOutputTypeDef = TypedDict(
     "MovSettingsOutputTypeDef",
     {
         "ClapAtom": MovClapAtomType,
         "CslgAtom": MovCslgAtomType,
         "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
         "PaddingControl": MovPaddingControlType,
         "Reference": MovReferenceType,
     },
-    total=False,
 )
 
 Mp4SettingsOutputTypeDef = TypedDict(
     "Mp4SettingsOutputTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "CslgAtom": Mp4CslgAtomType,
         "CttsVersion": int,
         "FreeSpaceBox": Mp4FreeSpaceBoxType,
         "MoovPlacement": Mp4MoovPlacementType,
         "Mp4MajorBrand": str,
     },
-    total=False,
 )
 
 MpdSettingsOutputTypeDef = TypedDict(
     "MpdSettingsOutputTypeDef",
     {
         "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
         "AudioDuration": MpdAudioDurationType,
@@ -2032,15 +1981,14 @@
         "Scte35Esam": MpdScte35EsamType,
         "Scte35Source": MpdScte35SourceType,
         "TimedMetadata": MpdTimedMetadataType,
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
-    total=False,
 )
 
 F4vSettingsTypeDef = TypedDict(
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
@@ -2122,14 +2070,25 @@
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
     total=False,
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
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
@@ -2137,15 +2096,14 @@
 
 DashAdditionalManifestOutputTypeDef = TypedDict(
     "DashAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -2157,15 +2115,14 @@
     "SpekeKeyProviderOutputTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": List[str],
         "Url": str,
     },
-    total=False,
 )
 
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
@@ -2181,15 +2138,14 @@
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
-    total=False,
 )
 
 DashIsoImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
@@ -2204,15 +2160,14 @@
 DeinterlacerOutputTypeDef = TypedDict(
     "DeinterlacerOutputTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
         "Mode": DeinterlacerModeType,
     },
-    total=False,
 )
 
 DeinterlacerTypeDef = TypedDict(
     "DeinterlacerTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
@@ -2238,19 +2193,20 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -2262,15 +2218,14 @@
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Url": str,
     },
-    total=False,
 )
 
 DisassociateCertificateRequestRequestTypeDef = TypedDict(
     "DisassociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
@@ -2278,15 +2233,14 @@
 
 DolbyVisionLevel6MetadataOutputTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataOutputTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
-    total=False,
 )
 
 DolbyVisionLevel6MetadataTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
@@ -2297,15 +2251,14 @@
 DvbNitSettingsOutputTypeDef = TypedDict(
     "DvbNitSettingsOutputTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
         "NitInterval": int,
     },
-    total=False,
 )
 
 DvbNitSettingsTypeDef = TypedDict(
     "DvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
@@ -2318,15 +2271,14 @@
     "DvbSdtSettingsOutputTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
-    total=False,
 )
 
 DvbSdtSettingsTypeDef = TypedDict(
     "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
@@ -2337,15 +2289,14 @@
 )
 
 DvbTdtSettingsOutputTypeDef = TypedDict(
     "DvbTdtSettingsOutputTypeDef",
     {
         "TdtInterval": int,
     },
-    total=False,
 )
 
 DvbTdtSettingsTypeDef = TypedDict(
     "DvbTdtSettingsTypeDef",
     {
         "TdtInterval": int,
     },
@@ -2353,15 +2304,14 @@
 )
 
 EsamManifestConfirmConditionNotificationOutputTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationOutputTypeDef",
     {
         "MccXml": str,
     },
-    total=False,
 )
 
 EsamManifestConfirmConditionNotificationTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationTypeDef",
     {
         "MccXml": str,
     },
@@ -2369,15 +2319,14 @@
 )
 
 EsamSignalProcessingNotificationOutputTypeDef = TypedDict(
     "EsamSignalProcessingNotificationOutputTypeDef",
     {
         "SccXml": str,
     },
-    total=False,
 )
 
 EsamSignalProcessingNotificationTypeDef = TypedDict(
     "EsamSignalProcessingNotificationTypeDef",
     {
         "SccXml": str,
     },
@@ -2386,15 +2335,14 @@
 
 ExtendedDataServicesOutputTypeDef = TypedDict(
     "ExtendedDataServicesOutputTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
     },
-    total=False,
 )
 
 ExtendedDataServicesTypeDef = TypedDict(
     "ExtendedDataServicesTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
@@ -2406,15 +2354,14 @@
     "FrameCaptureSettingsOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "MaxCaptures": int,
         "Quality": int,
     },
-    total=False,
 )
 
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2441,15 +2388,14 @@
 PolicyOutputTypeDef = TypedDict(
     "PolicyOutputTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
         "S3Inputs": InputPolicyType,
     },
-    total=False,
 )
 
 GetPresetRequestRequestTypeDef = TypedDict(
     "GetPresetRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -2465,15 +2411,14 @@
 H264QvbrSettingsOutputTypeDef = TypedDict(
     "H264QvbrSettingsOutputTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
-    total=False,
 )
 
 H264QvbrSettingsTypeDef = TypedDict(
     "H264QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
@@ -2485,15 +2430,14 @@
 H265QvbrSettingsOutputTypeDef = TypedDict(
     "H265QvbrSettingsOutputTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
-    total=False,
 )
 
 H265QvbrSettingsTypeDef = TypedDict(
     "H265QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
@@ -2504,15 +2448,14 @@
 
 Hdr10PlusOutputTypeDef = TypedDict(
     "Hdr10PlusOutputTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
-    total=False,
 )
 
 Hdr10PlusTypeDef = TypedDict(
     "Hdr10PlusTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
@@ -2522,15 +2465,14 @@
 
 HlsAdditionalManifestOutputTypeDef = TypedDict(
     "HlsAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -2542,15 +2484,14 @@
     "HlsCaptionLanguageMappingOutputTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 HlsCaptionLanguageMappingTypeDef = TypedDict(
     "HlsCaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
@@ -2566,15 +2507,14 @@
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
-    total=False,
 )
 
 HlsImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "HlsImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
@@ -2593,34 +2533,31 @@
         "AudioOnlyContainer": HlsAudioOnlyContainerType,
         "AudioRenditionSets": str,
         "AudioTrackType": HlsAudioTrackTypeType,
         "DescriptiveVideoServiceFlag": HlsDescriptiveVideoServiceFlagType,
         "IFrameOnlyManifest": HlsIFrameOnlyManifestType,
         "SegmentModifier": str,
     },
-    total=False,
 )
 
 HopDestinationOutputTypeDef = TypedDict(
     "HopDestinationOutputTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
-    total=False,
 )
 
 Id3InsertionOutputTypeDef = TypedDict(
     "Id3InsertionOutputTypeDef",
     {
         "Id3": str,
         "Timecode": str,
     },
-    total=False,
 )
 
 Id3InsertionTypeDef = TypedDict(
     "Id3InsertionTypeDef",
     {
         "Id3": str,
         "Timecode": str,
@@ -2639,15 +2576,14 @@
         "ImageX": int,
         "ImageY": int,
         "Layer": int,
         "Opacity": int,
         "StartTime": str,
         "Width": int,
     },
-    total=False,
 )
 
 InsertableImageTypeDef = TypedDict(
     "InsertableImageTypeDef",
     {
         "Duration": int,
         "FadeIn": int,
@@ -2666,15 +2602,14 @@
 
 InputClippingOutputTypeDef = TypedDict(
     "InputClippingOutputTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
     },
-    total=False,
 )
 
 InputClippingTypeDef = TypedDict(
     "InputClippingTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
@@ -2686,15 +2621,14 @@
     "InputDecryptionSettingsOutputTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
-    total=False,
 )
 
 InputDecryptionSettingsTypeDef = TypedDict(
     "InputDecryptionSettingsTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
@@ -2705,26 +2639,24 @@
 )
 
 InputVideoGeneratorOutputTypeDef = TypedDict(
     "InputVideoGeneratorOutputTypeDef",
     {
         "Duration": int,
     },
-    total=False,
 )
 
 RectangleOutputTypeDef = TypedDict(
     "RectangleOutputTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
-    total=False,
 )
 
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
@@ -2744,15 +2676,14 @@
 
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
-    total=False,
 )
 
 KantarWatermarkSettingsOutputTypeDef = TypedDict(
     "KantarWatermarkSettingsOutputTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -2764,24 +2695,22 @@
         "Metadata3": str,
         "Metadata4": str,
         "Metadata5": str,
         "Metadata6": str,
         "Metadata7": str,
         "Metadata8": str,
     },
-    total=False,
 )
 
 NielsenConfigurationOutputTypeDef = TypedDict(
     "NielsenConfigurationOutputTypeDef",
     {
         "BreakoutCode": int,
         "DistributorId": str,
     },
-    total=False,
 )
 
 NielsenNonLinearWatermarkSettingsOutputTypeDef = TypedDict(
     "NielsenNonLinearWatermarkSettingsOutputTypeDef",
     {
         "ActiveWatermarkProcess": NielsenActiveWatermarkProcessTypeType,
         "AdiFilename": str,
@@ -2791,26 +2720,24 @@
         "EpisodeId": str,
         "MetadataDestination": str,
         "SourceId": int,
         "SourceWatermarkStatus": NielsenSourceWatermarkStatusTypeType,
         "TicServerUrl": str,
         "UniqueTicPerAudioTrack": NielsenUniqueTicPerAudioTrackTypeType,
     },
-    total=False,
 )
 
 TimecodeConfigOutputTypeDef = TypedDict(
     "TimecodeConfigOutputTypeDef",
     {
         "Anchor": str,
         "Source": TimecodeSourceType,
         "Start": str,
         "TimestampOffset": str,
     },
-    total=False,
 )
 
 KantarWatermarkSettingsTypeDef = TypedDict(
     "KantarWatermarkSettingsTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -2870,114 +2797,69 @@
 QueueTransitionTypeDef = TypedDict(
     "QueueTransitionTypeDef",
     {
         "DestinationQueue": str,
         "SourceQueue": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
-    total=False,
 )
 
 WarningGroupTypeDef = TypedDict(
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
     },
 )
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -2994,23 +2876,21 @@
 
 ResourceTagsTypeDef = TypedDict(
     "ResourceTagsTypeDef",
     {
         "Arn": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 M2tsScte35EsamOutputTypeDef = TypedDict(
     "M2tsScte35EsamOutputTypeDef",
     {
         "Scte35EsamPid": int,
     },
-    total=False,
 )
 
 M2tsScte35EsamTypeDef = TypedDict(
     "M2tsScte35EsamTypeDef",
     {
         "Scte35EsamPid": int,
     },
@@ -3019,24 +2899,22 @@
 
 MotionImageInsertionFramerateOutputTypeDef = TypedDict(
     "MotionImageInsertionFramerateOutputTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
-    total=False,
 )
 
 MotionImageInsertionOffsetOutputTypeDef = TypedDict(
     "MotionImageInsertionOffsetOutputTypeDef",
     {
         "ImageX": int,
         "ImageY": int,
     },
-    total=False,
 )
 
 MotionImageInsertionFramerateTypeDef = TypedDict(
     "MotionImageInsertionFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -3086,15 +2964,14 @@
         "SlowPal": Mpeg2SlowPalType,
         "Softness": int,
         "SpatialAdaptiveQuantization": Mpeg2SpatialAdaptiveQuantizationType,
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
-    total=False,
 )
 
 Mpeg2SettingsTypeDef = TypedDict(
     "Mpeg2SettingsTypeDef",
     {
         "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
         "Bitrate": int,
@@ -3135,15 +3012,14 @@
 
 MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
     "MsSmoothAdditionalManifestOutputTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": List[str],
     },
-    total=False,
 )
 
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
@@ -3153,15 +3029,14 @@
 
 MxfXavcProfileSettingsOutputTypeDef = TypedDict(
     "MxfXavcProfileSettingsOutputTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
     },
-    total=False,
 )
 
 MxfXavcProfileSettingsTypeDef = TypedDict(
     "MxfXavcProfileSettingsTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
@@ -3173,15 +3048,14 @@
     "NexGuardFileMarkerSettingsOutputTypeDef",
     {
         "License": str,
         "Payload": int,
         "Preset": str,
         "Strength": WatermarkingStrengthType,
     },
-    total=False,
 )
 
 NexGuardFileMarkerSettingsTypeDef = TypedDict(
     "NexGuardFileMarkerSettingsTypeDef",
     {
         "License": str,
         "Payload": int,
@@ -3192,15 +3066,14 @@
 )
 
 NoiseReducerFilterSettingsOutputTypeDef = TypedDict(
     "NoiseReducerFilterSettingsOutputTypeDef",
     {
         "Strength": int,
     },
-    total=False,
 )
 
 NoiseReducerFilterSettingsTypeDef = TypedDict(
     "NoiseReducerFilterSettingsTypeDef",
     {
         "Strength": int,
     },
@@ -3210,27 +3083,25 @@
 NoiseReducerSpatialFilterSettingsOutputTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsOutputTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
         "Strength": int,
     },
-    total=False,
 )
 
 NoiseReducerTemporalFilterSettingsOutputTypeDef = TypedDict(
     "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     {
         "AggressiveMode": int,
         "PostTemporalSharpening": NoiseFilterPostTemporalSharpeningType,
         "PostTemporalSharpeningStrength": NoiseFilterPostTemporalSharpeningStrengthType,
         "Speed": int,
         "Strength": int,
     },
-    total=False,
 )
 
 NoiseReducerSpatialFilterSettingsTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
@@ -3253,25 +3124,14 @@
 
 VideoDetailTypeDef = TypedDict(
     "VideoDetailTypeDef",
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
-    total=False,
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
 )
 
 PolicyTypeDef = TypedDict(
     "PolicyTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
@@ -3293,15 +3153,14 @@
         "ParControl": ProresParControlType,
         "ParDenominator": int,
         "ParNumerator": int,
         "ScanTypeConversionMode": ProresScanTypeConversionModeType,
         "SlowPal": ProresSlowPalType,
         "Telecine": ProresTelecineType,
     },
-    total=False,
 )
 
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
@@ -3326,34 +3185,21 @@
         "Commitment": Literal["ONE_YEAR"],
         "ExpiresAt": datetime,
         "PurchasedAt": datetime,
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
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
 
 S3DestinationAccessControlOutputTypeDef = TypedDict(
     "S3DestinationAccessControlOutputTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
-    total=False,
 )
 
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
@@ -3363,15 +3209,14 @@
 S3EncryptionSettingsOutputTypeDef = TypedDict(
     "S3EncryptionSettingsOutputTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
         "KmsKeyArn": str,
     },
-    total=False,
 )
 
 S3EncryptionSettingsTypeDef = TypedDict(
     "S3EncryptionSettingsTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
@@ -3391,15 +3236,14 @@
 TimecodeBurninOutputTypeDef = TypedDict(
     "TimecodeBurninOutputTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
         "Prefix": str,
     },
-    total=False,
 )
 
 TimecodeBurninTypeDef = TypedDict(
     "TimecodeBurninTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
@@ -3436,15 +3280,14 @@
         "FramerateNumerator": int,
         "InterlaceMode": Vc3InterlaceModeType,
         "ScanTypeConversionMode": Vc3ScanTypeConversionModeType,
         "SlowPal": Vc3SlowPalType,
         "Telecine": Vc3TelecineType,
         "Vc3Class": Vc3ClassType,
     },
-    total=False,
 )
 
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
@@ -3472,15 +3315,14 @@
         "MaxBitrate": int,
         "ParControl": Vp8ParControlType,
         "ParDenominator": int,
         "ParNumerator": int,
         "QualityTuningLevel": Vp8QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
-    total=False,
 )
 
 Vp9SettingsOutputTypeDef = TypedDict(
     "Vp9SettingsOutputTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp9FramerateControlType,
@@ -3492,15 +3334,14 @@
         "MaxBitrate": int,
         "ParControl": Vp9ParControlType,
         "ParDenominator": int,
         "ParNumerator": int,
         "QualityTuningLevel": Vp9QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
-    total=False,
 )
 
 Vp8SettingsTypeDef = TypedDict(
     "Vp8SettingsTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp8FramerateControlType,
@@ -3540,15 +3381,14 @@
 )
 
 Xavc4kIntraCbgProfileSettingsOutputTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
-    total=False,
 )
 
 Xavc4kIntraCbgProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
@@ -3556,15 +3396,14 @@
 )
 
 Xavc4kIntraVbrProfileSettingsOutputTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
-    total=False,
 )
 
 Xavc4kIntraVbrProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
@@ -3579,15 +3418,14 @@
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
         "GopClosedCadence": int,
         "HrdBufferSize": int,
         "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
         "Slices": int,
     },
-    total=False,
 )
 
 Xavc4kProfileSettingsTypeDef = TypedDict(
     "Xavc4kProfileSettingsTypeDef",
     {
         "BitrateClass": Xavc4kProfileBitrateClassType,
         "CodecProfile": Xavc4kProfileCodecProfileType,
@@ -3602,15 +3440,14 @@
 )
 
 XavcHdIntraCbgProfileSettingsOutputTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsOutputTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
-    total=False,
 )
 
 XavcHdIntraCbgProfileSettingsTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
@@ -3626,15 +3463,14 @@
         "GopClosedCadence": int,
         "HrdBufferSize": int,
         "InterlaceMode": XavcInterlaceModeType,
         "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
         "Slices": int,
         "Telecine": XavcHdProfileTelecineType,
     },
-    total=False,
 )
 
 XavcHdProfileSettingsTypeDef = TypedDict(
     "XavcHdProfileSettingsTypeDef",
     {
         "BitrateClass": XavcHdProfileBitrateClassType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
@@ -3660,15 +3496,14 @@
         "Eac3Settings": Eac3SettingsOutputTypeDef,
         "Mp2Settings": Mp2SettingsOutputTypeDef,
         "Mp3Settings": Mp3SettingsOutputTypeDef,
         "OpusSettings": OpusSettingsOutputTypeDef,
         "VorbisSettings": VorbisSettingsOutputTypeDef,
         "WavSettings": WavSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
@@ -3690,15 +3525,14 @@
     {
         "AllowedRenditions": List[AllowedRenditionSizeOutputTypeDef],
         "ForceIncludeRenditions": List[ForceIncludeRenditionSizeOutputTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeOutputTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeOutputTypeDef,
         "Type": RuleTypeType,
     },
-    total=False,
 )
 
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
@@ -3722,15 +3556,14 @@
         "MaxBitrate": int,
         "NumberBFramesBetweenReferenceFrames": int,
         "QvbrSettings": Av1QvbrSettingsOutputTypeDef,
         "RateControlMode": Literal["QVBR"],
         "Slices": int,
         "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
     },
-    total=False,
 )
 
 Av1SettingsTypeDef = TypedDict(
     "Av1SettingsTypeDef",
     {
         "AdaptiveQuantization": Av1AdaptiveQuantizationType,
         "BitDepth": Av1BitDepthType,
@@ -3759,15 +3592,14 @@
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "InterlaceMode": AvcIntraInterlaceModeType,
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
-    total=False,
 )
 
 AvcIntraSettingsTypeDef = TypedDict(
     "AvcIntraSettingsTypeDef",
     {
         "AvcIntraClass": AvcIntraClassType,
         "AvcIntraUhdSettings": AvcIntraUhdSettingsTypeDef,
@@ -3793,15 +3625,14 @@
         "ImscDestinationSettings": ImscDestinationSettingsOutputTypeDef,
         "SccDestinationSettings": SccDestinationSettingsOutputTypeDef,
         "SrtDestinationSettings": SrtDestinationSettingsOutputTypeDef,
         "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
         "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
         "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
@@ -3823,15 +3654,14 @@
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateOutputTypeDef,
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
-    total=False,
 )
 
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
@@ -3844,15 +3674,14 @@
 )
 
 ChannelMappingOutputTypeDef = TypedDict(
     "ChannelMappingOutputTypeDef",
     {
         "OutputChannels": List[OutputChannelMappingOutputTypeDef],
     },
-    total=False,
 )
 
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
@@ -3865,15 +3694,14 @@
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
         "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
-    total=False,
 )
 
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
@@ -3895,15 +3723,14 @@
         "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
         "HdrToSdrToneMapper": HDRToSDRToneMapperType,
         "Hue": int,
         "SampleRangeConversion": SampleRangeConversionType,
         "Saturation": int,
         "SdrReferenceWhiteLevel": int,
     },
-    total=False,
 )
 
 VideoSelectorOutputTypeDef = TypedDict(
     "VideoSelectorOutputTypeDef",
     {
         "AlphaBehavior": AlphaBehaviorType,
         "ColorSpace": ColorSpaceType,
@@ -3912,15 +3739,14 @@
         "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
         "PadVideo": PadVideoType,
         "Pid": int,
         "ProgramNumber": int,
         "Rotate": InputRotateType,
         "SampleRange": InputSampleRangeType,
     },
-    total=False,
 )
 
 ColorCorrectorTypeDef = TypedDict(
     "ColorCorrectorTypeDef",
     {
         "Brightness": int,
         "ClipLimits": ClipLimitsTypeDef,
@@ -3999,37 +3825,34 @@
 
 DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
     "DashIsoEncryptionSettingsOutputTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 HlsEncryptionSettingsOutputTypeDef = TypedDict(
     "HlsEncryptionSettingsOutputTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": HlsEncryptionTypeType,
         "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
         "OfflineEncrypted": HlsOfflineEncryptedType,
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
         "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
         "Type": HlsKeyProviderTypeType,
     },
-    total=False,
 )
 
 MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
     "MsSmoothEncryptionSettingsOutputTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
     },
-    total=False,
 )
 
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
@@ -4055,32 +3878,83 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    {
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DolbyVisionOutputTypeDef = TypedDict(
     "DolbyVisionOutputTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataOutputTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
         "Mapping": DolbyVisionMappingType,
         "Profile": DolbyVisionProfileType,
     },
-    total=False,
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
@@ -4095,15 +3969,14 @@
     {
         "ManifestConfirmConditionNotification": (
             EsamManifestConfirmConditionNotificationOutputTypeDef
         ),
         "ResponseSignalPreroll": int,
         "SignalProcessingNotification": EsamSignalProcessingNotificationOutputTypeDef,
     },
-    total=False,
 )
 
 EsamSettingsTypeDef = TypedDict(
     "EsamSettingsTypeDef",
     {
         "ManifestConfirmConditionNotification": EsamManifestConfirmConditionNotificationTypeDef,
         "ResponseSignalPreroll": int,
@@ -4112,23 +3985,23 @@
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 H264SettingsOutputTypeDef = TypedDict(
     "H264SettingsOutputTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -4170,15 +4043,14 @@
         "Softness": int,
         "SpatialAdaptiveQuantization": H264SpatialAdaptiveQuantizationType,
         "Syntax": H264SyntaxType,
         "Telecine": H264TelecineType,
         "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
         "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
-    total=False,
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
@@ -4268,15 +4140,14 @@
         "Telecine": H265TelecineType,
         "TemporalAdaptiveQuantization": H265TemporalAdaptiveQuantizationType,
         "TemporalIds": H265TemporalIdsType,
         "Tiles": H265TilesType,
         "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
         "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
     },
-    total=False,
 )
 
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
@@ -4325,23 +4196,21 @@
 )
 
 OutputSettingsOutputTypeDef = TypedDict(
     "OutputSettingsOutputTypeDef",
     {
         "HlsSettings": HlsSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 TimedMetadataInsertionOutputTypeDef = TypedDict(
     "TimedMetadataInsertionOutputTypeDef",
     {
         "Id3Insertions": List[Id3InsertionOutputTypeDef],
     },
-    total=False,
 )
 
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
@@ -4350,15 +4219,14 @@
 
 ImageInserterOutputTypeDef = TypedDict(
     "ImageInserterOutputTypeDef",
     {
         "InsertableImages": List[InsertableImageOutputTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
-    total=False,
 )
 
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
@@ -4366,15 +4234,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 M2tsSettingsOutputTypeDef = TypedDict(
     "M2tsSettingsOutputTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
@@ -4413,15 +4281,14 @@
         "SegmentationMarkers": M2tsSegmentationMarkersType,
         "SegmentationStyle": M2tsSegmentationStyleType,
         "SegmentationTime": float,
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
-    total=False,
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
@@ -4472,15 +4339,14 @@
         "Framerate": MotionImageInsertionFramerateOutputTypeDef,
         "Input": str,
         "InsertionMode": MotionImageInsertionModeType,
         "Offset": MotionImageInsertionOffsetOutputTypeDef,
         "Playback": MotionImagePlaybackType,
         "StartTime": str,
     },
-    total=False,
 )
 
 MotionImageInserterTypeDef = TypedDict(
     "MotionImageInserterTypeDef",
     {
         "Framerate": MotionImageInsertionFramerateTypeDef,
         "Input": str,
@@ -4495,15 +4361,14 @@
 MxfSettingsOutputTypeDef = TypedDict(
     "MxfSettingsOutputTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
         "XavcProfileSettings": MxfXavcProfileSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 MxfSettingsTypeDef = TypedDict(
     "MxfSettingsTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
@@ -4513,15 +4378,14 @@
 )
 
 PartnerWatermarkingOutputTypeDef = TypedDict(
     "PartnerWatermarkingOutputTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 PartnerWatermarkingTypeDef = TypedDict(
     "PartnerWatermarkingTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsTypeDef,
     },
@@ -4532,15 +4396,14 @@
     "NoiseReducerOutputTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsOutputTypeDef,
         "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsOutputTypeDef,
         "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 NoiseReducerTypeDef = TypedDict(
     "NoiseReducerTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsTypeDef,
@@ -4552,57 +4415,46 @@
 
 OutputDetailTypeDef = TypedDict(
     "OutputDetailTypeDef",
     {
         "DurationInMs": int,
         "VideoDetails": VideoDetailTypeDef,
     },
-    total=False,
 )
 
 PutPolicyRequestRequestTypeDef = TypedDict(
     "PutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 
-_RequiredQueueTypeDef = TypedDict(
-    "_RequiredQueueTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalQueueTypeDef = TypedDict(
-    "_OptionalQueueTypeDef",
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
         "PricingPlan": PricingPlanType,
         "ProgressingJobsCount": int,
         "ReservationPlan": ReservationPlanTypeDef,
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
-    total=False,
 )
 
-class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
-    pass
-
 S3DestinationSettingsOutputTypeDef = TypedDict(
     "S3DestinationSettingsOutputTypeDef",
     {
         "AccessControl": S3DestinationAccessControlOutputTypeDef,
         "Encryption": S3EncryptionSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
@@ -4626,15 +4478,14 @@
         "TemporalAdaptiveQuantization": XavcTemporalAdaptiveQuantizationType,
         "Xavc4kIntraCbgProfileSettings": Xavc4kIntraCbgProfileSettingsOutputTypeDef,
         "Xavc4kIntraVbrProfileSettings": Xavc4kIntraVbrProfileSettingsOutputTypeDef,
         "Xavc4kProfileSettings": Xavc4kProfileSettingsOutputTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsOutputTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 XavcSettingsTypeDef = TypedDict(
     "XavcSettingsTypeDef",
     {
         "AdaptiveQuantization": XavcAdaptiveQuantizationType,
         "EntropyEncoding": XavcEntropyEncodingType,
@@ -4660,15 +4511,14 @@
     "AutomatedAbrSettingsOutputTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": List[AutomatedAbrRuleOutputTypeDef],
     },
-    total=False,
 )
 
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
@@ -4683,26 +4533,24 @@
     {
         "CaptionSelectorName": str,
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 CaptionDescriptionPresetOutputTypeDef = TypedDict(
     "CaptionDescriptionPresetOutputTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
@@ -4720,15 +4568,14 @@
         "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
         "FileSourceSettings": FileSourceSettingsOutputTypeDef,
         "SourceType": CaptionSourceTypeType,
         "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
         "TrackSourceSettings": TrackSourceSettingsOutputTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionSourceSettingsTypeDef = TypedDict(
     "CaptionSourceSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
@@ -4745,15 +4592,14 @@
 RemixSettingsOutputTypeDef = TypedDict(
     "RemixSettingsOutputTypeDef",
     {
         "ChannelMapping": ChannelMappingOutputTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
-    total=False,
 )
 
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
@@ -4771,15 +4617,14 @@
         "M2tsSettings": M2tsSettingsOutputTypeDef,
         "M3u8Settings": M3u8SettingsOutputTypeDef,
         "MovSettings": MovSettingsOutputTypeDef,
         "Mp4Settings": Mp4SettingsOutputTypeDef,
         "MpdSettings": MpdSettingsOutputTypeDef,
         "MxfSettings": MxfSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
@@ -4802,15 +4647,14 @@
         "DolbyVision": DolbyVisionOutputTypeDef,
         "Hdr10Plus": Hdr10PlusOutputTypeDef,
         "ImageInserter": ImageInserterOutputTypeDef,
         "NoiseReducer": NoiseReducerOutputTypeDef,
         "PartnerWatermarking": PartnerWatermarkingOutputTypeDef,
         "TimecodeBurnin": TimecodeBurninOutputTypeDef,
     },
-    total=False,
 )
 
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
@@ -4825,56 +4669,54 @@
 )
 
 OutputGroupDetailTypeDef = TypedDict(
     "OutputGroupDetailTypeDef",
     {
         "OutputDetails": List[OutputDetailTypeDef],
     },
-    total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DestinationSettingsOutputTypeDef = TypedDict(
     "DestinationSettingsOutputTypeDef",
     {
         "S3Settings": S3DestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
     },
@@ -4893,15 +4735,14 @@
         "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
         "ProresSettings": ProresSettingsOutputTypeDef,
         "Vc3Settings": Vc3SettingsOutputTypeDef,
         "Vp8Settings": Vp8SettingsOutputTypeDef,
         "Vp9Settings": Vp9SettingsOutputTypeDef,
         "XavcSettings": XavcSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "Av1Settings": Av1SettingsTypeDef,
         "AvcIntraSettings": AvcIntraSettingsTypeDef,
@@ -4920,15 +4761,14 @@
 )
 
 AutomatedEncodingSettingsOutputTypeDef = TypedDict(
     "AutomatedEncodingSettingsOutputTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
@@ -4938,15 +4778,14 @@
 CaptionSelectorOutputTypeDef = TypedDict(
     "CaptionSelectorOutputTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
@@ -4966,15 +4805,14 @@
         "CodecSettings": AudioCodecSettingsOutputTypeDef,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageCodeControl": AudioLanguageCodeControlType,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "StreamName": str,
     },
-    total=False,
 )
 
 AudioSelectorOutputTypeDef = TypedDict(
     "AudioSelectorOutputTypeDef",
     {
         "AudioDurationCorrection": AudioDurationCorrectionType,
         "CustomLanguageCode": str,
@@ -4985,15 +4823,14 @@
         "Offset": int,
         "Pids": List[int],
         "ProgramSelection": int,
         "RemixSettings": RemixSettingsOutputTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": List[int],
     },
-    total=False,
 )
 
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
@@ -5056,15 +4893,14 @@
         "StreamInfResolution": CmafStreamInfResolutionType,
         "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
         "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
-    total=False,
 )
 
 DashIsoGroupSettingsOutputTypeDef = TypedDict(
     "DashIsoGroupSettingsOutputTypeDef",
     {
         "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
@@ -5084,24 +4920,22 @@
         "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
         "SegmentControl": DashIsoSegmentControlType,
         "SegmentLength": int,
         "SegmentLengthControl": DashIsoSegmentLengthControlType,
         "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
         "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
     },
-    total=False,
 )
 
 FileGroupSettingsOutputTypeDef = TypedDict(
     "FileGroupSettingsOutputTypeDef",
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 HlsGroupSettingsOutputTypeDef = TypedDict(
     "HlsGroupSettingsOutputTypeDef",
     {
         "AdMarkers": List[HlsAdMarkersType],
         "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
@@ -5132,30 +4966,28 @@
         "SegmentsPerSubdirectory": int,
         "StreamInfResolution": HlsStreamInfResolutionType,
         "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
-    total=False,
 )
 
 MsSmoothGroupSettingsOutputTypeDef = TypedDict(
     "MsSmoothGroupSettingsOutputTypeDef",
     {
         "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsOutputTypeDef,
         "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
-    total=False,
 )
 
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
@@ -5294,15 +5126,14 @@
         "RespondToAfd": RespondToAfdType,
         "ScalingBehavior": ScalingBehaviorType,
         "Sharpness": int,
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
         "Width": int,
     },
-    total=False,
 )
 
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
@@ -5347,15 +5178,14 @@
         "PsiControl": InputPsiControlType,
         "SupplementalImps": List[str],
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorOutputTypeDef,
         "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateOutputTypeDef = TypedDict(
     "InputTemplateOutputTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
@@ -5374,15 +5204,14 @@
         "Position": RectangleOutputTypeDef,
         "ProgramNumber": int,
         "PsiControl": InputPsiControlType,
         "TimecodeSource": InputTimecodeSourceType,
         "TimecodeStart": str,
         "VideoSelector": VideoSelectorOutputTypeDef,
     },
-    total=False,
 )
 
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
@@ -5445,15 +5274,14 @@
         "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
         "FileGroupSettings": FileGroupSettingsOutputTypeDef,
         "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
         "Type": OutputGroupTypeType,
     },
-    total=False,
 )
 
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
@@ -5473,26 +5301,24 @@
         "ContainerSettings": ContainerSettingsOutputTypeDef,
         "Extension": str,
         "NameModifier": str,
         "OutputSettings": OutputSettingsOutputTypeDef,
         "Preset": str,
         "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsOutputTypeDef = TypedDict(
     "PresetSettingsOutputTypeDef",
     {
         "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
         "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
         "ContainerSettings": ContainerSettingsOutputTypeDef,
         "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsTypeDef = TypedDict(
     "PresetSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
@@ -5507,52 +5333,42 @@
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
         "Outputs": List[OutputTypeDef],
     },
-    total=False,
 )
 
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
     total=False,
 )
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsOutputTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
     {
         "Arn": str,
         "Category": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
         "Type": TypeType,
     },
-    total=False,
 )
 
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": PresetSettingsTypeDef,
     },
 )
@@ -5604,15 +5420,14 @@
         "MotionImageInserter": MotionImageInserterOutputTypeDef,
         "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
         "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
         "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobTemplateSettingsOutputTypeDef = TypedDict(
     "JobTemplateSettingsOutputTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingOutputTypeDef,
@@ -5623,15 +5438,14 @@
         "MotionImageInserter": MotionImageInserterOutputTypeDef,
         "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
         "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
         "OutputGroups": List[OutputGroupOutputTypeDef],
         "TimecodeConfig": TimecodeConfigOutputTypeDef,
         "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
     },
-    total=False,
 )
 
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
@@ -5668,52 +5482,45 @@
     total=False,
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPresetResponseTypeDef = TypedDict(
     "GetPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "NextToken": str,
         "Presets": List[PresetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePresetResponseTypeDef = TypedDict(
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsOutputTypeDef,
-    },
-)
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+JobTypeDef = TypedDict(
+    "JobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
         "ClientRequestToken": str,
         "CreatedAt": datetime,
@@ -5726,55 +5533,44 @@
         "JobTemplate": str,
         "Messages": JobMessagesTypeDef,
         "OutputGroupDetails": List[OutputGroupDetailTypeDef],
         "Priority": int,
         "Queue": str,
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
+        "Role": str,
+        "Settings": JobSettingsOutputTypeDef,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
-    total=False,
 )
 
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
-    {
-        "Name": str,
-        "Settings": JobTemplateSettingsOutputTypeDef,
-    },
-)
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+JobTemplateTypeDef = TypedDict(
+    "JobTemplateTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "Arn": str,
         "Category": str,
         "CreatedAt": datetime,
         "Description": str,
         "HopDestinations": List[HopDestinationOutputTypeDef],
         "LastUpdated": datetime,
+        "Name": str,
         "Priority": int,
         "Queue": str,
+        "Settings": JobTemplateSettingsOutputTypeDef,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Type": TypeType,
     },
-    total=False,
 )
 
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
-    pass
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Role": str,
         "Settings": JobSettingsTypeDef,
     },
 )
@@ -5854,60 +5650,60 @@
 ):
     pass
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaConvert 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.9
+Summary: Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
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
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -852,27 +852,28 @@
     MpdSettingsOutputTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
@@ -927,21 +928,17 @@
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateOutputTypeDef,
     MotionImageInsertionOffsetOutputTypeDef,
@@ -958,20 +955,18 @@
     NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsOutputTypeDef,
     NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
     PolicyTypeDef,
     ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
@@ -1016,14 +1011,19 @@
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsOutputTypeDef,
     HlsEncryptionSettingsOutputTypeDef,
     MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyResponseTypeDef,
```

### Comparing `mypy-boto3-mediaconvert-1.28.12/mypy_boto3_mediaconvert.egg-info/SOURCES.txt` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.12/setup.py` & `mypy-boto3-mediaconvert-1.28.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconvert",
-    version="1.28.12",
+    version="1.28.9",
     packages=["mypy_boto3_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConvert 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

