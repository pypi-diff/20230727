# Comparing `tmp/mypy-boto3-medialive-1.28.1.tar.gz` & `tmp/mypy-boto3-medialive-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.28.1.tar", last modified: Fri Jul  7 19:32:38 2023, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
```

## Comparing `mypy-boto3-medialive-1.28.1.tar` & `mypy-boto3-medialive-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.907384 mypy-boto3-medialive-1.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37511 2023-07-07 19:32:38.903385 mypy-boto3-medialive-1.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36018 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.899385 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52938 2023-07-07 19:32:22.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52848 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39506 2023-07-07 19:32:22.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39504 2023-07-07 19:32:22.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-07 19:32:22.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-07 19:32:22.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   149204 2023-07-07 19:32:26.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   149055 2023-07-07 19:32:24.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:32:21.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-07 19:32:22.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-07 19:32:22.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37511 2023-07-07 19:32:38.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-07 19:32:38.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 19:32:38.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 19:32:38.000000 mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:32:38.907384 mypy-boto3-medialive-1.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-07 19:32:20.000000 mypy-boto3-medialive-1.28.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43563 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42068 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.376443 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52938 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52848 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-07-27 05:26:14.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   214218 2023-07-27 05:26:19.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214003 2023-07-27 05:26:17.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-27 05:26:13.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43563 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:35:00.000000 mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.380443 mypy-boto3-medialive-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:26:12.000000 mypy-boto3-medialive-1.28.12/setup.py
```

### Comparing `mypy-boto3-medialive-1.28.1/LICENSE` & `mypy-boto3-medialive-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/PKG-INFO` & `mypy-boto3-medialive-1.28.12/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.1
-Summary: Type annotations for boto3.MediaLive 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaLive 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-medialive?color=blue)](https://pypistats.org/packages/mypy-boto3-medialive)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -674,61 +674,93 @@
 ### Typed dictionaries
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
+    AccountConfigurationOutputTypeDef,
     AccountConfigurationTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
+    ArchiveS3SettingsOutputTypeDef,
     ArchiveS3SettingsTypeDef,
+    OutputLocationRefOutputTypeDef,
     OutputLocationRefTypeDef,
+    InputChannelLevelOutputTypeDef,
     InputChannelLevelTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioDolbyEDecodeOutputTypeDef,
     AudioDolbyEDecodeTypeDef,
+    AudioHlsRenditionSelectionOutputTypeDef,
     AudioHlsRenditionSelectionTypeDef,
+    AudioLanguageSelectionOutputTypeDef,
     AudioLanguageSelectionTypeDef,
-    InputLocationTypeDef,
+    InputLocationOutputTypeDef,
+    AudioPidSelectionOutputTypeDef,
     AudioPidSelectionTypeDef,
+    AudioSilenceFailoverSettingsOutputTypeDef,
     AudioSilenceFailoverSettingsTypeDef,
+    AudioTrackOutputTypeDef,
     AudioTrackTypeDef,
+    InputLocationTypeDef,
+    EsamOutputTypeDef,
+    Scte35SpliceInsertOutputTypeDef,
+    Scte35TimeSignalAposOutputTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
-    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
+    EbuTtDDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    CaptionLanguageMappingOutputTypeDef,
     CaptionLanguageMappingTypeDef,
+    CaptionRectangleOutputTypeDef,
     CaptionRectangleTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    Scte20SourceSettingsOutputTypeDef,
+    Scte27SourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     Scte20SourceSettingsTypeDef,
     Scte27SourceSettingsTypeDef,
+    CdiInputSpecificationOutputTypeDef,
     CdiInputSpecificationTypeDef,
     ChannelEgressEndpointTypeDef,
-    InputSpecificationTypeDef,
+    InputSpecificationOutputTypeDef,
     MaintenanceStatusTypeDef,
     VpcOutputSettingsDescriptionTypeDef,
     PipelineDetailTypeDef,
     ClaimDeviceRequestRequestTypeDef,
+    InputSpecificationTypeDef,
     MaintenanceCreateSettingsTypeDef,
     VpcOutputSettingsTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputVpcRequestTypeDef,
     MediaConnectFlowRequestTypeDef,
@@ -739,149 +771,218 @@
     DeleteChannelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DeleteInputSecurityGroupRequestRequestTypeDef,
     DeleteMultiplexProgramRequestRequestTypeDef,
     MultiplexProgramPacketIdentifiersMapTypeDef,
     MultiplexProgramPipelineDetailTypeDef,
     DeleteMultiplexRequestRequestTypeDef,
+    MultiplexSettingsOutputTypeDef,
     DeleteReservationRequestRequestTypeDef,
-    RenewalSettingsTypeDef,
+    RenewalSettingsOutputTypeDef,
     ReservationResourceSpecificationTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
+    InputDeviceSettingsOutputTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeThumbnailsRequestRequestTypeDef,
-    DvbNitSettingsTypeDef,
-    DvbSdtSettingsTypeDef,
-    DvbTdtSettingsTypeDef,
+    DvbNitSettingsOutputTypeDef,
+    DvbSdtSettingsOutputTypeDef,
+    DvbTdtSettingsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FeatureActivationsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    ThumbnailConfigurationOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     TimecodeConfigTypeDef,
+    InputLossFailoverSettingsOutputTypeDef,
+    VideoBlackFailoverSettingsOutputTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
-    FecOutputSettingsTypeDef,
+    FecOutputSettingsOutputTypeDef,
+    FixedModeScheduleActionStartSettingsOutputTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
-    Fmp4HlsSettingsTypeDef,
+    Fmp4HlsSettingsOutputTypeDef,
+    FollowModeScheduleActionStartSettingsOutputTypeDef,
     FollowModeScheduleActionStartSettingsTypeDef,
+    FrameCaptureS3SettingsOutputTypeDef,
     FrameCaptureS3SettingsTypeDef,
-    FrameCaptureOutputSettingsTypeDef,
+    FrameCaptureOutputSettingsOutputTypeDef,
+    TimecodeBurninSettingsOutputTypeDef,
     TimecodeBurninSettingsTypeDef,
+    H264ColorSpaceSettingsOutputTypeDef,
     H264ColorSpaceSettingsTypeDef,
+    TemporalFilterSettingsOutputTypeDef,
     TemporalFilterSettingsTypeDef,
+    Hdr10SettingsOutputTypeDef,
     Hdr10SettingsTypeDef,
+    HlsAkamaiSettingsOutputTypeDef,
     HlsAkamaiSettingsTypeDef,
+    HlsBasicPutSettingsOutputTypeDef,
     HlsBasicPutSettingsTypeDef,
+    HlsMediaStoreSettingsOutputTypeDef,
+    HlsS3SettingsOutputTypeDef,
+    HlsWebdavSettingsOutputTypeDef,
     HlsMediaStoreSettingsTypeDef,
     HlsS3SettingsTypeDef,
     HlsWebdavSettingsTypeDef,
+    HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
     HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
+    HlsInputSettingsOutputTypeDef,
     HlsInputSettingsTypeDef,
+    HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
+    StartTimecodeOutputTypeDef,
+    StopTimecodeOutputTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    M3u8SettingsTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    M3u8SettingsOutputTypeDef,
     MaintenanceUpdateSettingsTypeDef,
+    MediaPackageOutputDestinationSettingsOutputTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
+    MotionGraphicsActivateScheduleActionSettingsOutputTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
+    MotionGraphicsSettingsOutputTypeDef,
     MotionGraphicsSettingsTypeDef,
-    MsSmoothOutputSettingsTypeDef,
+    MsSmoothOutputSettingsOutputTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
+    MultiplexProgramChannelDestinationSettingsOutputTypeDef,
     MultiplexProgramChannelDestinationSettingsTypeDef,
+    MultiplexProgramServiceDescriptorOutputTypeDef,
     MultiplexProgramServiceDescriptorTypeDef,
     MultiplexSettingsSummaryTypeDef,
+    MultiplexStatmuxVideoSettingsOutputTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
+    NielsenCBETOutputTypeDef,
     NielsenCBETTypeDef,
+    NielsenNaesIiNwOutputTypeDef,
     NielsenNaesIiNwTypeDef,
+    OutputDestinationSettingsOutputTypeDef,
     OutputDestinationSettingsTypeDef,
+    RtmpGroupSettingsOutputTypeDef,
+    UdpGroupSettingsOutputTypeDef,
     RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
+    PaginatorConfigTypeDef,
+    PipelinePauseStateSettingsOutputTypeDef,
     PipelinePauseStateSettingsTypeDef,
+    RenewalSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    Scte35InputScheduleActionSettingsOutputTypeDef,
+    Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
+    Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+    StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
+    Scte35DeliveryRestrictionsOutputTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
     StartMultiplexRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     StopMultiplexRequestRequestTypeDef,
     ThumbnailTypeDef,
     TransferInputDeviceRequestRequestTypeDef,
+    VideoSelectorPidOutputTypeDef,
     VideoSelectorPidTypeDef,
+    VideoSelectorProgramIdOutputTypeDef,
     VideoSelectorProgramIdTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
+    ArchiveCdnSettingsOutputTypeDef,
     ArchiveCdnSettingsTypeDef,
+    MediaPackageGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
+    MultiplexOutputSettingsOutputTypeDef,
+    RtmpOutputSettingsOutputTypeDef,
     MediaPackageGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
-    MultiplexOutputSettingsTypeDef,
-    RtmpOutputSettingsTypeDef,
+    AudioChannelMappingOutputTypeDef,
     AudioChannelMappingTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
-    AudioOnlyHlsSettingsTypeDef,
+    AudioOnlyHlsSettingsOutputTypeDef,
+    AvailBlankingOutputTypeDef,
+    BlackoutSlateOutputTypeDef,
+    BurnInDestinationSettingsOutputTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    InputLossBehaviorOutputTypeDef,
+    StaticImageActivateScheduleActionSettingsOutputTypeDef,
+    StaticKeySettingsOutputTypeDef,
+    AudioTrackSelectionOutputTypeDef,
+    AudioTrackSelectionTypeDef,
     AvailBlankingTypeDef,
     BlackoutSlateTypeDef,
     BurnInDestinationSettingsTypeDef,
     DvbSubDestinationSettingsTypeDef,
     InputLossBehaviorTypeDef,
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
-    AudioTrackSelectionTypeDef,
+    AvailSettingsOutputTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    DescribeAccountConfigurationResponseTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
-    PurchaseOfferingRequestRequestTypeDef,
-    UpdateReservationRequestRequestTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     DescribeChannelRequestChannelCreatedWaitTypeDef,
     DescribeChannelRequestChannelDeletedWaitTypeDef,
@@ -895,150 +996,197 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
-    M2tsSettingsTypeDef,
+    M2tsSettingsOutputTypeDef,
+    FailoverConditionSettingsOutputTypeDef,
     FailoverConditionSettingsTypeDef,
+    ScheduleActionStartSettingsOutputTypeDef,
     ScheduleActionStartSettingsTypeDef,
+    FrameCaptureCdnSettingsOutputTypeDef,
     FrameCaptureCdnSettingsTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
+    H264FilterSettingsOutputTypeDef,
+    H265FilterSettingsOutputTypeDef,
+    Mpeg2FilterSettingsOutputTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
     Mpeg2FilterSettingsTypeDef,
+    H265ColorSpaceSettingsOutputTypeDef,
+    VideoSelectorColorSpaceSettingsOutputTypeDef,
     H265ColorSpaceSettingsTypeDef,
     VideoSelectorColorSpaceSettingsTypeDef,
+    HlsCdnSettingsOutputTypeDef,
     HlsCdnSettingsTypeDef,
+    NetworkInputSettingsOutputTypeDef,
     NetworkInputSettingsTypeDef,
+    InputClippingSettingsOutputTypeDef,
     InputClippingSettingsTypeDef,
     InputDestinationTypeDef,
     UpdateInputDeviceRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
-    StandardHlsSettingsTypeDef,
+    StandardHlsSettingsOutputTypeDef,
+    MotionGraphicsConfigurationOutputTypeDef,
     MotionGraphicsConfigurationTypeDef,
     MultiplexOutputDestinationTypeDef,
     MultiplexSummaryTypeDef,
+    MultiplexVideoSettingsOutputTypeDef,
     MultiplexVideoSettingsTypeDef,
+    NielsenWatermarksSettingsOutputTypeDef,
     NielsenWatermarksSettingsTypeDef,
+    OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
+    PauseStateScheduleActionSettingsOutputTypeDef,
     PauseStateScheduleActionSettingsTypeDef,
+    PurchaseOfferingRequestRequestTypeDef,
+    UpdateReservationRequestRequestTypeDef,
+    Scte35SegmentationDescriptorOutputTypeDef,
     Scte35SegmentationDescriptorTypeDef,
     ThumbnailDetailTypeDef,
+    VideoSelectorSettingsOutputTypeDef,
     VideoSelectorSettingsTypeDef,
+    ArchiveGroupSettingsOutputTypeDef,
     ArchiveGroupSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
+    GlobalConfigurationOutputTypeDef,
+    KeyProviderSettingsOutputTypeDef,
+    AudioSelectorSettingsOutputTypeDef,
+    AudioSelectorSettingsTypeDef,
     CaptionDestinationSettingsTypeDef,
     GlobalConfigurationTypeDef,
     KeyProviderSettingsTypeDef,
-    AudioSelectorSettingsTypeDef,
+    AvailConfigurationOutputTypeDef,
     AvailConfigurationTypeDef,
+    CaptionSelectorSettingsOutputTypeDef,
     CaptionSelectorSettingsTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     UpdateReservationResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
-    ArchiveContainerSettingsTypeDef,
-    UdpContainerSettingsTypeDef,
+    ArchiveContainerSettingsOutputTypeDef,
+    UdpContainerSettingsOutputTypeDef,
+    FailoverConditionOutputTypeDef,
     FailoverConditionTypeDef,
+    FrameCaptureGroupSettingsOutputTypeDef,
     FrameCaptureGroupSettingsTypeDef,
+    H264SettingsOutputTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     H264SettingsTypeDef,
     Mpeg2SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
+    InputPrepareScheduleActionSettingsOutputTypeDef,
+    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputPrepareScheduleActionSettingsTypeDef,
     InputSwitchScheduleActionSettingsTypeDef,
     DescribeInputResponseTypeDef,
     InputTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
     DeleteMultiplexResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
+    MultiplexProgramSettingsOutputTypeDef,
     MultiplexProgramSettingsTypeDef,
+    AudioWatermarkSettingsOutputTypeDef,
     AudioWatermarkSettingsTypeDef,
     UpdateChannelClassRequestRequestTypeDef,
+    Scte35DescriptorSettingsOutputTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
+    VideoSelectorOutputTypeDef,
     VideoSelectorTypeDef,
+    CaptionDescriptionOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    AudioSelectorOutputTypeDef,
+    AudioSelectorTypeDef,
     CaptionDescriptionTypeDef,
     HlsGroupSettingsTypeDef,
-    AudioSelectorTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
-    ArchiveOutputSettingsTypeDef,
-    UdpOutputSettingsTypeDef,
+    ArchiveOutputSettingsOutputTypeDef,
+    UdpOutputSettingsOutputTypeDef,
+    AutomaticInputFailoverSettingsOutputTypeDef,
     AutomaticInputFailoverSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     CreateInputResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     ListInputsResponseTypeDef,
     UpdateInputResponseTypeDef,
-    HlsOutputSettingsTypeDef,
+    HlsOutputSettingsOutputTypeDef,
     CreateMultiplexResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
-    CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
+    CreateMultiplexProgramRequestRequestTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
+    AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
+    Scte35DescriptorOutputTypeDef,
     Scte35DescriptorTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
+    InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
+    Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
     Scte35TimeSignalScheduleActionSettingsTypeDef,
+    InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
+    ScheduleActionSettingsOutputTypeDef,
     ScheduleActionSettingsTypeDef,
     ChannelSummaryTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
+    ScheduleActionOutputTypeDef,
     ScheduleActionTypeDef,
     ListChannelsResponseTypeDef,
+    EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
-    BatchScheduleActionCreateRequestTypeDef,
     BatchScheduleActionCreateResultTypeDef,
     BatchScheduleActionDeleteResultTypeDef,
     DescribeScheduleResponseTypeDef,
+    BatchScheduleActionCreateRequestTypeDef,
     ChannelTypeDef,
-    CreateChannelRequestRequestTypeDef,
     DeleteChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     StartChannelResponseTypeDef,
     StopChannelResponseTypeDef,
+    CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    BatchUpdateScheduleRequestRequestTypeDef,
     BatchUpdateScheduleResponseTypeDef,
+    BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.1/README.md` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-medialive
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaLive 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 medialive type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-medialive?color=blue)](https://pypistats.org/packages/mypy-boto3-medialive)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -642,61 +674,93 @@
 ### Typed dictionaries
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
+    AccountConfigurationOutputTypeDef,
     AccountConfigurationTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
+    ArchiveS3SettingsOutputTypeDef,
     ArchiveS3SettingsTypeDef,
+    OutputLocationRefOutputTypeDef,
     OutputLocationRefTypeDef,
+    InputChannelLevelOutputTypeDef,
     InputChannelLevelTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioDolbyEDecodeOutputTypeDef,
     AudioDolbyEDecodeTypeDef,
+    AudioHlsRenditionSelectionOutputTypeDef,
     AudioHlsRenditionSelectionTypeDef,
+    AudioLanguageSelectionOutputTypeDef,
     AudioLanguageSelectionTypeDef,
-    InputLocationTypeDef,
+    InputLocationOutputTypeDef,
+    AudioPidSelectionOutputTypeDef,
     AudioPidSelectionTypeDef,
+    AudioSilenceFailoverSettingsOutputTypeDef,
     AudioSilenceFailoverSettingsTypeDef,
+    AudioTrackOutputTypeDef,
     AudioTrackTypeDef,
+    InputLocationTypeDef,
+    EsamOutputTypeDef,
+    Scte35SpliceInsertOutputTypeDef,
+    Scte35TimeSignalAposOutputTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
-    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
+    EbuTtDDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    CaptionLanguageMappingOutputTypeDef,
     CaptionLanguageMappingTypeDef,
+    CaptionRectangleOutputTypeDef,
     CaptionRectangleTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    Scte20SourceSettingsOutputTypeDef,
+    Scte27SourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     Scte20SourceSettingsTypeDef,
     Scte27SourceSettingsTypeDef,
+    CdiInputSpecificationOutputTypeDef,
     CdiInputSpecificationTypeDef,
     ChannelEgressEndpointTypeDef,
-    InputSpecificationTypeDef,
+    InputSpecificationOutputTypeDef,
     MaintenanceStatusTypeDef,
     VpcOutputSettingsDescriptionTypeDef,
     PipelineDetailTypeDef,
     ClaimDeviceRequestRequestTypeDef,
+    InputSpecificationTypeDef,
     MaintenanceCreateSettingsTypeDef,
     VpcOutputSettingsTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputVpcRequestTypeDef,
     MediaConnectFlowRequestTypeDef,
@@ -707,149 +771,218 @@
     DeleteChannelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DeleteInputSecurityGroupRequestRequestTypeDef,
     DeleteMultiplexProgramRequestRequestTypeDef,
     MultiplexProgramPacketIdentifiersMapTypeDef,
     MultiplexProgramPipelineDetailTypeDef,
     DeleteMultiplexRequestRequestTypeDef,
+    MultiplexSettingsOutputTypeDef,
     DeleteReservationRequestRequestTypeDef,
-    RenewalSettingsTypeDef,
+    RenewalSettingsOutputTypeDef,
     ReservationResourceSpecificationTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
+    InputDeviceSettingsOutputTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeThumbnailsRequestRequestTypeDef,
-    DvbNitSettingsTypeDef,
-    DvbSdtSettingsTypeDef,
-    DvbTdtSettingsTypeDef,
+    DvbNitSettingsOutputTypeDef,
+    DvbSdtSettingsOutputTypeDef,
+    DvbTdtSettingsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FeatureActivationsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    ThumbnailConfigurationOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     TimecodeConfigTypeDef,
+    InputLossFailoverSettingsOutputTypeDef,
+    VideoBlackFailoverSettingsOutputTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
-    FecOutputSettingsTypeDef,
+    FecOutputSettingsOutputTypeDef,
+    FixedModeScheduleActionStartSettingsOutputTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
-    Fmp4HlsSettingsTypeDef,
+    Fmp4HlsSettingsOutputTypeDef,
+    FollowModeScheduleActionStartSettingsOutputTypeDef,
     FollowModeScheduleActionStartSettingsTypeDef,
+    FrameCaptureS3SettingsOutputTypeDef,
     FrameCaptureS3SettingsTypeDef,
-    FrameCaptureOutputSettingsTypeDef,
+    FrameCaptureOutputSettingsOutputTypeDef,
+    TimecodeBurninSettingsOutputTypeDef,
     TimecodeBurninSettingsTypeDef,
+    H264ColorSpaceSettingsOutputTypeDef,
     H264ColorSpaceSettingsTypeDef,
+    TemporalFilterSettingsOutputTypeDef,
     TemporalFilterSettingsTypeDef,
+    Hdr10SettingsOutputTypeDef,
     Hdr10SettingsTypeDef,
+    HlsAkamaiSettingsOutputTypeDef,
     HlsAkamaiSettingsTypeDef,
+    HlsBasicPutSettingsOutputTypeDef,
     HlsBasicPutSettingsTypeDef,
+    HlsMediaStoreSettingsOutputTypeDef,
+    HlsS3SettingsOutputTypeDef,
+    HlsWebdavSettingsOutputTypeDef,
     HlsMediaStoreSettingsTypeDef,
     HlsS3SettingsTypeDef,
     HlsWebdavSettingsTypeDef,
+    HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
     HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
+    HlsInputSettingsOutputTypeDef,
     HlsInputSettingsTypeDef,
+    HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
+    StartTimecodeOutputTypeDef,
+    StopTimecodeOutputTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    M3u8SettingsTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    M3u8SettingsOutputTypeDef,
     MaintenanceUpdateSettingsTypeDef,
+    MediaPackageOutputDestinationSettingsOutputTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
+    MotionGraphicsActivateScheduleActionSettingsOutputTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
+    MotionGraphicsSettingsOutputTypeDef,
     MotionGraphicsSettingsTypeDef,
-    MsSmoothOutputSettingsTypeDef,
+    MsSmoothOutputSettingsOutputTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
+    MultiplexProgramChannelDestinationSettingsOutputTypeDef,
     MultiplexProgramChannelDestinationSettingsTypeDef,
+    MultiplexProgramServiceDescriptorOutputTypeDef,
     MultiplexProgramServiceDescriptorTypeDef,
     MultiplexSettingsSummaryTypeDef,
+    MultiplexStatmuxVideoSettingsOutputTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
+    NielsenCBETOutputTypeDef,
     NielsenCBETTypeDef,
+    NielsenNaesIiNwOutputTypeDef,
     NielsenNaesIiNwTypeDef,
+    OutputDestinationSettingsOutputTypeDef,
     OutputDestinationSettingsTypeDef,
+    RtmpGroupSettingsOutputTypeDef,
+    UdpGroupSettingsOutputTypeDef,
     RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
+    PaginatorConfigTypeDef,
+    PipelinePauseStateSettingsOutputTypeDef,
     PipelinePauseStateSettingsTypeDef,
+    RenewalSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    Scte35InputScheduleActionSettingsOutputTypeDef,
+    Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
+    Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+    StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
+    Scte35DeliveryRestrictionsOutputTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
     StartMultiplexRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     StopMultiplexRequestRequestTypeDef,
     ThumbnailTypeDef,
     TransferInputDeviceRequestRequestTypeDef,
+    VideoSelectorPidOutputTypeDef,
     VideoSelectorPidTypeDef,
+    VideoSelectorProgramIdOutputTypeDef,
     VideoSelectorProgramIdTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
+    ArchiveCdnSettingsOutputTypeDef,
     ArchiveCdnSettingsTypeDef,
+    MediaPackageGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
+    MultiplexOutputSettingsOutputTypeDef,
+    RtmpOutputSettingsOutputTypeDef,
     MediaPackageGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
-    MultiplexOutputSettingsTypeDef,
-    RtmpOutputSettingsTypeDef,
+    AudioChannelMappingOutputTypeDef,
     AudioChannelMappingTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
-    AudioOnlyHlsSettingsTypeDef,
+    AudioOnlyHlsSettingsOutputTypeDef,
+    AvailBlankingOutputTypeDef,
+    BlackoutSlateOutputTypeDef,
+    BurnInDestinationSettingsOutputTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    InputLossBehaviorOutputTypeDef,
+    StaticImageActivateScheduleActionSettingsOutputTypeDef,
+    StaticKeySettingsOutputTypeDef,
+    AudioTrackSelectionOutputTypeDef,
+    AudioTrackSelectionTypeDef,
     AvailBlankingTypeDef,
     BlackoutSlateTypeDef,
     BurnInDestinationSettingsTypeDef,
     DvbSubDestinationSettingsTypeDef,
     InputLossBehaviorTypeDef,
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
-    AudioTrackSelectionTypeDef,
+    AvailSettingsOutputTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    DescribeAccountConfigurationResponseTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
-    PurchaseOfferingRequestRequestTypeDef,
-    UpdateReservationRequestRequestTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     DescribeChannelRequestChannelCreatedWaitTypeDef,
     DescribeChannelRequestChannelDeletedWaitTypeDef,
@@ -863,150 +996,197 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
-    M2tsSettingsTypeDef,
+    M2tsSettingsOutputTypeDef,
+    FailoverConditionSettingsOutputTypeDef,
     FailoverConditionSettingsTypeDef,
+    ScheduleActionStartSettingsOutputTypeDef,
     ScheduleActionStartSettingsTypeDef,
+    FrameCaptureCdnSettingsOutputTypeDef,
     FrameCaptureCdnSettingsTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
+    H264FilterSettingsOutputTypeDef,
+    H265FilterSettingsOutputTypeDef,
+    Mpeg2FilterSettingsOutputTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
     Mpeg2FilterSettingsTypeDef,
+    H265ColorSpaceSettingsOutputTypeDef,
+    VideoSelectorColorSpaceSettingsOutputTypeDef,
     H265ColorSpaceSettingsTypeDef,
     VideoSelectorColorSpaceSettingsTypeDef,
+    HlsCdnSettingsOutputTypeDef,
     HlsCdnSettingsTypeDef,
+    NetworkInputSettingsOutputTypeDef,
     NetworkInputSettingsTypeDef,
+    InputClippingSettingsOutputTypeDef,
     InputClippingSettingsTypeDef,
     InputDestinationTypeDef,
     UpdateInputDeviceRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
-    StandardHlsSettingsTypeDef,
+    StandardHlsSettingsOutputTypeDef,
+    MotionGraphicsConfigurationOutputTypeDef,
     MotionGraphicsConfigurationTypeDef,
     MultiplexOutputDestinationTypeDef,
     MultiplexSummaryTypeDef,
+    MultiplexVideoSettingsOutputTypeDef,
     MultiplexVideoSettingsTypeDef,
+    NielsenWatermarksSettingsOutputTypeDef,
     NielsenWatermarksSettingsTypeDef,
+    OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
+    PauseStateScheduleActionSettingsOutputTypeDef,
     PauseStateScheduleActionSettingsTypeDef,
+    PurchaseOfferingRequestRequestTypeDef,
+    UpdateReservationRequestRequestTypeDef,
+    Scte35SegmentationDescriptorOutputTypeDef,
     Scte35SegmentationDescriptorTypeDef,
     ThumbnailDetailTypeDef,
+    VideoSelectorSettingsOutputTypeDef,
     VideoSelectorSettingsTypeDef,
+    ArchiveGroupSettingsOutputTypeDef,
     ArchiveGroupSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
+    GlobalConfigurationOutputTypeDef,
+    KeyProviderSettingsOutputTypeDef,
+    AudioSelectorSettingsOutputTypeDef,
+    AudioSelectorSettingsTypeDef,
     CaptionDestinationSettingsTypeDef,
     GlobalConfigurationTypeDef,
     KeyProviderSettingsTypeDef,
-    AudioSelectorSettingsTypeDef,
+    AvailConfigurationOutputTypeDef,
     AvailConfigurationTypeDef,
+    CaptionSelectorSettingsOutputTypeDef,
     CaptionSelectorSettingsTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     UpdateReservationResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
-    ArchiveContainerSettingsTypeDef,
-    UdpContainerSettingsTypeDef,
+    ArchiveContainerSettingsOutputTypeDef,
+    UdpContainerSettingsOutputTypeDef,
+    FailoverConditionOutputTypeDef,
     FailoverConditionTypeDef,
+    FrameCaptureGroupSettingsOutputTypeDef,
     FrameCaptureGroupSettingsTypeDef,
+    H264SettingsOutputTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     H264SettingsTypeDef,
     Mpeg2SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
+    InputPrepareScheduleActionSettingsOutputTypeDef,
+    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputPrepareScheduleActionSettingsTypeDef,
     InputSwitchScheduleActionSettingsTypeDef,
     DescribeInputResponseTypeDef,
     InputTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
     DeleteMultiplexResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
+    MultiplexProgramSettingsOutputTypeDef,
     MultiplexProgramSettingsTypeDef,
+    AudioWatermarkSettingsOutputTypeDef,
     AudioWatermarkSettingsTypeDef,
     UpdateChannelClassRequestRequestTypeDef,
+    Scte35DescriptorSettingsOutputTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
+    VideoSelectorOutputTypeDef,
     VideoSelectorTypeDef,
+    CaptionDescriptionOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    AudioSelectorOutputTypeDef,
+    AudioSelectorTypeDef,
     CaptionDescriptionTypeDef,
     HlsGroupSettingsTypeDef,
-    AudioSelectorTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
-    ArchiveOutputSettingsTypeDef,
-    UdpOutputSettingsTypeDef,
+    ArchiveOutputSettingsOutputTypeDef,
+    UdpOutputSettingsOutputTypeDef,
+    AutomaticInputFailoverSettingsOutputTypeDef,
     AutomaticInputFailoverSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     CreateInputResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     ListInputsResponseTypeDef,
     UpdateInputResponseTypeDef,
-    HlsOutputSettingsTypeDef,
+    HlsOutputSettingsOutputTypeDef,
     CreateMultiplexResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
-    CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
+    CreateMultiplexProgramRequestRequestTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
+    AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
+    Scte35DescriptorOutputTypeDef,
     Scte35DescriptorTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
+    InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
+    Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
     Scte35TimeSignalScheduleActionSettingsTypeDef,
+    InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
+    ScheduleActionSettingsOutputTypeDef,
     ScheduleActionSettingsTypeDef,
     ChannelSummaryTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
+    ScheduleActionOutputTypeDef,
     ScheduleActionTypeDef,
     ListChannelsResponseTypeDef,
+    EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
-    BatchScheduleActionCreateRequestTypeDef,
     BatchScheduleActionCreateResultTypeDef,
     BatchScheduleActionDeleteResultTypeDef,
     DescribeScheduleResponseTypeDef,
+    BatchScheduleActionCreateRequestTypeDef,
     ChannelTypeDef,
-    CreateChannelRequestRequestTypeDef,
     DeleteChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     StartChannelResponseTypeDef,
     StopChannelResponseTypeDef,
+    CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    BatchUpdateScheduleRequestRequestTypeDef,
     BatchUpdateScheduleResponseTypeDef,
+    BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.28.1\nVersion:         1.28.1\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaLive 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.1")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,14 +896,15 @@
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
@@ -982,26 +983,28 @@
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

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -894,14 +894,15 @@
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
@@ -980,26 +981,28 @@
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

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,120 +82,120 @@
 class DescribeSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 
 class ListInputDeviceTransfersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
     """
 
     def paginate(
-        self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TransferType: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
         """
 
 
 class ListInputDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
         """
 
 
 class ListInputSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
         """
 
 
 class ListInputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
         """
 
 
 class ListMultiplexProgramsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
     """
 
     def paginate(
-        self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, MultiplexId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
         """
 
 
 class ListMultiplexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
         """
 
 
@@ -214,15 +214,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
         """
 
 
@@ -239,13 +239,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,113 +79,113 @@
 class DescribeSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 class ListInputDeviceTransfersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
     """
 
     def paginate(
-        self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TransferType: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
         """
 
 class ListInputDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
         """
 
 class ListInputSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
         """
 
 class ListInputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
         """
 
 class ListMultiplexProgramsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
     """
 
     def paginate(
-        self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, MultiplexId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
         """
 
 class ListMultiplexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
         """
 
 class ListOfferingsPaginator(Paginator):
@@ -203,15 +203,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
         """
 
 class ListReservationsPaginator(Paginator):
@@ -227,13 +227,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for medialive service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
+    from mypy_boto3_medialive.type_defs import AacSettingsOutputTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from botocore.response import StreamingBody
@@ -287,61 +287,93 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
+    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
     "AcceptInputDeviceTransferRequestRequestTypeDef",
+    "AccountConfigurationOutputTypeDef",
     "AccountConfigurationTypeDef",
+    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
+    "ArchiveS3SettingsOutputTypeDef",
     "ArchiveS3SettingsTypeDef",
+    "OutputLocationRefOutputTypeDef",
     "OutputLocationRefTypeDef",
+    "InputChannelLevelOutputTypeDef",
     "InputChannelLevelTypeDef",
+    "Eac3AtmosSettingsOutputTypeDef",
+    "Eac3SettingsOutputTypeDef",
+    "Mp2SettingsOutputTypeDef",
+    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "WavSettingsTypeDef",
+    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
+    "AudioDolbyEDecodeOutputTypeDef",
     "AudioDolbyEDecodeTypeDef",
+    "AudioHlsRenditionSelectionOutputTypeDef",
     "AudioHlsRenditionSelectionTypeDef",
+    "AudioLanguageSelectionOutputTypeDef",
     "AudioLanguageSelectionTypeDef",
-    "InputLocationTypeDef",
+    "InputLocationOutputTypeDef",
+    "AudioPidSelectionOutputTypeDef",
     "AudioPidSelectionTypeDef",
+    "AudioSilenceFailoverSettingsOutputTypeDef",
     "AudioSilenceFailoverSettingsTypeDef",
+    "AudioTrackOutputTypeDef",
     "AudioTrackTypeDef",
+    "InputLocationTypeDef",
+    "EsamOutputTypeDef",
+    "Scte35SpliceInsertOutputTypeDef",
+    "Scte35TimeSignalAposOutputTypeDef",
     "EsamTypeDef",
     "Scte35SpliceInsertTypeDef",
     "Scte35TimeSignalAposTypeDef",
     "BatchDeleteRequestRequestTypeDef",
     "BatchFailedResultModelTypeDef",
     "BatchSuccessfulResultModelTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchScheduleActionDeleteRequestTypeDef",
     "BatchStartRequestRequestTypeDef",
     "BatchStopRequestRequestTypeDef",
     "CancelInputDeviceTransferRequestRequestTypeDef",
+    "EbuTtDDestinationSettingsOutputTypeDef",
+    "TtmlDestinationSettingsOutputTypeDef",
+    "WebvttDestinationSettingsOutputTypeDef",
     "EbuTtDDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
+    "CaptionLanguageMappingOutputTypeDef",
     "CaptionLanguageMappingTypeDef",
+    "CaptionRectangleOutputTypeDef",
     "CaptionRectangleTypeDef",
+    "DvbSubSourceSettingsOutputTypeDef",
+    "EmbeddedSourceSettingsOutputTypeDef",
+    "Scte20SourceSettingsOutputTypeDef",
+    "Scte27SourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "Scte20SourceSettingsTypeDef",
     "Scte27SourceSettingsTypeDef",
+    "CdiInputSpecificationOutputTypeDef",
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
-    "InputSpecificationTypeDef",
+    "InputSpecificationOutputTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
+    "InputSpecificationTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
     "MediaConnectFlowRequestTypeDef",
@@ -352,149 +384,218 @@
     "DeleteChannelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DeleteInputSecurityGroupRequestRequestTypeDef",
     "DeleteMultiplexProgramRequestRequestTypeDef",
     "MultiplexProgramPacketIdentifiersMapTypeDef",
     "MultiplexProgramPipelineDetailTypeDef",
     "DeleteMultiplexRequestRequestTypeDef",
+    "MultiplexSettingsOutputTypeDef",
     "DeleteReservationRequestRequestTypeDef",
-    "RenewalSettingsTypeDef",
+    "RenewalSettingsOutputTypeDef",
     "ReservationResourceSpecificationTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
+    "DescribeInputDeviceThumbnailResponseTypeDef",
     "DescribeInputRequestRequestTypeDef",
+    "InputDeviceSettingsOutputTypeDef",
     "InputSourceTypeDef",
     "MediaConnectFlowTypeDef",
     "DescribeInputSecurityGroupRequestRequestTypeDef",
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DescribeThumbnailsRequestRequestTypeDef",
-    "DvbNitSettingsTypeDef",
-    "DvbSdtSettingsTypeDef",
-    "DvbTdtSettingsTypeDef",
+    "DvbNitSettingsOutputTypeDef",
+    "DvbSdtSettingsOutputTypeDef",
+    "DvbTdtSettingsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FeatureActivationsOutputTypeDef",
+    "NielsenConfigurationOutputTypeDef",
+    "ThumbnailConfigurationOutputTypeDef",
+    "TimecodeConfigOutputTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
+    "InputLossFailoverSettingsOutputTypeDef",
+    "VideoBlackFailoverSettingsOutputTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
-    "FecOutputSettingsTypeDef",
+    "FecOutputSettingsOutputTypeDef",
+    "FixedModeScheduleActionStartSettingsOutputTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
-    "Fmp4HlsSettingsTypeDef",
+    "Fmp4HlsSettingsOutputTypeDef",
+    "FollowModeScheduleActionStartSettingsOutputTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
+    "FrameCaptureS3SettingsOutputTypeDef",
     "FrameCaptureS3SettingsTypeDef",
-    "FrameCaptureOutputSettingsTypeDef",
+    "FrameCaptureOutputSettingsOutputTypeDef",
+    "TimecodeBurninSettingsOutputTypeDef",
     "TimecodeBurninSettingsTypeDef",
+    "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
+    "TemporalFilterSettingsOutputTypeDef",
     "TemporalFilterSettingsTypeDef",
+    "Hdr10SettingsOutputTypeDef",
     "Hdr10SettingsTypeDef",
+    "HlsAkamaiSettingsOutputTypeDef",
     "HlsAkamaiSettingsTypeDef",
+    "HlsBasicPutSettingsOutputTypeDef",
     "HlsBasicPutSettingsTypeDef",
+    "HlsMediaStoreSettingsOutputTypeDef",
+    "HlsS3SettingsOutputTypeDef",
+    "HlsWebdavSettingsOutputTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
     "HlsWebdavSettingsTypeDef",
+    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
+    "HlsInputSettingsOutputTypeDef",
     "HlsInputSettingsTypeDef",
+    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
+    "StartTimecodeOutputTypeDef",
+    "StopTimecodeOutputTypeDef",
     "StartTimecodeTypeDef",
     "StopTimecodeTypeDef",
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "InputDeviceRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
+    "ListInputsRequestListInputsPaginateTypeDef",
     "ListInputsRequestRequestTypeDef",
+    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "M3u8SettingsTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "M3u8SettingsOutputTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
+    "MediaPackageOutputDestinationSettingsOutputTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
+    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
+    "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
-    "MsSmoothOutputSettingsTypeDef",
+    "MsSmoothOutputSettingsOutputTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
+    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
+    "MultiplexProgramServiceDescriptorOutputTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
+    "MultiplexStatmuxVideoSettingsOutputTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
+    "NielsenCBETOutputTypeDef",
     "NielsenCBETTypeDef",
+    "NielsenNaesIiNwOutputTypeDef",
     "NielsenNaesIiNwTypeDef",
+    "OutputDestinationSettingsOutputTypeDef",
     "OutputDestinationSettingsTypeDef",
+    "RtmpGroupSettingsOutputTypeDef",
+    "UdpGroupSettingsOutputTypeDef",
     "RtmpGroupSettingsTypeDef",
     "UdpGroupSettingsTypeDef",
+    "PaginatorConfigTypeDef",
+    "PipelinePauseStateSettingsOutputTypeDef",
     "PipelinePauseStateSettingsTypeDef",
+    "RenewalSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "Scte35InputScheduleActionSettingsOutputTypeDef",
+    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
+    "Scte35SpliceInsertScheduleActionSettingsOutputTypeDef",
+    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
+    "Scte35DeliveryRestrictionsOutputTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
+    "VideoSelectorPidOutputTypeDef",
     "VideoSelectorPidTypeDef",
+    "VideoSelectorProgramIdOutputTypeDef",
     "VideoSelectorProgramIdTypeDef",
+    "DescribeAccountConfigurationResponseTypeDef",
+    "UpdateAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
+    "ArchiveCdnSettingsOutputTypeDef",
     "ArchiveCdnSettingsTypeDef",
+    "MediaPackageGroupSettingsOutputTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
+    "MultiplexOutputSettingsOutputTypeDef",
+    "RtmpOutputSettingsOutputTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
-    "MultiplexOutputSettingsTypeDef",
-    "RtmpOutputSettingsTypeDef",
+    "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
-    "AudioOnlyHlsSettingsTypeDef",
+    "AudioOnlyHlsSettingsOutputTypeDef",
+    "AvailBlankingOutputTypeDef",
+    "BlackoutSlateOutputTypeDef",
+    "BurnInDestinationSettingsOutputTypeDef",
+    "DvbSubDestinationSettingsOutputTypeDef",
+    "InputLossBehaviorOutputTypeDef",
+    "StaticImageActivateScheduleActionSettingsOutputTypeDef",
+    "StaticKeySettingsOutputTypeDef",
+    "AudioTrackSelectionOutputTypeDef",
+    "AudioTrackSelectionTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AudioTrackSelectionTypeDef",
+    "AvailSettingsOutputTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
-    "DescribeAccountConfigurationResponseTypeDef",
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateAccountConfigurationResponseTypeDef",
+    "TeletextSourceSettingsOutputTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
-    "PurchaseOfferingRequestRequestTypeDef",
-    "UpdateReservationRequestRequestTypeDef",
     "DeleteReservationResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "DescribeChannelRequestChannelCreatedWaitTypeDef",
     "DescribeChannelRequestChannelDeletedWaitTypeDef",
@@ -508,148 +609,211 @@
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
-    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    "ListInputsRequestListInputsPaginateTypeDef",
-    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    "M2tsSettingsTypeDef",
+    "M2tsSettingsOutputTypeDef",
+    "FailoverConditionSettingsOutputTypeDef",
     "FailoverConditionSettingsTypeDef",
+    "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
+    "FrameCaptureCdnSettingsOutputTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
+    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
+    "H264FilterSettingsOutputTypeDef",
+    "H265FilterSettingsOutputTypeDef",
+    "Mpeg2FilterSettingsOutputTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
+    "H265ColorSpaceSettingsOutputTypeDef",
+    "VideoSelectorColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
+    "HlsCdnSettingsOutputTypeDef",
     "HlsCdnSettingsTypeDef",
+    "NetworkInputSettingsOutputTypeDef",
     "NetworkInputSettingsTypeDef",
+    "InputClippingSettingsOutputTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
-    "StandardHlsSettingsTypeDef",
+    "StandardHlsSettingsOutputTypeDef",
+    "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
+    "MultiplexVideoSettingsOutputTypeDef",
     "MultiplexVideoSettingsTypeDef",
+    "NielsenWatermarksSettingsOutputTypeDef",
     "NielsenWatermarksSettingsTypeDef",
+    "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
+    "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
+    "PurchaseOfferingRequestRequestTypeDef",
+    "UpdateReservationRequestRequestTypeDef",
+    "Scte35SegmentationDescriptorOutputTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
     "ThumbnailDetailTypeDef",
+    "VideoSelectorSettingsOutputTypeDef",
     "VideoSelectorSettingsTypeDef",
+    "ArchiveGroupSettingsOutputTypeDef",
     "ArchiveGroupSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
+    "GlobalConfigurationOutputTypeDef",
+    "KeyProviderSettingsOutputTypeDef",
+    "AudioSelectorSettingsOutputTypeDef",
+    "AudioSelectorSettingsTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "GlobalConfigurationTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AudioSelectorSettingsTypeDef",
+    "AvailConfigurationOutputTypeDef",
     "AvailConfigurationTypeDef",
+    "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
-    "ArchiveContainerSettingsTypeDef",
-    "UdpContainerSettingsTypeDef",
+    "ArchiveContainerSettingsOutputTypeDef",
+    "UdpContainerSettingsOutputTypeDef",
+    "FailoverConditionOutputTypeDef",
     "FailoverConditionTypeDef",
+    "FrameCaptureGroupSettingsOutputTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
+    "H264SettingsOutputTypeDef",
+    "Mpeg2SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
-    "HlsSettingsTypeDef",
+    "HlsSettingsOutputTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
+    "MultiplexProgramSettingsOutputTypeDef",
     "MultiplexProgramSettingsTypeDef",
+    "AudioWatermarkSettingsOutputTypeDef",
     "AudioWatermarkSettingsTypeDef",
     "UpdateChannelClassRequestRequestTypeDef",
+    "Scte35DescriptorSettingsOutputTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
+    "VideoSelectorOutputTypeDef",
     "VideoSelectorTypeDef",
+    "CaptionDescriptionOutputTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
+    "AudioSelectorTypeDef",
     "CaptionDescriptionTypeDef",
     "HlsGroupSettingsTypeDef",
-    "AudioSelectorTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
-    "ArchiveOutputSettingsTypeDef",
-    "UdpOutputSettingsTypeDef",
+    "ArchiveOutputSettingsOutputTypeDef",
+    "UdpOutputSettingsOutputTypeDef",
+    "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
-    "HlsOutputSettingsTypeDef",
+    "HlsOutputSettingsOutputTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
-    "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
+    "CreateMultiplexProgramRequestRequestTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
+    "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
+    "Scte35DescriptorOutputTypeDef",
     "Scte35DescriptorTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
+    "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
-    "OutputSettingsTypeDef",
+    "OutputSettingsOutputTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
+    "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
+    "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
     "ChannelSummaryTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
+    "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
     "ListChannelsResponseTypeDef",
+    "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
-    "BatchScheduleActionCreateRequestTypeDef",
     "BatchScheduleActionCreateResultTypeDef",
     "BatchScheduleActionDeleteResultTypeDef",
     "DescribeScheduleResponseTypeDef",
+    "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
-    "CreateChannelRequestRequestTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
+    "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "BatchUpdateScheduleRequestRequestTypeDef",
     "BatchUpdateScheduleResponseTypeDef",
+    "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
+AacSettingsOutputTypeDef = TypedDict(
+    "AacSettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "CodingMode": AacCodingModeType,
+        "InputType": AacInputTypeType,
+        "Profile": AacProfileType,
+        "RateControlMode": AacRateControlModeType,
+        "RawFormat": AacRawFormatType,
+        "SampleRate": float,
+        "Spec": AacSpecType,
+        "VbrQuality": AacVbrQualityType,
+    },
+    total=False,
+)
+
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": AacCodingModeType,
         "InputType": AacInputTypeType,
         "Profile": AacProfileType,
@@ -658,14 +822,28 @@
         "SampleRate": float,
         "Spec": AacSpecType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
+Ac3SettingsOutputTypeDef = TypedDict(
+    "Ac3SettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "BitstreamMode": Ac3BitstreamModeType,
+        "CodingMode": Ac3CodingModeType,
+        "Dialnorm": int,
+        "DrcProfile": Ac3DrcProfileType,
+        "LfeFilter": Ac3LfeFilterType,
+        "MetadataControl": Ac3MetadataControlType,
+    },
+    total=False,
+)
+
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": float,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -679,54 +857,155 @@
 AcceptInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "AcceptInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
+AccountConfigurationOutputTypeDef = TypedDict(
+    "AccountConfigurationOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
 AccountConfigurationTypeDef = TypedDict(
     "AccountConfigurationTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+AncillarySourceSettingsOutputTypeDef = TypedDict(
+    "AncillarySourceSettingsOutputTypeDef",
+    {
+        "SourceAncillaryChannelNumber": int,
+    },
+    total=False,
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "SourceAncillaryChannelNumber": int,
     },
     total=False,
 )
 
+ArchiveS3SettingsOutputTypeDef = TypedDict(
+    "ArchiveS3SettingsOutputTypeDef",
+    {
+        "CannedAcl": S3CannedAclType,
+    },
+    total=False,
+)
+
 ArchiveS3SettingsTypeDef = TypedDict(
     "ArchiveS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
+OutputLocationRefOutputTypeDef = TypedDict(
+    "OutputLocationRefOutputTypeDef",
+    {
+        "DestinationRefId": str,
+    },
+    total=False,
+)
+
 OutputLocationRefTypeDef = TypedDict(
     "OutputLocationRefTypeDef",
     {
         "DestinationRefId": str,
     },
     total=False,
 )
 
+InputChannelLevelOutputTypeDef = TypedDict(
+    "InputChannelLevelOutputTypeDef",
+    {
+        "Gain": int,
+        "InputChannel": int,
+    },
+)
+
 InputChannelLevelTypeDef = TypedDict(
     "InputChannelLevelTypeDef",
     {
         "Gain": int,
         "InputChannel": int,
     },
 )
 
+Eac3AtmosSettingsOutputTypeDef = TypedDict(
+    "Eac3AtmosSettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "CodingMode": Eac3AtmosCodingModeType,
+        "Dialnorm": int,
+        "DrcLine": Eac3AtmosDrcLineType,
+        "DrcRf": Eac3AtmosDrcRfType,
+        "HeightTrim": float,
+        "SurroundTrim": float,
+    },
+    total=False,
+)
+
+Eac3SettingsOutputTypeDef = TypedDict(
+    "Eac3SettingsOutputTypeDef",
+    {
+        "AttenuationControl": Eac3AttenuationControlType,
+        "Bitrate": float,
+        "BitstreamMode": Eac3BitstreamModeType,
+        "CodingMode": Eac3CodingModeType,
+        "DcFilter": Eac3DcFilterType,
+        "Dialnorm": int,
+        "DrcLine": Eac3DrcLineType,
+        "DrcRf": Eac3DrcRfType,
+        "LfeControl": Eac3LfeControlType,
+        "LfeFilter": Eac3LfeFilterType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MetadataControl": Eac3MetadataControlType,
+        "PassthroughControl": Eac3PassthroughControlType,
+        "PhaseControl": Eac3PhaseControlType,
+        "StereoDownmix": Eac3StereoDownmixType,
+        "SurroundExMode": Eac3SurroundExModeType,
+        "SurroundMode": Eac3SurroundModeType,
+    },
+    total=False,
+)
+
+Mp2SettingsOutputTypeDef = TypedDict(
+    "Mp2SettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "CodingMode": Mp2CodingModeType,
+        "SampleRate": float,
+    },
+    total=False,
+)
+
+WavSettingsOutputTypeDef = TypedDict(
+    "WavSettingsOutputTypeDef",
+    {
+        "BitDepth": float,
+        "CodingMode": WavCodingModeType,
+        "SampleRate": float,
+    },
+    total=False,
+)
+
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": Eac3AtmosCodingModeType,
         "Dialnorm": int,
         "DrcLine": Eac3AtmosDrcLineType,
@@ -780,39 +1059,85 @@
         "BitDepth": float,
         "CodingMode": WavCodingModeType,
         "SampleRate": float,
     },
     total=False,
 )
 
+AudioNormalizationSettingsOutputTypeDef = TypedDict(
+    "AudioNormalizationSettingsOutputTypeDef",
+    {
+        "Algorithm": AudioNormalizationAlgorithmType,
+        "AlgorithmControl": Literal["CORRECT_AUDIO"],
+        "TargetLkfs": float,
+    },
+    total=False,
+)
+
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": Literal["CORRECT_AUDIO"],
         "TargetLkfs": float,
     },
     total=False,
 )
 
+AudioDolbyEDecodeOutputTypeDef = TypedDict(
+    "AudioDolbyEDecodeOutputTypeDef",
+    {
+        "ProgramSelection": DolbyEProgramSelectionType,
+    },
+)
+
 AudioDolbyEDecodeTypeDef = TypedDict(
     "AudioDolbyEDecodeTypeDef",
     {
         "ProgramSelection": DolbyEProgramSelectionType,
     },
 )
 
+AudioHlsRenditionSelectionOutputTypeDef = TypedDict(
+    "AudioHlsRenditionSelectionOutputTypeDef",
+    {
+        "GroupId": str,
+        "Name": str,
+    },
+)
+
 AudioHlsRenditionSelectionTypeDef = TypedDict(
     "AudioHlsRenditionSelectionTypeDef",
     {
         "GroupId": str,
         "Name": str,
     },
 )
 
+_RequiredAudioLanguageSelectionOutputTypeDef = TypedDict(
+    "_RequiredAudioLanguageSelectionOutputTypeDef",
+    {
+        "LanguageCode": str,
+    },
+)
+_OptionalAudioLanguageSelectionOutputTypeDef = TypedDict(
+    "_OptionalAudioLanguageSelectionOutputTypeDef",
+    {
+        "LanguageSelectionPolicy": AudioLanguageSelectionPolicyType,
+    },
+    total=False,
+)
+
+
+class AudioLanguageSelectionOutputTypeDef(
+    _RequiredAudioLanguageSelectionOutputTypeDef, _OptionalAudioLanguageSelectionOutputTypeDef
+):
+    pass
+
+
 _RequiredAudioLanguageSelectionTypeDef = TypedDict(
     "_RequiredAudioLanguageSelectionTypeDef",
     {
         "LanguageCode": str,
     },
 )
 _OptionalAudioLanguageSelectionTypeDef = TypedDict(
@@ -826,41 +1151,72 @@
 
 class AudioLanguageSelectionTypeDef(
     _RequiredAudioLanguageSelectionTypeDef, _OptionalAudioLanguageSelectionTypeDef
 ):
     pass
 
 
-_RequiredInputLocationTypeDef = TypedDict(
-    "_RequiredInputLocationTypeDef",
+_RequiredInputLocationOutputTypeDef = TypedDict(
+    "_RequiredInputLocationOutputTypeDef",
     {
         "Uri": str,
     },
 )
-_OptionalInputLocationTypeDef = TypedDict(
-    "_OptionalInputLocationTypeDef",
+_OptionalInputLocationOutputTypeDef = TypedDict(
+    "_OptionalInputLocationOutputTypeDef",
     {
         "PasswordParam": str,
         "Username": str,
     },
     total=False,
 )
 
 
-class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
+class InputLocationOutputTypeDef(
+    _RequiredInputLocationOutputTypeDef, _OptionalInputLocationOutputTypeDef
+):
     pass
 
 
+AudioPidSelectionOutputTypeDef = TypedDict(
+    "AudioPidSelectionOutputTypeDef",
+    {
+        "Pid": int,
+    },
+)
+
 AudioPidSelectionTypeDef = TypedDict(
     "AudioPidSelectionTypeDef",
     {
         "Pid": int,
     },
 )
 
+_RequiredAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
+    "_RequiredAudioSilenceFailoverSettingsOutputTypeDef",
+    {
+        "AudioSelectorName": str,
+    },
+)
+_OptionalAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
+    "_OptionalAudioSilenceFailoverSettingsOutputTypeDef",
+    {
+        "AudioSilenceThresholdMsec": int,
+    },
+    total=False,
+)
+
+
+class AudioSilenceFailoverSettingsOutputTypeDef(
+    _RequiredAudioSilenceFailoverSettingsOutputTypeDef,
+    _OptionalAudioSilenceFailoverSettingsOutputTypeDef,
+):
+    pass
+
+
 _RequiredAudioSilenceFailoverSettingsTypeDef = TypedDict(
     "_RequiredAudioSilenceFailoverSettingsTypeDef",
     {
         "AudioSelectorName": str,
     },
 )
 _OptionalAudioSilenceFailoverSettingsTypeDef = TypedDict(
@@ -874,21 +1230,91 @@
 
 class AudioSilenceFailoverSettingsTypeDef(
     _RequiredAudioSilenceFailoverSettingsTypeDef, _OptionalAudioSilenceFailoverSettingsTypeDef
 ):
     pass
 
 
+AudioTrackOutputTypeDef = TypedDict(
+    "AudioTrackOutputTypeDef",
+    {
+        "Track": int,
+    },
+)
+
 AudioTrackTypeDef = TypedDict(
     "AudioTrackTypeDef",
     {
         "Track": int,
     },
 )
 
+_RequiredInputLocationTypeDef = TypedDict(
+    "_RequiredInputLocationTypeDef",
+    {
+        "Uri": str,
+    },
+)
+_OptionalInputLocationTypeDef = TypedDict(
+    "_OptionalInputLocationTypeDef",
+    {
+        "PasswordParam": str,
+        "Username": str,
+    },
+    total=False,
+)
+
+
+class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
+    pass
+
+
+_RequiredEsamOutputTypeDef = TypedDict(
+    "_RequiredEsamOutputTypeDef",
+    {
+        "AcquisitionPointId": str,
+        "PoisEndpoint": str,
+    },
+)
+_OptionalEsamOutputTypeDef = TypedDict(
+    "_OptionalEsamOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "PasswordParam": str,
+        "Username": str,
+        "ZoneIdentity": str,
+    },
+    total=False,
+)
+
+
+class EsamOutputTypeDef(_RequiredEsamOutputTypeDef, _OptionalEsamOutputTypeDef):
+    pass
+
+
+Scte35SpliceInsertOutputTypeDef = TypedDict(
+    "Scte35SpliceInsertOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "NoRegionalBlackoutFlag": Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
+        "WebDeliveryAllowedFlag": Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
+    },
+    total=False,
+)
+
+Scte35TimeSignalAposOutputTypeDef = TypedDict(
+    "Scte35TimeSignalAposOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "NoRegionalBlackoutFlag": Scte35AposNoRegionalBlackoutBehaviorType,
+        "WebDeliveryAllowedFlag": Scte35AposWebDeliveryAllowedBehaviorType,
+    },
+    total=False,
+)
+
 _RequiredEsamTypeDef = TypedDict(
     "_RequiredEsamTypeDef",
     {
         "AcquisitionPointId": str,
         "PoisEndpoint": str,
     },
 )
@@ -956,25 +1382,14 @@
         "Arn": str,
         "Id": str,
         "State": str,
     },
     total=False,
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
 BatchScheduleActionDeleteRequestTypeDef = TypedDict(
     "BatchScheduleActionDeleteRequestTypeDef",
     {
         "ActionNames": Sequence[str],
     },
 )
 
@@ -999,14 +1414,41 @@
 CancelInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "CancelInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
+EbuTtDDestinationSettingsOutputTypeDef = TypedDict(
+    "EbuTtDDestinationSettingsOutputTypeDef",
+    {
+        "CopyrightHolder": str,
+        "FillLineGap": EbuTtDFillLineGapControlType,
+        "FontFamily": str,
+        "StyleControl": EbuTtDDestinationStyleControlType,
+    },
+    total=False,
+)
+
+TtmlDestinationSettingsOutputTypeDef = TypedDict(
+    "TtmlDestinationSettingsOutputTypeDef",
+    {
+        "StyleControl": TtmlDestinationStyleControlType,
+    },
+    total=False,
+)
+
+WebvttDestinationSettingsOutputTypeDef = TypedDict(
+    "WebvttDestinationSettingsOutputTypeDef",
+    {
+        "StyleControl": WebvttDestinationStyleControlType,
+    },
+    total=False,
+)
+
 EbuTtDDestinationSettingsTypeDef = TypedDict(
     "EbuTtDDestinationSettingsTypeDef",
     {
         "CopyrightHolder": str,
         "FillLineGap": EbuTtDFillLineGapControlType,
         "FontFamily": str,
         "StyleControl": EbuTtDDestinationStyleControlType,
@@ -1026,33 +1468,90 @@
     "WebvttDestinationSettingsTypeDef",
     {
         "StyleControl": WebvttDestinationStyleControlType,
     },
     total=False,
 )
 
+CaptionLanguageMappingOutputTypeDef = TypedDict(
+    "CaptionLanguageMappingOutputTypeDef",
+    {
+        "CaptionChannel": int,
+        "LanguageCode": str,
+        "LanguageDescription": str,
+    },
+)
+
 CaptionLanguageMappingTypeDef = TypedDict(
     "CaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "LanguageCode": str,
         "LanguageDescription": str,
     },
 )
 
+CaptionRectangleOutputTypeDef = TypedDict(
+    "CaptionRectangleOutputTypeDef",
+    {
+        "Height": float,
+        "LeftOffset": float,
+        "TopOffset": float,
+        "Width": float,
+    },
+)
+
 CaptionRectangleTypeDef = TypedDict(
     "CaptionRectangleTypeDef",
     {
         "Height": float,
         "LeftOffset": float,
         "TopOffset": float,
         "Width": float,
     },
 )
 
+DvbSubSourceSettingsOutputTypeDef = TypedDict(
+    "DvbSubSourceSettingsOutputTypeDef",
+    {
+        "OcrLanguage": DvbSubOcrLanguageType,
+        "Pid": int,
+    },
+    total=False,
+)
+
+EmbeddedSourceSettingsOutputTypeDef = TypedDict(
+    "EmbeddedSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": EmbeddedConvert608To708Type,
+        "Scte20Detection": EmbeddedScte20DetectionType,
+        "Source608ChannelNumber": int,
+        "Source608TrackNumber": int,
+    },
+    total=False,
+)
+
+Scte20SourceSettingsOutputTypeDef = TypedDict(
+    "Scte20SourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": Scte20Convert608To708Type,
+        "Source608ChannelNumber": int,
+    },
+    total=False,
+)
+
+Scte27SourceSettingsOutputTypeDef = TypedDict(
+    "Scte27SourceSettingsOutputTypeDef",
+    {
+        "OcrLanguage": Scte27OcrLanguageType,
+        "Pid": int,
+    },
+    total=False,
+)
+
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "OcrLanguage": DvbSubOcrLanguageType,
         "Pid": int,
     },
     total=False,
@@ -1083,14 +1582,22 @@
     {
         "OcrLanguage": Scte27OcrLanguageType,
         "Pid": int,
     },
     total=False,
 )
 
+CdiInputSpecificationOutputTypeDef = TypedDict(
+    "CdiInputSpecificationOutputTypeDef",
+    {
+        "Resolution": CdiInputResolutionType,
+    },
+    total=False,
+)
+
 CdiInputSpecificationTypeDef = TypedDict(
     "CdiInputSpecificationTypeDef",
     {
         "Resolution": CdiInputResolutionType,
     },
     total=False,
 )
@@ -1099,16 +1606,16 @@
     "ChannelEgressEndpointTypeDef",
     {
         "SourceIp": str,
     },
     total=False,
 )
 
-InputSpecificationTypeDef = TypedDict(
-    "InputSpecificationTypeDef",
+InputSpecificationOutputTypeDef = TypedDict(
+    "InputSpecificationOutputTypeDef",
     {
         "Codec": InputCodecType,
         "MaximumBitrate": InputMaximumBitrateType,
         "Resolution": InputResolutionType,
     },
     total=False,
 )
@@ -1151,14 +1658,24 @@
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+InputSpecificationTypeDef = TypedDict(
+    "InputSpecificationTypeDef",
+    {
+        "Codec": InputCodecType,
+        "MaximumBitrate": InputMaximumBitrateType,
+        "Resolution": InputResolutionType,
+    },
+    total=False,
+)
+
 MaintenanceCreateSettingsTypeDef = TypedDict(
     "MaintenanceCreateSettingsTypeDef",
     {
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceStartTime": str,
     },
     total=False,
@@ -1375,23 +1892,46 @@
 DeleteMultiplexRequestRequestTypeDef = TypedDict(
     "DeleteMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 
+_RequiredMultiplexSettingsOutputTypeDef = TypedDict(
+    "_RequiredMultiplexSettingsOutputTypeDef",
+    {
+        "TransportStreamBitrate": int,
+        "TransportStreamId": int,
+    },
+)
+_OptionalMultiplexSettingsOutputTypeDef = TypedDict(
+    "_OptionalMultiplexSettingsOutputTypeDef",
+    {
+        "MaximumVideoBufferDelayMilliseconds": int,
+        "TransportStreamReservedBitrate": int,
+    },
+    total=False,
+)
+
+
+class MultiplexSettingsOutputTypeDef(
+    _RequiredMultiplexSettingsOutputTypeDef, _OptionalMultiplexSettingsOutputTypeDef
+):
+    pass
+
+
 DeleteReservationRequestRequestTypeDef = TypedDict(
     "DeleteReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-RenewalSettingsTypeDef = TypedDict(
-    "RenewalSettingsTypeDef",
+RenewalSettingsOutputTypeDef = TypedDict(
+    "RenewalSettingsOutputTypeDef",
     {
         "AutomaticRenewal": ReservationAutomaticRenewalType,
         "RenewalCount": int,
     },
     total=False,
 )
 
@@ -1496,21 +2036,41 @@
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
     {
         "InputDeviceId": str,
         "Accept": Literal["image/jpeg"],
     },
 )
 
+DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ContentType": Literal["image/jpeg"],
+        "ContentLength": int,
+        "ETag": str,
+        "LastModified": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 
+InputDeviceSettingsOutputTypeDef = TypedDict(
+    "InputDeviceSettingsOutputTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
 InputSourceTypeDef = TypedDict(
     "InputSourceTypeDef",
     {
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
@@ -1565,24 +2125,36 @@
 DescribeReservationRequestRequestTypeDef = TypedDict(
     "DescribeReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ChannelId": str,
+    },
+)
+_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
+    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeScheduleRequestRequestTypeDef = TypedDict(
@@ -1606,53 +2178,107 @@
     {
         "ChannelId": str,
         "PipelineId": str,
         "ThumbnailType": str,
     },
 )
 
-_RequiredDvbNitSettingsTypeDef = TypedDict(
-    "_RequiredDvbNitSettingsTypeDef",
+_RequiredDvbNitSettingsOutputTypeDef = TypedDict(
+    "_RequiredDvbNitSettingsOutputTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
     },
 )
-_OptionalDvbNitSettingsTypeDef = TypedDict(
-    "_OptionalDvbNitSettingsTypeDef",
+_OptionalDvbNitSettingsOutputTypeDef = TypedDict(
+    "_OptionalDvbNitSettingsOutputTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
 
-class DvbNitSettingsTypeDef(_RequiredDvbNitSettingsTypeDef, _OptionalDvbNitSettingsTypeDef):
+class DvbNitSettingsOutputTypeDef(
+    _RequiredDvbNitSettingsOutputTypeDef, _OptionalDvbNitSettingsOutputTypeDef
+):
     pass
 
 
-DvbSdtSettingsTypeDef = TypedDict(
-    "DvbSdtSettingsTypeDef",
+DvbSdtSettingsOutputTypeDef = TypedDict(
+    "DvbSdtSettingsOutputTypeDef",
     {
         "OutputSdt": DvbSdtOutputSdtType,
         "RepInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
-DvbTdtSettingsTypeDef = TypedDict(
-    "DvbTdtSettingsTypeDef",
+DvbTdtSettingsOutputTypeDef = TypedDict(
+    "DvbTdtSettingsOutputTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FeatureActivationsOutputTypeDef = TypedDict(
+    "FeatureActivationsOutputTypeDef",
+    {
+        "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
+    },
+    total=False,
+)
+
+NielsenConfigurationOutputTypeDef = TypedDict(
+    "NielsenConfigurationOutputTypeDef",
+    {
+        "DistributorId": str,
+        "NielsenPcmToId3Tagging": NielsenPcmToId3TaggingStateType,
+    },
+    total=False,
+)
+
+ThumbnailConfigurationOutputTypeDef = TypedDict(
+    "ThumbnailConfigurationOutputTypeDef",
+    {
+        "State": ThumbnailStateType,
+    },
+)
+
+_RequiredTimecodeConfigOutputTypeDef = TypedDict(
+    "_RequiredTimecodeConfigOutputTypeDef",
+    {
+        "Source": TimecodeConfigSourceType,
+    },
+)
+_OptionalTimecodeConfigOutputTypeDef = TypedDict(
+    "_OptionalTimecodeConfigOutputTypeDef",
+    {
+        "SyncThreshold": int,
+    },
+    total=False,
+)
+
+
+class TimecodeConfigOutputTypeDef(
+    _RequiredTimecodeConfigOutputTypeDef, _OptionalTimecodeConfigOutputTypeDef
+):
+    pass
+
+
 FeatureActivationsTypeDef = TypedDict(
     "FeatureActivationsTypeDef",
     {
         "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
     },
     total=False,
 )
@@ -1688,14 +2314,31 @@
 )
 
 
 class TimecodeConfigTypeDef(_RequiredTimecodeConfigTypeDef, _OptionalTimecodeConfigTypeDef):
     pass
 
 
+InputLossFailoverSettingsOutputTypeDef = TypedDict(
+    "InputLossFailoverSettingsOutputTypeDef",
+    {
+        "InputLossThresholdMsec": int,
+    },
+    total=False,
+)
+
+VideoBlackFailoverSettingsOutputTypeDef = TypedDict(
+    "VideoBlackFailoverSettingsOutputTypeDef",
+    {
+        "BlackDetectThreshold": float,
+        "VideoBlackThresholdMsec": int,
+    },
+    total=False,
+)
+
 InputLossFailoverSettingsTypeDef = TypedDict(
     "InputLossFailoverSettingsTypeDef",
     {
         "InputLossThresholdMsec": int,
     },
     total=False,
 )
@@ -1705,65 +2348,110 @@
     {
         "BlackDetectThreshold": float,
         "VideoBlackThresholdMsec": int,
     },
     total=False,
 )
 
-FecOutputSettingsTypeDef = TypedDict(
-    "FecOutputSettingsTypeDef",
+FecOutputSettingsOutputTypeDef = TypedDict(
+    "FecOutputSettingsOutputTypeDef",
     {
         "ColumnDepth": int,
         "IncludeFec": FecOutputIncludeFecType,
         "RowLength": int,
     },
     total=False,
 )
 
+FixedModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "FixedModeScheduleActionStartSettingsOutputTypeDef",
+    {
+        "Time": str,
+    },
+)
+
 FixedModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FixedModeScheduleActionStartSettingsTypeDef",
     {
         "Time": str,
     },
 )
 
-Fmp4HlsSettingsTypeDef = TypedDict(
-    "Fmp4HlsSettingsTypeDef",
+Fmp4HlsSettingsOutputTypeDef = TypedDict(
+    "Fmp4HlsSettingsOutputTypeDef",
     {
         "AudioRenditionSets": str,
         "NielsenId3Behavior": Fmp4NielsenId3BehaviorType,
         "TimedMetadataBehavior": Fmp4TimedMetadataBehaviorType,
     },
     total=False,
 )
 
+FollowModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "FollowModeScheduleActionStartSettingsOutputTypeDef",
+    {
+        "FollowPoint": FollowPointType,
+        "ReferenceActionName": str,
+    },
+)
+
 FollowModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FollowModeScheduleActionStartSettingsTypeDef",
     {
         "FollowPoint": FollowPointType,
         "ReferenceActionName": str,
     },
 )
 
+FrameCaptureS3SettingsOutputTypeDef = TypedDict(
+    "FrameCaptureS3SettingsOutputTypeDef",
+    {
+        "CannedAcl": S3CannedAclType,
+    },
+    total=False,
+)
+
 FrameCaptureS3SettingsTypeDef = TypedDict(
     "FrameCaptureS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
-FrameCaptureOutputSettingsTypeDef = TypedDict(
-    "FrameCaptureOutputSettingsTypeDef",
+FrameCaptureOutputSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureOutputSettingsOutputTypeDef",
     {
         "NameModifier": str,
     },
     total=False,
 )
 
+_RequiredTimecodeBurninSettingsOutputTypeDef = TypedDict(
+    "_RequiredTimecodeBurninSettingsOutputTypeDef",
+    {
+        "FontSize": TimecodeBurninFontSizeType,
+        "Position": TimecodeBurninPositionType,
+    },
+)
+_OptionalTimecodeBurninSettingsOutputTypeDef = TypedDict(
+    "_OptionalTimecodeBurninSettingsOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+
+class TimecodeBurninSettingsOutputTypeDef(
+    _RequiredTimecodeBurninSettingsOutputTypeDef, _OptionalTimecodeBurninSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredTimecodeBurninSettingsTypeDef = TypedDict(
     "_RequiredTimecodeBurninSettingsTypeDef",
     {
         "FontSize": TimecodeBurninFontSizeType,
         "Position": TimecodeBurninPositionType,
     },
 )
@@ -1778,67 +2466,152 @@
 
 class TimecodeBurninSettingsTypeDef(
     _RequiredTimecodeBurninSettingsTypeDef, _OptionalTimecodeBurninSettingsTypeDef
 ):
     pass
 
 
+H264ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H264ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": Dict[str, Any],
+        "Rec601Settings": Dict[str, Any],
+        "Rec709Settings": Dict[str, Any],
+    },
+    total=False,
+)
+
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "Rec601Settings": Mapping[str, Any],
         "Rec709Settings": Mapping[str, Any],
     },
     total=False,
 )
 
+TemporalFilterSettingsOutputTypeDef = TypedDict(
+    "TemporalFilterSettingsOutputTypeDef",
+    {
+        "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
+        "Strength": TemporalFilterStrengthType,
+    },
+    total=False,
+)
+
 TemporalFilterSettingsTypeDef = TypedDict(
     "TemporalFilterSettingsTypeDef",
     {
         "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
         "Strength": TemporalFilterStrengthType,
     },
     total=False,
 )
 
+Hdr10SettingsOutputTypeDef = TypedDict(
+    "Hdr10SettingsOutputTypeDef",
+    {
+        "MaxCll": int,
+        "MaxFall": int,
+    },
+    total=False,
+)
+
 Hdr10SettingsTypeDef = TypedDict(
     "Hdr10SettingsTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
+HlsAkamaiSettingsOutputTypeDef = TypedDict(
+    "HlsAkamaiSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "HttpTransferMode": HlsAkamaiHttpTransferModeType,
+        "NumRetries": int,
+        "RestartDelay": int,
+        "Salt": str,
+        "Token": str,
+    },
+    total=False,
+)
+
 HlsAkamaiSettingsTypeDef = TypedDict(
     "HlsAkamaiSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "HttpTransferMode": HlsAkamaiHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
         "Salt": str,
         "Token": str,
     },
     total=False,
 )
 
+HlsBasicPutSettingsOutputTypeDef = TypedDict(
+    "HlsBasicPutSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "NumRetries": int,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
 HlsBasicPutSettingsTypeDef = TypedDict(
     "HlsBasicPutSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
+HlsMediaStoreSettingsOutputTypeDef = TypedDict(
+    "HlsMediaStoreSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "MediaStoreStorageClass": Literal["TEMPORAL"],
+        "NumRetries": int,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
+HlsS3SettingsOutputTypeDef = TypedDict(
+    "HlsS3SettingsOutputTypeDef",
+    {
+        "CannedAcl": S3CannedAclType,
+    },
+    total=False,
+)
+
+HlsWebdavSettingsOutputTypeDef = TypedDict(
+    "HlsWebdavSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "HttpTransferMode": HlsWebdavHttpTransferModeType,
+        "NumRetries": int,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
 HlsMediaStoreSettingsTypeDef = TypedDict(
     "HlsMediaStoreSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "MediaStoreStorageClass": Literal["TEMPORAL"],
         "NumRetries": int,
@@ -1863,42 +2636,87 @@
         "HttpTransferMode": HlsWebdavHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
+HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef = TypedDict(
+    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
+    {
+        "Tag": str,
+        "Id3": str,
+    },
+    total=False,
+)
+
 HlsId3SegmentTaggingScheduleActionSettingsTypeDef = TypedDict(
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
     {
         "Tag": str,
         "Id3": str,
     },
     total=False,
 )
 
+HlsInputSettingsOutputTypeDef = TypedDict(
+    "HlsInputSettingsOutputTypeDef",
+    {
+        "Bandwidth": int,
+        "BufferSegments": int,
+        "Retries": int,
+        "RetryInterval": int,
+        "Scte35Source": HlsScte35SourceTypeType,
+    },
+    total=False,
+)
+
 HlsInputSettingsTypeDef = TypedDict(
     "HlsInputSettingsTypeDef",
     {
         "Bandwidth": int,
         "BufferSegments": int,
         "Retries": int,
         "RetryInterval": int,
         "Scte35Source": HlsScte35SourceTypeType,
     },
     total=False,
 )
 
+HlsTimedMetadataScheduleActionSettingsOutputTypeDef = TypedDict(
+    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
+    {
+        "Id3": str,
+    },
+)
+
 HlsTimedMetadataScheduleActionSettingsTypeDef = TypedDict(
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
     {
         "Id3": str,
     },
 )
 
+StartTimecodeOutputTypeDef = TypedDict(
+    "StartTimecodeOutputTypeDef",
+    {
+        "Timecode": str,
+    },
+    total=False,
+)
+
+StopTimecodeOutputTypeDef = TypedDict(
+    "StopTimecodeOutputTypeDef",
+    {
+        "LastFrameClippingBehavior": LastFrameClippingBehaviorType,
+        "Timecode": str,
+    },
+    total=False,
+)
+
 StartTimecodeTypeDef = TypedDict(
     "StartTimecodeTypeDef",
     {
         "Timecode": str,
     },
     total=False,
 )
@@ -1935,23 +2753,53 @@
     "InputDeviceRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "TransferType": str,
+    },
+)
+_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
+    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "_RequiredListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
     },
 )
 _OptionalListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
@@ -1978,41 +2826,87 @@
         "Message": str,
         "TargetCustomerId": str,
         "TransferType": InputDeviceTransferTypeType,
     },
     total=False,
 )
 
+ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputDevicesRequestRequestTypeDef = TypedDict(
     "ListInputDevicesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputSecurityGroupsRequestRequestTypeDef = TypedDict(
     "ListInputSecurityGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputsRequestListInputsPaginateTypeDef = TypedDict(
+    "ListInputsRequestListInputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputsRequestRequestTypeDef = TypedDict(
     "ListInputsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "MultiplexId": str,
+    },
+)
+_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
+    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListMultiplexProgramsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiplexProgramsRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalListMultiplexProgramsRequestRequestTypeDef = TypedDict(
@@ -2037,23 +2931,49 @@
     {
         "ChannelId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
+ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMultiplexesRequestRequestTypeDef = TypedDict(
     "ListMultiplexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "ChannelConfiguration": str,
+        "Codec": str,
+        "Duration": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "ChannelConfiguration": str,
         "Codec": str,
         "Duration": str,
@@ -2065,14 +2985,30 @@
         "ResourceType": str,
         "SpecialFeature": str,
         "VideoQuality": str,
     },
     total=False,
 )
 
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "Codec": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "Codec": str,
         "MaxResults": int,
         "MaximumBitrate": str,
@@ -2089,16 +3025,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-M3u8SettingsTypeDef = TypedDict(
-    "M3u8SettingsTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+M3u8SettingsOutputTypeDef = TypedDict(
+    "M3u8SettingsOutputTypeDef",
     {
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "EcmPid": str,
         "NielsenId3Behavior": M3u8NielsenId3BehaviorType,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
@@ -2123,43 +3067,70 @@
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceScheduledDate": str,
         "MaintenanceStartTime": str,
     },
     total=False,
 )
 
+MediaPackageOutputDestinationSettingsOutputTypeDef = TypedDict(
+    "MediaPackageOutputDestinationSettingsOutputTypeDef",
+    {
+        "ChannelId": str,
+    },
+    total=False,
+)
+
 MediaPackageOutputDestinationSettingsTypeDef = TypedDict(
     "MediaPackageOutputDestinationSettingsTypeDef",
     {
         "ChannelId": str,
     },
     total=False,
 )
 
+MotionGraphicsActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
+    {
+        "Duration": int,
+        "PasswordParam": str,
+        "Url": str,
+        "Username": str,
+    },
+    total=False,
+)
+
 MotionGraphicsActivateScheduleActionSettingsTypeDef = TypedDict(
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     {
         "Duration": int,
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
+MotionGraphicsSettingsOutputTypeDef = TypedDict(
+    "MotionGraphicsSettingsOutputTypeDef",
+    {
+        "HtmlMotionGraphicsSettings": Dict[str, Any],
+    },
+    total=False,
+)
+
 MotionGraphicsSettingsTypeDef = TypedDict(
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-MsSmoothOutputSettingsTypeDef = TypedDict(
-    "MsSmoothOutputSettingsTypeDef",
+MsSmoothOutputSettingsOutputTypeDef = TypedDict(
+    "MsSmoothOutputSettingsOutputTypeDef",
     {
         "H265PackagingType": MsSmoothH265PackagingTypeType,
         "NameModifier": str,
     },
     total=False,
 )
 
@@ -2167,23 +3138,40 @@
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     {
         "EntitlementArn": str,
     },
     total=False,
 )
 
+MultiplexProgramChannelDestinationSettingsOutputTypeDef = TypedDict(
+    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
+    {
+        "MultiplexId": str,
+        "ProgramName": str,
+    },
+    total=False,
+)
+
 MultiplexProgramChannelDestinationSettingsTypeDef = TypedDict(
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
+MultiplexProgramServiceDescriptorOutputTypeDef = TypedDict(
+    "MultiplexProgramServiceDescriptorOutputTypeDef",
+    {
+        "ProviderName": str,
+        "ServiceName": str,
+    },
+)
+
 MultiplexProgramServiceDescriptorTypeDef = TypedDict(
     "MultiplexProgramServiceDescriptorTypeDef",
     {
         "ProviderName": str,
         "ServiceName": str,
     },
 )
@@ -2192,33 +3180,74 @@
     "MultiplexSettingsSummaryTypeDef",
     {
         "TransportStreamBitrate": int,
     },
     total=False,
 )
 
+MultiplexStatmuxVideoSettingsOutputTypeDef = TypedDict(
+    "MultiplexStatmuxVideoSettingsOutputTypeDef",
+    {
+        "MaximumBitrate": int,
+        "MinimumBitrate": int,
+        "Priority": int,
+    },
+    total=False,
+)
+
 MultiplexStatmuxVideoSettingsTypeDef = TypedDict(
     "MultiplexStatmuxVideoSettingsTypeDef",
     {
         "MaximumBitrate": int,
         "MinimumBitrate": int,
         "Priority": int,
     },
     total=False,
 )
 
+NielsenCBETOutputTypeDef = TypedDict(
+    "NielsenCBETOutputTypeDef",
+    {
+        "CbetCheckDigitString": str,
+        "CbetStepaside": NielsenWatermarksCbetStepasideType,
+        "Csid": str,
+    },
+)
+
 NielsenCBETTypeDef = TypedDict(
     "NielsenCBETTypeDef",
     {
         "CbetCheckDigitString": str,
         "CbetStepaside": NielsenWatermarksCbetStepasideType,
         "Csid": str,
     },
 )
 
+_RequiredNielsenNaesIiNwOutputTypeDef = TypedDict(
+    "_RequiredNielsenNaesIiNwOutputTypeDef",
+    {
+        "CheckDigitString": str,
+        "Sid": float,
+    },
+)
+_OptionalNielsenNaesIiNwOutputTypeDef = TypedDict(
+    "_OptionalNielsenNaesIiNwOutputTypeDef",
+    {
+        "Timezone": NielsenWatermarkTimezonesType,
+    },
+    total=False,
+)
+
+
+class NielsenNaesIiNwOutputTypeDef(
+    _RequiredNielsenNaesIiNwOutputTypeDef, _OptionalNielsenNaesIiNwOutputTypeDef
+):
+    pass
+
+
 _RequiredNielsenNaesIiNwTypeDef = TypedDict(
     "_RequiredNielsenNaesIiNwTypeDef",
     {
         "CheckDigitString": str,
         "Sid": float,
     },
 )
@@ -2231,25 +3260,60 @@
 )
 
 
 class NielsenNaesIiNwTypeDef(_RequiredNielsenNaesIiNwTypeDef, _OptionalNielsenNaesIiNwTypeDef):
     pass
 
 
+OutputDestinationSettingsOutputTypeDef = TypedDict(
+    "OutputDestinationSettingsOutputTypeDef",
+    {
+        "PasswordParam": str,
+        "StreamName": str,
+        "Url": str,
+        "Username": str,
+    },
+    total=False,
+)
+
 OutputDestinationSettingsTypeDef = TypedDict(
     "OutputDestinationSettingsTypeDef",
     {
         "PasswordParam": str,
         "StreamName": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
+RtmpGroupSettingsOutputTypeDef = TypedDict(
+    "RtmpGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[Literal["ON_CUE_POINT_SCTE35"]],
+        "AuthenticationScheme": AuthenticationSchemeType,
+        "CacheFullBehavior": RtmpCacheFullBehaviorType,
+        "CacheLength": int,
+        "CaptionData": RtmpCaptionDataType,
+        "InputLossAction": InputLossActionForRtmpOutType,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
+UdpGroupSettingsOutputTypeDef = TypedDict(
+    "UdpGroupSettingsOutputTypeDef",
+    {
+        "InputLossAction": InputLossActionForUdpOutType,
+        "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+    },
+    total=False,
+)
+
 RtmpGroupSettingsTypeDef = TypedDict(
     "RtmpGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[Literal["ON_CUE_POINT_SCTE35"]],
         "AuthenticationScheme": AuthenticationSchemeType,
         "CacheFullBehavior": RtmpCacheFullBehaviorType,
         "CacheLength": int,
@@ -2266,21 +3330,47 @@
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+PipelinePauseStateSettingsOutputTypeDef = TypedDict(
+    "PipelinePauseStateSettingsOutputTypeDef",
+    {
+        "PipelineId": PipelineIdType,
+    },
+)
+
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
+RenewalSettingsTypeDef = TypedDict(
+    "RenewalSettingsTypeDef",
+    {
+        "AutomaticRenewal": ReservationAutomaticRenewalType,
+        "RenewalCount": int,
+    },
+    total=False,
+)
+
 _RequiredRebootInputDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredRebootInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 _OptionalRebootInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2301,14 +3391,85 @@
 RejectInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "RejectInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
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
+_RequiredScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredScte35InputScheduleActionSettingsOutputTypeDef",
+    {
+        "Mode": Scte35InputModeType,
+    },
+)
+_OptionalScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalScte35InputScheduleActionSettingsOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+    },
+    total=False,
+)
+
+
+class Scte35InputScheduleActionSettingsOutputTypeDef(
+    _RequiredScte35InputScheduleActionSettingsOutputTypeDef,
+    _OptionalScte35InputScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
+
+Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef = TypedDict(
+    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
+    {
+        "SpliceEventId": int,
+    },
+)
+
+_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
+    {
+        "SpliceEventId": int,
+    },
+)
+_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
+
+class Scte35SpliceInsertScheduleActionSettingsOutputTypeDef(
+    _RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+    _OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
+
+StaticImageDeactivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
+    {
+        "FadeOut": int,
+        "Layer": int,
+    },
+    total=False,
+)
+
 _RequiredScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredScte35InputScheduleActionSettingsTypeDef",
     {
         "Mode": Scte35InputModeType,
     },
 )
 _OptionalScte35InputScheduleActionSettingsTypeDef = TypedDict(
@@ -2361,14 +3522,24 @@
     {
         "FadeOut": int,
         "Layer": int,
     },
     total=False,
 )
 
+Scte35DeliveryRestrictionsOutputTypeDef = TypedDict(
+    "Scte35DeliveryRestrictionsOutputTypeDef",
+    {
+        "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
+        "DeviceRestrictions": Scte35DeviceRestrictionsType,
+        "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
+        "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
+    },
+)
+
 Scte35DeliveryRestrictionsTypeDef = TypedDict(
     "Scte35DeliveryRestrictionsTypeDef",
     {
         "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
         "DeviceRestrictions": Scte35DeviceRestrictionsType,
         "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
         "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
@@ -2441,61 +3612,101 @@
 class TransferInputDeviceRequestRequestTypeDef(
     _RequiredTransferInputDeviceRequestRequestTypeDef,
     _OptionalTransferInputDeviceRequestRequestTypeDef,
 ):
     pass
 
 
+VideoSelectorPidOutputTypeDef = TypedDict(
+    "VideoSelectorPidOutputTypeDef",
+    {
+        "Pid": int,
+    },
+    total=False,
+)
+
 VideoSelectorPidTypeDef = TypedDict(
     "VideoSelectorPidTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
 
+VideoSelectorProgramIdOutputTypeDef = TypedDict(
+    "VideoSelectorProgramIdOutputTypeDef",
+    {
+        "ProgramId": int,
+    },
+    total=False,
+)
+
 VideoSelectorProgramIdTypeDef = TypedDict(
     "VideoSelectorProgramIdTypeDef",
     {
         "ProgramId": int,
     },
     total=False,
 )
 
+DescribeAccountConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
     },
     total=False,
 )
 
+ArchiveCdnSettingsOutputTypeDef = TypedDict(
+    "ArchiveCdnSettingsOutputTypeDef",
+    {
+        "ArchiveS3Settings": ArchiveS3SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": ArchiveS3SettingsTypeDef,
     },
     total=False,
 )
 
-MediaPackageGroupSettingsTypeDef = TypedDict(
-    "MediaPackageGroupSettingsTypeDef",
+MediaPackageGroupSettingsOutputTypeDef = TypedDict(
+    "MediaPackageGroupSettingsOutputTypeDef",
     {
-        "Destination": OutputLocationRefTypeDef,
+        "Destination": OutputLocationRefOutputTypeDef,
     },
 )
 
-_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_RequiredMsSmoothGroupSettingsTypeDef",
+_RequiredMsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredMsSmoothGroupSettingsOutputTypeDef",
     {
-        "Destination": OutputLocationRefTypeDef,
+        "Destination": OutputLocationRefOutputTypeDef,
     },
 )
-_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_OptionalMsSmoothGroupSettingsTypeDef",
+_OptionalMsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalMsSmoothGroupSettingsOutputTypeDef",
     {
         "AcquisitionPointId": str,
         "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
         "CertificateMode": SmoothGroupCertificateModeType,
         "ConnectionRetryInterval": int,
         "EventId": str,
         "EventIdMode": SmoothGroupEventIdModeType,
@@ -2512,83 +3723,324 @@
         "TimestampOffset": str,
         "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
 
-class MsSmoothGroupSettingsTypeDef(
-    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
+class MsSmoothGroupSettingsOutputTypeDef(
+    _RequiredMsSmoothGroupSettingsOutputTypeDef, _OptionalMsSmoothGroupSettingsOutputTypeDef
+):
+    pass
+
+
+MultiplexOutputSettingsOutputTypeDef = TypedDict(
+    "MultiplexOutputSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+
+_RequiredRtmpOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredRtmpOutputSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalRtmpOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalRtmpOutputSettingsOutputTypeDef",
+    {
+        "CertificateMode": RtmpOutputCertificateModeType,
+        "ConnectionRetryInterval": int,
+        "NumRetries": int,
+    },
+    total=False,
+)
+
+
+class RtmpOutputSettingsOutputTypeDef(
+    _RequiredRtmpOutputSettingsOutputTypeDef, _OptionalRtmpOutputSettingsOutputTypeDef
 ):
     pass
 
 
-MultiplexOutputSettingsTypeDef = TypedDict(
-    "MultiplexOutputSettingsTypeDef",
+MediaPackageGroupSettingsTypeDef = TypedDict(
+    "MediaPackageGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 
-_RequiredRtmpOutputSettingsTypeDef = TypedDict(
-    "_RequiredRtmpOutputSettingsTypeDef",
+_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_RequiredMsSmoothGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalRtmpOutputSettingsTypeDef = TypedDict(
-    "_OptionalRtmpOutputSettingsTypeDef",
+_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_OptionalMsSmoothGroupSettingsTypeDef",
     {
-        "CertificateMode": RtmpOutputCertificateModeType,
+        "AcquisitionPointId": str,
+        "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
+        "CertificateMode": SmoothGroupCertificateModeType,
         "ConnectionRetryInterval": int,
+        "EventId": str,
+        "EventIdMode": SmoothGroupEventIdModeType,
+        "EventStopBehavior": SmoothGroupEventStopBehaviorType,
+        "FilecacheDuration": int,
+        "FragmentLength": int,
+        "InputLossAction": InputLossActionForMsSmoothOutType,
         "NumRetries": int,
+        "RestartDelay": int,
+        "SegmentationMode": SmoothGroupSegmentationModeType,
+        "SendDelayMs": int,
+        "SparseTrackType": SmoothGroupSparseTrackTypeType,
+        "StreamManifestBehavior": SmoothGroupStreamManifestBehaviorType,
+        "TimestampOffset": str,
+        "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
 
-class RtmpOutputSettingsTypeDef(
-    _RequiredRtmpOutputSettingsTypeDef, _OptionalRtmpOutputSettingsTypeDef
+class MsSmoothGroupSettingsTypeDef(
+    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
 ):
     pass
 
 
+AudioChannelMappingOutputTypeDef = TypedDict(
+    "AudioChannelMappingOutputTypeDef",
+    {
+        "InputChannelLevels": List[InputChannelLevelOutputTypeDef],
+        "OutputChannel": int,
+    },
+)
+
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
         "InputChannelLevels": Sequence[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
 
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": AacSettingsOutputTypeDef,
+        "Ac3Settings": Ac3SettingsOutputTypeDef,
+        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
+        "Eac3Settings": Eac3SettingsOutputTypeDef,
+        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "PassThroughSettings": Dict[str, Any],
+        "WavSettings": WavSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
         "Eac3Settings": Eac3SettingsTypeDef,
         "Mp2Settings": Mp2SettingsTypeDef,
         "PassThroughSettings": Mapping[str, Any],
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
-AudioOnlyHlsSettingsTypeDef = TypedDict(
-    "AudioOnlyHlsSettingsTypeDef",
+AudioOnlyHlsSettingsOutputTypeDef = TypedDict(
+    "AudioOnlyHlsSettingsOutputTypeDef",
     {
         "AudioGroupId": str,
-        "AudioOnlyImage": InputLocationTypeDef,
+        "AudioOnlyImage": InputLocationOutputTypeDef,
         "AudioTrackType": AudioOnlyHlsTrackTypeType,
         "SegmentType": AudioOnlyHlsSegmentTypeType,
     },
     total=False,
 )
 
+AvailBlankingOutputTypeDef = TypedDict(
+    "AvailBlankingOutputTypeDef",
+    {
+        "AvailBlankingImage": InputLocationOutputTypeDef,
+        "State": AvailBlankingStateType,
+    },
+    total=False,
+)
+
+BlackoutSlateOutputTypeDef = TypedDict(
+    "BlackoutSlateOutputTypeDef",
+    {
+        "BlackoutSlateImage": InputLocationOutputTypeDef,
+        "NetworkEndBlackout": BlackoutSlateNetworkEndBlackoutType,
+        "NetworkEndBlackoutImage": InputLocationOutputTypeDef,
+        "NetworkId": str,
+        "State": BlackoutSlateStateType,
+    },
+    total=False,
+)
+
+BurnInDestinationSettingsOutputTypeDef = TypedDict(
+    "BurnInDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": BurnInAlignmentType,
+        "BackgroundColor": BurnInBackgroundColorType,
+        "BackgroundOpacity": int,
+        "Font": InputLocationOutputTypeDef,
+        "FontColor": BurnInFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontSize": str,
+        "OutlineColor": BurnInOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": BurnInShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "TeletextGridControl": BurnInTeletextGridControlType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+    total=False,
+)
+
+DvbSubDestinationSettingsOutputTypeDef = TypedDict(
+    "DvbSubDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": DvbSubDestinationAlignmentType,
+        "BackgroundColor": DvbSubDestinationBackgroundColorType,
+        "BackgroundOpacity": int,
+        "Font": InputLocationOutputTypeDef,
+        "FontColor": DvbSubDestinationFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontSize": str,
+        "OutlineColor": DvbSubDestinationOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": DvbSubDestinationShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "TeletextGridControl": DvbSubDestinationTeletextGridControlType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+    total=False,
+)
+
+InputLossBehaviorOutputTypeDef = TypedDict(
+    "InputLossBehaviorOutputTypeDef",
+    {
+        "BlackFrameMsec": int,
+        "InputLossImageColor": str,
+        "InputLossImageSlate": InputLocationOutputTypeDef,
+        "InputLossImageType": InputLossImageTypeType,
+        "RepeatFrameMsec": int,
+    },
+    total=False,
+)
+
+_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef",
+    {
+        "Image": InputLocationOutputTypeDef,
+    },
+)
+_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef",
+    {
+        "Duration": int,
+        "FadeIn": int,
+        "FadeOut": int,
+        "Height": int,
+        "ImageX": int,
+        "ImageY": int,
+        "Layer": int,
+        "Opacity": int,
+        "Width": int,
+    },
+    total=False,
+)
+
+
+class StaticImageActivateScheduleActionSettingsOutputTypeDef(
+    _RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef,
+    _OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
+
+_RequiredStaticKeySettingsOutputTypeDef = TypedDict(
+    "_RequiredStaticKeySettingsOutputTypeDef",
+    {
+        "StaticKeyValue": str,
+    },
+)
+_OptionalStaticKeySettingsOutputTypeDef = TypedDict(
+    "_OptionalStaticKeySettingsOutputTypeDef",
+    {
+        "KeyProviderServer": InputLocationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class StaticKeySettingsOutputTypeDef(
+    _RequiredStaticKeySettingsOutputTypeDef, _OptionalStaticKeySettingsOutputTypeDef
+):
+    pass
+
+
+_RequiredAudioTrackSelectionOutputTypeDef = TypedDict(
+    "_RequiredAudioTrackSelectionOutputTypeDef",
+    {
+        "Tracks": List[AudioTrackOutputTypeDef],
+    },
+)
+_OptionalAudioTrackSelectionOutputTypeDef = TypedDict(
+    "_OptionalAudioTrackSelectionOutputTypeDef",
+    {
+        "DolbyEDecode": AudioDolbyEDecodeOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AudioTrackSelectionOutputTypeDef(
+    _RequiredAudioTrackSelectionOutputTypeDef, _OptionalAudioTrackSelectionOutputTypeDef
+):
+    pass
+
+
+_RequiredAudioTrackSelectionTypeDef = TypedDict(
+    "_RequiredAudioTrackSelectionTypeDef",
+    {
+        "Tracks": Sequence[AudioTrackTypeDef],
+    },
+)
+_OptionalAudioTrackSelectionTypeDef = TypedDict(
+    "_OptionalAudioTrackSelectionTypeDef",
+    {
+        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
+    },
+    total=False,
+)
+
+
+class AudioTrackSelectionTypeDef(
+    _RequiredAudioTrackSelectionTypeDef, _OptionalAudioTrackSelectionTypeDef
+):
+    pass
+
+
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": InputLocationTypeDef,
         "State": AvailBlankingStateType,
     },
     total=False,
@@ -2713,35 +4165,24 @@
 
 class StaticKeySettingsTypeDef(
     _RequiredStaticKeySettingsTypeDef, _OptionalStaticKeySettingsTypeDef
 ):
     pass
 
 
-_RequiredAudioTrackSelectionTypeDef = TypedDict(
-    "_RequiredAudioTrackSelectionTypeDef",
+AvailSettingsOutputTypeDef = TypedDict(
+    "AvailSettingsOutputTypeDef",
     {
-        "Tracks": Sequence[AudioTrackTypeDef],
-    },
-)
-_OptionalAudioTrackSelectionTypeDef = TypedDict(
-    "_OptionalAudioTrackSelectionTypeDef",
-    {
-        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
+        "Esam": EsamOutputTypeDef,
+        "Scte35SpliceInsert": Scte35SpliceInsertOutputTypeDef,
+        "Scte35TimeSignalApos": Scte35TimeSignalAposOutputTypeDef,
     },
     total=False,
 )
 
-
-class AudioTrackSelectionTypeDef(
-    _RequiredAudioTrackSelectionTypeDef, _OptionalAudioTrackSelectionTypeDef
-):
-    pass
-
-
 AvailSettingsTypeDef = TypedDict(
     "AvailSettingsTypeDef",
     {
         "Esam": EsamTypeDef,
         "Scte35SpliceInsert": Scte35SpliceInsertTypeDef,
         "Scte35TimeSignalApos": Scte35TimeSignalAposTypeDef,
     },
@@ -2749,77 +4190,43 @@
 )
 
 BatchDeleteResponseTypeDef = TypedDict(
     "BatchDeleteResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStartResponseTypeDef = TypedDict(
     "BatchStartResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStopResponseTypeDef = TypedDict(
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountConfigurationResponseTypeDef = TypedDict(
-    "DescribeAccountConfigurationResponseTypeDef",
-    {
-        "AccountConfiguration": AccountConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ContentType": Literal["image/jpeg"],
-        "ContentLength": int,
-        "ETag": str,
-        "LastModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
+TeletextSourceSettingsOutputTypeDef = TypedDict(
+    "TeletextSourceSettingsOutputTypeDef",
     {
-        "AccountConfiguration": AccountConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "OutputRectangle": CaptionRectangleOutputTypeDef,
+        "PageNumber": str,
     },
+    total=False,
 )
 
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
         "PageNumber": str,
@@ -2919,62 +4326,14 @@
 
 class UpdateMultiplexRequestRequestTypeDef(
     _RequiredUpdateMultiplexRequestRequestTypeDef, _OptionalUpdateMultiplexRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_RequiredPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Count": int,
-        "OfferingId": str,
-    },
-)
-_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_OptionalPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-        "RequestId": str,
-        "Start": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class PurchaseOfferingRequestRequestTypeDef(
-    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReservationRequestRequestTypeDef",
-    {
-        "ReservationId": str,
-    },
-)
-_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReservationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateReservationRequestRequestTypeDef(
-    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
-):
-    pass
-
-
 DeleteReservationResponseTypeDef = TypedDict(
     "DeleteReservationResponseTypeDef",
     {
         "Arn": str,
         "Count": int,
         "CurrencyCode": str,
         "Duration": int,
@@ -2982,22 +4341,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
+        "RenewalSettings": RenewalSettingsOutputTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Arn": str,
@@ -3007,15 +4366,15 @@
         "FixedPrice": float,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Arn": str,
@@ -3026,22 +4385,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
+        "RenewalSettings": RenewalSettingsOutputTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "Arn": str,
@@ -3070,15 +4429,15 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
+        "RenewalSettings": RenewalSettingsOutputTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
     },
@@ -3339,15 +4698,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
         "Arn": str,
@@ -3379,28 +4738,28 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputSecurityGroupTypeDef = TypedDict(
     "InputSecurityGroupTypeDef",
     {
         "Arn": str,
@@ -3409,172 +4768,32 @@
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "ChannelId": str,
-    },
-)
-_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
-    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-):
-    pass
-
-
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "TransferType": str,
-    },
-)
-_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
-    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-):
-    pass
-
-
-ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputsRequestListInputsPaginateTypeDef = TypedDict(
-    "ListInputsRequestListInputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "MultiplexId": str,
-    },
-)
-_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
-    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-):
-    pass
-
-
-ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "ChannelConfiguration": str,
-        "Codec": str,
-        "Duration": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "Codec": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-M2tsSettingsTypeDef = TypedDict(
-    "M2tsSettingsTypeDef",
+M2tsSettingsOutputTypeDef = TypedDict(
+    "M2tsSettingsOutputTypeDef",
     {
         "AbsentInputAudioBehavior": M2tsAbsentInputAudioBehaviorType,
         "Arib": M2tsAribType,
         "AribCaptionsPid": str,
         "AribCaptionsPidControl": M2tsAribCaptionsPidControlType,
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "AudioStreamType": M2tsAudioStreamTypeType,
         "Bitrate": int,
         "BufferModel": M2tsBufferModelType,
         "CcDescriptor": M2tsCcDescriptorType,
-        "DvbNitSettings": DvbNitSettingsTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsTypeDef,
+        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
         "DvbSubPids": str,
-        "DvbTdtSettings": DvbTdtSettingsTypeDef,
+        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
         "DvbTeletextPid": str,
         "Ebif": M2tsEbifControlType,
         "EbpAudioInterval": M2tsAudioIntervalType,
         "EbpLookaheadMs": int,
         "EbpPlacement": M2tsEbpPlacementType,
         "EcmPid": str,
         "EsRateInPes": M2tsEsRateInPesType,
@@ -3604,52 +4823,114 @@
         "TransportStreamId": int,
         "VideoPid": str,
         "Scte35PrerollPullupMilliseconds": float,
     },
     total=False,
 )
 
+FailoverConditionSettingsOutputTypeDef = TypedDict(
+    "FailoverConditionSettingsOutputTypeDef",
+    {
+        "AudioSilenceSettings": AudioSilenceFailoverSettingsOutputTypeDef,
+        "InputLossSettings": InputLossFailoverSettingsOutputTypeDef,
+        "VideoBlackSettings": VideoBlackFailoverSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": AudioSilenceFailoverSettingsTypeDef,
         "InputLossSettings": InputLossFailoverSettingsTypeDef,
         "VideoBlackSettings": VideoBlackFailoverSettingsTypeDef,
     },
     total=False,
 )
 
+ScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionStartSettingsOutputTypeDef",
+    {
+        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsOutputTypeDef,
+        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsOutputTypeDef,
+        "ImmediateModeScheduleActionStartSettings": Dict[str, Any],
+    },
+    total=False,
+)
+
 ScheduleActionStartSettingsTypeDef = TypedDict(
     "ScheduleActionStartSettingsTypeDef",
     {
         "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
         "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Mapping[str, Any],
     },
     total=False,
 )
 
+FrameCaptureCdnSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureCdnSettingsOutputTypeDef",
+    {
+        "FrameCaptureS3Settings": FrameCaptureS3SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 FrameCaptureCdnSettingsTypeDef = TypedDict(
     "FrameCaptureCdnSettingsTypeDef",
     {
         "FrameCaptureS3Settings": FrameCaptureS3SettingsTypeDef,
     },
     total=False,
 )
 
+FrameCaptureSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureSettingsOutputTypeDef",
+    {
+        "CaptureInterval": int,
+        "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "CaptureInterval": int,
         "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
+H264FilterSettingsOutputTypeDef = TypedDict(
+    "H264FilterSettingsOutputTypeDef",
+    {
+        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+H265FilterSettingsOutputTypeDef = TypedDict(
+    "H265FilterSettingsOutputTypeDef",
+    {
+        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+Mpeg2FilterSettingsOutputTypeDef = TypedDict(
+    "Mpeg2FilterSettingsOutputTypeDef",
+    {
+        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 H264FilterSettingsTypeDef = TypedDict(
     "H264FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
@@ -3666,14 +4947,34 @@
     "Mpeg2FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
 
+H265ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H265ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": Dict[str, Any],
+        "DolbyVision81Settings": Dict[str, Any],
+        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
+        "Rec601Settings": Dict[str, Any],
+        "Rec709Settings": Dict[str, Any],
+    },
+    total=False,
+)
+
+VideoSelectorColorSpaceSettingsOutputTypeDef = TypedDict(
+    "VideoSelectorColorSpaceSettingsOutputTypeDef",
+    {
+        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "DolbyVision81Settings": Mapping[str, Any],
         "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Mapping[str, Any],
@@ -3686,35 +4987,78 @@
     "VideoSelectorColorSpaceSettingsTypeDef",
     {
         "Hdr10Settings": Hdr10SettingsTypeDef,
     },
     total=False,
 )
 
+HlsCdnSettingsOutputTypeDef = TypedDict(
+    "HlsCdnSettingsOutputTypeDef",
+    {
+        "HlsAkamaiSettings": HlsAkamaiSettingsOutputTypeDef,
+        "HlsBasicPutSettings": HlsBasicPutSettingsOutputTypeDef,
+        "HlsMediaStoreSettings": HlsMediaStoreSettingsOutputTypeDef,
+        "HlsS3Settings": HlsS3SettingsOutputTypeDef,
+        "HlsWebdavSettings": HlsWebdavSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 HlsCdnSettingsTypeDef = TypedDict(
     "HlsCdnSettingsTypeDef",
     {
         "HlsAkamaiSettings": HlsAkamaiSettingsTypeDef,
         "HlsBasicPutSettings": HlsBasicPutSettingsTypeDef,
         "HlsMediaStoreSettings": HlsMediaStoreSettingsTypeDef,
         "HlsS3Settings": HlsS3SettingsTypeDef,
         "HlsWebdavSettings": HlsWebdavSettingsTypeDef,
     },
     total=False,
 )
 
+NetworkInputSettingsOutputTypeDef = TypedDict(
+    "NetworkInputSettingsOutputTypeDef",
+    {
+        "HlsInputSettings": HlsInputSettingsOutputTypeDef,
+        "ServerValidation": NetworkInputServerValidationType,
+    },
+    total=False,
+)
+
 NetworkInputSettingsTypeDef = TypedDict(
     "NetworkInputSettingsTypeDef",
     {
         "HlsInputSettings": HlsInputSettingsTypeDef,
         "ServerValidation": NetworkInputServerValidationType,
     },
     total=False,
 )
 
+_RequiredInputClippingSettingsOutputTypeDef = TypedDict(
+    "_RequiredInputClippingSettingsOutputTypeDef",
+    {
+        "InputTimecodeSource": InputTimecodeSourceType,
+    },
+)
+_OptionalInputClippingSettingsOutputTypeDef = TypedDict(
+    "_OptionalInputClippingSettingsOutputTypeDef",
+    {
+        "StartTimecode": StartTimecodeOutputTypeDef,
+        "StopTimecode": StopTimecodeOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class InputClippingSettingsOutputTypeDef(
+    _RequiredInputClippingSettingsOutputTypeDef, _OptionalInputClippingSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredInputClippingSettingsTypeDef = TypedDict(
     "_RequiredInputClippingSettingsTypeDef",
     {
         "InputTimecodeSource": InputTimecodeSourceType,
     },
 )
 _OptionalInputClippingSettingsTypeDef = TypedDict(
@@ -3795,44 +5139,66 @@
 
 
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStandardHlsSettingsTypeDef = TypedDict(
-    "_RequiredStandardHlsSettingsTypeDef",
+_RequiredStandardHlsSettingsOutputTypeDef = TypedDict(
+    "_RequiredStandardHlsSettingsOutputTypeDef",
     {
-        "M3u8Settings": M3u8SettingsTypeDef,
+        "M3u8Settings": M3u8SettingsOutputTypeDef,
     },
 )
-_OptionalStandardHlsSettingsTypeDef = TypedDict(
-    "_OptionalStandardHlsSettingsTypeDef",
+_OptionalStandardHlsSettingsOutputTypeDef = TypedDict(
+    "_OptionalStandardHlsSettingsOutputTypeDef",
     {
         "AudioRenditionSets": str,
     },
     total=False,
 )
 
 
-class StandardHlsSettingsTypeDef(
-    _RequiredStandardHlsSettingsTypeDef, _OptionalStandardHlsSettingsTypeDef
+class StandardHlsSettingsOutputTypeDef(
+    _RequiredStandardHlsSettingsOutputTypeDef, _OptionalStandardHlsSettingsOutputTypeDef
+):
+    pass
+
+
+_RequiredMotionGraphicsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredMotionGraphicsConfigurationOutputTypeDef",
+    {
+        "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
+    },
+)
+_OptionalMotionGraphicsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalMotionGraphicsConfigurationOutputTypeDef",
+    {
+        "MotionGraphicsInsertion": MotionGraphicsInsertionType,
+    },
+    total=False,
+)
+
+
+class MotionGraphicsConfigurationOutputTypeDef(
+    _RequiredMotionGraphicsConfigurationOutputTypeDef,
+    _OptionalMotionGraphicsConfigurationOutputTypeDef,
 ):
     pass
 
 
 _RequiredMotionGraphicsConfigurationTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationTypeDef",
     {
@@ -3874,52 +5240,169 @@
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+MultiplexVideoSettingsOutputTypeDef = TypedDict(
+    "MultiplexVideoSettingsOutputTypeDef",
+    {
+        "ConstantBitrate": int,
+        "StatmuxSettings": MultiplexStatmuxVideoSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 MultiplexVideoSettingsTypeDef = TypedDict(
     "MultiplexVideoSettingsTypeDef",
     {
         "ConstantBitrate": int,
         "StatmuxSettings": MultiplexStatmuxVideoSettingsTypeDef,
     },
     total=False,
 )
 
+NielsenWatermarksSettingsOutputTypeDef = TypedDict(
+    "NielsenWatermarksSettingsOutputTypeDef",
+    {
+        "NielsenCbetSettings": NielsenCBETOutputTypeDef,
+        "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
+        "NielsenNaesIiNwSettings": NielsenNaesIiNwOutputTypeDef,
+    },
+    total=False,
+)
+
 NielsenWatermarksSettingsTypeDef = TypedDict(
     "NielsenWatermarksSettingsTypeDef",
     {
         "NielsenCbetSettings": NielsenCBETTypeDef,
         "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
         "NielsenNaesIiNwSettings": NielsenNaesIiNwTypeDef,
     },
     total=False,
 )
 
+OutputDestinationOutputTypeDef = TypedDict(
+    "OutputDestinationOutputTypeDef",
+    {
+        "Id": str,
+        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsOutputTypeDef],
+        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsOutputTypeDef,
+        "Settings": List[OutputDestinationSettingsOutputTypeDef],
+    },
+    total=False,
+)
+
 OutputDestinationTypeDef = TypedDict(
     "OutputDestinationTypeDef",
     {
         "Id": str,
         "MediaPackageSettings": Sequence[MediaPackageOutputDestinationSettingsTypeDef],
         "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
         "Settings": Sequence[OutputDestinationSettingsTypeDef],
     },
     total=False,
 )
 
+PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "PauseStateScheduleActionSettingsOutputTypeDef",
+    {
+        "Pipelines": List[PipelinePauseStateSettingsOutputTypeDef],
+    },
+    total=False,
+)
+
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
         "Pipelines": Sequence[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
 
+_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_RequiredPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Count": int,
+        "OfferingId": str,
+    },
+)
+_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_OptionalPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+        "RequestId": str,
+        "Start": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class PurchaseOfferingRequestRequestTypeDef(
+    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReservationRequestRequestTypeDef",
+    {
+        "ReservationId": str,
+    },
+)
+_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReservationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateReservationRequestRequestTypeDef(
+    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredScte35SegmentationDescriptorOutputTypeDef = TypedDict(
+    "_RequiredScte35SegmentationDescriptorOutputTypeDef",
+    {
+        "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
+        "SegmentationEventId": int,
+    },
+)
+_OptionalScte35SegmentationDescriptorOutputTypeDef = TypedDict(
+    "_OptionalScte35SegmentationDescriptorOutputTypeDef",
+    {
+        "DeliveryRestrictions": Scte35DeliveryRestrictionsOutputTypeDef,
+        "SegmentNum": int,
+        "SegmentationDuration": int,
+        "SegmentationTypeId": int,
+        "SegmentationUpid": str,
+        "SegmentationUpidType": int,
+        "SegmentsExpected": int,
+        "SubSegmentNum": int,
+        "SubSegmentsExpected": int,
+    },
+    total=False,
+)
+
+
+class Scte35SegmentationDescriptorOutputTypeDef(
+    _RequiredScte35SegmentationDescriptorOutputTypeDef,
+    _OptionalScte35SegmentationDescriptorOutputTypeDef,
+):
+    pass
+
+
 _RequiredScte35SegmentationDescriptorTypeDef = TypedDict(
     "_RequiredScte35SegmentationDescriptorTypeDef",
     {
         "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
         "SegmentationEventId": int,
     },
 )
@@ -3951,23 +5434,54 @@
     {
         "PipelineId": str,
         "Thumbnails": List[ThumbnailTypeDef],
     },
     total=False,
 )
 
+VideoSelectorSettingsOutputTypeDef = TypedDict(
+    "VideoSelectorSettingsOutputTypeDef",
+    {
+        "VideoSelectorPid": VideoSelectorPidOutputTypeDef,
+        "VideoSelectorProgramId": VideoSelectorProgramIdOutputTypeDef,
+    },
+    total=False,
+)
+
 VideoSelectorSettingsTypeDef = TypedDict(
     "VideoSelectorSettingsTypeDef",
     {
         "VideoSelectorPid": VideoSelectorPidTypeDef,
         "VideoSelectorProgramId": VideoSelectorProgramIdTypeDef,
     },
     total=False,
 )
 
+_RequiredArchiveGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredArchiveGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalArchiveGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalArchiveGroupSettingsOutputTypeDef",
+    {
+        "ArchiveCdnSettings": ArchiveCdnSettingsOutputTypeDef,
+        "RolloverInterval": int,
+    },
+    total=False,
+)
+
+
+class ArchiveGroupSettingsOutputTypeDef(
+    _RequiredArchiveGroupSettingsOutputTypeDef, _OptionalArchiveGroupSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredArchiveGroupSettingsTypeDef = TypedDict(
     "_RequiredArchiveGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalArchiveGroupSettingsTypeDef = TypedDict(
@@ -3982,14 +5496,36 @@
 
 class ArchiveGroupSettingsTypeDef(
     _RequiredArchiveGroupSettingsTypeDef, _OptionalArchiveGroupSettingsTypeDef
 ):
     pass
 
 
+_RequiredRemixSettingsOutputTypeDef = TypedDict(
+    "_RequiredRemixSettingsOutputTypeDef",
+    {
+        "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
+    },
+)
+_OptionalRemixSettingsOutputTypeDef = TypedDict(
+    "_OptionalRemixSettingsOutputTypeDef",
+    {
+        "ChannelsIn": int,
+        "ChannelsOut": int,
+    },
+    total=False,
+)
+
+
+class RemixSettingsOutputTypeDef(
+    _RequiredRemixSettingsOutputTypeDef, _OptionalRemixSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredRemixSettingsTypeDef = TypedDict(
     "_RequiredRemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
     },
 )
 _OptionalRemixSettingsTypeDef = TypedDict(
@@ -4002,14 +5538,77 @@
 )
 
 
 class RemixSettingsTypeDef(_RequiredRemixSettingsTypeDef, _OptionalRemixSettingsTypeDef):
     pass
 
 
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "AribDestinationSettings": Dict[str, Any],
+        "BurnInDestinationSettings": BurnInDestinationSettingsOutputTypeDef,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
+        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsOutputTypeDef,
+        "EmbeddedDestinationSettings": Dict[str, Any],
+        "EmbeddedPlusScte20DestinationSettings": Dict[str, Any],
+        "RtmpCaptionInfoDestinationSettings": Dict[str, Any],
+        "Scte20PlusEmbeddedDestinationSettings": Dict[str, Any],
+        "Scte27DestinationSettings": Dict[str, Any],
+        "SmpteTtDestinationSettings": Dict[str, Any],
+        "TeletextDestinationSettings": Dict[str, Any],
+        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+GlobalConfigurationOutputTypeDef = TypedDict(
+    "GlobalConfigurationOutputTypeDef",
+    {
+        "InitialAudioGain": int,
+        "InputEndAction": GlobalConfigurationInputEndActionType,
+        "InputLossBehavior": InputLossBehaviorOutputTypeDef,
+        "OutputLockingMode": GlobalConfigurationOutputLockingModeType,
+        "OutputTimingSource": GlobalConfigurationOutputTimingSourceType,
+        "SupportLowFramerateInputs": GlobalConfigurationLowFramerateInputsType,
+    },
+    total=False,
+)
+
+KeyProviderSettingsOutputTypeDef = TypedDict(
+    "KeyProviderSettingsOutputTypeDef",
+    {
+        "StaticKeySettings": StaticKeySettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+AudioSelectorSettingsOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsOutputTypeDef",
+    {
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionOutputTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionOutputTypeDef,
+        "AudioPidSelection": AudioPidSelectionOutputTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+AudioSelectorSettingsTypeDef = TypedDict(
+    "AudioSelectorSettingsTypeDef",
+    {
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
+        "AudioPidSelection": AudioPidSelectionTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionTypeDef,
+    },
+    total=False,
+)
+
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "AribDestinationSettings": Mapping[str, Any],
         "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
@@ -4043,33 +5642,44 @@
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": StaticKeySettingsTypeDef,
     },
     total=False,
 )
 
-AudioSelectorSettingsTypeDef = TypedDict(
-    "AudioSelectorSettingsTypeDef",
+AvailConfigurationOutputTypeDef = TypedDict(
+    "AvailConfigurationOutputTypeDef",
     {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
-        "AudioPidSelection": AudioPidSelectionTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionTypeDef,
+        "AvailSettings": AvailSettingsOutputTypeDef,
     },
     total=False,
 )
 
 AvailConfigurationTypeDef = TypedDict(
     "AvailConfigurationTypeDef",
     {
         "AvailSettings": AvailSettingsTypeDef,
     },
     total=False,
 )
 
+CaptionSelectorSettingsOutputTypeDef = TypedDict(
+    "CaptionSelectorSettingsOutputTypeDef",
+    {
+        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "AribSourceSettings": Dict[str, Any],
+        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
+        "Scte20SourceSettings": Scte20SourceSettingsOutputTypeDef,
+        "Scte27SourceSettings": Scte27SourceSettingsOutputTypeDef,
+        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 CaptionSelectorSettingsTypeDef = TypedDict(
     "CaptionSelectorSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "AribSourceSettings": Mapping[str, Any],
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
         "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
@@ -4081,102 +5691,131 @@
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReservationResponseTypeDef = TypedDict(
     "UpdateReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInputSecurityGroupResponseTypeDef = TypedDict(
     "CreateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ArchiveContainerSettingsTypeDef = TypedDict(
-    "ArchiveContainerSettingsTypeDef",
+ArchiveContainerSettingsOutputTypeDef = TypedDict(
+    "ArchiveContainerSettingsOutputTypeDef",
     {
-        "M2tsSettings": M2tsSettingsTypeDef,
-        "RawSettings": Mapping[str, Any],
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
+        "RawSettings": Dict[str, Any],
     },
     total=False,
 )
 
-UdpContainerSettingsTypeDef = TypedDict(
-    "UdpContainerSettingsTypeDef",
+UdpContainerSettingsOutputTypeDef = TypedDict(
+    "UdpContainerSettingsOutputTypeDef",
     {
-        "M2tsSettings": M2tsSettingsTypeDef,
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+FailoverConditionOutputTypeDef = TypedDict(
+    "FailoverConditionOutputTypeDef",
+    {
+        "FailoverConditionSettings": FailoverConditionSettingsOutputTypeDef,
     },
     total=False,
 )
 
 FailoverConditionTypeDef = TypedDict(
     "FailoverConditionTypeDef",
     {
         "FailoverConditionSettings": FailoverConditionSettingsTypeDef,
     },
     total=False,
 )
 
+_RequiredFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredFrameCaptureGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalFrameCaptureGroupSettingsOutputTypeDef",
+    {
+        "FrameCaptureCdnSettings": FrameCaptureCdnSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FrameCaptureGroupSettingsOutputTypeDef(
+    _RequiredFrameCaptureGroupSettingsOutputTypeDef, _OptionalFrameCaptureGroupSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredFrameCaptureGroupSettingsTypeDef = TypedDict(
     "_RequiredFrameCaptureGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalFrameCaptureGroupSettingsTypeDef = TypedDict(
@@ -4190,14 +5829,99 @@
 
 class FrameCaptureGroupSettingsTypeDef(
     _RequiredFrameCaptureGroupSettingsTypeDef, _OptionalFrameCaptureGroupSettingsTypeDef
 ):
     pass
 
 
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H264AdaptiveQuantizationType,
+        "AfdSignaling": AfdSignalingType,
+        "Bitrate": int,
+        "BufFillPct": int,
+        "BufSize": int,
+        "ColorMetadata": H264ColorMetadataType,
+        "ColorSpaceSettings": H264ColorSpaceSettingsOutputTypeDef,
+        "EntropyEncoding": H264EntropyEncodingType,
+        "FilterSettings": H264FilterSettingsOutputTypeDef,
+        "FixedAfd": FixedAfdType,
+        "FlickerAq": H264FlickerAqType,
+        "ForceFieldPictures": H264ForceFieldPicturesType,
+        "FramerateControl": H264FramerateControlType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H264GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopNumBFrames": int,
+        "GopSize": float,
+        "GopSizeUnits": H264GopSizeUnitsType,
+        "Level": H264LevelType,
+        "LookAheadRateControl": H264LookAheadRateControlType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumRefFrames": int,
+        "ParControl": H264ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "Profile": H264ProfileType,
+        "QualityLevel": H264QualityLevelType,
+        "QvbrQualityLevel": int,
+        "RateControlMode": H264RateControlModeType,
+        "ScanType": H264ScanTypeType,
+        "SceneChangeDetect": H264SceneChangeDetectType,
+        "Slices": int,
+        "Softness": int,
+        "SpatialAq": H264SpatialAqType,
+        "SubgopLength": H264SubGopLengthType,
+        "Syntax": H264SyntaxType,
+        "TemporalAq": H264TemporalAqType,
+        "TimecodeInsertion": H264TimecodeInsertionBehaviorType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredMpeg2SettingsOutputTypeDef = TypedDict(
+    "_RequiredMpeg2SettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+_OptionalMpeg2SettingsOutputTypeDef = TypedDict(
+    "_OptionalMpeg2SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
+        "AfdSignaling": AfdSignalingType,
+        "ColorMetadata": Mpeg2ColorMetadataType,
+        "ColorSpace": Mpeg2ColorSpaceType,
+        "DisplayAspectRatio": Mpeg2DisplayRatioType,
+        "FilterSettings": Mpeg2FilterSettingsOutputTypeDef,
+        "FixedAfd": FixedAfdType,
+        "GopClosedCadence": int,
+        "GopNumBFrames": int,
+        "GopSize": float,
+        "GopSizeUnits": Mpeg2GopSizeUnitsType,
+        "ScanType": Mpeg2ScanTypeType,
+        "SubgopLength": Mpeg2SubGopLengthType,
+        "TimecodeInsertion": Mpeg2TimecodeInsertionBehaviorType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class Mpeg2SettingsOutputTypeDef(
+    _RequiredMpeg2SettingsOutputTypeDef, _OptionalMpeg2SettingsOutputTypeDef
+):
+    pass
+
+
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
@@ -4273,14 +5997,63 @@
 )
 
 
 class Mpeg2SettingsTypeDef(_RequiredMpeg2SettingsTypeDef, _OptionalMpeg2SettingsTypeDef):
     pass
 
 
+_RequiredH265SettingsOutputTypeDef = TypedDict(
+    "_RequiredH265SettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+_OptionalH265SettingsOutputTypeDef = TypedDict(
+    "_OptionalH265SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H265AdaptiveQuantizationType,
+        "AfdSignaling": AfdSignalingType,
+        "AlternativeTransferFunction": H265AlternativeTransferFunctionType,
+        "Bitrate": int,
+        "BufSize": int,
+        "ColorMetadata": H265ColorMetadataType,
+        "ColorSpaceSettings": H265ColorSpaceSettingsOutputTypeDef,
+        "FilterSettings": H265FilterSettingsOutputTypeDef,
+        "FixedAfd": FixedAfdType,
+        "FlickerAq": H265FlickerAqType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H265GopSizeUnitsType,
+        "Level": H265LevelType,
+        "LookAheadRateControl": H265LookAheadRateControlType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "Profile": H265ProfileType,
+        "QvbrQualityLevel": int,
+        "RateControlMode": H265RateControlModeType,
+        "ScanType": H265ScanTypeType,
+        "SceneChangeDetect": H265SceneChangeDetectType,
+        "Slices": int,
+        "Tier": H265TierType,
+        "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class H265SettingsOutputTypeDef(
+    _RequiredH265SettingsOutputTypeDef, _OptionalH265SettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredH265SettingsTypeDef = TypedDict(
     "_RequiredH265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -4320,14 +6093,47 @@
 )
 
 
 class H265SettingsTypeDef(_RequiredH265SettingsTypeDef, _OptionalH265SettingsTypeDef):
     pass
 
 
+InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "UrlPath": List[str],
+    },
+    total=False,
+)
+
+_RequiredInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredInputSwitchScheduleActionSettingsOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+    },
+)
+_OptionalInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalInputSwitchScheduleActionSettingsOutputTypeDef",
+    {
+        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "UrlPath": List[str],
+    },
+    total=False,
+)
+
+
+class InputSwitchScheduleActionSettingsOutputTypeDef(
+    _RequiredInputSwitchScheduleActionSettingsOutputTypeDef,
+    _OptionalInputSwitchScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
+
 InputPrepareScheduleActionSettingsTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
         "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": Sequence[str],
     },
@@ -4361,105 +6167,105 @@
     "DescribeInputResponseTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsTypeDef],
+        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsTypeDef],
+        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
     },
     total=False,
 )
 
-HlsSettingsTypeDef = TypedDict(
-    "HlsSettingsTypeDef",
+HlsSettingsOutputTypeDef = TypedDict(
+    "HlsSettingsOutputTypeDef",
     {
-        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsTypeDef,
-        "Fmp4HlsSettings": Fmp4HlsSettingsTypeDef,
-        "FrameCaptureHlsSettings": Mapping[str, Any],
-        "StandardHlsSettings": StandardHlsSettingsTypeDef,
+        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsOutputTypeDef,
+        "Fmp4HlsSettings": Fmp4HlsSettingsOutputTypeDef,
+        "FrameCaptureHlsSettings": Dict[str, Any],
+        "StandardHlsSettings": StandardHlsSettingsOutputTypeDef,
     },
     total=False,
 )
 
 DeleteMultiplexResponseTypeDef = TypedDict(
     "DeleteMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexResponseTypeDef = TypedDict(
     "DescribeMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexTypeDef = TypedDict(
     "MultiplexTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
@@ -4468,50 +6274,73 @@
 StartMultiplexResponseTypeDef = TypedDict(
     "StartMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopMultiplexResponseTypeDef = TypedDict(
     "StopMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredMultiplexProgramSettingsOutputTypeDef = TypedDict(
+    "_RequiredMultiplexProgramSettingsOutputTypeDef",
+    {
+        "ProgramNumber": int,
+    },
+)
+_OptionalMultiplexProgramSettingsOutputTypeDef = TypedDict(
+    "_OptionalMultiplexProgramSettingsOutputTypeDef",
+    {
+        "PreferredChannelPipeline": PreferredChannelPipelineType,
+        "ServiceDescriptor": MultiplexProgramServiceDescriptorOutputTypeDef,
+        "VideoSettings": MultiplexVideoSettingsOutputTypeDef,
     },
+    total=False,
 )
 
+
+class MultiplexProgramSettingsOutputTypeDef(
+    _RequiredMultiplexProgramSettingsOutputTypeDef, _OptionalMultiplexProgramSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredMultiplexProgramSettingsTypeDef = TypedDict(
     "_RequiredMultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
     },
 )
 _OptionalMultiplexProgramSettingsTypeDef = TypedDict(
@@ -4527,14 +6356,22 @@
 
 class MultiplexProgramSettingsTypeDef(
     _RequiredMultiplexProgramSettingsTypeDef, _OptionalMultiplexProgramSettingsTypeDef
 ):
     pass
 
 
+AudioWatermarkSettingsOutputTypeDef = TypedDict(
+    "AudioWatermarkSettingsOutputTypeDef",
+    {
+        "NielsenWatermarksSettings": NielsenWatermarksSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AudioWatermarkSettingsTypeDef = TypedDict(
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
 )
@@ -4558,40 +6395,185 @@
 class UpdateChannelClassRequestRequestTypeDef(
     _RequiredUpdateChannelClassRequestRequestTypeDef,
     _OptionalUpdateChannelClassRequestRequestTypeDef,
 ):
     pass
 
 
+Scte35DescriptorSettingsOutputTypeDef = TypedDict(
+    "Scte35DescriptorSettingsOutputTypeDef",
+    {
+        "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorOutputTypeDef,
+    },
+)
+
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
 DescribeThumbnailsResponseTypeDef = TypedDict(
     "DescribeThumbnailsResponseTypeDef",
     {
         "ThumbnailDetails": List[ThumbnailDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+VideoSelectorOutputTypeDef = TypedDict(
+    "VideoSelectorOutputTypeDef",
+    {
+        "ColorSpace": VideoSelectorColorSpaceType,
+        "ColorSpaceSettings": VideoSelectorColorSpaceSettingsOutputTypeDef,
+        "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
+        "SelectorSettings": VideoSelectorSettingsOutputTypeDef,
     },
+    total=False,
 )
 
 VideoSelectorTypeDef = TypedDict(
     "VideoSelectorTypeDef",
     {
         "ColorSpace": VideoSelectorColorSpaceType,
         "ColorSpaceSettings": VideoSelectorColorSpaceSettingsTypeDef,
         "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
         "SelectorSettings": VideoSelectorSettingsTypeDef,
     },
     total=False,
 )
 
+_RequiredCaptionDescriptionOutputTypeDef = TypedDict(
+    "_RequiredCaptionDescriptionOutputTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "Name": str,
+    },
+)
+_OptionalCaptionDescriptionOutputTypeDef = TypedDict(
+    "_OptionalCaptionDescriptionOutputTypeDef",
+    {
+        "Accessibility": AccessibilityTypeType,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": str,
+        "LanguageDescription": str,
+    },
+    total=False,
+)
+
+
+class CaptionDescriptionOutputTypeDef(
+    _RequiredCaptionDescriptionOutputTypeDef, _OptionalCaptionDescriptionOutputTypeDef
+):
+    pass
+
+
+_RequiredHlsGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredHlsGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalHlsGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalHlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "BaseUrlContent": str,
+        "BaseUrlContent1": str,
+        "BaseUrlManifest": str,
+        "BaseUrlManifest1": str,
+        "CaptionLanguageMappings": List[CaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "ConstantIv": str,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "DiscontinuityTags": HlsDiscontinuityTagsType,
+        "EncryptionType": HlsEncryptionTypeType,
+        "HlsCdnSettings": HlsCdnSettingsOutputTypeDef,
+        "HlsId3SegmentTagging": HlsId3SegmentTaggingStateType,
+        "IFrameOnlyPlaylists": IFrameOnlyPlaylistTypeType,
+        "IncompleteSegmentBehavior": HlsIncompleteSegmentBehaviorType,
+        "IndexNSegments": int,
+        "InputLossAction": InputLossActionForHlsOutType,
+        "IvInManifest": HlsIvInManifestType,
+        "IvSource": HlsIvSourceType,
+        "KeepSegments": int,
+        "KeyFormat": str,
+        "KeyFormatVersions": str,
+        "KeyProviderSettings": KeyProviderSettingsOutputTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinSegmentLength": int,
+        "Mode": HlsModeType,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimeClock": HlsProgramDateTimeClockType,
+        "ProgramDateTimePeriod": int,
+        "RedundantManifest": HlsRedundantManifestType,
+        "SegmentLength": int,
+        "SegmentationMode": HlsSegmentationModeType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+        "TsFileMode": HlsTsFileModeType,
+    },
+    total=False,
+)
+
+
+class HlsGroupSettingsOutputTypeDef(
+    _RequiredHlsGroupSettingsOutputTypeDef, _OptionalHlsGroupSettingsOutputTypeDef
+):
+    pass
+
+
+_RequiredAudioSelectorOutputTypeDef = TypedDict(
+    "_RequiredAudioSelectorOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorOutputTypeDef = TypedDict(
+    "_OptionalAudioSelectorOutputTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AudioSelectorOutputTypeDef(
+    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
+):
+    pass
+
+
+_RequiredAudioSelectorTypeDef = TypedDict(
+    "_RequiredAudioSelectorTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorTypeDef = TypedDict(
+    "_OptionalAudioSelectorTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
+    pass
+
+
 _RequiredCaptionDescriptionTypeDef = TypedDict(
     "_RequiredCaptionDescriptionTypeDef",
     {
         "CaptionSelectorName": str,
         "Name": str,
     },
 )
@@ -4669,30 +6651,33 @@
 )
 
 
 class HlsGroupSettingsTypeDef(_RequiredHlsGroupSettingsTypeDef, _OptionalHlsGroupSettingsTypeDef):
     pass
 
 
-_RequiredAudioSelectorTypeDef = TypedDict(
-    "_RequiredAudioSelectorTypeDef",
+_RequiredCaptionSelectorOutputTypeDef = TypedDict(
+    "_RequiredCaptionSelectorOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalAudioSelectorTypeDef = TypedDict(
-    "_OptionalAudioSelectorTypeDef",
+_OptionalCaptionSelectorOutputTypeDef = TypedDict(
+    "_OptionalCaptionSelectorOutputTypeDef",
     {
-        "SelectorSettings": AudioSelectorSettingsTypeDef,
+        "LanguageCode": str,
+        "SelectorSettings": CaptionSelectorSettingsOutputTypeDef,
     },
     total=False,
 )
 
 
-class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
+class CaptionSelectorOutputTypeDef(
+    _RequiredCaptionSelectorOutputTypeDef, _OptionalCaptionSelectorOutputTypeDef
+):
     pass
 
 
 _RequiredCaptionSelectorTypeDef = TypedDict(
     "_RequiredCaptionSelectorTypeDef",
     {
         "Name": str,
@@ -4708,55 +6693,79 @@
 )
 
 
 class CaptionSelectorTypeDef(_RequiredCaptionSelectorTypeDef, _OptionalCaptionSelectorTypeDef):
     pass
 
 
-_RequiredArchiveOutputSettingsTypeDef = TypedDict(
-    "_RequiredArchiveOutputSettingsTypeDef",
+_RequiredArchiveOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredArchiveOutputSettingsOutputTypeDef",
     {
-        "ContainerSettings": ArchiveContainerSettingsTypeDef,
+        "ContainerSettings": ArchiveContainerSettingsOutputTypeDef,
     },
 )
-_OptionalArchiveOutputSettingsTypeDef = TypedDict(
-    "_OptionalArchiveOutputSettingsTypeDef",
+_OptionalArchiveOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalArchiveOutputSettingsOutputTypeDef",
     {
         "Extension": str,
         "NameModifier": str,
     },
     total=False,
 )
 
 
-class ArchiveOutputSettingsTypeDef(
-    _RequiredArchiveOutputSettingsTypeDef, _OptionalArchiveOutputSettingsTypeDef
+class ArchiveOutputSettingsOutputTypeDef(
+    _RequiredArchiveOutputSettingsOutputTypeDef, _OptionalArchiveOutputSettingsOutputTypeDef
 ):
     pass
 
 
-_RequiredUdpOutputSettingsTypeDef = TypedDict(
-    "_RequiredUdpOutputSettingsTypeDef",
+_RequiredUdpOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredUdpOutputSettingsOutputTypeDef",
     {
-        "ContainerSettings": UdpContainerSettingsTypeDef,
-        "Destination": OutputLocationRefTypeDef,
+        "ContainerSettings": UdpContainerSettingsOutputTypeDef,
+        "Destination": OutputLocationRefOutputTypeDef,
     },
 )
-_OptionalUdpOutputSettingsTypeDef = TypedDict(
-    "_OptionalUdpOutputSettingsTypeDef",
+_OptionalUdpOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalUdpOutputSettingsOutputTypeDef",
     {
         "BufferMsec": int,
-        "FecOutputSettings": FecOutputSettingsTypeDef,
+        "FecOutputSettings": FecOutputSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class UdpOutputSettingsOutputTypeDef(
+    _RequiredUdpOutputSettingsOutputTypeDef, _OptionalUdpOutputSettingsOutputTypeDef
+):
+    pass
+
+
+_RequiredAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
+    "_RequiredAutomaticInputFailoverSettingsOutputTypeDef",
+    {
+        "SecondaryInputId": str,
+    },
+)
+_OptionalAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
+    "_OptionalAutomaticInputFailoverSettingsOutputTypeDef",
+    {
+        "ErrorClearTimeMsec": int,
+        "FailoverConditions": List[FailoverConditionOutputTypeDef],
+        "InputPreference": InputPreferenceType,
     },
     total=False,
 )
 
 
-class UdpOutputSettingsTypeDef(
-    _RequiredUdpOutputSettingsTypeDef, _OptionalUdpOutputSettingsTypeDef
+class AutomaticInputFailoverSettingsOutputTypeDef(
+    _RequiredAutomaticInputFailoverSettingsOutputTypeDef,
+    _OptionalAutomaticInputFailoverSettingsOutputTypeDef,
 ):
     pass
 
 
 _RequiredAutomaticInputFailoverSettingsTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsTypeDef",
     {
@@ -4776,14 +6785,25 @@
 
 class AutomaticInputFailoverSettingsTypeDef(
     _RequiredAutomaticInputFailoverSettingsTypeDef, _OptionalAutomaticInputFailoverSettingsTypeDef
 ):
     pass
 
 
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "H264Settings": H264SettingsOutputTypeDef,
+        "H265Settings": H265SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
         "H264Settings": H264SettingsTypeDef,
         "H265Settings": H265SettingsTypeDef,
         "Mpeg2Settings": Mpeg2SettingsTypeDef,
@@ -4791,128 +6811,128 @@
     total=False,
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePartnerInputResponseTypeDef = TypedDict(
     "CreatePartnerInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredHlsOutputSettingsTypeDef = TypedDict(
-    "_RequiredHlsOutputSettingsTypeDef",
+_RequiredHlsOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredHlsOutputSettingsOutputTypeDef",
     {
-        "HlsSettings": HlsSettingsTypeDef,
+        "HlsSettings": HlsSettingsOutputTypeDef,
     },
 )
-_OptionalHlsOutputSettingsTypeDef = TypedDict(
-    "_OptionalHlsOutputSettingsTypeDef",
+_OptionalHlsOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalHlsOutputSettingsOutputTypeDef",
     {
         "H265PackagingType": HlsH265PackagingTypeType,
         "NameModifier": str,
         "SegmentModifier": str,
     },
     total=False,
 )
 
 
-class HlsOutputSettingsTypeDef(
-    _RequiredHlsOutputSettingsTypeDef, _OptionalHlsOutputSettingsTypeDef
+class HlsOutputSettingsOutputTypeDef(
+    _RequiredHlsOutputSettingsOutputTypeDef, _OptionalHlsOutputSettingsOutputTypeDef
 ):
     pass
 
 
 CreateMultiplexResponseTypeDef = TypedDict(
     "CreateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexResponseTypeDef = TypedDict(
     "UpdateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
-    "CreateMultiplexProgramRequestRequestTypeDef",
-    {
-        "MultiplexId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
-        "ProgramName": str,
-        "RequestId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMultiplexProgramResponseTypeDef = TypedDict(
     "DeleteMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexProgramResponseTypeDef = TypedDict(
     "DescribeMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexProgramTypeDef = TypedDict(
     "MultiplexProgramTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
     },
     total=False,
 )
 
+CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
+    "CreateMultiplexProgramRequestRequestTypeDef",
+    {
+        "MultiplexId": str,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "ProgramName": str,
+        "RequestId": str,
+    },
+)
+
 _RequiredUpdateMultiplexProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
 )
@@ -4928,14 +6948,44 @@
 class UpdateMultiplexProgramRequestRequestTypeDef(
     _RequiredUpdateMultiplexProgramRequestRequestTypeDef,
     _OptionalUpdateMultiplexProgramRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredAudioDescriptionOutputTypeDef = TypedDict(
+    "_RequiredAudioDescriptionOutputTypeDef",
+    {
+        "AudioSelectorName": str,
+        "Name": str,
+    },
+)
+_OptionalAudioDescriptionOutputTypeDef = TypedDict(
+    "_OptionalAudioDescriptionOutputTypeDef",
+    {
+        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
+        "AudioType": AudioTypeType,
+        "AudioTypeControl": AudioDescriptionAudioTypeControlType,
+        "AudioWatermarkingSettings": AudioWatermarkSettingsOutputTypeDef,
+        "CodecSettings": AudioCodecSettingsOutputTypeDef,
+        "LanguageCode": str,
+        "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "StreamName": str,
+    },
+    total=False,
+)
+
+
+class AudioDescriptionOutputTypeDef(
+    _RequiredAudioDescriptionOutputTypeDef, _OptionalAudioDescriptionOutputTypeDef
+):
+    pass
+
+
 _RequiredAudioDescriptionTypeDef = TypedDict(
     "_RequiredAudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
@@ -4956,21 +7006,43 @@
 )
 
 
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
 
+Scte35DescriptorOutputTypeDef = TypedDict(
+    "Scte35DescriptorOutputTypeDef",
+    {
+        "Scte35DescriptorSettings": Scte35DescriptorSettingsOutputTypeDef,
+    },
+)
+
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "ArchiveGroupSettings": ArchiveGroupSettingsOutputTypeDef,
+        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsOutputTypeDef,
+        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
+        "MediaPackageGroupSettings": MediaPackageGroupSettingsOutputTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "MultiplexGroupSettings": Dict[str, Any],
+        "RtmpGroupSettings": RtmpGroupSettingsOutputTypeDef,
+        "UdpGroupSettings": UdpGroupSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
         "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
@@ -4978,14 +7050,32 @@
         "MultiplexGroupSettings": Mapping[str, Any],
         "RtmpGroupSettings": RtmpGroupSettingsTypeDef,
         "UdpGroupSettings": UdpGroupSettingsTypeDef,
     },
     total=False,
 )
 
+InputSettingsOutputTypeDef = TypedDict(
+    "InputSettingsOutputTypeDef",
+    {
+        "AudioSelectors": List[AudioSelectorOutputTypeDef],
+        "CaptionSelectors": List[CaptionSelectorOutputTypeDef],
+        "DeblockFilter": InputDeblockFilterType,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "FilterStrength": int,
+        "InputFilter": InputFilterType,
+        "NetworkInputSettings": NetworkInputSettingsOutputTypeDef,
+        "Scte35Pid": int,
+        "Smpte2038DataPreference": Smpte2038DataPreferenceType,
+        "SourceEndBehavior": InputSourceEndBehaviorType,
+        "VideoSelector": VideoSelectorOutputTypeDef,
+    },
+    total=False,
+)
+
 InputSettingsTypeDef = TypedDict(
     "InputSettingsTypeDef",
     {
         "AudioSelectors": Sequence[AudioSelectorTypeDef],
         "CaptionSelectors": Sequence[CaptionSelectorTypeDef],
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
@@ -4996,14 +7086,40 @@
         "Smpte2038DataPreference": Smpte2038DataPreferenceType,
         "SourceEndBehavior": InputSourceEndBehaviorType,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
+_RequiredVideoDescriptionOutputTypeDef = TypedDict(
+    "_RequiredVideoDescriptionOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalVideoDescriptionOutputTypeDef = TypedDict(
+    "_OptionalVideoDescriptionOutputTypeDef",
+    {
+        "CodecSettings": VideoCodecSettingsOutputTypeDef,
+        "Height": int,
+        "RespondToAfd": VideoDescriptionRespondToAfdType,
+        "ScalingBehavior": VideoDescriptionScalingBehaviorType,
+        "Sharpness": int,
+        "Width": int,
+    },
+    total=False,
+)
+
+
+class VideoDescriptionOutputTypeDef(
+    _RequiredVideoDescriptionOutputTypeDef, _OptionalVideoDescriptionOutputTypeDef
+):
+    pass
+
+
 _RequiredVideoDescriptionTypeDef = TypedDict(
     "_RequiredVideoDescriptionTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVideoDescriptionTypeDef = TypedDict(
@@ -5020,85 +7136,125 @@
 )
 
 
 class VideoDescriptionTypeDef(_RequiredVideoDescriptionTypeDef, _OptionalVideoDescriptionTypeDef):
     pass
 
 
-OutputSettingsTypeDef = TypedDict(
-    "OutputSettingsTypeDef",
+OutputSettingsOutputTypeDef = TypedDict(
+    "OutputSettingsOutputTypeDef",
     {
-        "ArchiveOutputSettings": ArchiveOutputSettingsTypeDef,
-        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsTypeDef,
-        "HlsOutputSettings": HlsOutputSettingsTypeDef,
-        "MediaPackageOutputSettings": Mapping[str, Any],
-        "MsSmoothOutputSettings": MsSmoothOutputSettingsTypeDef,
-        "MultiplexOutputSettings": MultiplexOutputSettingsTypeDef,
-        "RtmpOutputSettings": RtmpOutputSettingsTypeDef,
-        "UdpOutputSettings": UdpOutputSettingsTypeDef,
+        "ArchiveOutputSettings": ArchiveOutputSettingsOutputTypeDef,
+        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsOutputTypeDef,
+        "HlsOutputSettings": HlsOutputSettingsOutputTypeDef,
+        "MediaPackageOutputSettings": Dict[str, Any],
+        "MsSmoothOutputSettings": MsSmoothOutputSettingsOutputTypeDef,
+        "MultiplexOutputSettings": MultiplexOutputSettingsOutputTypeDef,
+        "RtmpOutputSettings": RtmpOutputSettingsOutputTypeDef,
+        "UdpOutputSettings": UdpOutputSettingsOutputTypeDef,
     },
     total=False,
 )
 
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
+    {
+        "Scte35Descriptors": List[Scte35DescriptorOutputTypeDef],
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
     },
 )
 
+InputAttachmentOutputTypeDef = TypedDict(
+    "InputAttachmentOutputTypeDef",
+    {
+        "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsOutputTypeDef,
+        "InputAttachmentName": str,
+        "InputId": str,
+        "InputSettings": InputSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 InputAttachmentTypeDef = TypedDict(
     "InputAttachmentTypeDef",
     {
         "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsTypeDef,
         "InputAttachmentName": str,
         "InputId": str,
         "InputSettings": InputSettingsTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
-        "OutputSettings": OutputSettingsTypeDef,
+        "OutputSettings": OutputSettingsOutputTypeDef,
     },
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
-        "AudioDescriptionNames": Sequence[str],
-        "CaptionDescriptionNames": Sequence[str],
+        "AudioDescriptionNames": List[str],
+        "CaptionDescriptionNames": List[str],
         "OutputName": str,
         "VideoDescriptionName": str,
     },
     total=False,
 )
 
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
 
+ScheduleActionSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionSettingsOutputTypeDef",
+    {
+        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
+        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
+        "InputPrepareSettings": InputPrepareScheduleActionSettingsOutputTypeDef,
+        "InputSwitchSettings": InputSwitchScheduleActionSettingsOutputTypeDef,
+        "MotionGraphicsImageActivateSettings": (
+            MotionGraphicsActivateScheduleActionSettingsOutputTypeDef
+        ),
+        "MotionGraphicsImageDeactivateSettings": Dict[str, Any],
+        "PauseStateSettings": PauseStateScheduleActionSettingsOutputTypeDef,
+        "Scte35InputSettings": Scte35InputScheduleActionSettingsOutputTypeDef,
+        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
+        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+        "Scte35TimeSignalSettings": Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
+        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsOutputTypeDef,
+        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
         "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
         "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
         "InputPrepareSettings": InputPrepareScheduleActionSettingsTypeDef,
         "InputSwitchSettings": InputSwitchScheduleActionSettingsTypeDef,
@@ -5115,33 +7271,55 @@
     total=False,
 )
 
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
+_RequiredOutputGroupOutputTypeDef = TypedDict(
+    "_RequiredOutputGroupOutputTypeDef",
+    {
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
+    },
+)
+_OptionalOutputGroupOutputTypeDef = TypedDict(
+    "_OptionalOutputGroupOutputTypeDef",
+    {
+        "Name": str,
+    },
+    total=False,
+)
+
+
+class OutputGroupOutputTypeDef(
+    _RequiredOutputGroupOutputTypeDef, _OptionalOutputGroupOutputTypeDef
+):
+    pass
+
+
 _RequiredOutputGroupTypeDef = TypedDict(
     "_RequiredOutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
 )
@@ -5154,32 +7332,73 @@
 )
 
 
 class OutputGroupTypeDef(_RequiredOutputGroupTypeDef, _OptionalOutputGroupTypeDef):
     pass
 
 
+ScheduleActionOutputTypeDef = TypedDict(
+    "ScheduleActionOutputTypeDef",
+    {
+        "ActionName": str,
+        "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
+        "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
+    },
+)
+
 ScheduleActionTypeDef = TypedDict(
     "ScheduleActionTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEncoderSettingsOutputTypeDef = TypedDict(
+    "_RequiredEncoderSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
+    },
+)
+_OptionalEncoderSettingsOutputTypeDef = TypedDict(
+    "_OptionalEncoderSettingsOutputTypeDef",
+    {
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "AvailConfiguration": AvailConfigurationOutputTypeDef,
+        "BlackoutSlate": BlackoutSlateOutputTypeDef,
+        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
+        "FeatureActivations": FeatureActivationsOutputTypeDef,
+        "GlobalConfiguration": GlobalConfigurationOutputTypeDef,
+        "MotionGraphicsConfiguration": MotionGraphicsConfigurationOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "ThumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EncoderSettingsOutputTypeDef(
+    _RequiredEncoderSettingsOutputTypeDef, _OptionalEncoderSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": Sequence[VideoDescriptionTypeDef],
@@ -5202,188 +7421,188 @@
 )
 
 
 class EncoderSettingsTypeDef(_RequiredEncoderSettingsTypeDef, _OptionalEncoderSettingsTypeDef):
     pass
 
 
-BatchScheduleActionCreateRequestTypeDef = TypedDict(
-    "BatchScheduleActionCreateRequestTypeDef",
-    {
-        "ScheduleActions": Sequence[ScheduleActionTypeDef],
-    },
-)
-
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 
 BatchScheduleActionDeleteResultTypeDef = TypedDict(
     "BatchScheduleActionDeleteResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
-        "ScheduleActions": List[ScheduleActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchScheduleActionCreateRequestTypeDef = TypedDict(
+    "BatchScheduleActionCreateRequestTypeDef",
+    {
+        "ScheduleActions": Sequence[ScheduleActionTypeDef],
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
-CreateChannelRequestRequestTypeDef = TypedDict(
-    "CreateChannelRequestRequestTypeDef",
-    {
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[OutputDestinationTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
-        "LogLevel": LogLevelType,
-        "Maintenance": MaintenanceCreateSettingsTypeDef,
-        "Name": str,
-        "RequestId": str,
-        "Reserved": str,
-        "RoleArn": str,
-        "Tags": Mapping[str, str],
-        "Vpc": VpcOutputSettingsTypeDef,
-    },
-    total=False,
-)
-
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateChannelRequestRequestTypeDef = TypedDict(
+    "CreateChannelRequestRequestTypeDef",
+    {
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "ChannelClass": ChannelClassType,
+        "Destinations": Sequence[OutputDestinationTypeDef],
+        "EncoderSettings": EncoderSettingsTypeDef,
+        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputSpecification": InputSpecificationTypeDef,
+        "LogLevel": LogLevelType,
+        "Maintenance": MaintenanceCreateSettingsTypeDef,
+        "Name": str,
+        "RequestId": str,
+        "Reserved": str,
+        "RoleArn": str,
+        "Tags": Mapping[str, str],
+        "Vpc": VpcOutputSettingsTypeDef,
     },
+    total=False,
 )
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
@@ -5407,14 +7626,23 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
+BatchUpdateScheduleResponseTypeDef = TypedDict(
+    "BatchUpdateScheduleResponseTypeDef",
+    {
+        "Creates": BatchScheduleActionCreateResultTypeDef,
+        "Deletes": BatchScheduleActionDeleteResultTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
@@ -5430,39 +7658,30 @@
 class BatchUpdateScheduleRequestRequestTypeDef(
     _RequiredBatchUpdateScheduleRequestRequestTypeDef,
     _OptionalBatchUpdateScheduleRequestRequestTypeDef,
 ):
     pass
 
 
-BatchUpdateScheduleResponseTypeDef = TypedDict(
-    "BatchUpdateScheduleResponseTypeDef",
-    {
-        "Creates": BatchScheduleActionCreateResultTypeDef,
-        "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelClassResponseTypeDef = TypedDict(
     "UpdateChannelClassResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for medialive service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
+    from mypy_boto3_medialive.type_defs import AacSettingsOutputTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from botocore.response import StreamingBody
@@ -286,61 +286,93 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
+    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
     "AcceptInputDeviceTransferRequestRequestTypeDef",
+    "AccountConfigurationOutputTypeDef",
     "AccountConfigurationTypeDef",
+    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
+    "ArchiveS3SettingsOutputTypeDef",
     "ArchiveS3SettingsTypeDef",
+    "OutputLocationRefOutputTypeDef",
     "OutputLocationRefTypeDef",
+    "InputChannelLevelOutputTypeDef",
     "InputChannelLevelTypeDef",
+    "Eac3AtmosSettingsOutputTypeDef",
+    "Eac3SettingsOutputTypeDef",
+    "Mp2SettingsOutputTypeDef",
+    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "WavSettingsTypeDef",
+    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
+    "AudioDolbyEDecodeOutputTypeDef",
     "AudioDolbyEDecodeTypeDef",
+    "AudioHlsRenditionSelectionOutputTypeDef",
     "AudioHlsRenditionSelectionTypeDef",
+    "AudioLanguageSelectionOutputTypeDef",
     "AudioLanguageSelectionTypeDef",
-    "InputLocationTypeDef",
+    "InputLocationOutputTypeDef",
+    "AudioPidSelectionOutputTypeDef",
     "AudioPidSelectionTypeDef",
+    "AudioSilenceFailoverSettingsOutputTypeDef",
     "AudioSilenceFailoverSettingsTypeDef",
+    "AudioTrackOutputTypeDef",
     "AudioTrackTypeDef",
+    "InputLocationTypeDef",
+    "EsamOutputTypeDef",
+    "Scte35SpliceInsertOutputTypeDef",
+    "Scte35TimeSignalAposOutputTypeDef",
     "EsamTypeDef",
     "Scte35SpliceInsertTypeDef",
     "Scte35TimeSignalAposTypeDef",
     "BatchDeleteRequestRequestTypeDef",
     "BatchFailedResultModelTypeDef",
     "BatchSuccessfulResultModelTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchScheduleActionDeleteRequestTypeDef",
     "BatchStartRequestRequestTypeDef",
     "BatchStopRequestRequestTypeDef",
     "CancelInputDeviceTransferRequestRequestTypeDef",
+    "EbuTtDDestinationSettingsOutputTypeDef",
+    "TtmlDestinationSettingsOutputTypeDef",
+    "WebvttDestinationSettingsOutputTypeDef",
     "EbuTtDDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
+    "CaptionLanguageMappingOutputTypeDef",
     "CaptionLanguageMappingTypeDef",
+    "CaptionRectangleOutputTypeDef",
     "CaptionRectangleTypeDef",
+    "DvbSubSourceSettingsOutputTypeDef",
+    "EmbeddedSourceSettingsOutputTypeDef",
+    "Scte20SourceSettingsOutputTypeDef",
+    "Scte27SourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "Scte20SourceSettingsTypeDef",
     "Scte27SourceSettingsTypeDef",
+    "CdiInputSpecificationOutputTypeDef",
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
-    "InputSpecificationTypeDef",
+    "InputSpecificationOutputTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
+    "InputSpecificationTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
     "MediaConnectFlowRequestTypeDef",
@@ -351,149 +383,218 @@
     "DeleteChannelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DeleteInputSecurityGroupRequestRequestTypeDef",
     "DeleteMultiplexProgramRequestRequestTypeDef",
     "MultiplexProgramPacketIdentifiersMapTypeDef",
     "MultiplexProgramPipelineDetailTypeDef",
     "DeleteMultiplexRequestRequestTypeDef",
+    "MultiplexSettingsOutputTypeDef",
     "DeleteReservationRequestRequestTypeDef",
-    "RenewalSettingsTypeDef",
+    "RenewalSettingsOutputTypeDef",
     "ReservationResourceSpecificationTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
+    "DescribeInputDeviceThumbnailResponseTypeDef",
     "DescribeInputRequestRequestTypeDef",
+    "InputDeviceSettingsOutputTypeDef",
     "InputSourceTypeDef",
     "MediaConnectFlowTypeDef",
     "DescribeInputSecurityGroupRequestRequestTypeDef",
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DescribeThumbnailsRequestRequestTypeDef",
-    "DvbNitSettingsTypeDef",
-    "DvbSdtSettingsTypeDef",
-    "DvbTdtSettingsTypeDef",
+    "DvbNitSettingsOutputTypeDef",
+    "DvbSdtSettingsOutputTypeDef",
+    "DvbTdtSettingsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FeatureActivationsOutputTypeDef",
+    "NielsenConfigurationOutputTypeDef",
+    "ThumbnailConfigurationOutputTypeDef",
+    "TimecodeConfigOutputTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
+    "InputLossFailoverSettingsOutputTypeDef",
+    "VideoBlackFailoverSettingsOutputTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
-    "FecOutputSettingsTypeDef",
+    "FecOutputSettingsOutputTypeDef",
+    "FixedModeScheduleActionStartSettingsOutputTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
-    "Fmp4HlsSettingsTypeDef",
+    "Fmp4HlsSettingsOutputTypeDef",
+    "FollowModeScheduleActionStartSettingsOutputTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
+    "FrameCaptureS3SettingsOutputTypeDef",
     "FrameCaptureS3SettingsTypeDef",
-    "FrameCaptureOutputSettingsTypeDef",
+    "FrameCaptureOutputSettingsOutputTypeDef",
+    "TimecodeBurninSettingsOutputTypeDef",
     "TimecodeBurninSettingsTypeDef",
+    "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
+    "TemporalFilterSettingsOutputTypeDef",
     "TemporalFilterSettingsTypeDef",
+    "Hdr10SettingsOutputTypeDef",
     "Hdr10SettingsTypeDef",
+    "HlsAkamaiSettingsOutputTypeDef",
     "HlsAkamaiSettingsTypeDef",
+    "HlsBasicPutSettingsOutputTypeDef",
     "HlsBasicPutSettingsTypeDef",
+    "HlsMediaStoreSettingsOutputTypeDef",
+    "HlsS3SettingsOutputTypeDef",
+    "HlsWebdavSettingsOutputTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
     "HlsWebdavSettingsTypeDef",
+    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
+    "HlsInputSettingsOutputTypeDef",
     "HlsInputSettingsTypeDef",
+    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
+    "StartTimecodeOutputTypeDef",
+    "StopTimecodeOutputTypeDef",
     "StartTimecodeTypeDef",
     "StopTimecodeTypeDef",
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "InputDeviceRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
+    "ListInputsRequestListInputsPaginateTypeDef",
     "ListInputsRequestRequestTypeDef",
+    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "M3u8SettingsTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "M3u8SettingsOutputTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
+    "MediaPackageOutputDestinationSettingsOutputTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
+    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
+    "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
-    "MsSmoothOutputSettingsTypeDef",
+    "MsSmoothOutputSettingsOutputTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
+    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
+    "MultiplexProgramServiceDescriptorOutputTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
+    "MultiplexStatmuxVideoSettingsOutputTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
+    "NielsenCBETOutputTypeDef",
     "NielsenCBETTypeDef",
+    "NielsenNaesIiNwOutputTypeDef",
     "NielsenNaesIiNwTypeDef",
+    "OutputDestinationSettingsOutputTypeDef",
     "OutputDestinationSettingsTypeDef",
+    "RtmpGroupSettingsOutputTypeDef",
+    "UdpGroupSettingsOutputTypeDef",
     "RtmpGroupSettingsTypeDef",
     "UdpGroupSettingsTypeDef",
+    "PaginatorConfigTypeDef",
+    "PipelinePauseStateSettingsOutputTypeDef",
     "PipelinePauseStateSettingsTypeDef",
+    "RenewalSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "Scte35InputScheduleActionSettingsOutputTypeDef",
+    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
+    "Scte35SpliceInsertScheduleActionSettingsOutputTypeDef",
+    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
+    "Scte35DeliveryRestrictionsOutputTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
+    "VideoSelectorPidOutputTypeDef",
     "VideoSelectorPidTypeDef",
+    "VideoSelectorProgramIdOutputTypeDef",
     "VideoSelectorProgramIdTypeDef",
+    "DescribeAccountConfigurationResponseTypeDef",
+    "UpdateAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
+    "ArchiveCdnSettingsOutputTypeDef",
     "ArchiveCdnSettingsTypeDef",
+    "MediaPackageGroupSettingsOutputTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
+    "MultiplexOutputSettingsOutputTypeDef",
+    "RtmpOutputSettingsOutputTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
-    "MultiplexOutputSettingsTypeDef",
-    "RtmpOutputSettingsTypeDef",
+    "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
-    "AudioOnlyHlsSettingsTypeDef",
+    "AudioOnlyHlsSettingsOutputTypeDef",
+    "AvailBlankingOutputTypeDef",
+    "BlackoutSlateOutputTypeDef",
+    "BurnInDestinationSettingsOutputTypeDef",
+    "DvbSubDestinationSettingsOutputTypeDef",
+    "InputLossBehaviorOutputTypeDef",
+    "StaticImageActivateScheduleActionSettingsOutputTypeDef",
+    "StaticKeySettingsOutputTypeDef",
+    "AudioTrackSelectionOutputTypeDef",
+    "AudioTrackSelectionTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AudioTrackSelectionTypeDef",
+    "AvailSettingsOutputTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
-    "DescribeAccountConfigurationResponseTypeDef",
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateAccountConfigurationResponseTypeDef",
+    "TeletextSourceSettingsOutputTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
-    "PurchaseOfferingRequestRequestTypeDef",
-    "UpdateReservationRequestRequestTypeDef",
     "DeleteReservationResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "DescribeChannelRequestChannelCreatedWaitTypeDef",
     "DescribeChannelRequestChannelDeletedWaitTypeDef",
@@ -507,148 +608,211 @@
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
-    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    "ListInputsRequestListInputsPaginateTypeDef",
-    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    "M2tsSettingsTypeDef",
+    "M2tsSettingsOutputTypeDef",
+    "FailoverConditionSettingsOutputTypeDef",
     "FailoverConditionSettingsTypeDef",
+    "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
+    "FrameCaptureCdnSettingsOutputTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
+    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
+    "H264FilterSettingsOutputTypeDef",
+    "H265FilterSettingsOutputTypeDef",
+    "Mpeg2FilterSettingsOutputTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
+    "H265ColorSpaceSettingsOutputTypeDef",
+    "VideoSelectorColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
+    "HlsCdnSettingsOutputTypeDef",
     "HlsCdnSettingsTypeDef",
+    "NetworkInputSettingsOutputTypeDef",
     "NetworkInputSettingsTypeDef",
+    "InputClippingSettingsOutputTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
-    "StandardHlsSettingsTypeDef",
+    "StandardHlsSettingsOutputTypeDef",
+    "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
+    "MultiplexVideoSettingsOutputTypeDef",
     "MultiplexVideoSettingsTypeDef",
+    "NielsenWatermarksSettingsOutputTypeDef",
     "NielsenWatermarksSettingsTypeDef",
+    "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
+    "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
+    "PurchaseOfferingRequestRequestTypeDef",
+    "UpdateReservationRequestRequestTypeDef",
+    "Scte35SegmentationDescriptorOutputTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
     "ThumbnailDetailTypeDef",
+    "VideoSelectorSettingsOutputTypeDef",
     "VideoSelectorSettingsTypeDef",
+    "ArchiveGroupSettingsOutputTypeDef",
     "ArchiveGroupSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
+    "GlobalConfigurationOutputTypeDef",
+    "KeyProviderSettingsOutputTypeDef",
+    "AudioSelectorSettingsOutputTypeDef",
+    "AudioSelectorSettingsTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "GlobalConfigurationTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AudioSelectorSettingsTypeDef",
+    "AvailConfigurationOutputTypeDef",
     "AvailConfigurationTypeDef",
+    "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
-    "ArchiveContainerSettingsTypeDef",
-    "UdpContainerSettingsTypeDef",
+    "ArchiveContainerSettingsOutputTypeDef",
+    "UdpContainerSettingsOutputTypeDef",
+    "FailoverConditionOutputTypeDef",
     "FailoverConditionTypeDef",
+    "FrameCaptureGroupSettingsOutputTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
+    "H264SettingsOutputTypeDef",
+    "Mpeg2SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
-    "HlsSettingsTypeDef",
+    "HlsSettingsOutputTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
+    "MultiplexProgramSettingsOutputTypeDef",
     "MultiplexProgramSettingsTypeDef",
+    "AudioWatermarkSettingsOutputTypeDef",
     "AudioWatermarkSettingsTypeDef",
     "UpdateChannelClassRequestRequestTypeDef",
+    "Scte35DescriptorSettingsOutputTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
+    "VideoSelectorOutputTypeDef",
     "VideoSelectorTypeDef",
+    "CaptionDescriptionOutputTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
+    "AudioSelectorTypeDef",
     "CaptionDescriptionTypeDef",
     "HlsGroupSettingsTypeDef",
-    "AudioSelectorTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
-    "ArchiveOutputSettingsTypeDef",
-    "UdpOutputSettingsTypeDef",
+    "ArchiveOutputSettingsOutputTypeDef",
+    "UdpOutputSettingsOutputTypeDef",
+    "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
-    "HlsOutputSettingsTypeDef",
+    "HlsOutputSettingsOutputTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
-    "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
+    "CreateMultiplexProgramRequestRequestTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
+    "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
+    "Scte35DescriptorOutputTypeDef",
     "Scte35DescriptorTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
+    "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
-    "OutputSettingsTypeDef",
+    "OutputSettingsOutputTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
+    "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
+    "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
     "ChannelSummaryTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
+    "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
     "ListChannelsResponseTypeDef",
+    "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
-    "BatchScheduleActionCreateRequestTypeDef",
     "BatchScheduleActionCreateResultTypeDef",
     "BatchScheduleActionDeleteResultTypeDef",
     "DescribeScheduleResponseTypeDef",
+    "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
-    "CreateChannelRequestRequestTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
+    "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "BatchUpdateScheduleRequestRequestTypeDef",
     "BatchUpdateScheduleResponseTypeDef",
+    "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
+AacSettingsOutputTypeDef = TypedDict(
+    "AacSettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "CodingMode": AacCodingModeType,
+        "InputType": AacInputTypeType,
+        "Profile": AacProfileType,
+        "RateControlMode": AacRateControlModeType,
+        "RawFormat": AacRawFormatType,
+        "SampleRate": float,
+        "Spec": AacSpecType,
+        "VbrQuality": AacVbrQualityType,
+    },
+    total=False,
+)
+
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": AacCodingModeType,
         "InputType": AacInputTypeType,
         "Profile": AacProfileType,
@@ -657,14 +821,28 @@
         "SampleRate": float,
         "Spec": AacSpecType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
+Ac3SettingsOutputTypeDef = TypedDict(
+    "Ac3SettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "BitstreamMode": Ac3BitstreamModeType,
+        "CodingMode": Ac3CodingModeType,
+        "Dialnorm": int,
+        "DrcProfile": Ac3DrcProfileType,
+        "LfeFilter": Ac3LfeFilterType,
+        "MetadataControl": Ac3MetadataControlType,
+    },
+    total=False,
+)
+
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": float,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -678,54 +856,155 @@
 AcceptInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "AcceptInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
+AccountConfigurationOutputTypeDef = TypedDict(
+    "AccountConfigurationOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
 AccountConfigurationTypeDef = TypedDict(
     "AccountConfigurationTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+AncillarySourceSettingsOutputTypeDef = TypedDict(
+    "AncillarySourceSettingsOutputTypeDef",
+    {
+        "SourceAncillaryChannelNumber": int,
+    },
+    total=False,
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "SourceAncillaryChannelNumber": int,
     },
     total=False,
 )
 
+ArchiveS3SettingsOutputTypeDef = TypedDict(
+    "ArchiveS3SettingsOutputTypeDef",
+    {
+        "CannedAcl": S3CannedAclType,
+    },
+    total=False,
+)
+
 ArchiveS3SettingsTypeDef = TypedDict(
     "ArchiveS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
+OutputLocationRefOutputTypeDef = TypedDict(
+    "OutputLocationRefOutputTypeDef",
+    {
+        "DestinationRefId": str,
+    },
+    total=False,
+)
+
 OutputLocationRefTypeDef = TypedDict(
     "OutputLocationRefTypeDef",
     {
         "DestinationRefId": str,
     },
     total=False,
 )
 
+InputChannelLevelOutputTypeDef = TypedDict(
+    "InputChannelLevelOutputTypeDef",
+    {
+        "Gain": int,
+        "InputChannel": int,
+    },
+)
+
 InputChannelLevelTypeDef = TypedDict(
     "InputChannelLevelTypeDef",
     {
         "Gain": int,
         "InputChannel": int,
     },
 )
 
+Eac3AtmosSettingsOutputTypeDef = TypedDict(
+    "Eac3AtmosSettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "CodingMode": Eac3AtmosCodingModeType,
+        "Dialnorm": int,
+        "DrcLine": Eac3AtmosDrcLineType,
+        "DrcRf": Eac3AtmosDrcRfType,
+        "HeightTrim": float,
+        "SurroundTrim": float,
+    },
+    total=False,
+)
+
+Eac3SettingsOutputTypeDef = TypedDict(
+    "Eac3SettingsOutputTypeDef",
+    {
+        "AttenuationControl": Eac3AttenuationControlType,
+        "Bitrate": float,
+        "BitstreamMode": Eac3BitstreamModeType,
+        "CodingMode": Eac3CodingModeType,
+        "DcFilter": Eac3DcFilterType,
+        "Dialnorm": int,
+        "DrcLine": Eac3DrcLineType,
+        "DrcRf": Eac3DrcRfType,
+        "LfeControl": Eac3LfeControlType,
+        "LfeFilter": Eac3LfeFilterType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MetadataControl": Eac3MetadataControlType,
+        "PassthroughControl": Eac3PassthroughControlType,
+        "PhaseControl": Eac3PhaseControlType,
+        "StereoDownmix": Eac3StereoDownmixType,
+        "SurroundExMode": Eac3SurroundExModeType,
+        "SurroundMode": Eac3SurroundModeType,
+    },
+    total=False,
+)
+
+Mp2SettingsOutputTypeDef = TypedDict(
+    "Mp2SettingsOutputTypeDef",
+    {
+        "Bitrate": float,
+        "CodingMode": Mp2CodingModeType,
+        "SampleRate": float,
+    },
+    total=False,
+)
+
+WavSettingsOutputTypeDef = TypedDict(
+    "WavSettingsOutputTypeDef",
+    {
+        "BitDepth": float,
+        "CodingMode": WavCodingModeType,
+        "SampleRate": float,
+    },
+    total=False,
+)
+
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": float,
         "CodingMode": Eac3AtmosCodingModeType,
         "Dialnorm": int,
         "DrcLine": Eac3AtmosDrcLineType,
@@ -779,39 +1058,83 @@
         "BitDepth": float,
         "CodingMode": WavCodingModeType,
         "SampleRate": float,
     },
     total=False,
 )
 
+AudioNormalizationSettingsOutputTypeDef = TypedDict(
+    "AudioNormalizationSettingsOutputTypeDef",
+    {
+        "Algorithm": AudioNormalizationAlgorithmType,
+        "AlgorithmControl": Literal["CORRECT_AUDIO"],
+        "TargetLkfs": float,
+    },
+    total=False,
+)
+
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": Literal["CORRECT_AUDIO"],
         "TargetLkfs": float,
     },
     total=False,
 )
 
+AudioDolbyEDecodeOutputTypeDef = TypedDict(
+    "AudioDolbyEDecodeOutputTypeDef",
+    {
+        "ProgramSelection": DolbyEProgramSelectionType,
+    },
+)
+
 AudioDolbyEDecodeTypeDef = TypedDict(
     "AudioDolbyEDecodeTypeDef",
     {
         "ProgramSelection": DolbyEProgramSelectionType,
     },
 )
 
+AudioHlsRenditionSelectionOutputTypeDef = TypedDict(
+    "AudioHlsRenditionSelectionOutputTypeDef",
+    {
+        "GroupId": str,
+        "Name": str,
+    },
+)
+
 AudioHlsRenditionSelectionTypeDef = TypedDict(
     "AudioHlsRenditionSelectionTypeDef",
     {
         "GroupId": str,
         "Name": str,
     },
 )
 
+_RequiredAudioLanguageSelectionOutputTypeDef = TypedDict(
+    "_RequiredAudioLanguageSelectionOutputTypeDef",
+    {
+        "LanguageCode": str,
+    },
+)
+_OptionalAudioLanguageSelectionOutputTypeDef = TypedDict(
+    "_OptionalAudioLanguageSelectionOutputTypeDef",
+    {
+        "LanguageSelectionPolicy": AudioLanguageSelectionPolicyType,
+    },
+    total=False,
+)
+
+class AudioLanguageSelectionOutputTypeDef(
+    _RequiredAudioLanguageSelectionOutputTypeDef, _OptionalAudioLanguageSelectionOutputTypeDef
+):
+    pass
+
 _RequiredAudioLanguageSelectionTypeDef = TypedDict(
     "_RequiredAudioLanguageSelectionTypeDef",
     {
         "LanguageCode": str,
     },
 )
 _OptionalAudioLanguageSelectionTypeDef = TypedDict(
@@ -823,39 +1146,68 @@
 )
 
 class AudioLanguageSelectionTypeDef(
     _RequiredAudioLanguageSelectionTypeDef, _OptionalAudioLanguageSelectionTypeDef
 ):
     pass
 
-_RequiredInputLocationTypeDef = TypedDict(
-    "_RequiredInputLocationTypeDef",
+_RequiredInputLocationOutputTypeDef = TypedDict(
+    "_RequiredInputLocationOutputTypeDef",
     {
         "Uri": str,
     },
 )
-_OptionalInputLocationTypeDef = TypedDict(
-    "_OptionalInputLocationTypeDef",
+_OptionalInputLocationOutputTypeDef = TypedDict(
+    "_OptionalInputLocationOutputTypeDef",
     {
         "PasswordParam": str,
         "Username": str,
     },
     total=False,
 )
 
-class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
+class InputLocationOutputTypeDef(
+    _RequiredInputLocationOutputTypeDef, _OptionalInputLocationOutputTypeDef
+):
     pass
 
+AudioPidSelectionOutputTypeDef = TypedDict(
+    "AudioPidSelectionOutputTypeDef",
+    {
+        "Pid": int,
+    },
+)
+
 AudioPidSelectionTypeDef = TypedDict(
     "AudioPidSelectionTypeDef",
     {
         "Pid": int,
     },
 )
 
+_RequiredAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
+    "_RequiredAudioSilenceFailoverSettingsOutputTypeDef",
+    {
+        "AudioSelectorName": str,
+    },
+)
+_OptionalAudioSilenceFailoverSettingsOutputTypeDef = TypedDict(
+    "_OptionalAudioSilenceFailoverSettingsOutputTypeDef",
+    {
+        "AudioSilenceThresholdMsec": int,
+    },
+    total=False,
+)
+
+class AudioSilenceFailoverSettingsOutputTypeDef(
+    _RequiredAudioSilenceFailoverSettingsOutputTypeDef,
+    _OptionalAudioSilenceFailoverSettingsOutputTypeDef,
+):
+    pass
+
 _RequiredAudioSilenceFailoverSettingsTypeDef = TypedDict(
     "_RequiredAudioSilenceFailoverSettingsTypeDef",
     {
         "AudioSelectorName": str,
     },
 )
 _OptionalAudioSilenceFailoverSettingsTypeDef = TypedDict(
@@ -867,21 +1219,87 @@
 )
 
 class AudioSilenceFailoverSettingsTypeDef(
     _RequiredAudioSilenceFailoverSettingsTypeDef, _OptionalAudioSilenceFailoverSettingsTypeDef
 ):
     pass
 
+AudioTrackOutputTypeDef = TypedDict(
+    "AudioTrackOutputTypeDef",
+    {
+        "Track": int,
+    },
+)
+
 AudioTrackTypeDef = TypedDict(
     "AudioTrackTypeDef",
     {
         "Track": int,
     },
 )
 
+_RequiredInputLocationTypeDef = TypedDict(
+    "_RequiredInputLocationTypeDef",
+    {
+        "Uri": str,
+    },
+)
+_OptionalInputLocationTypeDef = TypedDict(
+    "_OptionalInputLocationTypeDef",
+    {
+        "PasswordParam": str,
+        "Username": str,
+    },
+    total=False,
+)
+
+class InputLocationTypeDef(_RequiredInputLocationTypeDef, _OptionalInputLocationTypeDef):
+    pass
+
+_RequiredEsamOutputTypeDef = TypedDict(
+    "_RequiredEsamOutputTypeDef",
+    {
+        "AcquisitionPointId": str,
+        "PoisEndpoint": str,
+    },
+)
+_OptionalEsamOutputTypeDef = TypedDict(
+    "_OptionalEsamOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "PasswordParam": str,
+        "Username": str,
+        "ZoneIdentity": str,
+    },
+    total=False,
+)
+
+class EsamOutputTypeDef(_RequiredEsamOutputTypeDef, _OptionalEsamOutputTypeDef):
+    pass
+
+Scte35SpliceInsertOutputTypeDef = TypedDict(
+    "Scte35SpliceInsertOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "NoRegionalBlackoutFlag": Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
+        "WebDeliveryAllowedFlag": Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
+    },
+    total=False,
+)
+
+Scte35TimeSignalAposOutputTypeDef = TypedDict(
+    "Scte35TimeSignalAposOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "NoRegionalBlackoutFlag": Scte35AposNoRegionalBlackoutBehaviorType,
+        "WebDeliveryAllowedFlag": Scte35AposWebDeliveryAllowedBehaviorType,
+    },
+    total=False,
+)
+
 _RequiredEsamTypeDef = TypedDict(
     "_RequiredEsamTypeDef",
     {
         "AcquisitionPointId": str,
         "PoisEndpoint": str,
     },
 )
@@ -947,25 +1365,14 @@
         "Arn": str,
         "Id": str,
         "State": str,
     },
     total=False,
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
 BatchScheduleActionDeleteRequestTypeDef = TypedDict(
     "BatchScheduleActionDeleteRequestTypeDef",
     {
         "ActionNames": Sequence[str],
     },
 )
 
@@ -990,14 +1397,41 @@
 CancelInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "CancelInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
+EbuTtDDestinationSettingsOutputTypeDef = TypedDict(
+    "EbuTtDDestinationSettingsOutputTypeDef",
+    {
+        "CopyrightHolder": str,
+        "FillLineGap": EbuTtDFillLineGapControlType,
+        "FontFamily": str,
+        "StyleControl": EbuTtDDestinationStyleControlType,
+    },
+    total=False,
+)
+
+TtmlDestinationSettingsOutputTypeDef = TypedDict(
+    "TtmlDestinationSettingsOutputTypeDef",
+    {
+        "StyleControl": TtmlDestinationStyleControlType,
+    },
+    total=False,
+)
+
+WebvttDestinationSettingsOutputTypeDef = TypedDict(
+    "WebvttDestinationSettingsOutputTypeDef",
+    {
+        "StyleControl": WebvttDestinationStyleControlType,
+    },
+    total=False,
+)
+
 EbuTtDDestinationSettingsTypeDef = TypedDict(
     "EbuTtDDestinationSettingsTypeDef",
     {
         "CopyrightHolder": str,
         "FillLineGap": EbuTtDFillLineGapControlType,
         "FontFamily": str,
         "StyleControl": EbuTtDDestinationStyleControlType,
@@ -1017,33 +1451,90 @@
     "WebvttDestinationSettingsTypeDef",
     {
         "StyleControl": WebvttDestinationStyleControlType,
     },
     total=False,
 )
 
+CaptionLanguageMappingOutputTypeDef = TypedDict(
+    "CaptionLanguageMappingOutputTypeDef",
+    {
+        "CaptionChannel": int,
+        "LanguageCode": str,
+        "LanguageDescription": str,
+    },
+)
+
 CaptionLanguageMappingTypeDef = TypedDict(
     "CaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "LanguageCode": str,
         "LanguageDescription": str,
     },
 )
 
+CaptionRectangleOutputTypeDef = TypedDict(
+    "CaptionRectangleOutputTypeDef",
+    {
+        "Height": float,
+        "LeftOffset": float,
+        "TopOffset": float,
+        "Width": float,
+    },
+)
+
 CaptionRectangleTypeDef = TypedDict(
     "CaptionRectangleTypeDef",
     {
         "Height": float,
         "LeftOffset": float,
         "TopOffset": float,
         "Width": float,
     },
 )
 
+DvbSubSourceSettingsOutputTypeDef = TypedDict(
+    "DvbSubSourceSettingsOutputTypeDef",
+    {
+        "OcrLanguage": DvbSubOcrLanguageType,
+        "Pid": int,
+    },
+    total=False,
+)
+
+EmbeddedSourceSettingsOutputTypeDef = TypedDict(
+    "EmbeddedSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": EmbeddedConvert608To708Type,
+        "Scte20Detection": EmbeddedScte20DetectionType,
+        "Source608ChannelNumber": int,
+        "Source608TrackNumber": int,
+    },
+    total=False,
+)
+
+Scte20SourceSettingsOutputTypeDef = TypedDict(
+    "Scte20SourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": Scte20Convert608To708Type,
+        "Source608ChannelNumber": int,
+    },
+    total=False,
+)
+
+Scte27SourceSettingsOutputTypeDef = TypedDict(
+    "Scte27SourceSettingsOutputTypeDef",
+    {
+        "OcrLanguage": Scte27OcrLanguageType,
+        "Pid": int,
+    },
+    total=False,
+)
+
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "OcrLanguage": DvbSubOcrLanguageType,
         "Pid": int,
     },
     total=False,
@@ -1074,14 +1565,22 @@
     {
         "OcrLanguage": Scte27OcrLanguageType,
         "Pid": int,
     },
     total=False,
 )
 
+CdiInputSpecificationOutputTypeDef = TypedDict(
+    "CdiInputSpecificationOutputTypeDef",
+    {
+        "Resolution": CdiInputResolutionType,
+    },
+    total=False,
+)
+
 CdiInputSpecificationTypeDef = TypedDict(
     "CdiInputSpecificationTypeDef",
     {
         "Resolution": CdiInputResolutionType,
     },
     total=False,
 )
@@ -1090,16 +1589,16 @@
     "ChannelEgressEndpointTypeDef",
     {
         "SourceIp": str,
     },
     total=False,
 )
 
-InputSpecificationTypeDef = TypedDict(
-    "InputSpecificationTypeDef",
+InputSpecificationOutputTypeDef = TypedDict(
+    "InputSpecificationOutputTypeDef",
     {
         "Codec": InputCodecType,
         "MaximumBitrate": InputMaximumBitrateType,
         "Resolution": InputResolutionType,
     },
     total=False,
 )
@@ -1142,14 +1641,24 @@
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+InputSpecificationTypeDef = TypedDict(
+    "InputSpecificationTypeDef",
+    {
+        "Codec": InputCodecType,
+        "MaximumBitrate": InputMaximumBitrateType,
+        "Resolution": InputResolutionType,
+    },
+    total=False,
+)
+
 MaintenanceCreateSettingsTypeDef = TypedDict(
     "MaintenanceCreateSettingsTypeDef",
     {
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceStartTime": str,
     },
     total=False,
@@ -1356,23 +1865,44 @@
 DeleteMultiplexRequestRequestTypeDef = TypedDict(
     "DeleteMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 
+_RequiredMultiplexSettingsOutputTypeDef = TypedDict(
+    "_RequiredMultiplexSettingsOutputTypeDef",
+    {
+        "TransportStreamBitrate": int,
+        "TransportStreamId": int,
+    },
+)
+_OptionalMultiplexSettingsOutputTypeDef = TypedDict(
+    "_OptionalMultiplexSettingsOutputTypeDef",
+    {
+        "MaximumVideoBufferDelayMilliseconds": int,
+        "TransportStreamReservedBitrate": int,
+    },
+    total=False,
+)
+
+class MultiplexSettingsOutputTypeDef(
+    _RequiredMultiplexSettingsOutputTypeDef, _OptionalMultiplexSettingsOutputTypeDef
+):
+    pass
+
 DeleteReservationRequestRequestTypeDef = TypedDict(
     "DeleteReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-RenewalSettingsTypeDef = TypedDict(
-    "RenewalSettingsTypeDef",
+RenewalSettingsOutputTypeDef = TypedDict(
+    "RenewalSettingsOutputTypeDef",
     {
         "AutomaticRenewal": ReservationAutomaticRenewalType,
         "RenewalCount": int,
     },
     total=False,
 )
 
@@ -1477,21 +2007,41 @@
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
     {
         "InputDeviceId": str,
         "Accept": Literal["image/jpeg"],
     },
 )
 
+DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ContentType": Literal["image/jpeg"],
+        "ContentLength": int,
+        "ETag": str,
+        "LastModified": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 
+InputDeviceSettingsOutputTypeDef = TypedDict(
+    "InputDeviceSettingsOutputTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
 InputSourceTypeDef = TypedDict(
     "InputSourceTypeDef",
     {
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
@@ -1546,24 +2096,34 @@
 DescribeReservationRequestRequestTypeDef = TypedDict(
     "DescribeReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ChannelId": str,
+    },
+)
+_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
+    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeScheduleRequestRequestTypeDef = TypedDict(
@@ -1585,51 +2145,103 @@
     {
         "ChannelId": str,
         "PipelineId": str,
         "ThumbnailType": str,
     },
 )
 
-_RequiredDvbNitSettingsTypeDef = TypedDict(
-    "_RequiredDvbNitSettingsTypeDef",
+_RequiredDvbNitSettingsOutputTypeDef = TypedDict(
+    "_RequiredDvbNitSettingsOutputTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
     },
 )
-_OptionalDvbNitSettingsTypeDef = TypedDict(
-    "_OptionalDvbNitSettingsTypeDef",
+_OptionalDvbNitSettingsOutputTypeDef = TypedDict(
+    "_OptionalDvbNitSettingsOutputTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
-class DvbNitSettingsTypeDef(_RequiredDvbNitSettingsTypeDef, _OptionalDvbNitSettingsTypeDef):
+class DvbNitSettingsOutputTypeDef(
+    _RequiredDvbNitSettingsOutputTypeDef, _OptionalDvbNitSettingsOutputTypeDef
+):
     pass
 
-DvbSdtSettingsTypeDef = TypedDict(
-    "DvbSdtSettingsTypeDef",
+DvbSdtSettingsOutputTypeDef = TypedDict(
+    "DvbSdtSettingsOutputTypeDef",
     {
         "OutputSdt": DvbSdtOutputSdtType,
         "RepInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
-DvbTdtSettingsTypeDef = TypedDict(
-    "DvbTdtSettingsTypeDef",
+DvbTdtSettingsOutputTypeDef = TypedDict(
+    "DvbTdtSettingsOutputTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FeatureActivationsOutputTypeDef = TypedDict(
+    "FeatureActivationsOutputTypeDef",
+    {
+        "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
+    },
+    total=False,
+)
+
+NielsenConfigurationOutputTypeDef = TypedDict(
+    "NielsenConfigurationOutputTypeDef",
+    {
+        "DistributorId": str,
+        "NielsenPcmToId3Tagging": NielsenPcmToId3TaggingStateType,
+    },
+    total=False,
+)
+
+ThumbnailConfigurationOutputTypeDef = TypedDict(
+    "ThumbnailConfigurationOutputTypeDef",
+    {
+        "State": ThumbnailStateType,
+    },
+)
+
+_RequiredTimecodeConfigOutputTypeDef = TypedDict(
+    "_RequiredTimecodeConfigOutputTypeDef",
+    {
+        "Source": TimecodeConfigSourceType,
+    },
+)
+_OptionalTimecodeConfigOutputTypeDef = TypedDict(
+    "_OptionalTimecodeConfigOutputTypeDef",
+    {
+        "SyncThreshold": int,
+    },
+    total=False,
+)
+
+class TimecodeConfigOutputTypeDef(
+    _RequiredTimecodeConfigOutputTypeDef, _OptionalTimecodeConfigOutputTypeDef
+):
+    pass
+
 FeatureActivationsTypeDef = TypedDict(
     "FeatureActivationsTypeDef",
     {
         "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
     },
     total=False,
 )
@@ -1663,14 +2275,31 @@
     },
     total=False,
 )
 
 class TimecodeConfigTypeDef(_RequiredTimecodeConfigTypeDef, _OptionalTimecodeConfigTypeDef):
     pass
 
+InputLossFailoverSettingsOutputTypeDef = TypedDict(
+    "InputLossFailoverSettingsOutputTypeDef",
+    {
+        "InputLossThresholdMsec": int,
+    },
+    total=False,
+)
+
+VideoBlackFailoverSettingsOutputTypeDef = TypedDict(
+    "VideoBlackFailoverSettingsOutputTypeDef",
+    {
+        "BlackDetectThreshold": float,
+        "VideoBlackThresholdMsec": int,
+    },
+    total=False,
+)
+
 InputLossFailoverSettingsTypeDef = TypedDict(
     "InputLossFailoverSettingsTypeDef",
     {
         "InputLossThresholdMsec": int,
     },
     total=False,
 )
@@ -1680,65 +2309,108 @@
     {
         "BlackDetectThreshold": float,
         "VideoBlackThresholdMsec": int,
     },
     total=False,
 )
 
-FecOutputSettingsTypeDef = TypedDict(
-    "FecOutputSettingsTypeDef",
+FecOutputSettingsOutputTypeDef = TypedDict(
+    "FecOutputSettingsOutputTypeDef",
     {
         "ColumnDepth": int,
         "IncludeFec": FecOutputIncludeFecType,
         "RowLength": int,
     },
     total=False,
 )
 
+FixedModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "FixedModeScheduleActionStartSettingsOutputTypeDef",
+    {
+        "Time": str,
+    },
+)
+
 FixedModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FixedModeScheduleActionStartSettingsTypeDef",
     {
         "Time": str,
     },
 )
 
-Fmp4HlsSettingsTypeDef = TypedDict(
-    "Fmp4HlsSettingsTypeDef",
+Fmp4HlsSettingsOutputTypeDef = TypedDict(
+    "Fmp4HlsSettingsOutputTypeDef",
     {
         "AudioRenditionSets": str,
         "NielsenId3Behavior": Fmp4NielsenId3BehaviorType,
         "TimedMetadataBehavior": Fmp4TimedMetadataBehaviorType,
     },
     total=False,
 )
 
+FollowModeScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "FollowModeScheduleActionStartSettingsOutputTypeDef",
+    {
+        "FollowPoint": FollowPointType,
+        "ReferenceActionName": str,
+    },
+)
+
 FollowModeScheduleActionStartSettingsTypeDef = TypedDict(
     "FollowModeScheduleActionStartSettingsTypeDef",
     {
         "FollowPoint": FollowPointType,
         "ReferenceActionName": str,
     },
 )
 
+FrameCaptureS3SettingsOutputTypeDef = TypedDict(
+    "FrameCaptureS3SettingsOutputTypeDef",
+    {
+        "CannedAcl": S3CannedAclType,
+    },
+    total=False,
+)
+
 FrameCaptureS3SettingsTypeDef = TypedDict(
     "FrameCaptureS3SettingsTypeDef",
     {
         "CannedAcl": S3CannedAclType,
     },
     total=False,
 )
 
-FrameCaptureOutputSettingsTypeDef = TypedDict(
-    "FrameCaptureOutputSettingsTypeDef",
+FrameCaptureOutputSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureOutputSettingsOutputTypeDef",
     {
         "NameModifier": str,
     },
     total=False,
 )
 
+_RequiredTimecodeBurninSettingsOutputTypeDef = TypedDict(
+    "_RequiredTimecodeBurninSettingsOutputTypeDef",
+    {
+        "FontSize": TimecodeBurninFontSizeType,
+        "Position": TimecodeBurninPositionType,
+    },
+)
+_OptionalTimecodeBurninSettingsOutputTypeDef = TypedDict(
+    "_OptionalTimecodeBurninSettingsOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+class TimecodeBurninSettingsOutputTypeDef(
+    _RequiredTimecodeBurninSettingsOutputTypeDef, _OptionalTimecodeBurninSettingsOutputTypeDef
+):
+    pass
+
 _RequiredTimecodeBurninSettingsTypeDef = TypedDict(
     "_RequiredTimecodeBurninSettingsTypeDef",
     {
         "FontSize": TimecodeBurninFontSizeType,
         "Position": TimecodeBurninPositionType,
     },
 )
@@ -1751,67 +2423,152 @@
 )
 
 class TimecodeBurninSettingsTypeDef(
     _RequiredTimecodeBurninSettingsTypeDef, _OptionalTimecodeBurninSettingsTypeDef
 ):
     pass
 
+H264ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H264ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": Dict[str, Any],
+        "Rec601Settings": Dict[str, Any],
+        "Rec709Settings": Dict[str, Any],
+    },
+    total=False,
+)
+
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "Rec601Settings": Mapping[str, Any],
         "Rec709Settings": Mapping[str, Any],
     },
     total=False,
 )
 
+TemporalFilterSettingsOutputTypeDef = TypedDict(
+    "TemporalFilterSettingsOutputTypeDef",
+    {
+        "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
+        "Strength": TemporalFilterStrengthType,
+    },
+    total=False,
+)
+
 TemporalFilterSettingsTypeDef = TypedDict(
     "TemporalFilterSettingsTypeDef",
     {
         "PostFilterSharpening": TemporalFilterPostFilterSharpeningType,
         "Strength": TemporalFilterStrengthType,
     },
     total=False,
 )
 
+Hdr10SettingsOutputTypeDef = TypedDict(
+    "Hdr10SettingsOutputTypeDef",
+    {
+        "MaxCll": int,
+        "MaxFall": int,
+    },
+    total=False,
+)
+
 Hdr10SettingsTypeDef = TypedDict(
     "Hdr10SettingsTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
+HlsAkamaiSettingsOutputTypeDef = TypedDict(
+    "HlsAkamaiSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "HttpTransferMode": HlsAkamaiHttpTransferModeType,
+        "NumRetries": int,
+        "RestartDelay": int,
+        "Salt": str,
+        "Token": str,
+    },
+    total=False,
+)
+
 HlsAkamaiSettingsTypeDef = TypedDict(
     "HlsAkamaiSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "HttpTransferMode": HlsAkamaiHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
         "Salt": str,
         "Token": str,
     },
     total=False,
 )
 
+HlsBasicPutSettingsOutputTypeDef = TypedDict(
+    "HlsBasicPutSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "NumRetries": int,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
 HlsBasicPutSettingsTypeDef = TypedDict(
     "HlsBasicPutSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
+HlsMediaStoreSettingsOutputTypeDef = TypedDict(
+    "HlsMediaStoreSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "MediaStoreStorageClass": Literal["TEMPORAL"],
+        "NumRetries": int,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
+HlsS3SettingsOutputTypeDef = TypedDict(
+    "HlsS3SettingsOutputTypeDef",
+    {
+        "CannedAcl": S3CannedAclType,
+    },
+    total=False,
+)
+
+HlsWebdavSettingsOutputTypeDef = TypedDict(
+    "HlsWebdavSettingsOutputTypeDef",
+    {
+        "ConnectionRetryInterval": int,
+        "FilecacheDuration": int,
+        "HttpTransferMode": HlsWebdavHttpTransferModeType,
+        "NumRetries": int,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
 HlsMediaStoreSettingsTypeDef = TypedDict(
     "HlsMediaStoreSettingsTypeDef",
     {
         "ConnectionRetryInterval": int,
         "FilecacheDuration": int,
         "MediaStoreStorageClass": Literal["TEMPORAL"],
         "NumRetries": int,
@@ -1836,42 +2593,87 @@
         "HttpTransferMode": HlsWebdavHttpTransferModeType,
         "NumRetries": int,
         "RestartDelay": int,
     },
     total=False,
 )
 
+HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef = TypedDict(
+    "HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef",
+    {
+        "Tag": str,
+        "Id3": str,
+    },
+    total=False,
+)
+
 HlsId3SegmentTaggingScheduleActionSettingsTypeDef = TypedDict(
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
     {
         "Tag": str,
         "Id3": str,
     },
     total=False,
 )
 
+HlsInputSettingsOutputTypeDef = TypedDict(
+    "HlsInputSettingsOutputTypeDef",
+    {
+        "Bandwidth": int,
+        "BufferSegments": int,
+        "Retries": int,
+        "RetryInterval": int,
+        "Scte35Source": HlsScte35SourceTypeType,
+    },
+    total=False,
+)
+
 HlsInputSettingsTypeDef = TypedDict(
     "HlsInputSettingsTypeDef",
     {
         "Bandwidth": int,
         "BufferSegments": int,
         "Retries": int,
         "RetryInterval": int,
         "Scte35Source": HlsScte35SourceTypeType,
     },
     total=False,
 )
 
+HlsTimedMetadataScheduleActionSettingsOutputTypeDef = TypedDict(
+    "HlsTimedMetadataScheduleActionSettingsOutputTypeDef",
+    {
+        "Id3": str,
+    },
+)
+
 HlsTimedMetadataScheduleActionSettingsTypeDef = TypedDict(
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
     {
         "Id3": str,
     },
 )
 
+StartTimecodeOutputTypeDef = TypedDict(
+    "StartTimecodeOutputTypeDef",
+    {
+        "Timecode": str,
+    },
+    total=False,
+)
+
+StopTimecodeOutputTypeDef = TypedDict(
+    "StopTimecodeOutputTypeDef",
+    {
+        "LastFrameClippingBehavior": LastFrameClippingBehaviorType,
+        "Timecode": str,
+    },
+    total=False,
+)
+
 StartTimecodeTypeDef = TypedDict(
     "StartTimecodeTypeDef",
     {
         "Timecode": str,
     },
     total=False,
 )
@@ -1908,23 +2710,51 @@
     "InputDeviceRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "TransferType": str,
+    },
+)
+_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
+    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+):
+    pass
+
 _RequiredListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "_RequiredListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
     },
 )
 _OptionalListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
@@ -1949,41 +2779,85 @@
         "Message": str,
         "TargetCustomerId": str,
         "TransferType": InputDeviceTransferTypeType,
     },
     total=False,
 )
 
+ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputDevicesRequestRequestTypeDef = TypedDict(
     "ListInputDevicesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputSecurityGroupsRequestRequestTypeDef = TypedDict(
     "ListInputSecurityGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputsRequestListInputsPaginateTypeDef = TypedDict(
+    "ListInputsRequestListInputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputsRequestRequestTypeDef = TypedDict(
     "ListInputsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "MultiplexId": str,
+    },
+)
+_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
+    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+):
+    pass
+
 _RequiredListMultiplexProgramsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiplexProgramsRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalListMultiplexProgramsRequestRequestTypeDef = TypedDict(
@@ -2006,23 +2880,49 @@
     {
         "ChannelId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
+ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMultiplexesRequestRequestTypeDef = TypedDict(
     "ListMultiplexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "ChannelConfiguration": str,
+        "Codec": str,
+        "Duration": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "ChannelConfiguration": str,
         "Codec": str,
         "Duration": str,
@@ -2034,14 +2934,30 @@
         "ResourceType": str,
         "SpecialFeature": str,
         "VideoQuality": str,
     },
     total=False,
 )
 
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "Codec": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "Codec": str,
         "MaxResults": int,
         "MaximumBitrate": str,
@@ -2058,16 +2974,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-M3u8SettingsTypeDef = TypedDict(
-    "M3u8SettingsTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+M3u8SettingsOutputTypeDef = TypedDict(
+    "M3u8SettingsOutputTypeDef",
     {
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "EcmPid": str,
         "NielsenId3Behavior": M3u8NielsenId3BehaviorType,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
@@ -2092,43 +3016,70 @@
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceScheduledDate": str,
         "MaintenanceStartTime": str,
     },
     total=False,
 )
 
+MediaPackageOutputDestinationSettingsOutputTypeDef = TypedDict(
+    "MediaPackageOutputDestinationSettingsOutputTypeDef",
+    {
+        "ChannelId": str,
+    },
+    total=False,
+)
+
 MediaPackageOutputDestinationSettingsTypeDef = TypedDict(
     "MediaPackageOutputDestinationSettingsTypeDef",
     {
         "ChannelId": str,
     },
     total=False,
 )
 
+MotionGraphicsActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "MotionGraphicsActivateScheduleActionSettingsOutputTypeDef",
+    {
+        "Duration": int,
+        "PasswordParam": str,
+        "Url": str,
+        "Username": str,
+    },
+    total=False,
+)
+
 MotionGraphicsActivateScheduleActionSettingsTypeDef = TypedDict(
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     {
         "Duration": int,
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
+MotionGraphicsSettingsOutputTypeDef = TypedDict(
+    "MotionGraphicsSettingsOutputTypeDef",
+    {
+        "HtmlMotionGraphicsSettings": Dict[str, Any],
+    },
+    total=False,
+)
+
 MotionGraphicsSettingsTypeDef = TypedDict(
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": Mapping[str, Any],
     },
     total=False,
 )
 
-MsSmoothOutputSettingsTypeDef = TypedDict(
-    "MsSmoothOutputSettingsTypeDef",
+MsSmoothOutputSettingsOutputTypeDef = TypedDict(
+    "MsSmoothOutputSettingsOutputTypeDef",
     {
         "H265PackagingType": MsSmoothH265PackagingTypeType,
         "NameModifier": str,
     },
     total=False,
 )
 
@@ -2136,23 +3087,40 @@
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     {
         "EntitlementArn": str,
     },
     total=False,
 )
 
+MultiplexProgramChannelDestinationSettingsOutputTypeDef = TypedDict(
+    "MultiplexProgramChannelDestinationSettingsOutputTypeDef",
+    {
+        "MultiplexId": str,
+        "ProgramName": str,
+    },
+    total=False,
+)
+
 MultiplexProgramChannelDestinationSettingsTypeDef = TypedDict(
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
+MultiplexProgramServiceDescriptorOutputTypeDef = TypedDict(
+    "MultiplexProgramServiceDescriptorOutputTypeDef",
+    {
+        "ProviderName": str,
+        "ServiceName": str,
+    },
+)
+
 MultiplexProgramServiceDescriptorTypeDef = TypedDict(
     "MultiplexProgramServiceDescriptorTypeDef",
     {
         "ProviderName": str,
         "ServiceName": str,
     },
 )
@@ -2161,33 +3129,72 @@
     "MultiplexSettingsSummaryTypeDef",
     {
         "TransportStreamBitrate": int,
     },
     total=False,
 )
 
+MultiplexStatmuxVideoSettingsOutputTypeDef = TypedDict(
+    "MultiplexStatmuxVideoSettingsOutputTypeDef",
+    {
+        "MaximumBitrate": int,
+        "MinimumBitrate": int,
+        "Priority": int,
+    },
+    total=False,
+)
+
 MultiplexStatmuxVideoSettingsTypeDef = TypedDict(
     "MultiplexStatmuxVideoSettingsTypeDef",
     {
         "MaximumBitrate": int,
         "MinimumBitrate": int,
         "Priority": int,
     },
     total=False,
 )
 
+NielsenCBETOutputTypeDef = TypedDict(
+    "NielsenCBETOutputTypeDef",
+    {
+        "CbetCheckDigitString": str,
+        "CbetStepaside": NielsenWatermarksCbetStepasideType,
+        "Csid": str,
+    },
+)
+
 NielsenCBETTypeDef = TypedDict(
     "NielsenCBETTypeDef",
     {
         "CbetCheckDigitString": str,
         "CbetStepaside": NielsenWatermarksCbetStepasideType,
         "Csid": str,
     },
 )
 
+_RequiredNielsenNaesIiNwOutputTypeDef = TypedDict(
+    "_RequiredNielsenNaesIiNwOutputTypeDef",
+    {
+        "CheckDigitString": str,
+        "Sid": float,
+    },
+)
+_OptionalNielsenNaesIiNwOutputTypeDef = TypedDict(
+    "_OptionalNielsenNaesIiNwOutputTypeDef",
+    {
+        "Timezone": NielsenWatermarkTimezonesType,
+    },
+    total=False,
+)
+
+class NielsenNaesIiNwOutputTypeDef(
+    _RequiredNielsenNaesIiNwOutputTypeDef, _OptionalNielsenNaesIiNwOutputTypeDef
+):
+    pass
+
 _RequiredNielsenNaesIiNwTypeDef = TypedDict(
     "_RequiredNielsenNaesIiNwTypeDef",
     {
         "CheckDigitString": str,
         "Sid": float,
     },
 )
@@ -2198,25 +3205,60 @@
     },
     total=False,
 )
 
 class NielsenNaesIiNwTypeDef(_RequiredNielsenNaesIiNwTypeDef, _OptionalNielsenNaesIiNwTypeDef):
     pass
 
+OutputDestinationSettingsOutputTypeDef = TypedDict(
+    "OutputDestinationSettingsOutputTypeDef",
+    {
+        "PasswordParam": str,
+        "StreamName": str,
+        "Url": str,
+        "Username": str,
+    },
+    total=False,
+)
+
 OutputDestinationSettingsTypeDef = TypedDict(
     "OutputDestinationSettingsTypeDef",
     {
         "PasswordParam": str,
         "StreamName": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
+RtmpGroupSettingsOutputTypeDef = TypedDict(
+    "RtmpGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[Literal["ON_CUE_POINT_SCTE35"]],
+        "AuthenticationScheme": AuthenticationSchemeType,
+        "CacheFullBehavior": RtmpCacheFullBehaviorType,
+        "CacheLength": int,
+        "CaptionData": RtmpCaptionDataType,
+        "InputLossAction": InputLossActionForRtmpOutType,
+        "RestartDelay": int,
+    },
+    total=False,
+)
+
+UdpGroupSettingsOutputTypeDef = TypedDict(
+    "UdpGroupSettingsOutputTypeDef",
+    {
+        "InputLossAction": InputLossActionForUdpOutType,
+        "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+    },
+    total=False,
+)
+
 RtmpGroupSettingsTypeDef = TypedDict(
     "RtmpGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[Literal["ON_CUE_POINT_SCTE35"]],
         "AuthenticationScheme": AuthenticationSchemeType,
         "CacheFullBehavior": RtmpCacheFullBehaviorType,
         "CacheLength": int,
@@ -2233,21 +3275,47 @@
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+PipelinePauseStateSettingsOutputTypeDef = TypedDict(
+    "PipelinePauseStateSettingsOutputTypeDef",
+    {
+        "PipelineId": PipelineIdType,
+    },
+)
+
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
+RenewalSettingsTypeDef = TypedDict(
+    "RenewalSettingsTypeDef",
+    {
+        "AutomaticRenewal": ReservationAutomaticRenewalType,
+        "RenewalCount": int,
+    },
+    total=False,
+)
+
 _RequiredRebootInputDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredRebootInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 _OptionalRebootInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2266,14 +3334,81 @@
 RejectInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "RejectInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
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
+_RequiredScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredScte35InputScheduleActionSettingsOutputTypeDef",
+    {
+        "Mode": Scte35InputModeType,
+    },
+)
+_OptionalScte35InputScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalScte35InputScheduleActionSettingsOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+    },
+    total=False,
+)
+
+class Scte35InputScheduleActionSettingsOutputTypeDef(
+    _RequiredScte35InputScheduleActionSettingsOutputTypeDef,
+    _OptionalScte35InputScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
+Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef = TypedDict(
+    "Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef",
+    {
+        "SpliceEventId": int,
+    },
+)
+
+_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
+    {
+        "SpliceEventId": int,
+    },
+)
+_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
+class Scte35SpliceInsertScheduleActionSettingsOutputTypeDef(
+    _RequiredScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+    _OptionalScte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
+StaticImageDeactivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "StaticImageDeactivateScheduleActionSettingsOutputTypeDef",
+    {
+        "FadeOut": int,
+        "Layer": int,
+    },
+    total=False,
+)
+
 _RequiredScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredScte35InputScheduleActionSettingsTypeDef",
     {
         "Mode": Scte35InputModeType,
     },
 )
 _OptionalScte35InputScheduleActionSettingsTypeDef = TypedDict(
@@ -2322,14 +3457,24 @@
     {
         "FadeOut": int,
         "Layer": int,
     },
     total=False,
 )
 
+Scte35DeliveryRestrictionsOutputTypeDef = TypedDict(
+    "Scte35DeliveryRestrictionsOutputTypeDef",
+    {
+        "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
+        "DeviceRestrictions": Scte35DeviceRestrictionsType,
+        "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
+        "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
+    },
+)
+
 Scte35DeliveryRestrictionsTypeDef = TypedDict(
     "Scte35DeliveryRestrictionsTypeDef",
     {
         "ArchiveAllowedFlag": Scte35ArchiveAllowedFlagType,
         "DeviceRestrictions": Scte35DeviceRestrictionsType,
         "NoRegionalBlackoutFlag": Scte35NoRegionalBlackoutFlagType,
         "WebDeliveryAllowedFlag": Scte35WebDeliveryAllowedFlagType,
@@ -2400,61 +3545,101 @@
 
 class TransferInputDeviceRequestRequestTypeDef(
     _RequiredTransferInputDeviceRequestRequestTypeDef,
     _OptionalTransferInputDeviceRequestRequestTypeDef,
 ):
     pass
 
+VideoSelectorPidOutputTypeDef = TypedDict(
+    "VideoSelectorPidOutputTypeDef",
+    {
+        "Pid": int,
+    },
+    total=False,
+)
+
 VideoSelectorPidTypeDef = TypedDict(
     "VideoSelectorPidTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
 
+VideoSelectorProgramIdOutputTypeDef = TypedDict(
+    "VideoSelectorProgramIdOutputTypeDef",
+    {
+        "ProgramId": int,
+    },
+    total=False,
+)
+
 VideoSelectorProgramIdTypeDef = TypedDict(
     "VideoSelectorProgramIdTypeDef",
     {
         "ProgramId": int,
     },
     total=False,
 )
 
+DescribeAccountConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
     },
     total=False,
 )
 
+ArchiveCdnSettingsOutputTypeDef = TypedDict(
+    "ArchiveCdnSettingsOutputTypeDef",
+    {
+        "ArchiveS3Settings": ArchiveS3SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": ArchiveS3SettingsTypeDef,
     },
     total=False,
 )
 
-MediaPackageGroupSettingsTypeDef = TypedDict(
-    "MediaPackageGroupSettingsTypeDef",
+MediaPackageGroupSettingsOutputTypeDef = TypedDict(
+    "MediaPackageGroupSettingsOutputTypeDef",
     {
-        "Destination": OutputLocationRefTypeDef,
+        "Destination": OutputLocationRefOutputTypeDef,
     },
 )
 
-_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_RequiredMsSmoothGroupSettingsTypeDef",
+_RequiredMsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredMsSmoothGroupSettingsOutputTypeDef",
     {
-        "Destination": OutputLocationRefTypeDef,
+        "Destination": OutputLocationRefOutputTypeDef,
     },
 )
-_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
-    "_OptionalMsSmoothGroupSettingsTypeDef",
+_OptionalMsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalMsSmoothGroupSettingsOutputTypeDef",
     {
         "AcquisitionPointId": str,
         "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
         "CertificateMode": SmoothGroupCertificateModeType,
         "ConnectionRetryInterval": int,
         "EventId": str,
         "EventIdMode": SmoothGroupEventIdModeType,
@@ -2470,80 +3655,311 @@
         "StreamManifestBehavior": SmoothGroupStreamManifestBehaviorType,
         "TimestampOffset": str,
         "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
-class MsSmoothGroupSettingsTypeDef(
-    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
+class MsSmoothGroupSettingsOutputTypeDef(
+    _RequiredMsSmoothGroupSettingsOutputTypeDef, _OptionalMsSmoothGroupSettingsOutputTypeDef
 ):
     pass
 
-MultiplexOutputSettingsTypeDef = TypedDict(
-    "MultiplexOutputSettingsTypeDef",
+MultiplexOutputSettingsOutputTypeDef = TypedDict(
+    "MultiplexOutputSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+
+_RequiredRtmpOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredRtmpOutputSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalRtmpOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalRtmpOutputSettingsOutputTypeDef",
+    {
+        "CertificateMode": RtmpOutputCertificateModeType,
+        "ConnectionRetryInterval": int,
+        "NumRetries": int,
+    },
+    total=False,
+)
+
+class RtmpOutputSettingsOutputTypeDef(
+    _RequiredRtmpOutputSettingsOutputTypeDef, _OptionalRtmpOutputSettingsOutputTypeDef
+):
+    pass
+
+MediaPackageGroupSettingsTypeDef = TypedDict(
+    "MediaPackageGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 
-_RequiredRtmpOutputSettingsTypeDef = TypedDict(
-    "_RequiredRtmpOutputSettingsTypeDef",
+_RequiredMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_RequiredMsSmoothGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
-_OptionalRtmpOutputSettingsTypeDef = TypedDict(
-    "_OptionalRtmpOutputSettingsTypeDef",
+_OptionalMsSmoothGroupSettingsTypeDef = TypedDict(
+    "_OptionalMsSmoothGroupSettingsTypeDef",
     {
-        "CertificateMode": RtmpOutputCertificateModeType,
+        "AcquisitionPointId": str,
+        "AudioOnlyTimecodeControl": SmoothGroupAudioOnlyTimecodeControlType,
+        "CertificateMode": SmoothGroupCertificateModeType,
         "ConnectionRetryInterval": int,
+        "EventId": str,
+        "EventIdMode": SmoothGroupEventIdModeType,
+        "EventStopBehavior": SmoothGroupEventStopBehaviorType,
+        "FilecacheDuration": int,
+        "FragmentLength": int,
+        "InputLossAction": InputLossActionForMsSmoothOutType,
         "NumRetries": int,
+        "RestartDelay": int,
+        "SegmentationMode": SmoothGroupSegmentationModeType,
+        "SendDelayMs": int,
+        "SparseTrackType": SmoothGroupSparseTrackTypeType,
+        "StreamManifestBehavior": SmoothGroupStreamManifestBehaviorType,
+        "TimestampOffset": str,
+        "TimestampOffsetMode": SmoothGroupTimestampOffsetModeType,
     },
     total=False,
 )
 
-class RtmpOutputSettingsTypeDef(
-    _RequiredRtmpOutputSettingsTypeDef, _OptionalRtmpOutputSettingsTypeDef
+class MsSmoothGroupSettingsTypeDef(
+    _RequiredMsSmoothGroupSettingsTypeDef, _OptionalMsSmoothGroupSettingsTypeDef
 ):
     pass
 
+AudioChannelMappingOutputTypeDef = TypedDict(
+    "AudioChannelMappingOutputTypeDef",
+    {
+        "InputChannelLevels": List[InputChannelLevelOutputTypeDef],
+        "OutputChannel": int,
+    },
+)
+
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
         "InputChannelLevels": Sequence[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
 
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": AacSettingsOutputTypeDef,
+        "Ac3Settings": Ac3SettingsOutputTypeDef,
+        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
+        "Eac3Settings": Eac3SettingsOutputTypeDef,
+        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "PassThroughSettings": Dict[str, Any],
+        "WavSettings": WavSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
         "Eac3Settings": Eac3SettingsTypeDef,
         "Mp2Settings": Mp2SettingsTypeDef,
         "PassThroughSettings": Mapping[str, Any],
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
-AudioOnlyHlsSettingsTypeDef = TypedDict(
-    "AudioOnlyHlsSettingsTypeDef",
+AudioOnlyHlsSettingsOutputTypeDef = TypedDict(
+    "AudioOnlyHlsSettingsOutputTypeDef",
     {
         "AudioGroupId": str,
-        "AudioOnlyImage": InputLocationTypeDef,
+        "AudioOnlyImage": InputLocationOutputTypeDef,
         "AudioTrackType": AudioOnlyHlsTrackTypeType,
         "SegmentType": AudioOnlyHlsSegmentTypeType,
     },
     total=False,
 )
 
+AvailBlankingOutputTypeDef = TypedDict(
+    "AvailBlankingOutputTypeDef",
+    {
+        "AvailBlankingImage": InputLocationOutputTypeDef,
+        "State": AvailBlankingStateType,
+    },
+    total=False,
+)
+
+BlackoutSlateOutputTypeDef = TypedDict(
+    "BlackoutSlateOutputTypeDef",
+    {
+        "BlackoutSlateImage": InputLocationOutputTypeDef,
+        "NetworkEndBlackout": BlackoutSlateNetworkEndBlackoutType,
+        "NetworkEndBlackoutImage": InputLocationOutputTypeDef,
+        "NetworkId": str,
+        "State": BlackoutSlateStateType,
+    },
+    total=False,
+)
+
+BurnInDestinationSettingsOutputTypeDef = TypedDict(
+    "BurnInDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": BurnInAlignmentType,
+        "BackgroundColor": BurnInBackgroundColorType,
+        "BackgroundOpacity": int,
+        "Font": InputLocationOutputTypeDef,
+        "FontColor": BurnInFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontSize": str,
+        "OutlineColor": BurnInOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": BurnInShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "TeletextGridControl": BurnInTeletextGridControlType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+    total=False,
+)
+
+DvbSubDestinationSettingsOutputTypeDef = TypedDict(
+    "DvbSubDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": DvbSubDestinationAlignmentType,
+        "BackgroundColor": DvbSubDestinationBackgroundColorType,
+        "BackgroundOpacity": int,
+        "Font": InputLocationOutputTypeDef,
+        "FontColor": DvbSubDestinationFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontSize": str,
+        "OutlineColor": DvbSubDestinationOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": DvbSubDestinationShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "TeletextGridControl": DvbSubDestinationTeletextGridControlType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+    total=False,
+)
+
+InputLossBehaviorOutputTypeDef = TypedDict(
+    "InputLossBehaviorOutputTypeDef",
+    {
+        "BlackFrameMsec": int,
+        "InputLossImageColor": str,
+        "InputLossImageSlate": InputLocationOutputTypeDef,
+        "InputLossImageType": InputLossImageTypeType,
+        "RepeatFrameMsec": int,
+    },
+    total=False,
+)
+
+_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef",
+    {
+        "Image": InputLocationOutputTypeDef,
+    },
+)
+_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef",
+    {
+        "Duration": int,
+        "FadeIn": int,
+        "FadeOut": int,
+        "Height": int,
+        "ImageX": int,
+        "ImageY": int,
+        "Layer": int,
+        "Opacity": int,
+        "Width": int,
+    },
+    total=False,
+)
+
+class StaticImageActivateScheduleActionSettingsOutputTypeDef(
+    _RequiredStaticImageActivateScheduleActionSettingsOutputTypeDef,
+    _OptionalStaticImageActivateScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
+_RequiredStaticKeySettingsOutputTypeDef = TypedDict(
+    "_RequiredStaticKeySettingsOutputTypeDef",
+    {
+        "StaticKeyValue": str,
+    },
+)
+_OptionalStaticKeySettingsOutputTypeDef = TypedDict(
+    "_OptionalStaticKeySettingsOutputTypeDef",
+    {
+        "KeyProviderServer": InputLocationOutputTypeDef,
+    },
+    total=False,
+)
+
+class StaticKeySettingsOutputTypeDef(
+    _RequiredStaticKeySettingsOutputTypeDef, _OptionalStaticKeySettingsOutputTypeDef
+):
+    pass
+
+_RequiredAudioTrackSelectionOutputTypeDef = TypedDict(
+    "_RequiredAudioTrackSelectionOutputTypeDef",
+    {
+        "Tracks": List[AudioTrackOutputTypeDef],
+    },
+)
+_OptionalAudioTrackSelectionOutputTypeDef = TypedDict(
+    "_OptionalAudioTrackSelectionOutputTypeDef",
+    {
+        "DolbyEDecode": AudioDolbyEDecodeOutputTypeDef,
+    },
+    total=False,
+)
+
+class AudioTrackSelectionOutputTypeDef(
+    _RequiredAudioTrackSelectionOutputTypeDef, _OptionalAudioTrackSelectionOutputTypeDef
+):
+    pass
+
+_RequiredAudioTrackSelectionTypeDef = TypedDict(
+    "_RequiredAudioTrackSelectionTypeDef",
+    {
+        "Tracks": Sequence[AudioTrackTypeDef],
+    },
+)
+_OptionalAudioTrackSelectionTypeDef = TypedDict(
+    "_OptionalAudioTrackSelectionTypeDef",
+    {
+        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
+    },
+    total=False,
+)
+
+class AudioTrackSelectionTypeDef(
+    _RequiredAudioTrackSelectionTypeDef, _OptionalAudioTrackSelectionTypeDef
+):
+    pass
+
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": InputLocationTypeDef,
         "State": AvailBlankingStateType,
     },
     total=False,
@@ -2664,33 +4080,24 @@
 )
 
 class StaticKeySettingsTypeDef(
     _RequiredStaticKeySettingsTypeDef, _OptionalStaticKeySettingsTypeDef
 ):
     pass
 
-_RequiredAudioTrackSelectionTypeDef = TypedDict(
-    "_RequiredAudioTrackSelectionTypeDef",
+AvailSettingsOutputTypeDef = TypedDict(
+    "AvailSettingsOutputTypeDef",
     {
-        "Tracks": Sequence[AudioTrackTypeDef],
-    },
-)
-_OptionalAudioTrackSelectionTypeDef = TypedDict(
-    "_OptionalAudioTrackSelectionTypeDef",
-    {
-        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
+        "Esam": EsamOutputTypeDef,
+        "Scte35SpliceInsert": Scte35SpliceInsertOutputTypeDef,
+        "Scte35TimeSignalApos": Scte35TimeSignalAposOutputTypeDef,
     },
     total=False,
 )
 
-class AudioTrackSelectionTypeDef(
-    _RequiredAudioTrackSelectionTypeDef, _OptionalAudioTrackSelectionTypeDef
-):
-    pass
-
 AvailSettingsTypeDef = TypedDict(
     "AvailSettingsTypeDef",
     {
         "Esam": EsamTypeDef,
         "Scte35SpliceInsert": Scte35SpliceInsertTypeDef,
         "Scte35TimeSignalApos": Scte35TimeSignalAposTypeDef,
     },
@@ -2698,77 +4105,43 @@
 )
 
 BatchDeleteResponseTypeDef = TypedDict(
     "BatchDeleteResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStartResponseTypeDef = TypedDict(
     "BatchStartResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStopResponseTypeDef = TypedDict(
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAccountConfigurationResponseTypeDef = TypedDict(
-    "DescribeAccountConfigurationResponseTypeDef",
+TeletextSourceSettingsOutputTypeDef = TypedDict(
+    "TeletextSourceSettingsOutputTypeDef",
     {
-        "AccountConfiguration": AccountConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ContentType": Literal["image/jpeg"],
-        "ContentLength": int,
-        "ETag": str,
-        "LastModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
-    {
-        "AccountConfiguration": AccountConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "OutputRectangle": CaptionRectangleOutputTypeDef,
+        "PageNumber": str,
     },
+    total=False,
 )
 
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
         "PageNumber": str,
@@ -2862,58 +4235,14 @@
 )
 
 class UpdateMultiplexRequestRequestTypeDef(
     _RequiredUpdateMultiplexRequestRequestTypeDef, _OptionalUpdateMultiplexRequestRequestTypeDef
 ):
     pass
 
-_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_RequiredPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Count": int,
-        "OfferingId": str,
-    },
-)
-_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
-    "_OptionalPurchaseOfferingRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-        "RequestId": str,
-        "Start": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class PurchaseOfferingRequestRequestTypeDef(
-    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReservationRequestRequestTypeDef",
-    {
-        "ReservationId": str,
-    },
-)
-_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReservationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
-    },
-    total=False,
-)
-
-class UpdateReservationRequestRequestTypeDef(
-    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
-):
-    pass
-
 DeleteReservationResponseTypeDef = TypedDict(
     "DeleteReservationResponseTypeDef",
     {
         "Arn": str,
         "Count": int,
         "CurrencyCode": str,
         "Duration": int,
@@ -2921,22 +4250,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
+        "RenewalSettings": RenewalSettingsOutputTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Arn": str,
@@ -2946,15 +4275,15 @@
         "FixedPrice": float,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Arn": str,
@@ -2965,22 +4294,22 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
+        "RenewalSettings": RenewalSettingsOutputTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "Arn": str,
@@ -3009,15 +4338,15 @@
         "End": str,
         "FixedPrice": float,
         "Name": str,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
-        "RenewalSettings": RenewalSettingsTypeDef,
+        "RenewalSettings": RenewalSettingsOutputTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
     },
@@ -3256,15 +4585,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
         "Arn": str,
@@ -3296,28 +4625,28 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputSecurityGroupTypeDef = TypedDict(
     "InputSecurityGroupTypeDef",
     {
         "Arn": str,
@@ -3326,166 +4655,32 @@
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "ChannelId": str,
-    },
-)
-_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
-    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-):
-    pass
-
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "TransferType": str,
-    },
-)
-_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
-    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-):
-    pass
-
-ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputsRequestListInputsPaginateTypeDef = TypedDict(
-    "ListInputsRequestListInputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "MultiplexId": str,
-    },
-)
-_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
-    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-):
-    pass
-
-ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "ChannelConfiguration": str,
-        "Codec": str,
-        "Duration": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "Codec": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-M2tsSettingsTypeDef = TypedDict(
-    "M2tsSettingsTypeDef",
+M2tsSettingsOutputTypeDef = TypedDict(
+    "M2tsSettingsOutputTypeDef",
     {
         "AbsentInputAudioBehavior": M2tsAbsentInputAudioBehaviorType,
         "Arib": M2tsAribType,
         "AribCaptionsPid": str,
         "AribCaptionsPidControl": M2tsAribCaptionsPidControlType,
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "AudioStreamType": M2tsAudioStreamTypeType,
         "Bitrate": int,
         "BufferModel": M2tsBufferModelType,
         "CcDescriptor": M2tsCcDescriptorType,
-        "DvbNitSettings": DvbNitSettingsTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsTypeDef,
+        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
         "DvbSubPids": str,
-        "DvbTdtSettings": DvbTdtSettingsTypeDef,
+        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
         "DvbTeletextPid": str,
         "Ebif": M2tsEbifControlType,
         "EbpAudioInterval": M2tsAudioIntervalType,
         "EbpLookaheadMs": int,
         "EbpPlacement": M2tsEbpPlacementType,
         "EcmPid": str,
         "EsRateInPes": M2tsEsRateInPesType,
@@ -3515,52 +4710,114 @@
         "TransportStreamId": int,
         "VideoPid": str,
         "Scte35PrerollPullupMilliseconds": float,
     },
     total=False,
 )
 
+FailoverConditionSettingsOutputTypeDef = TypedDict(
+    "FailoverConditionSettingsOutputTypeDef",
+    {
+        "AudioSilenceSettings": AudioSilenceFailoverSettingsOutputTypeDef,
+        "InputLossSettings": InputLossFailoverSettingsOutputTypeDef,
+        "VideoBlackSettings": VideoBlackFailoverSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": AudioSilenceFailoverSettingsTypeDef,
         "InputLossSettings": InputLossFailoverSettingsTypeDef,
         "VideoBlackSettings": VideoBlackFailoverSettingsTypeDef,
     },
     total=False,
 )
 
+ScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionStartSettingsOutputTypeDef",
+    {
+        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsOutputTypeDef,
+        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsOutputTypeDef,
+        "ImmediateModeScheduleActionStartSettings": Dict[str, Any],
+    },
+    total=False,
+)
+
 ScheduleActionStartSettingsTypeDef = TypedDict(
     "ScheduleActionStartSettingsTypeDef",
     {
         "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
         "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Mapping[str, Any],
     },
     total=False,
 )
 
+FrameCaptureCdnSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureCdnSettingsOutputTypeDef",
+    {
+        "FrameCaptureS3Settings": FrameCaptureS3SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 FrameCaptureCdnSettingsTypeDef = TypedDict(
     "FrameCaptureCdnSettingsTypeDef",
     {
         "FrameCaptureS3Settings": FrameCaptureS3SettingsTypeDef,
     },
     total=False,
 )
 
+FrameCaptureSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureSettingsOutputTypeDef",
+    {
+        "CaptureInterval": int,
+        "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "CaptureInterval": int,
         "CaptureIntervalUnits": FrameCaptureIntervalUnitType,
         "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
     },
     total=False,
 )
 
+H264FilterSettingsOutputTypeDef = TypedDict(
+    "H264FilterSettingsOutputTypeDef",
+    {
+        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+H265FilterSettingsOutputTypeDef = TypedDict(
+    "H265FilterSettingsOutputTypeDef",
+    {
+        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+Mpeg2FilterSettingsOutputTypeDef = TypedDict(
+    "Mpeg2FilterSettingsOutputTypeDef",
+    {
+        "TemporalFilterSettings": TemporalFilterSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 H264FilterSettingsTypeDef = TypedDict(
     "H264FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
@@ -3577,14 +4834,34 @@
     "Mpeg2FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
 
+H265ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H265ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": Dict[str, Any],
+        "DolbyVision81Settings": Dict[str, Any],
+        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
+        "Rec601Settings": Dict[str, Any],
+        "Rec709Settings": Dict[str, Any],
+    },
+    total=False,
+)
+
+VideoSelectorColorSpaceSettingsOutputTypeDef = TypedDict(
+    "VideoSelectorColorSpaceSettingsOutputTypeDef",
+    {
+        "Hdr10Settings": Hdr10SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "DolbyVision81Settings": Mapping[str, Any],
         "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Mapping[str, Any],
@@ -3597,35 +4874,76 @@
     "VideoSelectorColorSpaceSettingsTypeDef",
     {
         "Hdr10Settings": Hdr10SettingsTypeDef,
     },
     total=False,
 )
 
+HlsCdnSettingsOutputTypeDef = TypedDict(
+    "HlsCdnSettingsOutputTypeDef",
+    {
+        "HlsAkamaiSettings": HlsAkamaiSettingsOutputTypeDef,
+        "HlsBasicPutSettings": HlsBasicPutSettingsOutputTypeDef,
+        "HlsMediaStoreSettings": HlsMediaStoreSettingsOutputTypeDef,
+        "HlsS3Settings": HlsS3SettingsOutputTypeDef,
+        "HlsWebdavSettings": HlsWebdavSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 HlsCdnSettingsTypeDef = TypedDict(
     "HlsCdnSettingsTypeDef",
     {
         "HlsAkamaiSettings": HlsAkamaiSettingsTypeDef,
         "HlsBasicPutSettings": HlsBasicPutSettingsTypeDef,
         "HlsMediaStoreSettings": HlsMediaStoreSettingsTypeDef,
         "HlsS3Settings": HlsS3SettingsTypeDef,
         "HlsWebdavSettings": HlsWebdavSettingsTypeDef,
     },
     total=False,
 )
 
+NetworkInputSettingsOutputTypeDef = TypedDict(
+    "NetworkInputSettingsOutputTypeDef",
+    {
+        "HlsInputSettings": HlsInputSettingsOutputTypeDef,
+        "ServerValidation": NetworkInputServerValidationType,
+    },
+    total=False,
+)
+
 NetworkInputSettingsTypeDef = TypedDict(
     "NetworkInputSettingsTypeDef",
     {
         "HlsInputSettings": HlsInputSettingsTypeDef,
         "ServerValidation": NetworkInputServerValidationType,
     },
     total=False,
 )
 
+_RequiredInputClippingSettingsOutputTypeDef = TypedDict(
+    "_RequiredInputClippingSettingsOutputTypeDef",
+    {
+        "InputTimecodeSource": InputTimecodeSourceType,
+    },
+)
+_OptionalInputClippingSettingsOutputTypeDef = TypedDict(
+    "_OptionalInputClippingSettingsOutputTypeDef",
+    {
+        "StartTimecode": StartTimecodeOutputTypeDef,
+        "StopTimecode": StopTimecodeOutputTypeDef,
+    },
+    total=False,
+)
+
+class InputClippingSettingsOutputTypeDef(
+    _RequiredInputClippingSettingsOutputTypeDef, _OptionalInputClippingSettingsOutputTypeDef
+):
+    pass
+
 _RequiredInputClippingSettingsTypeDef = TypedDict(
     "_RequiredInputClippingSettingsTypeDef",
     {
         "InputTimecodeSource": InputTimecodeSourceType,
     },
 )
 _OptionalInputClippingSettingsTypeDef = TypedDict(
@@ -3700,43 +5018,63 @@
     pass
 
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStandardHlsSettingsTypeDef = TypedDict(
-    "_RequiredStandardHlsSettingsTypeDef",
+_RequiredStandardHlsSettingsOutputTypeDef = TypedDict(
+    "_RequiredStandardHlsSettingsOutputTypeDef",
     {
-        "M3u8Settings": M3u8SettingsTypeDef,
+        "M3u8Settings": M3u8SettingsOutputTypeDef,
     },
 )
-_OptionalStandardHlsSettingsTypeDef = TypedDict(
-    "_OptionalStandardHlsSettingsTypeDef",
+_OptionalStandardHlsSettingsOutputTypeDef = TypedDict(
+    "_OptionalStandardHlsSettingsOutputTypeDef",
     {
         "AudioRenditionSets": str,
     },
     total=False,
 )
 
-class StandardHlsSettingsTypeDef(
-    _RequiredStandardHlsSettingsTypeDef, _OptionalStandardHlsSettingsTypeDef
+class StandardHlsSettingsOutputTypeDef(
+    _RequiredStandardHlsSettingsOutputTypeDef, _OptionalStandardHlsSettingsOutputTypeDef
+):
+    pass
+
+_RequiredMotionGraphicsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredMotionGraphicsConfigurationOutputTypeDef",
+    {
+        "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
+    },
+)
+_OptionalMotionGraphicsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalMotionGraphicsConfigurationOutputTypeDef",
+    {
+        "MotionGraphicsInsertion": MotionGraphicsInsertionType,
+    },
+    total=False,
+)
+
+class MotionGraphicsConfigurationOutputTypeDef(
+    _RequiredMotionGraphicsConfigurationOutputTypeDef,
+    _OptionalMotionGraphicsConfigurationOutputTypeDef,
 ):
     pass
 
 _RequiredMotionGraphicsConfigurationTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
@@ -3775,52 +5113,163 @@
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+MultiplexVideoSettingsOutputTypeDef = TypedDict(
+    "MultiplexVideoSettingsOutputTypeDef",
+    {
+        "ConstantBitrate": int,
+        "StatmuxSettings": MultiplexStatmuxVideoSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 MultiplexVideoSettingsTypeDef = TypedDict(
     "MultiplexVideoSettingsTypeDef",
     {
         "ConstantBitrate": int,
         "StatmuxSettings": MultiplexStatmuxVideoSettingsTypeDef,
     },
     total=False,
 )
 
+NielsenWatermarksSettingsOutputTypeDef = TypedDict(
+    "NielsenWatermarksSettingsOutputTypeDef",
+    {
+        "NielsenCbetSettings": NielsenCBETOutputTypeDef,
+        "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
+        "NielsenNaesIiNwSettings": NielsenNaesIiNwOutputTypeDef,
+    },
+    total=False,
+)
+
 NielsenWatermarksSettingsTypeDef = TypedDict(
     "NielsenWatermarksSettingsTypeDef",
     {
         "NielsenCbetSettings": NielsenCBETTypeDef,
         "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
         "NielsenNaesIiNwSettings": NielsenNaesIiNwTypeDef,
     },
     total=False,
 )
 
+OutputDestinationOutputTypeDef = TypedDict(
+    "OutputDestinationOutputTypeDef",
+    {
+        "Id": str,
+        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsOutputTypeDef],
+        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsOutputTypeDef,
+        "Settings": List[OutputDestinationSettingsOutputTypeDef],
+    },
+    total=False,
+)
+
 OutputDestinationTypeDef = TypedDict(
     "OutputDestinationTypeDef",
     {
         "Id": str,
         "MediaPackageSettings": Sequence[MediaPackageOutputDestinationSettingsTypeDef],
         "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
         "Settings": Sequence[OutputDestinationSettingsTypeDef],
     },
     total=False,
 )
 
+PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "PauseStateScheduleActionSettingsOutputTypeDef",
+    {
+        "Pipelines": List[PipelinePauseStateSettingsOutputTypeDef],
+    },
+    total=False,
+)
+
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
         "Pipelines": Sequence[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
 
+_RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_RequiredPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Count": int,
+        "OfferingId": str,
+    },
+)
+_OptionalPurchaseOfferingRequestRequestTypeDef = TypedDict(
+    "_OptionalPurchaseOfferingRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+        "RequestId": str,
+        "Start": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PurchaseOfferingRequestRequestTypeDef(
+    _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReservationRequestRequestTypeDef",
+    {
+        "ReservationId": str,
+    },
+)
+_OptionalUpdateReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReservationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RenewalSettings": RenewalSettingsTypeDef,
+    },
+    total=False,
+)
+
+class UpdateReservationRequestRequestTypeDef(
+    _RequiredUpdateReservationRequestRequestTypeDef, _OptionalUpdateReservationRequestRequestTypeDef
+):
+    pass
+
+_RequiredScte35SegmentationDescriptorOutputTypeDef = TypedDict(
+    "_RequiredScte35SegmentationDescriptorOutputTypeDef",
+    {
+        "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
+        "SegmentationEventId": int,
+    },
+)
+_OptionalScte35SegmentationDescriptorOutputTypeDef = TypedDict(
+    "_OptionalScte35SegmentationDescriptorOutputTypeDef",
+    {
+        "DeliveryRestrictions": Scte35DeliveryRestrictionsOutputTypeDef,
+        "SegmentNum": int,
+        "SegmentationDuration": int,
+        "SegmentationTypeId": int,
+        "SegmentationUpid": str,
+        "SegmentationUpidType": int,
+        "SegmentsExpected": int,
+        "SubSegmentNum": int,
+        "SubSegmentsExpected": int,
+    },
+    total=False,
+)
+
+class Scte35SegmentationDescriptorOutputTypeDef(
+    _RequiredScte35SegmentationDescriptorOutputTypeDef,
+    _OptionalScte35SegmentationDescriptorOutputTypeDef,
+):
+    pass
+
 _RequiredScte35SegmentationDescriptorTypeDef = TypedDict(
     "_RequiredScte35SegmentationDescriptorTypeDef",
     {
         "SegmentationCancelIndicator": Scte35SegmentationCancelIndicatorType,
         "SegmentationEventId": int,
     },
 )
@@ -3850,23 +5299,52 @@
     {
         "PipelineId": str,
         "Thumbnails": List[ThumbnailTypeDef],
     },
     total=False,
 )
 
+VideoSelectorSettingsOutputTypeDef = TypedDict(
+    "VideoSelectorSettingsOutputTypeDef",
+    {
+        "VideoSelectorPid": VideoSelectorPidOutputTypeDef,
+        "VideoSelectorProgramId": VideoSelectorProgramIdOutputTypeDef,
+    },
+    total=False,
+)
+
 VideoSelectorSettingsTypeDef = TypedDict(
     "VideoSelectorSettingsTypeDef",
     {
         "VideoSelectorPid": VideoSelectorPidTypeDef,
         "VideoSelectorProgramId": VideoSelectorProgramIdTypeDef,
     },
     total=False,
 )
 
+_RequiredArchiveGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredArchiveGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalArchiveGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalArchiveGroupSettingsOutputTypeDef",
+    {
+        "ArchiveCdnSettings": ArchiveCdnSettingsOutputTypeDef,
+        "RolloverInterval": int,
+    },
+    total=False,
+)
+
+class ArchiveGroupSettingsOutputTypeDef(
+    _RequiredArchiveGroupSettingsOutputTypeDef, _OptionalArchiveGroupSettingsOutputTypeDef
+):
+    pass
+
 _RequiredArchiveGroupSettingsTypeDef = TypedDict(
     "_RequiredArchiveGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalArchiveGroupSettingsTypeDef = TypedDict(
@@ -3879,14 +5357,34 @@
 )
 
 class ArchiveGroupSettingsTypeDef(
     _RequiredArchiveGroupSettingsTypeDef, _OptionalArchiveGroupSettingsTypeDef
 ):
     pass
 
+_RequiredRemixSettingsOutputTypeDef = TypedDict(
+    "_RequiredRemixSettingsOutputTypeDef",
+    {
+        "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
+    },
+)
+_OptionalRemixSettingsOutputTypeDef = TypedDict(
+    "_OptionalRemixSettingsOutputTypeDef",
+    {
+        "ChannelsIn": int,
+        "ChannelsOut": int,
+    },
+    total=False,
+)
+
+class RemixSettingsOutputTypeDef(
+    _RequiredRemixSettingsOutputTypeDef, _OptionalRemixSettingsOutputTypeDef
+):
+    pass
+
 _RequiredRemixSettingsTypeDef = TypedDict(
     "_RequiredRemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
     },
 )
 _OptionalRemixSettingsTypeDef = TypedDict(
@@ -3897,14 +5395,77 @@
     },
     total=False,
 )
 
 class RemixSettingsTypeDef(_RequiredRemixSettingsTypeDef, _OptionalRemixSettingsTypeDef):
     pass
 
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "AribDestinationSettings": Dict[str, Any],
+        "BurnInDestinationSettings": BurnInDestinationSettingsOutputTypeDef,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
+        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsOutputTypeDef,
+        "EmbeddedDestinationSettings": Dict[str, Any],
+        "EmbeddedPlusScte20DestinationSettings": Dict[str, Any],
+        "RtmpCaptionInfoDestinationSettings": Dict[str, Any],
+        "Scte20PlusEmbeddedDestinationSettings": Dict[str, Any],
+        "Scte27DestinationSettings": Dict[str, Any],
+        "SmpteTtDestinationSettings": Dict[str, Any],
+        "TeletextDestinationSettings": Dict[str, Any],
+        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+GlobalConfigurationOutputTypeDef = TypedDict(
+    "GlobalConfigurationOutputTypeDef",
+    {
+        "InitialAudioGain": int,
+        "InputEndAction": GlobalConfigurationInputEndActionType,
+        "InputLossBehavior": InputLossBehaviorOutputTypeDef,
+        "OutputLockingMode": GlobalConfigurationOutputLockingModeType,
+        "OutputTimingSource": GlobalConfigurationOutputTimingSourceType,
+        "SupportLowFramerateInputs": GlobalConfigurationLowFramerateInputsType,
+    },
+    total=False,
+)
+
+KeyProviderSettingsOutputTypeDef = TypedDict(
+    "KeyProviderSettingsOutputTypeDef",
+    {
+        "StaticKeySettings": StaticKeySettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+AudioSelectorSettingsOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsOutputTypeDef",
+    {
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionOutputTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionOutputTypeDef,
+        "AudioPidSelection": AudioPidSelectionOutputTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+AudioSelectorSettingsTypeDef = TypedDict(
+    "AudioSelectorSettingsTypeDef",
+    {
+        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
+        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
+        "AudioPidSelection": AudioPidSelectionTypeDef,
+        "AudioTrackSelection": AudioTrackSelectionTypeDef,
+    },
+    total=False,
+)
+
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "AribDestinationSettings": Mapping[str, Any],
         "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
@@ -3938,33 +5499,44 @@
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": StaticKeySettingsTypeDef,
     },
     total=False,
 )
 
-AudioSelectorSettingsTypeDef = TypedDict(
-    "AudioSelectorSettingsTypeDef",
+AvailConfigurationOutputTypeDef = TypedDict(
+    "AvailConfigurationOutputTypeDef",
     {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
-        "AudioPidSelection": AudioPidSelectionTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionTypeDef,
+        "AvailSettings": AvailSettingsOutputTypeDef,
     },
     total=False,
 )
 
 AvailConfigurationTypeDef = TypedDict(
     "AvailConfigurationTypeDef",
     {
         "AvailSettings": AvailSettingsTypeDef,
     },
     total=False,
 )
 
+CaptionSelectorSettingsOutputTypeDef = TypedDict(
+    "CaptionSelectorSettingsOutputTypeDef",
+    {
+        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "AribSourceSettings": Dict[str, Any],
+        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
+        "Scte20SourceSettings": Scte20SourceSettingsOutputTypeDef,
+        "Scte27SourceSettings": Scte27SourceSettingsOutputTypeDef,
+        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 CaptionSelectorSettingsTypeDef = TypedDict(
     "CaptionSelectorSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "AribSourceSettings": Mapping[str, Any],
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
         "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
@@ -3976,102 +5548,129 @@
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReservationResponseTypeDef = TypedDict(
     "UpdateReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInputSecurityGroupResponseTypeDef = TypedDict(
     "CreateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ArchiveContainerSettingsOutputTypeDef = TypedDict(
+    "ArchiveContainerSettingsOutputTypeDef",
+    {
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
+        "RawSettings": Dict[str, Any],
     },
+    total=False,
 )
 
-ArchiveContainerSettingsTypeDef = TypedDict(
-    "ArchiveContainerSettingsTypeDef",
+UdpContainerSettingsOutputTypeDef = TypedDict(
+    "UdpContainerSettingsOutputTypeDef",
     {
-        "M2tsSettings": M2tsSettingsTypeDef,
-        "RawSettings": Mapping[str, Any],
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
     },
     total=False,
 )
 
-UdpContainerSettingsTypeDef = TypedDict(
-    "UdpContainerSettingsTypeDef",
+FailoverConditionOutputTypeDef = TypedDict(
+    "FailoverConditionOutputTypeDef",
     {
-        "M2tsSettings": M2tsSettingsTypeDef,
+        "FailoverConditionSettings": FailoverConditionSettingsOutputTypeDef,
     },
     total=False,
 )
 
 FailoverConditionTypeDef = TypedDict(
     "FailoverConditionTypeDef",
     {
         "FailoverConditionSettings": FailoverConditionSettingsTypeDef,
     },
     total=False,
 )
 
+_RequiredFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredFrameCaptureGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalFrameCaptureGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalFrameCaptureGroupSettingsOutputTypeDef",
+    {
+        "FrameCaptureCdnSettings": FrameCaptureCdnSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class FrameCaptureGroupSettingsOutputTypeDef(
+    _RequiredFrameCaptureGroupSettingsOutputTypeDef, _OptionalFrameCaptureGroupSettingsOutputTypeDef
+):
+    pass
+
 _RequiredFrameCaptureGroupSettingsTypeDef = TypedDict(
     "_RequiredFrameCaptureGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalFrameCaptureGroupSettingsTypeDef = TypedDict(
@@ -4083,14 +5682,97 @@
 )
 
 class FrameCaptureGroupSettingsTypeDef(
     _RequiredFrameCaptureGroupSettingsTypeDef, _OptionalFrameCaptureGroupSettingsTypeDef
 ):
     pass
 
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H264AdaptiveQuantizationType,
+        "AfdSignaling": AfdSignalingType,
+        "Bitrate": int,
+        "BufFillPct": int,
+        "BufSize": int,
+        "ColorMetadata": H264ColorMetadataType,
+        "ColorSpaceSettings": H264ColorSpaceSettingsOutputTypeDef,
+        "EntropyEncoding": H264EntropyEncodingType,
+        "FilterSettings": H264FilterSettingsOutputTypeDef,
+        "FixedAfd": FixedAfdType,
+        "FlickerAq": H264FlickerAqType,
+        "ForceFieldPictures": H264ForceFieldPicturesType,
+        "FramerateControl": H264FramerateControlType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H264GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopNumBFrames": int,
+        "GopSize": float,
+        "GopSizeUnits": H264GopSizeUnitsType,
+        "Level": H264LevelType,
+        "LookAheadRateControl": H264LookAheadRateControlType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumRefFrames": int,
+        "ParControl": H264ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "Profile": H264ProfileType,
+        "QualityLevel": H264QualityLevelType,
+        "QvbrQualityLevel": int,
+        "RateControlMode": H264RateControlModeType,
+        "ScanType": H264ScanTypeType,
+        "SceneChangeDetect": H264SceneChangeDetectType,
+        "Slices": int,
+        "Softness": int,
+        "SpatialAq": H264SpatialAqType,
+        "SubgopLength": H264SubGopLengthType,
+        "Syntax": H264SyntaxType,
+        "TemporalAq": H264TemporalAqType,
+        "TimecodeInsertion": H264TimecodeInsertionBehaviorType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredMpeg2SettingsOutputTypeDef = TypedDict(
+    "_RequiredMpeg2SettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+_OptionalMpeg2SettingsOutputTypeDef = TypedDict(
+    "_OptionalMpeg2SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
+        "AfdSignaling": AfdSignalingType,
+        "ColorMetadata": Mpeg2ColorMetadataType,
+        "ColorSpace": Mpeg2ColorSpaceType,
+        "DisplayAspectRatio": Mpeg2DisplayRatioType,
+        "FilterSettings": Mpeg2FilterSettingsOutputTypeDef,
+        "FixedAfd": FixedAfdType,
+        "GopClosedCadence": int,
+        "GopNumBFrames": int,
+        "GopSize": float,
+        "GopSizeUnits": Mpeg2GopSizeUnitsType,
+        "ScanType": Mpeg2ScanTypeType,
+        "SubgopLength": Mpeg2SubGopLengthType,
+        "TimecodeInsertion": Mpeg2TimecodeInsertionBehaviorType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class Mpeg2SettingsOutputTypeDef(
+    _RequiredMpeg2SettingsOutputTypeDef, _OptionalMpeg2SettingsOutputTypeDef
+):
+    pass
+
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
@@ -4164,14 +5846,61 @@
     },
     total=False,
 )
 
 class Mpeg2SettingsTypeDef(_RequiredMpeg2SettingsTypeDef, _OptionalMpeg2SettingsTypeDef):
     pass
 
+_RequiredH265SettingsOutputTypeDef = TypedDict(
+    "_RequiredH265SettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+_OptionalH265SettingsOutputTypeDef = TypedDict(
+    "_OptionalH265SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H265AdaptiveQuantizationType,
+        "AfdSignaling": AfdSignalingType,
+        "AlternativeTransferFunction": H265AlternativeTransferFunctionType,
+        "Bitrate": int,
+        "BufSize": int,
+        "ColorMetadata": H265ColorMetadataType,
+        "ColorSpaceSettings": H265ColorSpaceSettingsOutputTypeDef,
+        "FilterSettings": H265FilterSettingsOutputTypeDef,
+        "FixedAfd": FixedAfdType,
+        "FlickerAq": H265FlickerAqType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H265GopSizeUnitsType,
+        "Level": H265LevelType,
+        "LookAheadRateControl": H265LookAheadRateControlType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "Profile": H265ProfileType,
+        "QvbrQualityLevel": int,
+        "RateControlMode": H265RateControlModeType,
+        "ScanType": H265ScanTypeType,
+        "SceneChangeDetect": H265SceneChangeDetectType,
+        "Slices": int,
+        "Tier": H265TierType,
+        "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
+        "TimecodeBurninSettings": TimecodeBurninSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class H265SettingsOutputTypeDef(
+    _RequiredH265SettingsOutputTypeDef, _OptionalH265SettingsOutputTypeDef
+):
+    pass
+
 _RequiredH265SettingsTypeDef = TypedDict(
     "_RequiredH265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -4209,14 +5938,45 @@
     },
     total=False,
 )
 
 class H265SettingsTypeDef(_RequiredH265SettingsTypeDef, _OptionalH265SettingsTypeDef):
     pass
 
+InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "UrlPath": List[str],
+    },
+    total=False,
+)
+
+_RequiredInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_RequiredInputSwitchScheduleActionSettingsOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+    },
+)
+_OptionalInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
+    "_OptionalInputSwitchScheduleActionSettingsOutputTypeDef",
+    {
+        "InputClippingSettings": InputClippingSettingsOutputTypeDef,
+        "UrlPath": List[str],
+    },
+    total=False,
+)
+
+class InputSwitchScheduleActionSettingsOutputTypeDef(
+    _RequiredInputSwitchScheduleActionSettingsOutputTypeDef,
+    _OptionalInputSwitchScheduleActionSettingsOutputTypeDef,
+):
+    pass
+
 InputPrepareScheduleActionSettingsTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
         "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": Sequence[str],
     },
@@ -4248,105 +6008,105 @@
     "DescribeInputResponseTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsTypeDef],
+        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
         "Arn": str,
         "AttachedChannels": List[str],
         "Destinations": List[InputDestinationTypeDef],
         "Id": str,
         "InputClass": InputClassType,
-        "InputDevices": List[InputDeviceSettingsTypeDef],
+        "InputDevices": List[InputDeviceSettingsOutputTypeDef],
         "InputPartnerIds": List[str],
         "InputSourceType": InputSourceTypeType,
         "MediaConnectFlows": List[MediaConnectFlowTypeDef],
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
     },
     total=False,
 )
 
-HlsSettingsTypeDef = TypedDict(
-    "HlsSettingsTypeDef",
+HlsSettingsOutputTypeDef = TypedDict(
+    "HlsSettingsOutputTypeDef",
     {
-        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsTypeDef,
-        "Fmp4HlsSettings": Fmp4HlsSettingsTypeDef,
-        "FrameCaptureHlsSettings": Mapping[str, Any],
-        "StandardHlsSettings": StandardHlsSettingsTypeDef,
+        "AudioOnlyHlsSettings": AudioOnlyHlsSettingsOutputTypeDef,
+        "Fmp4HlsSettings": Fmp4HlsSettingsOutputTypeDef,
+        "FrameCaptureHlsSettings": Dict[str, Any],
+        "StandardHlsSettings": StandardHlsSettingsOutputTypeDef,
     },
     total=False,
 )
 
 DeleteMultiplexResponseTypeDef = TypedDict(
     "DeleteMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexResponseTypeDef = TypedDict(
     "DescribeMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexTypeDef = TypedDict(
     "MultiplexTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
     },
     total=False,
@@ -4355,50 +6115,71 @@
 StartMultiplexResponseTypeDef = TypedDict(
     "StartMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopMultiplexResponseTypeDef = TypedDict(
     "StopMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
-        "MultiplexSettings": MultiplexSettingsTypeDef,
+        "MultiplexSettings": MultiplexSettingsOutputTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMultiplexProgramSettingsOutputTypeDef = TypedDict(
+    "_RequiredMultiplexProgramSettingsOutputTypeDef",
+    {
+        "ProgramNumber": int,
+    },
+)
+_OptionalMultiplexProgramSettingsOutputTypeDef = TypedDict(
+    "_OptionalMultiplexProgramSettingsOutputTypeDef",
+    {
+        "PreferredChannelPipeline": PreferredChannelPipelineType,
+        "ServiceDescriptor": MultiplexProgramServiceDescriptorOutputTypeDef,
+        "VideoSettings": MultiplexVideoSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class MultiplexProgramSettingsOutputTypeDef(
+    _RequiredMultiplexProgramSettingsOutputTypeDef, _OptionalMultiplexProgramSettingsOutputTypeDef
+):
+    pass
+
 _RequiredMultiplexProgramSettingsTypeDef = TypedDict(
     "_RequiredMultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
     },
 )
 _OptionalMultiplexProgramSettingsTypeDef = TypedDict(
@@ -4412,14 +6193,22 @@
 )
 
 class MultiplexProgramSettingsTypeDef(
     _RequiredMultiplexProgramSettingsTypeDef, _OptionalMultiplexProgramSettingsTypeDef
 ):
     pass
 
+AudioWatermarkSettingsOutputTypeDef = TypedDict(
+    "AudioWatermarkSettingsOutputTypeDef",
+    {
+        "NielsenWatermarksSettings": NielsenWatermarksSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AudioWatermarkSettingsTypeDef = TypedDict(
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
 )
@@ -4441,40 +6230,177 @@
 
 class UpdateChannelClassRequestRequestTypeDef(
     _RequiredUpdateChannelClassRequestRequestTypeDef,
     _OptionalUpdateChannelClassRequestRequestTypeDef,
 ):
     pass
 
+Scte35DescriptorSettingsOutputTypeDef = TypedDict(
+    "Scte35DescriptorSettingsOutputTypeDef",
+    {
+        "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorOutputTypeDef,
+    },
+)
+
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
 DescribeThumbnailsResponseTypeDef = TypedDict(
     "DescribeThumbnailsResponseTypeDef",
     {
         "ThumbnailDetails": List[ThumbnailDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+VideoSelectorOutputTypeDef = TypedDict(
+    "VideoSelectorOutputTypeDef",
+    {
+        "ColorSpace": VideoSelectorColorSpaceType,
+        "ColorSpaceSettings": VideoSelectorColorSpaceSettingsOutputTypeDef,
+        "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
+        "SelectorSettings": VideoSelectorSettingsOutputTypeDef,
     },
+    total=False,
 )
 
 VideoSelectorTypeDef = TypedDict(
     "VideoSelectorTypeDef",
     {
         "ColorSpace": VideoSelectorColorSpaceType,
         "ColorSpaceSettings": VideoSelectorColorSpaceSettingsTypeDef,
         "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
         "SelectorSettings": VideoSelectorSettingsTypeDef,
     },
     total=False,
 )
 
+_RequiredCaptionDescriptionOutputTypeDef = TypedDict(
+    "_RequiredCaptionDescriptionOutputTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "Name": str,
+    },
+)
+_OptionalCaptionDescriptionOutputTypeDef = TypedDict(
+    "_OptionalCaptionDescriptionOutputTypeDef",
+    {
+        "Accessibility": AccessibilityTypeType,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": str,
+        "LanguageDescription": str,
+    },
+    total=False,
+)
+
+class CaptionDescriptionOutputTypeDef(
+    _RequiredCaptionDescriptionOutputTypeDef, _OptionalCaptionDescriptionOutputTypeDef
+):
+    pass
+
+_RequiredHlsGroupSettingsOutputTypeDef = TypedDict(
+    "_RequiredHlsGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefOutputTypeDef,
+    },
+)
+_OptionalHlsGroupSettingsOutputTypeDef = TypedDict(
+    "_OptionalHlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "BaseUrlContent": str,
+        "BaseUrlContent1": str,
+        "BaseUrlManifest": str,
+        "BaseUrlManifest1": str,
+        "CaptionLanguageMappings": List[CaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "ConstantIv": str,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "DiscontinuityTags": HlsDiscontinuityTagsType,
+        "EncryptionType": HlsEncryptionTypeType,
+        "HlsCdnSettings": HlsCdnSettingsOutputTypeDef,
+        "HlsId3SegmentTagging": HlsId3SegmentTaggingStateType,
+        "IFrameOnlyPlaylists": IFrameOnlyPlaylistTypeType,
+        "IncompleteSegmentBehavior": HlsIncompleteSegmentBehaviorType,
+        "IndexNSegments": int,
+        "InputLossAction": InputLossActionForHlsOutType,
+        "IvInManifest": HlsIvInManifestType,
+        "IvSource": HlsIvSourceType,
+        "KeepSegments": int,
+        "KeyFormat": str,
+        "KeyFormatVersions": str,
+        "KeyProviderSettings": KeyProviderSettingsOutputTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinSegmentLength": int,
+        "Mode": HlsModeType,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimeClock": HlsProgramDateTimeClockType,
+        "ProgramDateTimePeriod": int,
+        "RedundantManifest": HlsRedundantManifestType,
+        "SegmentLength": int,
+        "SegmentationMode": HlsSegmentationModeType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+        "TsFileMode": HlsTsFileModeType,
+    },
+    total=False,
+)
+
+class HlsGroupSettingsOutputTypeDef(
+    _RequiredHlsGroupSettingsOutputTypeDef, _OptionalHlsGroupSettingsOutputTypeDef
+):
+    pass
+
+_RequiredAudioSelectorOutputTypeDef = TypedDict(
+    "_RequiredAudioSelectorOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorOutputTypeDef = TypedDict(
+    "_OptionalAudioSelectorOutputTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class AudioSelectorOutputTypeDef(
+    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
+):
+    pass
+
+_RequiredAudioSelectorTypeDef = TypedDict(
+    "_RequiredAudioSelectorTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAudioSelectorTypeDef = TypedDict(
+    "_OptionalAudioSelectorTypeDef",
+    {
+        "SelectorSettings": AudioSelectorSettingsTypeDef,
+    },
+    total=False,
+)
+
+class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
+    pass
+
 _RequiredCaptionDescriptionTypeDef = TypedDict(
     "_RequiredCaptionDescriptionTypeDef",
     {
         "CaptionSelectorName": str,
         "Name": str,
     },
 )
@@ -4548,29 +6474,32 @@
     },
     total=False,
 )
 
 class HlsGroupSettingsTypeDef(_RequiredHlsGroupSettingsTypeDef, _OptionalHlsGroupSettingsTypeDef):
     pass
 
-_RequiredAudioSelectorTypeDef = TypedDict(
-    "_RequiredAudioSelectorTypeDef",
+_RequiredCaptionSelectorOutputTypeDef = TypedDict(
+    "_RequiredCaptionSelectorOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalAudioSelectorTypeDef = TypedDict(
-    "_OptionalAudioSelectorTypeDef",
+_OptionalCaptionSelectorOutputTypeDef = TypedDict(
+    "_OptionalCaptionSelectorOutputTypeDef",
     {
-        "SelectorSettings": AudioSelectorSettingsTypeDef,
+        "LanguageCode": str,
+        "SelectorSettings": CaptionSelectorSettingsOutputTypeDef,
     },
     total=False,
 )
 
-class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
+class CaptionSelectorOutputTypeDef(
+    _RequiredCaptionSelectorOutputTypeDef, _OptionalCaptionSelectorOutputTypeDef
+):
     pass
 
 _RequiredCaptionSelectorTypeDef = TypedDict(
     "_RequiredCaptionSelectorTypeDef",
     {
         "Name": str,
     },
@@ -4583,52 +6512,74 @@
     },
     total=False,
 )
 
 class CaptionSelectorTypeDef(_RequiredCaptionSelectorTypeDef, _OptionalCaptionSelectorTypeDef):
     pass
 
-_RequiredArchiveOutputSettingsTypeDef = TypedDict(
-    "_RequiredArchiveOutputSettingsTypeDef",
+_RequiredArchiveOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredArchiveOutputSettingsOutputTypeDef",
     {
-        "ContainerSettings": ArchiveContainerSettingsTypeDef,
+        "ContainerSettings": ArchiveContainerSettingsOutputTypeDef,
     },
 )
-_OptionalArchiveOutputSettingsTypeDef = TypedDict(
-    "_OptionalArchiveOutputSettingsTypeDef",
+_OptionalArchiveOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalArchiveOutputSettingsOutputTypeDef",
     {
         "Extension": str,
         "NameModifier": str,
     },
     total=False,
 )
 
-class ArchiveOutputSettingsTypeDef(
-    _RequiredArchiveOutputSettingsTypeDef, _OptionalArchiveOutputSettingsTypeDef
+class ArchiveOutputSettingsOutputTypeDef(
+    _RequiredArchiveOutputSettingsOutputTypeDef, _OptionalArchiveOutputSettingsOutputTypeDef
 ):
     pass
 
-_RequiredUdpOutputSettingsTypeDef = TypedDict(
-    "_RequiredUdpOutputSettingsTypeDef",
+_RequiredUdpOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredUdpOutputSettingsOutputTypeDef",
     {
-        "ContainerSettings": UdpContainerSettingsTypeDef,
-        "Destination": OutputLocationRefTypeDef,
+        "ContainerSettings": UdpContainerSettingsOutputTypeDef,
+        "Destination": OutputLocationRefOutputTypeDef,
     },
 )
-_OptionalUdpOutputSettingsTypeDef = TypedDict(
-    "_OptionalUdpOutputSettingsTypeDef",
+_OptionalUdpOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalUdpOutputSettingsOutputTypeDef",
     {
         "BufferMsec": int,
-        "FecOutputSettings": FecOutputSettingsTypeDef,
+        "FecOutputSettings": FecOutputSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class UdpOutputSettingsOutputTypeDef(
+    _RequiredUdpOutputSettingsOutputTypeDef, _OptionalUdpOutputSettingsOutputTypeDef
+):
+    pass
+
+_RequiredAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
+    "_RequiredAutomaticInputFailoverSettingsOutputTypeDef",
+    {
+        "SecondaryInputId": str,
+    },
+)
+_OptionalAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
+    "_OptionalAutomaticInputFailoverSettingsOutputTypeDef",
+    {
+        "ErrorClearTimeMsec": int,
+        "FailoverConditions": List[FailoverConditionOutputTypeDef],
+        "InputPreference": InputPreferenceType,
     },
     total=False,
 )
 
-class UdpOutputSettingsTypeDef(
-    _RequiredUdpOutputSettingsTypeDef, _OptionalUdpOutputSettingsTypeDef
+class AutomaticInputFailoverSettingsOutputTypeDef(
+    _RequiredAutomaticInputFailoverSettingsOutputTypeDef,
+    _OptionalAutomaticInputFailoverSettingsOutputTypeDef,
 ):
     pass
 
 _RequiredAutomaticInputFailoverSettingsTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsTypeDef",
     {
         "SecondaryInputId": str,
@@ -4645,14 +6596,25 @@
 )
 
 class AutomaticInputFailoverSettingsTypeDef(
     _RequiredAutomaticInputFailoverSettingsTypeDef, _OptionalAutomaticInputFailoverSettingsTypeDef
 ):
     pass
 
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "H264Settings": H264SettingsOutputTypeDef,
+        "H265Settings": H265SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
         "H264Settings": H264SettingsTypeDef,
         "H265Settings": H265SettingsTypeDef,
         "Mpeg2Settings": Mpeg2SettingsTypeDef,
@@ -4660,126 +6622,126 @@
     total=False,
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePartnerInputResponseTypeDef = TypedDict(
     "CreatePartnerInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredHlsOutputSettingsTypeDef = TypedDict(
-    "_RequiredHlsOutputSettingsTypeDef",
+_RequiredHlsOutputSettingsOutputTypeDef = TypedDict(
+    "_RequiredHlsOutputSettingsOutputTypeDef",
     {
-        "HlsSettings": HlsSettingsTypeDef,
+        "HlsSettings": HlsSettingsOutputTypeDef,
     },
 )
-_OptionalHlsOutputSettingsTypeDef = TypedDict(
-    "_OptionalHlsOutputSettingsTypeDef",
+_OptionalHlsOutputSettingsOutputTypeDef = TypedDict(
+    "_OptionalHlsOutputSettingsOutputTypeDef",
     {
         "H265PackagingType": HlsH265PackagingTypeType,
         "NameModifier": str,
         "SegmentModifier": str,
     },
     total=False,
 )
 
-class HlsOutputSettingsTypeDef(
-    _RequiredHlsOutputSettingsTypeDef, _OptionalHlsOutputSettingsTypeDef
+class HlsOutputSettingsOutputTypeDef(
+    _RequiredHlsOutputSettingsOutputTypeDef, _OptionalHlsOutputSettingsOutputTypeDef
 ):
     pass
 
 CreateMultiplexResponseTypeDef = TypedDict(
     "CreateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexResponseTypeDef = TypedDict(
     "UpdateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
-    "CreateMultiplexProgramRequestRequestTypeDef",
-    {
-        "MultiplexId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
-        "ProgramName": str,
-        "RequestId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMultiplexProgramResponseTypeDef = TypedDict(
     "DeleteMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexProgramResponseTypeDef = TypedDict(
     "DescribeMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexProgramTypeDef = TypedDict(
     "MultiplexProgramTypeDef",
     {
         "ChannelId": str,
-        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "MultiplexProgramSettings": MultiplexProgramSettingsOutputTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
     },
     total=False,
 )
 
+CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
+    "CreateMultiplexProgramRequestRequestTypeDef",
+    {
+        "MultiplexId": str,
+        "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
+        "ProgramName": str,
+        "RequestId": str,
+    },
+)
+
 _RequiredUpdateMultiplexProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
     },
 )
@@ -4793,14 +6755,42 @@
 
 class UpdateMultiplexProgramRequestRequestTypeDef(
     _RequiredUpdateMultiplexProgramRequestRequestTypeDef,
     _OptionalUpdateMultiplexProgramRequestRequestTypeDef,
 ):
     pass
 
+_RequiredAudioDescriptionOutputTypeDef = TypedDict(
+    "_RequiredAudioDescriptionOutputTypeDef",
+    {
+        "AudioSelectorName": str,
+        "Name": str,
+    },
+)
+_OptionalAudioDescriptionOutputTypeDef = TypedDict(
+    "_OptionalAudioDescriptionOutputTypeDef",
+    {
+        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
+        "AudioType": AudioTypeType,
+        "AudioTypeControl": AudioDescriptionAudioTypeControlType,
+        "AudioWatermarkingSettings": AudioWatermarkSettingsOutputTypeDef,
+        "CodecSettings": AudioCodecSettingsOutputTypeDef,
+        "LanguageCode": str,
+        "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "StreamName": str,
+    },
+    total=False,
+)
+
+class AudioDescriptionOutputTypeDef(
+    _RequiredAudioDescriptionOutputTypeDef, _OptionalAudioDescriptionOutputTypeDef
+):
+    pass
+
 _RequiredAudioDescriptionTypeDef = TypedDict(
     "_RequiredAudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
@@ -4819,21 +6809,43 @@
     },
     total=False,
 )
 
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
+Scte35DescriptorOutputTypeDef = TypedDict(
+    "Scte35DescriptorOutputTypeDef",
+    {
+        "Scte35DescriptorSettings": Scte35DescriptorSettingsOutputTypeDef,
+    },
+)
+
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "ArchiveGroupSettings": ArchiveGroupSettingsOutputTypeDef,
+        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsOutputTypeDef,
+        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
+        "MediaPackageGroupSettings": MediaPackageGroupSettingsOutputTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "MultiplexGroupSettings": Dict[str, Any],
+        "RtmpGroupSettings": RtmpGroupSettingsOutputTypeDef,
+        "UdpGroupSettings": UdpGroupSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
         "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
@@ -4841,14 +6853,32 @@
         "MultiplexGroupSettings": Mapping[str, Any],
         "RtmpGroupSettings": RtmpGroupSettingsTypeDef,
         "UdpGroupSettings": UdpGroupSettingsTypeDef,
     },
     total=False,
 )
 
+InputSettingsOutputTypeDef = TypedDict(
+    "InputSettingsOutputTypeDef",
+    {
+        "AudioSelectors": List[AudioSelectorOutputTypeDef],
+        "CaptionSelectors": List[CaptionSelectorOutputTypeDef],
+        "DeblockFilter": InputDeblockFilterType,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "FilterStrength": int,
+        "InputFilter": InputFilterType,
+        "NetworkInputSettings": NetworkInputSettingsOutputTypeDef,
+        "Scte35Pid": int,
+        "Smpte2038DataPreference": Smpte2038DataPreferenceType,
+        "SourceEndBehavior": InputSourceEndBehaviorType,
+        "VideoSelector": VideoSelectorOutputTypeDef,
+    },
+    total=False,
+)
+
 InputSettingsTypeDef = TypedDict(
     "InputSettingsTypeDef",
     {
         "AudioSelectors": Sequence[AudioSelectorTypeDef],
         "CaptionSelectors": Sequence[CaptionSelectorTypeDef],
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
@@ -4859,14 +6889,38 @@
         "Smpte2038DataPreference": Smpte2038DataPreferenceType,
         "SourceEndBehavior": InputSourceEndBehaviorType,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
+_RequiredVideoDescriptionOutputTypeDef = TypedDict(
+    "_RequiredVideoDescriptionOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalVideoDescriptionOutputTypeDef = TypedDict(
+    "_OptionalVideoDescriptionOutputTypeDef",
+    {
+        "CodecSettings": VideoCodecSettingsOutputTypeDef,
+        "Height": int,
+        "RespondToAfd": VideoDescriptionRespondToAfdType,
+        "ScalingBehavior": VideoDescriptionScalingBehaviorType,
+        "Sharpness": int,
+        "Width": int,
+    },
+    total=False,
+)
+
+class VideoDescriptionOutputTypeDef(
+    _RequiredVideoDescriptionOutputTypeDef, _OptionalVideoDescriptionOutputTypeDef
+):
+    pass
+
 _RequiredVideoDescriptionTypeDef = TypedDict(
     "_RequiredVideoDescriptionTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVideoDescriptionTypeDef = TypedDict(
@@ -4881,83 +6935,123 @@
     },
     total=False,
 )
 
 class VideoDescriptionTypeDef(_RequiredVideoDescriptionTypeDef, _OptionalVideoDescriptionTypeDef):
     pass
 
-OutputSettingsTypeDef = TypedDict(
-    "OutputSettingsTypeDef",
+OutputSettingsOutputTypeDef = TypedDict(
+    "OutputSettingsOutputTypeDef",
     {
-        "ArchiveOutputSettings": ArchiveOutputSettingsTypeDef,
-        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsTypeDef,
-        "HlsOutputSettings": HlsOutputSettingsTypeDef,
-        "MediaPackageOutputSettings": Mapping[str, Any],
-        "MsSmoothOutputSettings": MsSmoothOutputSettingsTypeDef,
-        "MultiplexOutputSettings": MultiplexOutputSettingsTypeDef,
-        "RtmpOutputSettings": RtmpOutputSettingsTypeDef,
-        "UdpOutputSettings": UdpOutputSettingsTypeDef,
+        "ArchiveOutputSettings": ArchiveOutputSettingsOutputTypeDef,
+        "FrameCaptureOutputSettings": FrameCaptureOutputSettingsOutputTypeDef,
+        "HlsOutputSettings": HlsOutputSettingsOutputTypeDef,
+        "MediaPackageOutputSettings": Dict[str, Any],
+        "MsSmoothOutputSettings": MsSmoothOutputSettingsOutputTypeDef,
+        "MultiplexOutputSettings": MultiplexOutputSettingsOutputTypeDef,
+        "RtmpOutputSettings": RtmpOutputSettingsOutputTypeDef,
+        "UdpOutputSettings": UdpOutputSettingsOutputTypeDef,
     },
     total=False,
 )
 
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
+    {
+        "Scte35Descriptors": List[Scte35DescriptorOutputTypeDef],
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
     },
 )
 
+InputAttachmentOutputTypeDef = TypedDict(
+    "InputAttachmentOutputTypeDef",
+    {
+        "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsOutputTypeDef,
+        "InputAttachmentName": str,
+        "InputId": str,
+        "InputSettings": InputSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 InputAttachmentTypeDef = TypedDict(
     "InputAttachmentTypeDef",
     {
         "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsTypeDef,
         "InputAttachmentName": str,
         "InputId": str,
         "InputSettings": InputSettingsTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
-        "OutputSettings": OutputSettingsTypeDef,
+        "OutputSettings": OutputSettingsOutputTypeDef,
     },
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
-        "AudioDescriptionNames": Sequence[str],
-        "CaptionDescriptionNames": Sequence[str],
+        "AudioDescriptionNames": List[str],
+        "CaptionDescriptionNames": List[str],
         "OutputName": str,
         "VideoDescriptionName": str,
     },
     total=False,
 )
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
+ScheduleActionSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionSettingsOutputTypeDef",
+    {
+        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
+        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
+        "InputPrepareSettings": InputPrepareScheduleActionSettingsOutputTypeDef,
+        "InputSwitchSettings": InputSwitchScheduleActionSettingsOutputTypeDef,
+        "MotionGraphicsImageActivateSettings": (
+            MotionGraphicsActivateScheduleActionSettingsOutputTypeDef
+        ),
+        "MotionGraphicsImageDeactivateSettings": Dict[str, Any],
+        "PauseStateSettings": PauseStateScheduleActionSettingsOutputTypeDef,
+        "Scte35InputSettings": Scte35InputScheduleActionSettingsOutputTypeDef,
+        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
+        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+        "Scte35TimeSignalSettings": Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
+        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsOutputTypeDef,
+        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
         "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
         "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
         "InputPrepareSettings": InputPrepareScheduleActionSettingsTypeDef,
         "InputSwitchSettings": InputSwitchScheduleActionSettingsTypeDef,
@@ -4974,33 +7068,53 @@
     total=False,
 )
 
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
+_RequiredOutputGroupOutputTypeDef = TypedDict(
+    "_RequiredOutputGroupOutputTypeDef",
+    {
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
+    },
+)
+_OptionalOutputGroupOutputTypeDef = TypedDict(
+    "_OptionalOutputGroupOutputTypeDef",
+    {
+        "Name": str,
+    },
+    total=False,
+)
+
+class OutputGroupOutputTypeDef(
+    _RequiredOutputGroupOutputTypeDef, _OptionalOutputGroupOutputTypeDef
+):
+    pass
+
 _RequiredOutputGroupTypeDef = TypedDict(
     "_RequiredOutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
 )
@@ -5011,32 +7125,71 @@
     },
     total=False,
 )
 
 class OutputGroupTypeDef(_RequiredOutputGroupTypeDef, _OptionalOutputGroupTypeDef):
     pass
 
+ScheduleActionOutputTypeDef = TypedDict(
+    "ScheduleActionOutputTypeDef",
+    {
+        "ActionName": str,
+        "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
+        "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
+    },
+)
+
 ScheduleActionTypeDef = TypedDict(
     "ScheduleActionTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEncoderSettingsOutputTypeDef = TypedDict(
+    "_RequiredEncoderSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
+    },
+)
+_OptionalEncoderSettingsOutputTypeDef = TypedDict(
+    "_OptionalEncoderSettingsOutputTypeDef",
+    {
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "AvailConfiguration": AvailConfigurationOutputTypeDef,
+        "BlackoutSlate": BlackoutSlateOutputTypeDef,
+        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
+        "FeatureActivations": FeatureActivationsOutputTypeDef,
+        "GlobalConfiguration": GlobalConfigurationOutputTypeDef,
+        "MotionGraphicsConfiguration": MotionGraphicsConfigurationOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "ThumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class EncoderSettingsOutputTypeDef(
+    _RequiredEncoderSettingsOutputTypeDef, _OptionalEncoderSettingsOutputTypeDef
+):
+    pass
+
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": Sequence[VideoDescriptionTypeDef],
@@ -5057,190 +7210,190 @@
     },
     total=False,
 )
 
 class EncoderSettingsTypeDef(_RequiredEncoderSettingsTypeDef, _OptionalEncoderSettingsTypeDef):
     pass
 
-BatchScheduleActionCreateRequestTypeDef = TypedDict(
-    "BatchScheduleActionCreateRequestTypeDef",
-    {
-        "ScheduleActions": Sequence[ScheduleActionTypeDef],
-    },
-)
-
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 
 BatchScheduleActionDeleteResultTypeDef = TypedDict(
     "BatchScheduleActionDeleteResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
-        "ScheduleActions": List[ScheduleActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchScheduleActionCreateRequestTypeDef = TypedDict(
+    "BatchScheduleActionCreateRequestTypeDef",
+    {
+        "ScheduleActions": Sequence[ScheduleActionTypeDef],
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
-CreateChannelRequestRequestTypeDef = TypedDict(
-    "CreateChannelRequestRequestTypeDef",
-    {
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[OutputDestinationTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
-        "LogLevel": LogLevelType,
-        "Maintenance": MaintenanceCreateSettingsTypeDef,
-        "Name": str,
-        "RequestId": str,
-        "Reserved": str,
-        "RoleArn": str,
-        "Tags": Mapping[str, str],
-        "Vpc": VpcOutputSettingsTypeDef,
-    },
-    total=False,
-)
-
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "CdiInputSpecification": CdiInputSpecificationOutputTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputSpecification": InputSpecificationOutputTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateChannelRequestRequestTypeDef = TypedDict(
+    "CreateChannelRequestRequestTypeDef",
+    {
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "ChannelClass": ChannelClassType,
+        "Destinations": Sequence[OutputDestinationTypeDef],
+        "EncoderSettings": EncoderSettingsTypeDef,
+        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputSpecification": InputSpecificationTypeDef,
+        "LogLevel": LogLevelType,
+        "Maintenance": MaintenanceCreateSettingsTypeDef,
+        "Name": str,
+        "RequestId": str,
+        "Reserved": str,
+        "RoleArn": str,
+        "Tags": Mapping[str, str],
+        "Vpc": VpcOutputSettingsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -5260,14 +7413,23 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+BatchUpdateScheduleResponseTypeDef = TypedDict(
+    "BatchUpdateScheduleResponseTypeDef",
+    {
+        "Creates": BatchScheduleActionCreateResultTypeDef,
+        "Deletes": BatchScheduleActionDeleteResultTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
@@ -5281,39 +7443,30 @@
 
 class BatchUpdateScheduleRequestRequestTypeDef(
     _RequiredBatchUpdateScheduleRequestRequestTypeDef,
     _OptionalBatchUpdateScheduleRequestRequestTypeDef,
 ):
     pass
 
-BatchUpdateScheduleResponseTypeDef = TypedDict(
-    "BatchUpdateScheduleResponseTypeDef",
-    {
-        "Creates": BatchScheduleActionCreateResultTypeDef,
-        "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelClassResponseTypeDef = TypedDict(
     "UpdateChannelClassResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive/waiter.pyi` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.28.12/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-medialive
-Version: 1.28.1
-Summary: Type annotations for boto3.MediaLive 1.28.1 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 medialive type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-medialive?color=blue)](https://pypistats.org/packages/mypy-boto3-medialive)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -674,61 +642,93 @@
 ### Typed dictionaries
 
 `mypy_boto3_medialive.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_medialive.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
     AcceptInputDeviceTransferRequestRequestTypeDef,
+    AccountConfigurationOutputTypeDef,
     AccountConfigurationTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
+    ArchiveS3SettingsOutputTypeDef,
     ArchiveS3SettingsTypeDef,
+    OutputLocationRefOutputTypeDef,
     OutputLocationRefTypeDef,
+    InputChannelLevelOutputTypeDef,
     InputChannelLevelTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioDolbyEDecodeOutputTypeDef,
     AudioDolbyEDecodeTypeDef,
+    AudioHlsRenditionSelectionOutputTypeDef,
     AudioHlsRenditionSelectionTypeDef,
+    AudioLanguageSelectionOutputTypeDef,
     AudioLanguageSelectionTypeDef,
-    InputLocationTypeDef,
+    InputLocationOutputTypeDef,
+    AudioPidSelectionOutputTypeDef,
     AudioPidSelectionTypeDef,
+    AudioSilenceFailoverSettingsOutputTypeDef,
     AudioSilenceFailoverSettingsTypeDef,
+    AudioTrackOutputTypeDef,
     AudioTrackTypeDef,
+    InputLocationTypeDef,
+    EsamOutputTypeDef,
+    Scte35SpliceInsertOutputTypeDef,
+    Scte35TimeSignalAposOutputTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
-    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
+    EbuTtDDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    CaptionLanguageMappingOutputTypeDef,
     CaptionLanguageMappingTypeDef,
+    CaptionRectangleOutputTypeDef,
     CaptionRectangleTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    Scte20SourceSettingsOutputTypeDef,
+    Scte27SourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     Scte20SourceSettingsTypeDef,
     Scte27SourceSettingsTypeDef,
+    CdiInputSpecificationOutputTypeDef,
     CdiInputSpecificationTypeDef,
     ChannelEgressEndpointTypeDef,
-    InputSpecificationTypeDef,
+    InputSpecificationOutputTypeDef,
     MaintenanceStatusTypeDef,
     VpcOutputSettingsDescriptionTypeDef,
     PipelineDetailTypeDef,
     ClaimDeviceRequestRequestTypeDef,
+    InputSpecificationTypeDef,
     MaintenanceCreateSettingsTypeDef,
     VpcOutputSettingsTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputVpcRequestTypeDef,
     MediaConnectFlowRequestTypeDef,
@@ -739,149 +739,218 @@
     DeleteChannelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DeleteInputSecurityGroupRequestRequestTypeDef,
     DeleteMultiplexProgramRequestRequestTypeDef,
     MultiplexProgramPacketIdentifiersMapTypeDef,
     MultiplexProgramPipelineDetailTypeDef,
     DeleteMultiplexRequestRequestTypeDef,
+    MultiplexSettingsOutputTypeDef,
     DeleteReservationRequestRequestTypeDef,
-    RenewalSettingsTypeDef,
+    RenewalSettingsOutputTypeDef,
     ReservationResourceSpecificationTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
+    InputDeviceSettingsOutputTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeThumbnailsRequestRequestTypeDef,
-    DvbNitSettingsTypeDef,
-    DvbSdtSettingsTypeDef,
-    DvbTdtSettingsTypeDef,
+    DvbNitSettingsOutputTypeDef,
+    DvbSdtSettingsOutputTypeDef,
+    DvbTdtSettingsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FeatureActivationsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    ThumbnailConfigurationOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     TimecodeConfigTypeDef,
+    InputLossFailoverSettingsOutputTypeDef,
+    VideoBlackFailoverSettingsOutputTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
-    FecOutputSettingsTypeDef,
+    FecOutputSettingsOutputTypeDef,
+    FixedModeScheduleActionStartSettingsOutputTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
-    Fmp4HlsSettingsTypeDef,
+    Fmp4HlsSettingsOutputTypeDef,
+    FollowModeScheduleActionStartSettingsOutputTypeDef,
     FollowModeScheduleActionStartSettingsTypeDef,
+    FrameCaptureS3SettingsOutputTypeDef,
     FrameCaptureS3SettingsTypeDef,
-    FrameCaptureOutputSettingsTypeDef,
+    FrameCaptureOutputSettingsOutputTypeDef,
+    TimecodeBurninSettingsOutputTypeDef,
     TimecodeBurninSettingsTypeDef,
+    H264ColorSpaceSettingsOutputTypeDef,
     H264ColorSpaceSettingsTypeDef,
+    TemporalFilterSettingsOutputTypeDef,
     TemporalFilterSettingsTypeDef,
+    Hdr10SettingsOutputTypeDef,
     Hdr10SettingsTypeDef,
+    HlsAkamaiSettingsOutputTypeDef,
     HlsAkamaiSettingsTypeDef,
+    HlsBasicPutSettingsOutputTypeDef,
     HlsBasicPutSettingsTypeDef,
+    HlsMediaStoreSettingsOutputTypeDef,
+    HlsS3SettingsOutputTypeDef,
+    HlsWebdavSettingsOutputTypeDef,
     HlsMediaStoreSettingsTypeDef,
     HlsS3SettingsTypeDef,
     HlsWebdavSettingsTypeDef,
+    HlsId3SegmentTaggingScheduleActionSettingsOutputTypeDef,
     HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
+    HlsInputSettingsOutputTypeDef,
     HlsInputSettingsTypeDef,
+    HlsTimedMetadataScheduleActionSettingsOutputTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
+    StartTimecodeOutputTypeDef,
+    StopTimecodeOutputTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    M3u8SettingsTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    M3u8SettingsOutputTypeDef,
     MaintenanceUpdateSettingsTypeDef,
+    MediaPackageOutputDestinationSettingsOutputTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
+    MotionGraphicsActivateScheduleActionSettingsOutputTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
+    MotionGraphicsSettingsOutputTypeDef,
     MotionGraphicsSettingsTypeDef,
-    MsSmoothOutputSettingsTypeDef,
+    MsSmoothOutputSettingsOutputTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
+    MultiplexProgramChannelDestinationSettingsOutputTypeDef,
     MultiplexProgramChannelDestinationSettingsTypeDef,
+    MultiplexProgramServiceDescriptorOutputTypeDef,
     MultiplexProgramServiceDescriptorTypeDef,
     MultiplexSettingsSummaryTypeDef,
+    MultiplexStatmuxVideoSettingsOutputTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
+    NielsenCBETOutputTypeDef,
     NielsenCBETTypeDef,
+    NielsenNaesIiNwOutputTypeDef,
     NielsenNaesIiNwTypeDef,
+    OutputDestinationSettingsOutputTypeDef,
     OutputDestinationSettingsTypeDef,
+    RtmpGroupSettingsOutputTypeDef,
+    UdpGroupSettingsOutputTypeDef,
     RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
+    PaginatorConfigTypeDef,
+    PipelinePauseStateSettingsOutputTypeDef,
     PipelinePauseStateSettingsTypeDef,
+    RenewalSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    Scte35InputScheduleActionSettingsOutputTypeDef,
+    Scte35ReturnToNetworkScheduleActionSettingsOutputTypeDef,
+    Scte35SpliceInsertScheduleActionSettingsOutputTypeDef,
+    StaticImageDeactivateScheduleActionSettingsOutputTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
+    Scte35DeliveryRestrictionsOutputTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
     StartMultiplexRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     StopMultiplexRequestRequestTypeDef,
     ThumbnailTypeDef,
     TransferInputDeviceRequestRequestTypeDef,
+    VideoSelectorPidOutputTypeDef,
     VideoSelectorPidTypeDef,
+    VideoSelectorProgramIdOutputTypeDef,
     VideoSelectorProgramIdTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
+    ArchiveCdnSettingsOutputTypeDef,
     ArchiveCdnSettingsTypeDef,
+    MediaPackageGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
+    MultiplexOutputSettingsOutputTypeDef,
+    RtmpOutputSettingsOutputTypeDef,
     MediaPackageGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
-    MultiplexOutputSettingsTypeDef,
-    RtmpOutputSettingsTypeDef,
+    AudioChannelMappingOutputTypeDef,
     AudioChannelMappingTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
-    AudioOnlyHlsSettingsTypeDef,
+    AudioOnlyHlsSettingsOutputTypeDef,
+    AvailBlankingOutputTypeDef,
+    BlackoutSlateOutputTypeDef,
+    BurnInDestinationSettingsOutputTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    InputLossBehaviorOutputTypeDef,
+    StaticImageActivateScheduleActionSettingsOutputTypeDef,
+    StaticKeySettingsOutputTypeDef,
+    AudioTrackSelectionOutputTypeDef,
+    AudioTrackSelectionTypeDef,
     AvailBlankingTypeDef,
     BlackoutSlateTypeDef,
     BurnInDestinationSettingsTypeDef,
     DvbSubDestinationSettingsTypeDef,
     InputLossBehaviorTypeDef,
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
-    AudioTrackSelectionTypeDef,
+    AvailSettingsOutputTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    DescribeAccountConfigurationResponseTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
-    PurchaseOfferingRequestRequestTypeDef,
-    UpdateReservationRequestRequestTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     DescribeChannelRequestChannelCreatedWaitTypeDef,
     DescribeChannelRequestChannelDeletedWaitTypeDef,
@@ -895,150 +964,197 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
-    M2tsSettingsTypeDef,
+    M2tsSettingsOutputTypeDef,
+    FailoverConditionSettingsOutputTypeDef,
     FailoverConditionSettingsTypeDef,
+    ScheduleActionStartSettingsOutputTypeDef,
     ScheduleActionStartSettingsTypeDef,
+    FrameCaptureCdnSettingsOutputTypeDef,
     FrameCaptureCdnSettingsTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
+    H264FilterSettingsOutputTypeDef,
+    H265FilterSettingsOutputTypeDef,
+    Mpeg2FilterSettingsOutputTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
     Mpeg2FilterSettingsTypeDef,
+    H265ColorSpaceSettingsOutputTypeDef,
+    VideoSelectorColorSpaceSettingsOutputTypeDef,
     H265ColorSpaceSettingsTypeDef,
     VideoSelectorColorSpaceSettingsTypeDef,
+    HlsCdnSettingsOutputTypeDef,
     HlsCdnSettingsTypeDef,
+    NetworkInputSettingsOutputTypeDef,
     NetworkInputSettingsTypeDef,
+    InputClippingSettingsOutputTypeDef,
     InputClippingSettingsTypeDef,
     InputDestinationTypeDef,
     UpdateInputDeviceRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
-    StandardHlsSettingsTypeDef,
+    StandardHlsSettingsOutputTypeDef,
+    MotionGraphicsConfigurationOutputTypeDef,
     MotionGraphicsConfigurationTypeDef,
     MultiplexOutputDestinationTypeDef,
     MultiplexSummaryTypeDef,
+    MultiplexVideoSettingsOutputTypeDef,
     MultiplexVideoSettingsTypeDef,
+    NielsenWatermarksSettingsOutputTypeDef,
     NielsenWatermarksSettingsTypeDef,
+    OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
+    PauseStateScheduleActionSettingsOutputTypeDef,
     PauseStateScheduleActionSettingsTypeDef,
+    PurchaseOfferingRequestRequestTypeDef,
+    UpdateReservationRequestRequestTypeDef,
+    Scte35SegmentationDescriptorOutputTypeDef,
     Scte35SegmentationDescriptorTypeDef,
     ThumbnailDetailTypeDef,
+    VideoSelectorSettingsOutputTypeDef,
     VideoSelectorSettingsTypeDef,
+    ArchiveGroupSettingsOutputTypeDef,
     ArchiveGroupSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
+    GlobalConfigurationOutputTypeDef,
+    KeyProviderSettingsOutputTypeDef,
+    AudioSelectorSettingsOutputTypeDef,
+    AudioSelectorSettingsTypeDef,
     CaptionDestinationSettingsTypeDef,
     GlobalConfigurationTypeDef,
     KeyProviderSettingsTypeDef,
-    AudioSelectorSettingsTypeDef,
+    AvailConfigurationOutputTypeDef,
     AvailConfigurationTypeDef,
+    CaptionSelectorSettingsOutputTypeDef,
     CaptionSelectorSettingsTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     UpdateReservationResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
-    ArchiveContainerSettingsTypeDef,
-    UdpContainerSettingsTypeDef,
+    ArchiveContainerSettingsOutputTypeDef,
+    UdpContainerSettingsOutputTypeDef,
+    FailoverConditionOutputTypeDef,
     FailoverConditionTypeDef,
+    FrameCaptureGroupSettingsOutputTypeDef,
     FrameCaptureGroupSettingsTypeDef,
+    H264SettingsOutputTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     H264SettingsTypeDef,
     Mpeg2SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
+    InputPrepareScheduleActionSettingsOutputTypeDef,
+    InputSwitchScheduleActionSettingsOutputTypeDef,
     InputPrepareScheduleActionSettingsTypeDef,
     InputSwitchScheduleActionSettingsTypeDef,
     DescribeInputResponseTypeDef,
     InputTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
     DeleteMultiplexResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     MultiplexTypeDef,
     StartMultiplexResponseTypeDef,
     StopMultiplexResponseTypeDef,
     ListMultiplexesResponseTypeDef,
+    MultiplexProgramSettingsOutputTypeDef,
     MultiplexProgramSettingsTypeDef,
+    AudioWatermarkSettingsOutputTypeDef,
     AudioWatermarkSettingsTypeDef,
     UpdateChannelClassRequestRequestTypeDef,
+    Scte35DescriptorSettingsOutputTypeDef,
     Scte35DescriptorSettingsTypeDef,
     DescribeThumbnailsResponseTypeDef,
+    VideoSelectorOutputTypeDef,
     VideoSelectorTypeDef,
+    CaptionDescriptionOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    AudioSelectorOutputTypeDef,
+    AudioSelectorTypeDef,
     CaptionDescriptionTypeDef,
     HlsGroupSettingsTypeDef,
-    AudioSelectorTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
-    ArchiveOutputSettingsTypeDef,
-    UdpOutputSettingsTypeDef,
+    ArchiveOutputSettingsOutputTypeDef,
+    UdpOutputSettingsOutputTypeDef,
+    AutomaticInputFailoverSettingsOutputTypeDef,
     AutomaticInputFailoverSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
     CreateInputResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     ListInputsResponseTypeDef,
     UpdateInputResponseTypeDef,
-    HlsOutputSettingsTypeDef,
+    HlsOutputSettingsOutputTypeDef,
     CreateMultiplexResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
-    CreateMultiplexProgramRequestRequestTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     MultiplexProgramTypeDef,
+    CreateMultiplexProgramRequestRequestTypeDef,
     UpdateMultiplexProgramRequestRequestTypeDef,
+    AudioDescriptionOutputTypeDef,
     AudioDescriptionTypeDef,
+    Scte35DescriptorOutputTypeDef,
     Scte35DescriptorTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
+    InputSettingsOutputTypeDef,
     InputSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
+    Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
     Scte35TimeSignalScheduleActionSettingsTypeDef,
+    InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     OutputTypeDef,
+    ScheduleActionSettingsOutputTypeDef,
     ScheduleActionSettingsTypeDef,
     ChannelSummaryTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
+    ScheduleActionOutputTypeDef,
     ScheduleActionTypeDef,
     ListChannelsResponseTypeDef,
+    EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
-    BatchScheduleActionCreateRequestTypeDef,
     BatchScheduleActionCreateResultTypeDef,
     BatchScheduleActionDeleteResultTypeDef,
     DescribeScheduleResponseTypeDef,
+    BatchScheduleActionCreateRequestTypeDef,
     ChannelTypeDef,
-    CreateChannelRequestRequestTypeDef,
     DeleteChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     StartChannelResponseTypeDef,
     StopChannelResponseTypeDef,
+    CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    BatchUpdateScheduleRequestRequestTypeDef,
     BatchUpdateScheduleResponseTypeDef,
+    BatchUpdateScheduleRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medialive-1.28.1/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.28.12/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.1/setup.py` & `mypy-boto3-medialive-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.28.1",
+    version="1.28.12",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaLive 1.28.1 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MediaLive 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

