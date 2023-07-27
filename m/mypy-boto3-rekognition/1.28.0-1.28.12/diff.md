# Comparing `tmp/mypy-boto3-rekognition-1.28.0.tar.gz` & `tmp/mypy-boto3-rekognition-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.28.0.tar", last modified: Thu Jul  6 21:00:25 2023, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-rekognition-1.28.0.tar` & `mypy-boto3-rekognition-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.554407 mypy-boto3-rekognition-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-07-06 21:00:25.554407 mypy-boto3-rekognition-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24890 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.542406 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57491 2023-07-06 20:53:07.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57401 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-06 20:53:07.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-06 20:53:07.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-07-06 20:53:07.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-06 20:53:07.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97128 2023-07-06 20:53:10.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97009 2023-07-06 20:53:09.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:03.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-06 20:53:07.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-06 20:53:07.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.554407 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-07-06 21:00:25.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 21:00:25.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:25.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 21:00:25.000000 mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:25.554407 mypy-boto3-rekognition-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:53:02.000000 mypy-boto3-rekognition-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25472 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57491 2023-07-27 11:44:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57401 2023-07-27 11:44:29.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-27 11:44:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   101004 2023-07-27 11:44:33.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100883 2023-07-27 11:44:32.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-27 11:44:31.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 11:49:30.000000 mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.229213 mypy-boto3-rekognition-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 11:44:28.000000 mypy-boto3-rekognition-1.28.12/setup.py
```

### Comparing `mypy-boto3-rekognition-1.28.0/LICENSE` & `mypy-boto3-rekognition-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/PKG-INFO` & `mypy-boto3-rekognition-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.0
-Summary: Type annotations for boto3.Rekognition 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Rekognition 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rekognition"></a>
 
 # mypy-boto3-rekognition
 
 [![PyPI - mypy-boto3-rekognition](https://img.shields.io/pypi/v/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,69 +428,62 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
+    ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
-    BoundingBoxTypeDef,
-    S3ObjectTypeDef,
+    BoundingBoxOutputTypeDef,
+    S3ObjectOutputTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BoundingBoxTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
+    ConnectedHomeSettingsOutputTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
-    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
     LivenessOutputConfigTypeDef,
-    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
-    CreateStreamProcessorResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
-    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
-    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
-    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
+    StreamProcessorDataSharingPreferenceOutputTypeDef,
+    StreamProcessorNotificationChannelOutputTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
@@ -503,190 +496,211 @@
     EyeOpenTypeDef,
     EyeglassesTypeDef,
     FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
+    FaceSearchSettingsOutputTypeDef,
     FaceSearchSettingsTypeDef,
-    PointTypeDef,
+    PointOutputTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
     GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
     GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
     GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
+    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
+    KinesisVideoStreamOutputTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    PaginatorConfigTypeDef,
+    OutputConfigOutputTypeDef,
+    PointTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
-    PutProjectPolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
+    StartShotDetectionFilterTypeDef,
+    StreamProcessingStopSelectorTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    CopyProjectVersionResponseTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    DeleteCollectionResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteProjectVersionResponseTypeDef,
+    DescribeCollectionResponseTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
-    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
-    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
+    GroundTruthManifestOutputTypeDef,
     SummaryTypeDef,
-    VideoTypeDef,
+    VideoOutputTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
     LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
-    RegionOfInterestTypeDef,
+    RegionOfInterestOutputTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
+    VideoTypeDef,
     HumanLoopConfigTypeDef,
+    StreamProcessorInputOutputTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
     UserMatchTypeDef,
+    RegionOfInterestTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    SearchUsersByImageRequestRequestTypeDef,
+    AssetOutputTypeDef,
     EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
     StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
-    DetectTextFiltersTypeDef,
-    StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
+    DetectTextFiltersTypeDef,
+    StartTextDetectionFiltersTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
+    TestingDataOutputTypeDef,
+    TrainingDataOutputTypeDef,
     ValidationDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
@@ -694,25 +708,28 @@
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-rekognition-1.28.0/README.md` & `mypy-boto3-rekognition-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rekognition"></a>
 
 # mypy-boto3-rekognition
 
 [![PyPI - mypy-boto3-rekognition](https://img.shields.io/pypi/v/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,69 +396,62 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
+    ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
-    BoundingBoxTypeDef,
-    S3ObjectTypeDef,
+    BoundingBoxOutputTypeDef,
+    S3ObjectOutputTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BoundingBoxTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
+    ConnectedHomeSettingsOutputTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
-    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
     LivenessOutputConfigTypeDef,
-    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
-    CreateStreamProcessorResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
-    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
-    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
-    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
+    StreamProcessorDataSharingPreferenceOutputTypeDef,
+    StreamProcessorNotificationChannelOutputTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
@@ -471,190 +464,211 @@
     EyeOpenTypeDef,
     EyeglassesTypeDef,
     FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
+    FaceSearchSettingsOutputTypeDef,
     FaceSearchSettingsTypeDef,
-    PointTypeDef,
+    PointOutputTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
     GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
     GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
     GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
+    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
+    KinesisVideoStreamOutputTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    PaginatorConfigTypeDef,
+    OutputConfigOutputTypeDef,
+    PointTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
-    PutProjectPolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
+    StartShotDetectionFilterTypeDef,
+    StreamProcessingStopSelectorTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    CopyProjectVersionResponseTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    DeleteCollectionResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteProjectVersionResponseTypeDef,
+    DescribeCollectionResponseTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
-    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
-    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
+    GroundTruthManifestOutputTypeDef,
     SummaryTypeDef,
-    VideoTypeDef,
+    VideoOutputTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
     LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
-    RegionOfInterestTypeDef,
+    RegionOfInterestOutputTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
+    VideoTypeDef,
     HumanLoopConfigTypeDef,
+    StreamProcessorInputOutputTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
     UserMatchTypeDef,
+    RegionOfInterestTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    SearchUsersByImageRequestRequestTypeDef,
+    AssetOutputTypeDef,
     EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
     StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
-    DetectTextFiltersTypeDef,
-    StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
+    DetectTextFiltersTypeDef,
+    StartTextDetectionFiltersTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
+    TestingDataOutputTypeDef,
+    TrainingDataOutputTypeDef,
     ValidationDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
@@ -662,25 +676,28 @@
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/__main__.py` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Rekognition 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Rekognition 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,14 +339,15 @@
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
@@ -425,26 +426,28 @@
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

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -337,14 +337,15 @@
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
@@ -423,26 +424,28 @@
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

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,167 +60,156 @@
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
     "ListUsersPaginator",
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
 class DescribeProjectVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectversionspaginator)
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProjectVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectversionspaginator)
         """
 
-
 class DescribeProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
     """
 
     def paginate(
-        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
         """
 
-
 class ListCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
         """
 
-
 class ListDatasetEntriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetentriespaginator)
     """
 
     def paginate(
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetentriespaginator)
         """
 
-
 class ListDatasetLabelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
     """
 
     def paginate(
-        self, *, DatasetArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DatasetArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetLabelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
         """
 
-
 class ListFacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
         """
 
-
 class ListProjectPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
     """
 
     def paginate(
-        self, *, ProjectArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
         """
 
-
 class ListStreamProcessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamProcessorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
         """
 
-
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,156 +60,167 @@
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
     "ListUsersPaginator",
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
 class DescribeProjectVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectversionspaginator)
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProjectVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectversionspaginator)
         """
 
+
 class DescribeProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
     """
 
     def paginate(
-        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#describeprojectspaginator)
         """
 
+
 class ListCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listcollectionspaginator)
         """
 
+
 class ListDatasetEntriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetentriespaginator)
     """
 
     def paginate(
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetentriespaginator)
         """
 
+
 class ListDatasetLabelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
     """
 
     def paginate(
-        self, *, DatasetArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DatasetArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetLabelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listdatasetlabelspaginator)
         """
 
+
 class ListFacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listfacespaginator)
         """
 
+
 class ListProjectPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
     """
 
     def paginate(
-        self, *, ProjectArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProjectArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListProjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listprojectpoliciespaginator)
         """
 
+
 class ListStreamProcessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamProcessorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#liststreamprocessorspaginator)
         """
 
+
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,69 +68,62 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
+    "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
-    "BoundingBoxTypeDef",
-    "S3ObjectTypeDef",
+    "BoundingBoxOutputTypeDef",
+    "S3ObjectOutputTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
+    "BoundingBoxTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
+    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
-    "CopyProjectVersionResponseTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
-    "CreateCollectionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
     "LivenessOutputConfigTypeDef",
-    "CreateFaceLivenessSessionResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateProjectVersionResponseTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
-    "CreateStreamProcessorResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
-    "DeleteCollectionResponseTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
     "UnsuccessfulFaceDeletionTypeDef",
     "DeleteProjectPolicyRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteProjectVersionRequestRequestTypeDef",
-    "DeleteProjectVersionResponseTypeDef",
     "DeleteStreamProcessorRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeCollectionRequestRequestTypeDef",
-    "DescribeCollectionResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
-    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
+    "StreamProcessorDataSharingPreferenceOutputTypeDef",
+    "StreamProcessorNotificationChannelOutputTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ProtectiveEquipmentSummarizationAttributesTypeDef",
     "ProtectiveEquipmentSummaryTypeDef",
@@ -143,190 +136,211 @@
     "EyeOpenTypeDef",
     "EyeglassesTypeDef",
     "FaceOccludedTypeDef",
     "GenderTypeDef",
     "MouthOpenTypeDef",
     "MustacheTypeDef",
     "SunglassesTypeDef",
+    "FaceSearchSettingsOutputTypeDef",
     "FaceSearchSettingsTypeDef",
-    "PointTypeDef",
+    "PointOutputTypeDef",
     "GetCelebrityInfoRequestRequestTypeDef",
     "GetCelebrityRecognitionRequestRequestTypeDef",
     "VideoMetadataTypeDef",
     "GetContentModerationRequestMetadataTypeDef",
     "GetContentModerationRequestRequestTypeDef",
     "GetFaceDetectionRequestRequestTypeDef",
     "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     "GetFaceSearchRequestRequestTypeDef",
     "GetLabelDetectionRequestMetadataTypeDef",
     "GetLabelDetectionRequestRequestTypeDef",
     "GetPersonTrackingRequestRequestTypeDef",
     "GetSegmentDetectionRequestRequestTypeDef",
     "SegmentTypeInfoTypeDef",
     "GetTextDetectionRequestRequestTypeDef",
+    "S3ObjectTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
+    "KinesisVideoStreamOutputTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
     "ListCollectionsRequestRequestTypeDef",
-    "ListCollectionsResponseTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     "ListDatasetLabelsRequestRequestTypeDef",
-    "ListFacesRequestListFacesPaginateTypeDef",
     "ListFacesRequestRequestTypeDef",
-    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     "ListProjectPoliciesRequestRequestTypeDef",
     "ProjectPolicyTypeDef",
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
-    "PaginatorConfigTypeDef",
+    "OutputConfigOutputTypeDef",
+    "PointTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
-    "PutProjectPolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchedFaceTypeDef",
     "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
     "TechnicalCueSegmentTypeDef",
+    "StartProjectVersionRequestRequestTypeDef",
+    "StartShotDetectionFilterTypeDef",
+    "StreamProcessingStopSelectorTypeDef",
+    "StopProjectVersionRequestRequestTypeDef",
+    "StopStreamProcessorRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "CopyProjectVersionResponseTypeDef",
+    "CreateCollectionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateFaceLivenessSessionResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateProjectVersionResponseTypeDef",
+    "CreateStreamProcessorResponseTypeDef",
+    "DeleteCollectionResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteProjectVersionResponseTypeDef",
+    "DescribeCollectionResponseTypeDef",
+    "ListCollectionsResponseTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutProjectPolicyResponseTypeDef",
     "StartCelebrityRecognitionResponseTypeDef",
     "StartContentModerationResponseTypeDef",
     "StartFaceDetectionResponseTypeDef",
     "StartFaceSearchResponseTypeDef",
     "StartLabelDetectionResponseTypeDef",
     "StartPersonTrackingResponseTypeDef",
-    "StartProjectVersionRequestRequestTypeDef",
     "StartProjectVersionResponseTypeDef",
-    "StartShotDetectionFilterTypeDef",
     "StartSegmentDetectionResponseTypeDef",
-    "StreamProcessingStopSelectorTypeDef",
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
-    "StopProjectVersionRequestRequestTypeDef",
     "StopProjectVersionResponseTypeDef",
-    "StopStreamProcessorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
-    "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
+    "GroundTruthManifestOutputTypeDef",
     "SummaryTypeDef",
-    "VideoTypeDef",
+    "VideoOutputTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
     "CreateFaceLivenessSessionRequestSettingsTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
     "DeleteFacesResponseTypeDef",
+    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    "ListFacesRequestListFacesPaginateTypeDef",
+    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
+    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
-    "RegionOfInterestTypeDef",
+    "RegionOfInterestOutputTypeDef",
+    "GroundTruthManifestTypeDef",
+    "ImageTypeDef",
+    "VideoTypeDef",
     "HumanLoopConfigTypeDef",
+    "StreamProcessorInputOutputTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
     "UserMatchTypeDef",
+    "RegionOfInterestTypeDef",
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
-    "AssetTypeDef",
-    "DatasetSourceTypeDef",
-    "CompareFacesRequestRequestTypeDef",
-    "DetectCustomLabelsRequestRequestTypeDef",
-    "DetectFacesRequestRequestTypeDef",
-    "DetectProtectiveEquipmentRequestRequestTypeDef",
-    "IndexFacesRequestRequestTypeDef",
-    "RecognizeCelebritiesRequestRequestTypeDef",
-    "SearchFacesByImageRequestRequestTypeDef",
-    "SearchUsersByImageRequestRequestTypeDef",
+    "AssetOutputTypeDef",
     "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
     "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
     "DescribeProjectsResponseTypeDef",
     "DetectLabelsImagePropertiesTypeDef",
     "LabelTypeDef",
-    "DetectLabelsRequestRequestTypeDef",
-    "StartLabelDetectionRequestRequestTypeDef",
     "CelebrityDetailTypeDef",
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
-    "DetectTextFiltersTypeDef",
-    "StartTextDetectionFiltersTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
+    "AssetTypeDef",
+    "DatasetSourceTypeDef",
+    "CompareFacesRequestRequestTypeDef",
+    "DetectCustomLabelsRequestRequestTypeDef",
+    "DetectFacesRequestRequestTypeDef",
+    "DetectLabelsRequestRequestTypeDef",
+    "DetectProtectiveEquipmentRequestRequestTypeDef",
+    "IndexFacesRequestRequestTypeDef",
+    "RecognizeCelebritiesRequestRequestTypeDef",
+    "SearchFacesByImageRequestRequestTypeDef",
+    "SearchUsersByImageRequestRequestTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartLabelDetectionRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
+    "DetectTextFiltersTypeDef",
+    "StartTextDetectionFiltersTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
-    "TestingDataTypeDef",
-    "TrainingDataTypeDef",
+    "TestingDataOutputTypeDef",
+    "TrainingDataOutputTypeDef",
     "ValidationDataTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
     "DetectLabelsResponseTypeDef",
     "LabelDetectionTypeDef",
     "CelebrityRecognitionTypeDef",
@@ -334,25 +348,28 @@
     "PersonDetectionTypeDef",
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
+    "TestingDataTypeDef",
+    "TrainingDataTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DetectTextRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "CreateProjectVersionRequestRequestTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
     "GetTextDetectionResponseTypeDef",
+    "CreateProjectVersionRequestRequestTypeDef",
     "ProjectVersionDescriptionTypeDef",
     "DescribeProjectVersionsResponseTypeDef",
 )
 
 AgeRangeTypeDef = TypedDict(
     "AgeRangeTypeDef",
     {
@@ -390,14 +407,25 @@
     "AssociatedFaceTypeDef",
     {
         "FaceId": str,
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
 UnsuccessfulFaceAssociationTypeDef = TypedDict(
     "UnsuccessfulFaceAssociationTypeDef",
     {
         "FaceId": str,
         "UserId": str,
         "Confidence": float,
         "Reasons": List[UnsuccessfulFaceAssociationReasonType],
@@ -412,27 +440,27 @@
         "DurationMillis": int,
         "SampleRate": int,
         "NumberOfChannels": int,
     },
     total=False,
 )
 
-BoundingBoxTypeDef = TypedDict(
-    "BoundingBoxTypeDef",
+BoundingBoxOutputTypeDef = TypedDict(
+    "BoundingBoxOutputTypeDef",
     {
         "Width": float,
         "Height": float,
         "Left": float,
         "Top": float,
     },
     total=False,
 )
 
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
+S3ObjectOutputTypeDef = TypedDict(
+    "S3ObjectOutputTypeDef",
     {
         "Bucket": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
@@ -451,14 +479,25 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
+BoundingBoxTypeDef = TypedDict(
+    "BoundingBoxTypeDef",
+    {
+        "Width": float,
+        "Height": float,
+        "Left": float,
+        "Top": float,
+    },
+    total=False,
+)
+
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -515,14 +554,35 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
+_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_RequiredConnectedHomeSettingsOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+)
+_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_OptionalConnectedHomeSettingsOutputTypeDef",
+    {
+        "MinConfidence": float,
+    },
+    total=False,
+)
+
+
+class ConnectedHomeSettingsOutputTypeDef(
+    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
@@ -555,22 +615,14 @@
     {
         "S3Bucket": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-CopyProjectVersionResponseTypeDef = TypedDict(
-    "CopyProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CoversBodyPartTypeDef = TypedDict(
     "CoversBodyPartTypeDef",
     {
         "Confidence": float,
         "Value": bool,
     },
     total=False,
@@ -593,32 +645,14 @@
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
 
-CreateCollectionResponseTypeDef = TypedDict(
-    "CreateCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "CollectionArn": str,
-        "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLivenessOutputConfigTypeDef = TypedDict(
     "_RequiredLivenessOutputConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalLivenessOutputConfigTypeDef = TypedDict(
@@ -632,67 +666,35 @@
 
 class LivenessOutputConfigTypeDef(
     _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
 ):
     pass
 
 
-CreateFaceLivenessSessionResponseTypeDef = TypedDict(
-    "CreateFaceLivenessSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "ProjectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProjectVersionResponseTypeDef = TypedDict(
-    "CreateProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StreamProcessorDataSharingPreferenceTypeDef = TypedDict(
     "StreamProcessorDataSharingPreferenceTypeDef",
     {
         "OptIn": bool,
     },
 )
 
 StreamProcessorNotificationChannelTypeDef = TypedDict(
     "StreamProcessorNotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
     },
 )
 
-CreateStreamProcessorResponseTypeDef = TypedDict(
-    "CreateStreamProcessorResponseTypeDef",
-    {
-        "StreamProcessorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "CollectionId": str,
         "UserId": str,
     },
 )
@@ -754,22 +756,14 @@
 DeleteCollectionRequestRequestTypeDef = TypedDict(
     "DeleteCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DeleteCollectionResponseTypeDef = TypedDict(
-    "DeleteCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -817,37 +811,21 @@
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "Status": ProjectStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectVersionRequestRequestTypeDef = TypedDict(
     "DeleteProjectVersionRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
     },
 )
 
-DeleteProjectVersionResponseTypeDef = TypedDict(
-    "DeleteProjectVersionResponseTypeDef",
-    {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteStreamProcessorRequestRequestTypeDef = TypedDict(
     "DeleteStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -876,56 +854,31 @@
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DescribeCollectionResponseTypeDef = TypedDict(
-    "DescribeCollectionResponseTypeDef",
-    {
-        "FaceCount": int,
-        "FaceModelVersion": str,
-        "CollectionARN": str,
-        "CreationTimestamp": datetime,
-        "UserCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
-_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "VersionNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
-    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-):
-    pass
-
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -951,23 +904,14 @@
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    {
-        "ProjectNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
     },
@@ -977,14 +921,28 @@
 DescribeStreamProcessorRequestRequestTypeDef = TypedDict(
     "DescribeStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StreamProcessorDataSharingPreferenceOutputTypeDef = TypedDict(
+    "StreamProcessorDataSharingPreferenceOutputTypeDef",
+    {
+        "OptIn": bool,
+    },
+)
+
+StreamProcessorNotificationChannelOutputTypeDef = TypedDict(
+    "StreamProcessorNotificationChannelOutputTypeDef",
+    {
+        "SNSTopicArn": str,
+    },
+)
+
 DetectLabelsImageQualityTypeDef = TypedDict(
     "DetectLabelsImageQualityTypeDef",
     {
         "Brightness": float,
         "Sharpness": float,
         "Contrast": float,
     },
@@ -1179,25 +1137,34 @@
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
 )
 
+FaceSearchSettingsOutputTypeDef = TypedDict(
+    "FaceSearchSettingsOutputTypeDef",
+    {
+        "CollectionId": str,
+        "FaceMatchThreshold": float,
+    },
+    total=False,
+)
+
 FaceSearchSettingsTypeDef = TypedDict(
     "FaceSearchSettingsTypeDef",
     {
         "CollectionId": str,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
-PointTypeDef = TypedDict(
-    "PointTypeDef",
+PointOutputTypeDef = TypedDict(
+    "PointOutputTypeDef",
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
@@ -1438,14 +1405,24 @@
 
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
 
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
+    {
+        "Bucket": str,
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -1454,14 +1431,22 @@
     "KinesisDataStreamTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
+KinesisVideoStreamOutputTypeDef = TypedDict(
+    "KinesisVideoStreamOutputTypeDef",
+    {
+        "Arn": str,
+    },
+    total=False,
+)
+
 KinesisVideoStreamStartSelectorTypeDef = TypedDict(
     "KinesisVideoStreamStartSelectorTypeDef",
     {
         "ProducerTimestamp": int,
         "FragmentNumber": str,
     },
     total=False,
@@ -1495,67 +1480,23 @@
     "ParentTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCollectionsResponseTypeDef = TypedDict(
-    "ListCollectionsResponseTypeDef",
-    {
-        "CollectionIds": List[str],
-        "NextToken": str,
-        "FaceModelVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ContainsLabels": Sequence[str],
-        "Labeled": bool,
-        "SourceRefContains": str,
-        "HasErrors": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
@@ -1575,45 +1516,14 @@
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
 
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
-    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestRequestTypeDef = TypedDict(
@@ -1628,38 +1538,14 @@
 
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_RequiredListFacesRequestListFacesPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_OptionalListFacesRequestListFacesPaginateTypeDef",
-    {
-        "UserId": str,
-        "FaceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFacesRequestListFacesPaginateTypeDef(
-    _RequiredListFacesRequestListFacesPaginateTypeDef,
-    _OptionalListFacesRequestListFacesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
@@ -1676,36 +1562,14 @@
 
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
-    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestRequestTypeDef = TypedDict(
@@ -1734,22 +1598,14 @@
         "PolicyDocument": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamProcessorsRequestRequestTypeDef = TypedDict(
     "ListStreamProcessorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1767,44 +1623,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1845,20 +1671,28 @@
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+OutputConfigOutputTypeDef = TypedDict(
+    "OutputConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "S3Bucket": str,
+        "S3KeyPrefix": str,
+    },
+    total=False,
+)
+
+PointTypeDef = TypedDict(
+    "PointTypeDef",
+    {
+        "X": float,
+        "Y": float,
     },
     total=False,
 )
 
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
@@ -1878,33 +1712,14 @@
 
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
 
-PutProjectPolicyResponseTypeDef = TypedDict(
-    "PutProjectPolicyResponseTypeDef",
-    {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-)
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
     total=False,
@@ -1987,243 +1802,363 @@
     {
         "Type": TechnicalCueTypeType,
         "Confidence": float,
     },
     total=False,
 )
 
-StartCelebrityRecognitionResponseTypeDef = TypedDict(
-    "StartCelebrityRecognitionResponseTypeDef",
+_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
+        "MinInferenceUnits": int,
     },
 )
+_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartProjectVersionRequestRequestTypeDef",
+    {
+        "MaxInferenceUnits": int,
+    },
+    total=False,
+)
 
-StartContentModerationResponseTypeDef = TypedDict(
-    "StartContentModerationResponseTypeDef",
+
+class StartProjectVersionRequestRequestTypeDef(
+    _RequiredStartProjectVersionRequestRequestTypeDef,
+    _OptionalStartProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+
+StartShotDetectionFilterTypeDef = TypedDict(
+    "StartShotDetectionFilterTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MinSegmentConfidence": float,
     },
+    total=False,
 )
 
-StartFaceDetectionResponseTypeDef = TypedDict(
-    "StartFaceDetectionResponseTypeDef",
+StreamProcessingStopSelectorTypeDef = TypedDict(
+    "StreamProcessingStopSelectorTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxDurationInSeconds": int,
     },
+    total=False,
 )
 
-StartFaceSearchResponseTypeDef = TypedDict(
-    "StartFaceSearchResponseTypeDef",
+StopProjectVersionRequestRequestTypeDef = TypedDict(
+    "StopProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
     },
 )
 
-StartLabelDetectionResponseTypeDef = TypedDict(
-    "StartLabelDetectionResponseTypeDef",
+StopStreamProcessorRequestRequestTypeDef = TypedDict(
+    "StopStreamProcessorRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
 
-StartPersonTrackingResponseTypeDef = TypedDict(
-    "StartPersonTrackingResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartProjectVersionRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+CopyProjectVersionResponseTypeDef = TypedDict(
+    "CopyProjectVersionResponseTypeDef",
     {
         "ProjectVersionArn": str,
-        "MinInferenceUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartProjectVersionRequestRequestTypeDef",
+
+CreateCollectionResponseTypeDef = TypedDict(
+    "CreateCollectionResponseTypeDef",
     {
-        "MaxInferenceUnits": int,
+        "StatusCode": int,
+        "CollectionArn": str,
+        "FaceModelVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class StartProjectVersionRequestRequestTypeDef(
-    _RequiredStartProjectVersionRequestRequestTypeDef,
-    _OptionalStartProjectVersionRequestRequestTypeDef,
-):
-    pass
+CreateFaceLivenessSessionResponseTypeDef = TypedDict(
+    "CreateFaceLivenessSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-StartProjectVersionResponseTypeDef = TypedDict(
-    "StartProjectVersionResponseTypeDef",
+CreateProjectVersionResponseTypeDef = TypedDict(
+    "CreateProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamProcessorResponseTypeDef = TypedDict(
+    "CreateStreamProcessorResponseTypeDef",
+    {
+        "StreamProcessorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCollectionResponseTypeDef = TypedDict(
+    "DeleteCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Status": ProjectStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectVersionResponseTypeDef = TypedDict(
+    "DeleteProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartShotDetectionFilterTypeDef = TypedDict(
-    "StartShotDetectionFilterTypeDef",
+DescribeCollectionResponseTypeDef = TypedDict(
+    "DescribeCollectionResponseTypeDef",
     {
-        "MinSegmentConfidence": float,
+        "FaceCount": int,
+        "FaceModelVersion": str,
+        "CollectionARN": str,
+        "CreationTimestamp": datetime,
+        "UserCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartSegmentDetectionResponseTypeDef = TypedDict(
-    "StartSegmentDetectionResponseTypeDef",
+ListCollectionsResponseTypeDef = TypedDict(
+    "ListCollectionsResponseTypeDef",
+    {
+        "CollectionIds": List[str],
+        "NextToken": str,
+        "FaceModelVersions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProjectPolicyResponseTypeDef = TypedDict(
+    "PutProjectPolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCelebrityRecognitionResponseTypeDef = TypedDict(
+    "StartCelebrityRecognitionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamProcessingStopSelectorTypeDef = TypedDict(
-    "StreamProcessingStopSelectorTypeDef",
+StartContentModerationResponseTypeDef = TypedDict(
+    "StartContentModerationResponseTypeDef",
     {
-        "MaxDurationInSeconds": int,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartStreamProcessorResponseTypeDef = TypedDict(
-    "StartStreamProcessorResponseTypeDef",
+StartFaceDetectionResponseTypeDef = TypedDict(
+    "StartFaceDetectionResponseTypeDef",
     {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTextDetectionResponseTypeDef = TypedDict(
-    "StartTextDetectionResponseTypeDef",
+StartFaceSearchResponseTypeDef = TypedDict(
+    "StartFaceSearchResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionRequestRequestTypeDef = TypedDict(
-    "StopProjectVersionRequestRequestTypeDef",
+StartLabelDetectionResponseTypeDef = TypedDict(
+    "StartLabelDetectionResponseTypeDef",
     {
-        "ProjectVersionArn": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionResponseTypeDef = TypedDict(
-    "StopProjectVersionResponseTypeDef",
+StartPersonTrackingResponseTypeDef = TypedDict(
+    "StartPersonTrackingResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartProjectVersionResponseTypeDef = TypedDict(
+    "StartProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopStreamProcessorRequestRequestTypeDef = TypedDict(
-    "StopStreamProcessorRequestRequestTypeDef",
+StartSegmentDetectionResponseTypeDef = TypedDict(
+    "StartSegmentDetectionResponseTypeDef",
     {
-        "Name": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartStreamProcessorResponseTypeDef = TypedDict(
+    "StartStreamProcessorResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartTextDetectionResponseTypeDef = TypedDict(
+    "StartTextDetectionResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopProjectVersionResponseTypeDef = TypedDict(
+    "StopProjectVersionResponseTypeDef",
+    {
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateFacesResponseTypeDef = TypedDict(
     "AssociateFacesResponseTypeDef",
     {
         "AssociatedFaces": List[AssociatedFaceTypeDef],
         "UnsuccessfulFaceAssociations": List[UnsuccessfulFaceAssociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedSourceImageFaceTypeDef = TypedDict(
     "ComparedSourceImageFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
     },
     total=False,
 )
 
 FaceTypeDef = TypedDict(
     "FaceTypeDef",
     {
         "FaceId": str,
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "ImageId": str,
         "ExternalImageId": str,
         "Confidence": float,
         "IndexFacesModelVersion": str,
         "UserId": str,
     },
     total=False,
 )
 
 AuditImageTypeDef = TypedDict(
     "AuditImageTypeDef",
     {
         "Bytes": bytes,
-        "S3Object": S3ObjectTypeDef,
-        "BoundingBox": BoundingBoxTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
     },
     total=False,
 )
 
-GroundTruthManifestTypeDef = TypedDict(
-    "GroundTruthManifestTypeDef",
+GroundTruthManifestOutputTypeDef = TypedDict(
+    "GroundTruthManifestOutputTypeDef",
     {
-        "S3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
-    {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
-        "S3Object": S3ObjectTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
-VideoTypeDef = TypedDict(
-    "VideoTypeDef",
+VideoOutputTypeDef = TypedDict(
+    "VideoOutputTypeDef",
     {
-        "S3Object": S3ObjectTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
 StartTechnicalCueDetectionFilterTypeDef = TypedDict(
     "StartTechnicalCueDetectionFilterTypeDef",
     {
@@ -2235,22 +2170,22 @@
 
 GetCelebrityInfoResponseTypeDef = TypedDict(
     "GetCelebrityInfoResponseTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "KnownGender": KnownGenderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "Landmarks": List[LandmarkTypeDef],
         "Pose": PoseTypeDef,
         "Quality": ImageQualityTypeDef,
         "Emotions": List[EmotionTypeDef],
         "Smile": SmileTypeDef,
     },
@@ -2303,15 +2238,15 @@
 ):
     pass
 
 
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
     },
     total=False,
 )
 
@@ -2366,18 +2301,182 @@
 )
 
 DeleteFacesResponseTypeDef = TypedDict(
     "DeleteFacesResponseTypeDef",
     {
         "DeletedFaces": List[str],
         "UnsuccessfulFaceDeletions": List[UnsuccessfulFaceDeletionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "VersionNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
+    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+):
+    pass
+
+
+DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    {
+        "ProjectNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ContainsLabels": Sequence[str],
+        "Labeled": bool,
+        "SourceRefContains": str,
+        "HasErrors": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
+    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_RequiredListFacesRequestListFacesPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_OptionalListFacesRequestListFacesPaginateTypeDef",
+    {
+        "UserId": str,
+        "FaceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFacesRequestListFacesPaginateTypeDef(
+    _RequiredListFacesRequestListFacesPaginateTypeDef,
+    _OptionalListFacesRequestListFacesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
+    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+):
+    pass
+
+
+ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
@@ -2441,15 +2540,15 @@
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
 )
 
 DetectLabelsSettingsTypeDef = TypedDict(
@@ -2471,39 +2570,39 @@
 
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFacesResponseTypeDef = TypedDict(
     "DisassociateFacesResponseTypeDef",
     {
         "DisassociatedFaces": List[DisassociatedFaceTypeDef],
         "UnsuccessfulFaceDisassociations": List[UnsuccessfulFaceDisassociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DistributeDatasetEntriesRequestRequestTypeDef = TypedDict(
     "DistributeDatasetEntriesRequestRequestTypeDef",
     {
         "Datasets": Sequence[DistributeDatasetTypeDef],
     },
 )
 
 FaceDetailTypeDef = TypedDict(
     "FaceDetailTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "AgeRange": AgeRangeTypeDef,
         "Smile": SmileTypeDef,
         "Eyeglasses": EyeglassesTypeDef,
         "Sunglasses": SunglassesTypeDef,
         "Gender": GenderTypeDef,
         "Beard": BeardTypeDef,
         "Mustache": MustacheTypeDef,
@@ -2516,37 +2615,71 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
+StreamProcessorSettingsOutputTypeDef = TypedDict(
+    "StreamProcessorSettingsOutputTypeDef",
+    {
+        "FaceSearch": FaceSearchSettingsOutputTypeDef,
+        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": List[PointTypeDef],
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Polygon": List[PointOutputTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestTypeDef = TypedDict(
-    "RegionOfInterestTypeDef",
+RegionOfInterestOutputTypeDef = TypedDict(
+    "RegionOfInterestOutputTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": Sequence[PointTypeDef],
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Polygon": List[PointOutputTypeDef],
+    },
+    total=False,
+)
+
+GroundTruthManifestTypeDef = TypedDict(
+    "GroundTruthManifestTypeDef",
+    {
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
+VideoTypeDef = TypedDict(
+    "VideoTypeDef",
+    {
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
@@ -2563,14 +2696,22 @@
 )
 
 
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
 
+StreamProcessorInputOutputTypeDef = TypedDict(
+    "StreamProcessorInputOutputTypeDef",
+    {
+        "KinesisVideoStream": KinesisVideoStreamOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2584,45 +2725,54 @@
 )
 
 ListProjectPoliciesResponseTypeDef = TypedDict(
     "ListProjectPoliciesResponseTypeDef",
     {
         "ProjectPolicies": List[ProjectPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamProcessorsResponseTypeDef = TypedDict(
     "ListStreamProcessorsResponseTypeDef",
     {
         "NextToken": str,
         "StreamProcessors": List[StreamProcessorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserMatchTypeDef = TypedDict(
     "UserMatchTypeDef",
     {
         "Similarity": float,
         "User": MatchedUserTypeDef,
     },
     total=False,
 )
 
+RegionOfInterestTypeDef = TypedDict(
+    "RegionOfInterestTypeDef",
+    {
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": Sequence[PointTypeDef],
+    },
+    total=False,
+)
+
 StreamProcessorOutputTypeDef = TypedDict(
     "StreamProcessorOutputTypeDef",
     {
         "KinesisDataStream": KinesisDataStreamTypeDef,
         "S3Destination": S3DestinationTypeDef,
     },
     total=False,
@@ -2658,30 +2808,265 @@
 
 ListFacesResponseTypeDef = TypedDict(
     "ListFacesResponseTypeDef",
     {
         "Faces": List[FaceTypeDef],
         "NextToken": str,
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceLivenessSessionResultsResponseTypeDef = TypedDict(
     "GetFaceLivenessSessionResultsResponseTypeDef",
     {
         "SessionId": str,
         "Status": LivenessSessionStatusType,
         "Confidence": float,
         "ReferenceImage": AuditImageTypeDef,
         "AuditImages": List[AuditImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssetOutputTypeDef = TypedDict(
+    "AssetOutputTypeDef",
+    {
+        "GroundTruthManifest": GroundTruthManifestOutputTypeDef,
+    },
+    total=False,
+)
+
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+CelebrityTypeDef = TypedDict(
+    "CelebrityTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Face": ComparedFaceTypeDef,
+        "MatchConfidence": float,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+CompareFacesMatchTypeDef = TypedDict(
+    "CompareFacesMatchTypeDef",
+    {
+        "Similarity": float,
+        "Face": ComparedFaceTypeDef,
+    },
+    total=False,
+)
+
+GetContentModerationResponseTypeDef = TypedDict(
+    "GetContentModerationResponseTypeDef",
+    {
+        "JobStatus": VideoJobStatusType,
+        "StatusMessage": str,
+        "VideoMetadata": VideoMetadataTypeDef,
+        "ModerationLabels": List[ContentModerationDetectionTypeDef],
+        "NextToken": str,
+        "ModerationModelVersion": str,
+        "JobId": str,
+        "Video": VideoOutputTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProtectiveEquipmentBodyPartTypeDef = TypedDict(
+    "ProtectiveEquipmentBodyPartTypeDef",
+    {
+        "Name": BodyPartType,
+        "Confidence": float,
+        "EquipmentDetections": List[EquipmentDetectionTypeDef],
+    },
+    total=False,
+)
+
+CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
+    {
+        "KmsKeyId": str,
+        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetDescription": DatasetDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListDatasetLabelsResponseTypeDef = TypedDict(
+    "ListDatasetLabelsResponseTypeDef",
+    {
+        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProjectsResponseTypeDef = TypedDict(
+    "DescribeProjectsResponseTypeDef",
+    {
+        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectLabelsImagePropertiesTypeDef = TypedDict(
+    "DetectLabelsImagePropertiesTypeDef",
+    {
+        "Quality": DetectLabelsImageQualityTypeDef,
+        "DominantColors": List[DominantColorTypeDef],
+        "Foreground": DetectLabelsImageForegroundTypeDef,
+        "Background": DetectLabelsImageBackgroundTypeDef,
+    },
+    total=False,
+)
+
+LabelTypeDef = TypedDict(
+    "LabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Instances": List[InstanceTypeDef],
+        "Parents": List[ParentTypeDef],
+        "Aliases": List[LabelAliasTypeDef],
+        "Categories": List[LabelCategoryTypeDef],
+    },
+    total=False,
+)
+
+CelebrityDetailTypeDef = TypedDict(
+    "CelebrityDetailTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Confidence": float,
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Face": FaceDetailTypeDef,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+DetectFacesResponseTypeDef = TypedDict(
+    "DetectFacesResponseTypeDef",
+    {
+        "FaceDetails": List[FaceDetailTypeDef],
+        "OrientationCorrection": OrientationCorrectionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FaceDetectionTypeDef = TypedDict(
+    "FaceDetectionTypeDef",
+    {
+        "Timestamp": int,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+FaceRecordTypeDef = TypedDict(
+    "FaceRecordTypeDef",
+    {
+        "Face": FaceTypeDef,
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+PersonDetailTypeDef = TypedDict(
+    "PersonDetailTypeDef",
+    {
+        "Index": int,
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+SearchedFaceDetailsTypeDef = TypedDict(
+    "SearchedFaceDetailsTypeDef",
+    {
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnindexedFaceTypeDef = TypedDict(
+    "UnindexedFaceTypeDef",
+    {
+        "Reasons": List[ReasonType],
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnsearchedFaceTypeDef = TypedDict(
+    "UnsearchedFaceTypeDef",
+    {
+        "FaceDetails": FaceDetailTypeDef,
+        "Reasons": List[UnsearchedFaceReasonType],
+    },
+    total=False,
+)
+
+CustomLabelTypeDef = TypedDict(
+    "CustomLabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+TextDetectionTypeDef = TypedDict(
+    "TextDetectionTypeDef",
+    {
+        "DetectedText": str,
+        "Type": TextTypesType,
+        "Id": int,
+        "ParentId": int,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
     },
     total=False,
 )
@@ -2759,14 +3144,38 @@
 
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectLabelsRequestRequestTypeDef",
+    {
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectLabelsRequestRequestTypeDef",
+    {
+        "MaxLabels": int,
+        "MinConfidence": float,
+        "Features": Sequence[DetectLabelsFeatureNameType],
+        "Settings": DetectLabelsSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class DetectLabelsRequestRequestTypeDef(
+    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
@@ -2863,23 +3272,14 @@
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
@@ -2971,305 +3371,120 @@
 
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
+_RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
+_OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartLabelDetectionRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
+        "MinConfidence": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
+        "Features": Sequence[Literal["GENERAL_LABELS"]],
+        "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
 
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
+class StartLabelDetectionRequestRequestTypeDef(
+    _RequiredStartLabelDetectionRequestRequestTypeDef,
+    _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
 
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
-CelebrityTypeDef = TypedDict(
-    "CelebrityTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Face": ComparedFaceTypeDef,
-        "MatchConfidence": float,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-CompareFacesMatchTypeDef = TypedDict(
-    "CompareFacesMatchTypeDef",
-    {
-        "Similarity": float,
-        "Face": ComparedFaceTypeDef,
-    },
-    total=False,
-)
-
-GetContentModerationResponseTypeDef = TypedDict(
-    "GetContentModerationResponseTypeDef",
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
     {
-        "JobStatus": VideoJobStatusType,
-        "StatusMessage": str,
-        "VideoMetadata": VideoMetadataTypeDef,
-        "ModerationLabels": List[ContentModerationDetectionTypeDef],
-        "NextToken": str,
-        "ModerationModelVersion": str,
-        "JobId": str,
         "Video": VideoTypeDef,
-        "JobTag": str,
-        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-ProtectiveEquipmentBodyPartTypeDef = TypedDict(
-    "ProtectiveEquipmentBodyPartTypeDef",
-    {
-        "Name": BodyPartType,
-        "Confidence": float,
-        "EquipmentDetections": List[EquipmentDetectionTypeDef],
-    },
-    total=False,
-)
-
-CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
-    "CreateFaceLivenessSessionRequestRequestTypeDef",
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
     {
-        "KmsKeyId": str,
-        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
         "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDatasetLabelsResponseTypeDef = TypedDict(
-    "ListDatasetLabelsResponseTypeDef",
-    {
-        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeProjectsResponseTypeDef = TypedDict(
-    "DescribeProjectsResponseTypeDef",
-    {
-        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DetectLabelsImagePropertiesTypeDef = TypedDict(
-    "DetectLabelsImagePropertiesTypeDef",
-    {
-        "Quality": DetectLabelsImageQualityTypeDef,
-        "DominantColors": List[DominantColorTypeDef],
-        "Foreground": DetectLabelsImageForegroundTypeDef,
-        "Background": DetectLabelsImageBackgroundTypeDef,
-    },
-    total=False,
-)
-
-LabelTypeDef = TypedDict(
-    "LabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Instances": List[InstanceTypeDef],
-        "Parents": List[ParentTypeDef],
-        "Aliases": List[LabelAliasTypeDef],
-        "Categories": List[LabelCategoryTypeDef],
-    },
-    total=False,
-)
-
-_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectLabelsRequestRequestTypeDef",
-    {
-        "MaxLabels": int,
-        "MinConfidence": float,
-        "Features": Sequence[DetectLabelsFeatureNameType],
-        "Settings": DetectLabelsSettingsTypeDef,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
     },
     total=False,
 )
 
 
-class DetectLabelsRequestRequestTypeDef(
-    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartLabelDetectionRequestRequestTypeDef",
+_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
-        "Video": VideoTypeDef,
+        "Image": ImageTypeDef,
     },
 )
-_OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartLabelDetectionRequestRequestTypeDef",
+_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
     {
-        "ClientRequestToken": str,
         "MinConfidence": float,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-        "Features": Sequence[Literal["GENERAL_LABELS"]],
-        "Settings": LabelDetectionSettingsTypeDef,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
     },
     total=False,
 )
 
 
-class StartLabelDetectionRequestRequestTypeDef(
-    _RequiredStartLabelDetectionRequestRequestTypeDef,
-    _OptionalStartLabelDetectionRequestRequestTypeDef,
+class DetectModerationLabelsRequestRequestTypeDef(
+    _RequiredDetectModerationLabelsRequestRequestTypeDef,
+    _OptionalDetectModerationLabelsRequestRequestTypeDef,
 ):
     pass
 
 
-CelebrityDetailTypeDef = TypedDict(
-    "CelebrityDetailTypeDef",
+_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredStartStreamProcessorRequestRequestTypeDef",
     {
-        "Urls": List[str],
         "Name": str,
-        "Id": str,
-        "Confidence": float,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-DetectFacesResponseTypeDef = TypedDict(
-    "DetectFacesResponseTypeDef",
-    {
-        "FaceDetails": List[FaceDetailTypeDef],
-        "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-FaceDetectionTypeDef = TypedDict(
-    "FaceDetectionTypeDef",
-    {
-        "Timestamp": int,
-        "Face": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-FaceRecordTypeDef = TypedDict(
-    "FaceRecordTypeDef",
-    {
-        "Face": FaceTypeDef,
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
-
-PersonDetailTypeDef = TypedDict(
-    "PersonDetailTypeDef",
+_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalStartStreamProcessorRequestRequestTypeDef",
     {
-        "Index": int,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
+        "StartSelector": StreamProcessingStartSelectorTypeDef,
+        "StopSelector": StreamProcessingStopSelectorTypeDef,
     },
     total=False,
 )
 
-SearchedFaceDetailsTypeDef = TypedDict(
-    "SearchedFaceDetailsTypeDef",
-    {
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
 
-UnindexedFaceTypeDef = TypedDict(
-    "UnindexedFaceTypeDef",
-    {
-        "Reasons": List[ReasonType],
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
+class StartStreamProcessorRequestRequestTypeDef(
+    _RequiredStartStreamProcessorRequestRequestTypeDef,
+    _OptionalStartStreamProcessorRequestRequestTypeDef,
+):
+    pass
 
-UnsearchedFaceTypeDef = TypedDict(
-    "UnsearchedFaceTypeDef",
-    {
-        "FaceDetails": FaceDetailTypeDef,
-        "Reasons": List[UnsearchedFaceReasonType],
-    },
-    total=False,
-)
 
-CustomLabelTypeDef = TypedDict(
-    "CustomLabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
-    },
-    total=False,
-)
-
-TextDetectionTypeDef = TypedDict(
-    "TextDetectionTypeDef",
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
     {
-        "DetectedText": str,
-        "Type": TextTypesType,
-        "Id": int,
-        "ParentId": int,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceTypeDef,
+        "SearchedUser": SearchedUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DetectTextFiltersTypeDef = TypedDict(
     "DetectTextFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
@@ -3307,71 +3522,14 @@
 class UpdateStreamProcessorRequestRequestTypeDef(
     _RequiredUpdateStreamProcessorRequestRequestTypeDef,
     _OptionalUpdateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
-    {
-        "MinConfidence": float,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DetectModerationLabelsRequestRequestTypeDef(
-    _RequiredDetectModerationLabelsRequestRequestTypeDef,
-    _OptionalDetectModerationLabelsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredStartStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalStartStreamProcessorRequestRequestTypeDef",
-    {
-        "StartSelector": StreamProcessingStartSelectorTypeDef,
-        "StopSelector": StreamProcessingStopSelectorTypeDef,
-    },
-    total=False,
-)
-
-
-class StartStreamProcessorRequestRequestTypeDef(
-    _RequiredStartStreamProcessorRequestRequestTypeDef,
-    _OptionalStartStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
-SearchUsersResponseTypeDef = TypedDict(
-    "SearchUsersResponseTypeDef",
-    {
-        "UserMatches": List[UserMatchTypeDef],
-        "FaceModelVersion": str,
-        "SearchedFace": SearchedFaceTypeDef,
-        "SearchedUser": SearchedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamProcessorRequestRequestTypeDef",
     {
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "Name": str,
         "Settings": StreamProcessorSettingsTypeDef,
@@ -3403,111 +3561,89 @@
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
-        "Input": StreamProcessorInputTypeDef,
+        "Input": StreamProcessorInputOutputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "Settings": StreamProcessorSettingsOutputTypeDef,
+        "NotificationChannel": StreamProcessorNotificationChannelOutputTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": List[VideoMetadataTypeDef],
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesByImageResponseTypeDef = TypedDict(
     "SearchFacesByImageResponseTypeDef",
     {
-        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
+        "SearchedFaceBoundingBox": BoundingBoxOutputTypeDef,
         "SearchedFaceConfidence": float,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesResponseTypeDef = TypedDict(
     "SearchFacesResponseTypeDef",
     {
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TestingDataTypeDef = TypedDict(
-    "TestingDataTypeDef",
+TestingDataOutputTypeDef = TypedDict(
+    "TestingDataOutputTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
+        "Assets": List[AssetOutputTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
-TrainingDataTypeDef = TypedDict(
-    "TrainingDataTypeDef",
+TrainingDataOutputTypeDef = TypedDict(
+    "TrainingDataOutputTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
+        "Assets": List[AssetOutputTypeDef],
     },
     total=False,
 )
 
 ValidationDataTypeDef = TypedDict(
     "ValidationDataTypeDef",
     {
-        "Assets": List[AssetTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "ProjectArn": str,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetSource": DatasetSourceTypeDef,
+        "Assets": List[AssetOutputTypeDef],
     },
     total=False,
 )
 
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -3532,49 +3668,49 @@
 
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompareFacesResponseTypeDef = TypedDict(
     "CompareFacesResponseTypeDef",
     {
         "SourceImageFace": ComparedSourceImageFaceTypeDef,
         "FaceMatches": List[CompareFacesMatchTypeDef],
         "UnmatchedFaces": List[ComparedFaceTypeDef],
         "SourceImageOrientationCorrection": OrientationCorrectionType,
         "TargetImageOrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "Id": int,
     },
     total=False,
 )
 
 DetectLabelsResponseTypeDef = TypedDict(
     "DetectLabelsResponseTypeDef",
     {
         "Labels": List[LabelTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "LabelModelVersion": str,
         "ImageProperties": DetectLabelsImagePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3600,17 +3736,17 @@
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3632,55 +3768,94 @@
 IndexFacesResponseTypeDef = TypedDict(
     "IndexFacesResponseTypeDef",
     {
         "FaceRecords": List[FaceRecordTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "FaceModelVersion": str,
         "UnindexedFaces": List[UnindexedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchUsersByImageResponseTypeDef = TypedDict(
     "SearchUsersByImageResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceDetailsTypeDef,
         "UnsearchedFaces": List[UnsearchedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectCustomLabelsResponseTypeDef = TypedDict(
     "DetectCustomLabelsResponseTypeDef",
     {
         "CustomLabels": List[CustomLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectTextResponseTypeDef = TypedDict(
     "DetectTextResponseTypeDef",
     {
         "TextDetections": List[TextDetectionTypeDef],
         "TextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TextDetectionResultTypeDef = TypedDict(
     "TextDetectionResultTypeDef",
     {
         "Timestamp": int,
         "TextDetection": TextDetectionTypeDef,
     },
     total=False,
 )
 
+TestingDataTypeDef = TypedDict(
+    "TestingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+        "AutoCreate": bool,
+    },
+    total=False,
+)
+
+TrainingDataTypeDef = TypedDict(
+    "TrainingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "ProjectArn": str,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetSource": DatasetSourceTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredDetectTextRequestRequestTypeDef = TypedDict(
     "_RequiredDetectTextRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectTextRequestRequestTypeDef = TypedDict(
@@ -3719,172 +3894,172 @@
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectVersionRequestRequestTypeDef",
-    {
-        "ProjectArn": str,
-        "VersionName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectVersionRequestRequestTypeDef",
-    {
-        "TrainingData": TrainingDataTypeDef,
-        "TestingData": TestingDataTypeDef,
-        "Tags": Mapping[str, str],
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class CreateProjectVersionRequestRequestTypeDef(
-    _RequiredCreateProjectVersionRequestRequestTypeDef,
-    _OptionalCreateProjectVersionRequestRequestTypeDef,
-):
-    pass
-
-
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataTypeDef,
-        "Output": TestingDataTypeDef,
+        "Input": TestingDataOutputTypeDef,
+        "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataTypeDef,
-        "Output": TrainingDataTypeDef,
+        "Input": TrainingDataOutputTypeDef,
+        "Output": TrainingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
     {
         "ProtectiveEquipmentModelVersion": str,
         "Persons": List[ProtectiveEquipmentPersonTypeDef],
         "Summary": ProtectiveEquipmentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLabelDetectionResponseTypeDef = TypedDict(
     "GetLabelDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
     "GetCelebrityRecognitionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectVersionRequestRequestTypeDef",
+    {
+        "ProjectArn": str,
+        "VersionName": str,
+        "OutputConfig": OutputConfigTypeDef,
+    },
+)
+_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectVersionRequestRequestTypeDef",
+    {
+        "TrainingData": TrainingDataTypeDef,
+        "TestingData": TestingDataTypeDef,
+        "Tags": Mapping[str, str],
+        "KmsKeyId": str,
     },
+    total=False,
 )
 
+
+class CreateProjectVersionRequestRequestTypeDef(
+    _RequiredCreateProjectVersionRequestRequestTypeDef,
+    _OptionalCreateProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
         "CreationTimestamp": datetime,
         "MinInferenceUnits": int,
         "Status": ProjectVersionStatusType,
         "StatusMessage": str,
         "BillableTrainingTimeInSeconds": int,
         "TrainingEndTimestamp": datetime,
-        "OutputConfig": OutputConfigTypeDef,
+        "OutputConfig": OutputConfigOutputTypeDef,
         "TrainingDataResult": TrainingDataResultTypeDef,
         "TestingDataResult": TestingDataResultTypeDef,
         "EvaluationResult": EvaluationResultTypeDef,
-        "ManifestSummary": GroundTruthManifestTypeDef,
+        "ManifestSummary": GroundTruthManifestOutputTypeDef,
         "KmsKeyId": str,
         "MaxInferenceUnits": int,
         "SourceProjectVersionArn": str,
     },
     total=False,
 )
 
 DescribeProjectVersionsResponseTypeDef = TypedDict(
     "DescribeProjectVersionsResponseTypeDef",
     {
         "ProjectVersionDescriptions": List[ProjectVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,69 +67,62 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
+    "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
-    "BoundingBoxTypeDef",
-    "S3ObjectTypeDef",
+    "BoundingBoxOutputTypeDef",
+    "S3ObjectOutputTypeDef",
     "BeardTypeDef",
     "BlackFrameTypeDef",
+    "BoundingBoxTypeDef",
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
+    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
-    "CopyProjectVersionResponseTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
-    "CreateCollectionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
     "LivenessOutputConfigTypeDef",
-    "CreateFaceLivenessSessionResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateProjectVersionResponseTypeDef",
     "StreamProcessorDataSharingPreferenceTypeDef",
     "StreamProcessorNotificationChannelTypeDef",
-    "CreateStreamProcessorResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DatasetChangesTypeDef",
     "DatasetStatsTypeDef",
     "DatasetLabelStatsTypeDef",
     "DatasetMetadataTypeDef",
     "DeleteCollectionRequestRequestTypeDef",
-    "DeleteCollectionResponseTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteFacesRequestRequestTypeDef",
     "UnsuccessfulFaceDeletionTypeDef",
     "DeleteProjectPolicyRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteProjectVersionRequestRequestTypeDef",
-    "DeleteProjectVersionResponseTypeDef",
     "DeleteStreamProcessorRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeCollectionRequestRequestTypeDef",
-    "DescribeCollectionResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
-    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeProjectVersionsRequestRequestTypeDef",
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     "DescribeProjectsRequestRequestTypeDef",
     "DescribeStreamProcessorRequestRequestTypeDef",
+    "StreamProcessorDataSharingPreferenceOutputTypeDef",
+    "StreamProcessorNotificationChannelOutputTypeDef",
     "DetectLabelsImageQualityTypeDef",
     "DominantColorTypeDef",
     "DetectLabelsImagePropertiesSettingsTypeDef",
     "GeneralLabelsSettingsTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ProtectiveEquipmentSummarizationAttributesTypeDef",
     "ProtectiveEquipmentSummaryTypeDef",
@@ -142,190 +135,211 @@
     "EyeOpenTypeDef",
     "EyeglassesTypeDef",
     "FaceOccludedTypeDef",
     "GenderTypeDef",
     "MouthOpenTypeDef",
     "MustacheTypeDef",
     "SunglassesTypeDef",
+    "FaceSearchSettingsOutputTypeDef",
     "FaceSearchSettingsTypeDef",
-    "PointTypeDef",
+    "PointOutputTypeDef",
     "GetCelebrityInfoRequestRequestTypeDef",
     "GetCelebrityRecognitionRequestRequestTypeDef",
     "VideoMetadataTypeDef",
     "GetContentModerationRequestMetadataTypeDef",
     "GetContentModerationRequestRequestTypeDef",
     "GetFaceDetectionRequestRequestTypeDef",
     "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     "GetFaceSearchRequestRequestTypeDef",
     "GetLabelDetectionRequestMetadataTypeDef",
     "GetLabelDetectionRequestRequestTypeDef",
     "GetPersonTrackingRequestRequestTypeDef",
     "GetSegmentDetectionRequestRequestTypeDef",
     "SegmentTypeInfoTypeDef",
     "GetTextDetectionRequestRequestTypeDef",
+    "S3ObjectTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "KinesisDataStreamTypeDef",
+    "KinesisVideoStreamOutputTypeDef",
     "KinesisVideoStreamStartSelectorTypeDef",
     "KinesisVideoStreamTypeDef",
     "LabelAliasTypeDef",
     "LabelCategoryTypeDef",
     "ParentTypeDef",
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
     "ListCollectionsRequestRequestTypeDef",
-    "ListCollectionsResponseTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     "ListDatasetLabelsRequestRequestTypeDef",
-    "ListFacesRequestListFacesPaginateTypeDef",
     "ListFacesRequestRequestTypeDef",
-    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     "ListProjectPoliciesRequestRequestTypeDef",
     "ProjectPolicyTypeDef",
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     "ListStreamProcessorsRequestRequestTypeDef",
     "StreamProcessorTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "MatchedUserTypeDef",
     "NotificationChannelTypeDef",
-    "PaginatorConfigTypeDef",
+    "OutputConfigOutputTypeDef",
+    "PointTypeDef",
     "PutProjectPolicyRequestRequestTypeDef",
-    "PutProjectPolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3DestinationTypeDef",
     "SearchFacesRequestRequestTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchedFaceTypeDef",
     "SearchedUserTypeDef",
     "ShotSegmentTypeDef",
     "TechnicalCueSegmentTypeDef",
+    "StartProjectVersionRequestRequestTypeDef",
+    "StartShotDetectionFilterTypeDef",
+    "StreamProcessingStopSelectorTypeDef",
+    "StopProjectVersionRequestRequestTypeDef",
+    "StopStreamProcessorRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "CopyProjectVersionResponseTypeDef",
+    "CreateCollectionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateFaceLivenessSessionResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateProjectVersionResponseTypeDef",
+    "CreateStreamProcessorResponseTypeDef",
+    "DeleteCollectionResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteProjectVersionResponseTypeDef",
+    "DescribeCollectionResponseTypeDef",
+    "ListCollectionsResponseTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutProjectPolicyResponseTypeDef",
     "StartCelebrityRecognitionResponseTypeDef",
     "StartContentModerationResponseTypeDef",
     "StartFaceDetectionResponseTypeDef",
     "StartFaceSearchResponseTypeDef",
     "StartLabelDetectionResponseTypeDef",
     "StartPersonTrackingResponseTypeDef",
-    "StartProjectVersionRequestRequestTypeDef",
     "StartProjectVersionResponseTypeDef",
-    "StartShotDetectionFilterTypeDef",
     "StartSegmentDetectionResponseTypeDef",
-    "StreamProcessingStopSelectorTypeDef",
     "StartStreamProcessorResponseTypeDef",
     "StartTextDetectionResponseTypeDef",
-    "StopProjectVersionRequestRequestTypeDef",
     "StopProjectVersionResponseTypeDef",
-    "StopStreamProcessorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "AssociateFacesResponseTypeDef",
     "ComparedSourceImageFaceTypeDef",
     "FaceTypeDef",
     "AuditImageTypeDef",
-    "GroundTruthManifestTypeDef",
-    "ImageTypeDef",
+    "GroundTruthManifestOutputTypeDef",
     "SummaryTypeDef",
-    "VideoTypeDef",
+    "VideoOutputTypeDef",
     "StartTechnicalCueDetectionFilterTypeDef",
     "GetCelebrityInfoResponseTypeDef",
     "ComparedFaceTypeDef",
     "StreamProcessorSettingsForUpdateTypeDef",
     "ContentModerationDetectionTypeDef",
     "CopyProjectVersionRequestRequestTypeDef",
     "EquipmentDetectionTypeDef",
     "CreateFaceLivenessSessionRequestSettingsTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetLabelDescriptionTypeDef",
     "ProjectDescriptionTypeDef",
     "DeleteFacesResponseTypeDef",
+    "DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    "ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    "ListFacesRequestListFacesPaginateTypeDef",
+    "ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     "DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     "DetectLabelsImageBackgroundTypeDef",
     "DetectLabelsImageForegroundTypeDef",
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
+    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
-    "RegionOfInterestTypeDef",
+    "RegionOfInterestOutputTypeDef",
+    "GroundTruthManifestTypeDef",
+    "ImageTypeDef",
+    "VideoTypeDef",
     "HumanLoopConfigTypeDef",
+    "StreamProcessorInputOutputTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
     "UserMatchTypeDef",
+    "RegionOfInterestTypeDef",
     "StreamProcessorOutputTypeDef",
     "SegmentDetectionTypeDef",
     "FaceMatchTypeDef",
     "ListFacesResponseTypeDef",
     "GetFaceLivenessSessionResultsResponseTypeDef",
-    "AssetTypeDef",
-    "DatasetSourceTypeDef",
-    "CompareFacesRequestRequestTypeDef",
-    "DetectCustomLabelsRequestRequestTypeDef",
-    "DetectFacesRequestRequestTypeDef",
-    "DetectProtectiveEquipmentRequestRequestTypeDef",
-    "IndexFacesRequestRequestTypeDef",
-    "RecognizeCelebritiesRequestRequestTypeDef",
-    "SearchFacesByImageRequestRequestTypeDef",
-    "SearchUsersByImageRequestRequestTypeDef",
+    "AssetOutputTypeDef",
     "EvaluationResultTypeDef",
-    "StartCelebrityRecognitionRequestRequestTypeDef",
-    "StartContentModerationRequestRequestTypeDef",
-    "StartFaceDetectionRequestRequestTypeDef",
-    "StartFaceSearchRequestRequestTypeDef",
-    "StartPersonTrackingRequestRequestTypeDef",
     "StartSegmentDetectionFiltersTypeDef",
     "CelebrityTypeDef",
     "CompareFacesMatchTypeDef",
     "GetContentModerationResponseTypeDef",
     "ProtectiveEquipmentBodyPartTypeDef",
     "CreateFaceLivenessSessionRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetLabelsResponseTypeDef",
     "DescribeProjectsResponseTypeDef",
     "DetectLabelsImagePropertiesTypeDef",
     "LabelTypeDef",
-    "DetectLabelsRequestRequestTypeDef",
-    "StartLabelDetectionRequestRequestTypeDef",
     "CelebrityDetailTypeDef",
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
-    "DetectTextFiltersTypeDef",
-    "StartTextDetectionFiltersTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
+    "AssetTypeDef",
+    "DatasetSourceTypeDef",
+    "CompareFacesRequestRequestTypeDef",
+    "DetectCustomLabelsRequestRequestTypeDef",
+    "DetectFacesRequestRequestTypeDef",
+    "DetectLabelsRequestRequestTypeDef",
+    "DetectProtectiveEquipmentRequestRequestTypeDef",
+    "IndexFacesRequestRequestTypeDef",
+    "RecognizeCelebritiesRequestRequestTypeDef",
+    "SearchFacesByImageRequestRequestTypeDef",
+    "SearchUsersByImageRequestRequestTypeDef",
+    "StartCelebrityRecognitionRequestRequestTypeDef",
+    "StartContentModerationRequestRequestTypeDef",
+    "StartFaceDetectionRequestRequestTypeDef",
+    "StartFaceSearchRequestRequestTypeDef",
+    "StartLabelDetectionRequestRequestTypeDef",
+    "StartPersonTrackingRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
+    "DetectTextFiltersTypeDef",
+    "StartTextDetectionFiltersTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
-    "TestingDataTypeDef",
-    "TrainingDataTypeDef",
+    "TestingDataOutputTypeDef",
+    "TrainingDataOutputTypeDef",
     "ValidationDataTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
     "DetectLabelsResponseTypeDef",
     "LabelDetectionTypeDef",
     "CelebrityRecognitionTypeDef",
@@ -333,25 +347,28 @@
     "PersonDetectionTypeDef",
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
+    "TestingDataTypeDef",
+    "TrainingDataTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DetectTextRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "CreateProjectVersionRequestRequestTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
     "GetTextDetectionResponseTypeDef",
+    "CreateProjectVersionRequestRequestTypeDef",
     "ProjectVersionDescriptionTypeDef",
     "DescribeProjectVersionsResponseTypeDef",
 )
 
 AgeRangeTypeDef = TypedDict(
     "AgeRangeTypeDef",
     {
@@ -387,14 +404,25 @@
     "AssociatedFaceTypeDef",
     {
         "FaceId": str,
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
 UnsuccessfulFaceAssociationTypeDef = TypedDict(
     "UnsuccessfulFaceAssociationTypeDef",
     {
         "FaceId": str,
         "UserId": str,
         "Confidence": float,
         "Reasons": List[UnsuccessfulFaceAssociationReasonType],
@@ -409,27 +437,27 @@
         "DurationMillis": int,
         "SampleRate": int,
         "NumberOfChannels": int,
     },
     total=False,
 )
 
-BoundingBoxTypeDef = TypedDict(
-    "BoundingBoxTypeDef",
+BoundingBoxOutputTypeDef = TypedDict(
+    "BoundingBoxOutputTypeDef",
     {
         "Width": float,
         "Height": float,
         "Left": float,
         "Top": float,
     },
     total=False,
 )
 
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
+S3ObjectOutputTypeDef = TypedDict(
+    "S3ObjectOutputTypeDef",
     {
         "Bucket": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
@@ -448,14 +476,25 @@
     {
         "MaxPixelThreshold": float,
         "MinCoveragePercentage": float,
     },
     total=False,
 )
 
+BoundingBoxTypeDef = TypedDict(
+    "BoundingBoxTypeDef",
+    {
+        "Width": float,
+        "Height": float,
+        "Left": float,
+        "Top": float,
+    },
+    total=False,
+)
+
 KnownGenderTypeDef = TypedDict(
     "KnownGenderTypeDef",
     {
         "Type": KnownGenderTypeType,
     },
     total=False,
 )
@@ -512,14 +551,33 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
+_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_RequiredConnectedHomeSettingsOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+)
+_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
+    "_OptionalConnectedHomeSettingsOutputTypeDef",
+    {
+        "MinConfidence": float,
+    },
+    total=False,
+)
+
+class ConnectedHomeSettingsOutputTypeDef(
+    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
+):
+    pass
+
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
@@ -550,22 +608,14 @@
     {
         "S3Bucket": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-CopyProjectVersionResponseTypeDef = TypedDict(
-    "CopyProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CoversBodyPartTypeDef = TypedDict(
     "CoversBodyPartTypeDef",
     {
         "Confidence": float,
         "Value": bool,
     },
     total=False,
@@ -586,32 +636,14 @@
 )
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
-CreateCollectionResponseTypeDef = TypedDict(
-    "CreateCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "CollectionArn": str,
-        "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLivenessOutputConfigTypeDef = TypedDict(
     "_RequiredLivenessOutputConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalLivenessOutputConfigTypeDef = TypedDict(
@@ -623,67 +655,35 @@
 )
 
 class LivenessOutputConfigTypeDef(
     _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
 ):
     pass
 
-CreateFaceLivenessSessionResponseTypeDef = TypedDict(
-    "CreateFaceLivenessSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "ProjectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProjectVersionResponseTypeDef = TypedDict(
-    "CreateProjectVersionResponseTypeDef",
-    {
-        "ProjectVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StreamProcessorDataSharingPreferenceTypeDef = TypedDict(
     "StreamProcessorDataSharingPreferenceTypeDef",
     {
         "OptIn": bool,
     },
 )
 
 StreamProcessorNotificationChannelTypeDef = TypedDict(
     "StreamProcessorNotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
     },
 )
 
-CreateStreamProcessorResponseTypeDef = TypedDict(
-    "CreateStreamProcessorResponseTypeDef",
-    {
-        "StreamProcessorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "CollectionId": str,
         "UserId": str,
     },
 )
@@ -743,22 +743,14 @@
 DeleteCollectionRequestRequestTypeDef = TypedDict(
     "DeleteCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DeleteCollectionResponseTypeDef = TypedDict(
-    "DeleteCollectionResponseTypeDef",
-    {
-        "StatusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -804,37 +796,21 @@
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "Status": ProjectStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectVersionRequestRequestTypeDef = TypedDict(
     "DeleteProjectVersionRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
     },
 )
 
-DeleteProjectVersionResponseTypeDef = TypedDict(
-    "DeleteProjectVersionResponseTypeDef",
-    {
-        "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteStreamProcessorRequestRequestTypeDef = TypedDict(
     "DeleteStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -861,54 +837,31 @@
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
-DescribeCollectionResponseTypeDef = TypedDict(
-    "DescribeCollectionResponseTypeDef",
-    {
-        "FaceCount": int,
-        "FaceModelVersion": str,
-        "CollectionARN": str,
-        "CreationTimestamp": datetime,
-        "UserCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
-_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "VersionNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
-    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
-):
-    pass
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -932,23 +885,14 @@
 
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
-DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
-    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
-    {
-        "ProjectNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
     },
@@ -958,14 +902,28 @@
 DescribeStreamProcessorRequestRequestTypeDef = TypedDict(
     "DescribeStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StreamProcessorDataSharingPreferenceOutputTypeDef = TypedDict(
+    "StreamProcessorDataSharingPreferenceOutputTypeDef",
+    {
+        "OptIn": bool,
+    },
+)
+
+StreamProcessorNotificationChannelOutputTypeDef = TypedDict(
+    "StreamProcessorNotificationChannelOutputTypeDef",
+    {
+        "SNSTopicArn": str,
+    },
+)
+
 DetectLabelsImageQualityTypeDef = TypedDict(
     "DetectLabelsImageQualityTypeDef",
     {
         "Brightness": float,
         "Sharpness": float,
         "Contrast": float,
     },
@@ -1158,25 +1116,34 @@
     {
         "Value": bool,
         "Confidence": float,
     },
     total=False,
 )
 
+FaceSearchSettingsOutputTypeDef = TypedDict(
+    "FaceSearchSettingsOutputTypeDef",
+    {
+        "CollectionId": str,
+        "FaceMatchThreshold": float,
+    },
+    total=False,
+)
+
 FaceSearchSettingsTypeDef = TypedDict(
     "FaceSearchSettingsTypeDef",
     {
         "CollectionId": str,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
-PointTypeDef = TypedDict(
-    "PointTypeDef",
+PointOutputTypeDef = TypedDict(
+    "PointOutputTypeDef",
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
@@ -1401,14 +1368,24 @@
 )
 
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
+    {
+        "Bucket": str,
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -1417,14 +1394,22 @@
     "KinesisDataStreamTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
+KinesisVideoStreamOutputTypeDef = TypedDict(
+    "KinesisVideoStreamOutputTypeDef",
+    {
+        "Arn": str,
+    },
+    total=False,
+)
+
 KinesisVideoStreamStartSelectorTypeDef = TypedDict(
     "KinesisVideoStreamStartSelectorTypeDef",
     {
         "ProducerTimestamp": int,
         "FragmentNumber": str,
     },
     total=False,
@@ -1458,65 +1443,23 @@
     "ParentTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
-    "ListCollectionsRequestListCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCollectionsResponseTypeDef = TypedDict(
-    "ListCollectionsResponseTypeDef",
-    {
-        "CollectionIds": List[str],
-        "NextToken": str,
-        "FaceModelVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ContainsLabels": Sequence[str],
-        "Labeled": bool,
-        "SourceRefContains": str,
-        "HasErrors": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetEntriesRequestRequestTypeDef = TypedDict(
@@ -1534,43 +1477,14 @@
 
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "DatasetArn": str,
-    },
-)
-_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
-    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestRequestTypeDef = TypedDict(
@@ -1583,36 +1497,14 @@
 )
 
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_RequiredListFacesRequestListFacesPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
-    "_OptionalListFacesRequestListFacesPaginateTypeDef",
-    {
-        "UserId": str,
-        "FaceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFacesRequestListFacesPaginateTypeDef(
-    _RequiredListFacesRequestListFacesPaginateTypeDef,
-    _OptionalListFacesRequestListFacesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
@@ -1627,34 +1519,14 @@
 )
 
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "ProjectArn": str,
-    },
-)
-_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
-    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestRequestTypeDef = TypedDict(
@@ -1681,22 +1553,14 @@
         "PolicyDocument": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
-    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamProcessorsRequestRequestTypeDef = TypedDict(
     "ListStreamProcessorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1714,42 +1578,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1788,20 +1624,28 @@
     "NotificationChannelTypeDef",
     {
         "SNSTopicArn": str,
         "RoleArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+OutputConfigOutputTypeDef = TypedDict(
+    "OutputConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "S3Bucket": str,
+        "S3KeyPrefix": str,
+    },
+    total=False,
+)
+
+PointTypeDef = TypedDict(
+    "PointTypeDef",
+    {
+        "X": float,
+        "Y": float,
     },
     total=False,
 )
 
 _RequiredPutProjectPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutProjectPolicyRequestRequestTypeDef",
     {
@@ -1819,33 +1663,14 @@
 )
 
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
-PutProjectPolicyResponseTypeDef = TypedDict(
-    "PutProjectPolicyResponseTypeDef",
-    {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-)
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
     total=False,
@@ -1924,241 +1749,361 @@
     {
         "Type": TechnicalCueTypeType,
         "Confidence": float,
     },
     total=False,
 )
 
-StartCelebrityRecognitionResponseTypeDef = TypedDict(
-    "StartCelebrityRecognitionResponseTypeDef",
+_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
+        "MinInferenceUnits": int,
     },
 )
+_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartProjectVersionRequestRequestTypeDef",
+    {
+        "MaxInferenceUnits": int,
+    },
+    total=False,
+)
 
-StartContentModerationResponseTypeDef = TypedDict(
-    "StartContentModerationResponseTypeDef",
+class StartProjectVersionRequestRequestTypeDef(
+    _RequiredStartProjectVersionRequestRequestTypeDef,
+    _OptionalStartProjectVersionRequestRequestTypeDef,
+):
+    pass
+
+StartShotDetectionFilterTypeDef = TypedDict(
+    "StartShotDetectionFilterTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MinSegmentConfidence": float,
     },
+    total=False,
 )
 
-StartFaceDetectionResponseTypeDef = TypedDict(
-    "StartFaceDetectionResponseTypeDef",
+StreamProcessingStopSelectorTypeDef = TypedDict(
+    "StreamProcessingStopSelectorTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxDurationInSeconds": int,
     },
+    total=False,
 )
 
-StartFaceSearchResponseTypeDef = TypedDict(
-    "StartFaceSearchResponseTypeDef",
+StopProjectVersionRequestRequestTypeDef = TypedDict(
+    "StopProjectVersionRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProjectVersionArn": str,
     },
 )
 
-StartLabelDetectionResponseTypeDef = TypedDict(
-    "StartLabelDetectionResponseTypeDef",
+StopStreamProcessorRequestRequestTypeDef = TypedDict(
+    "StopStreamProcessorRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
 
-StartPersonTrackingResponseTypeDef = TypedDict(
-    "StartPersonTrackingResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-_RequiredStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartProjectVersionRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+CopyProjectVersionResponseTypeDef = TypedDict(
+    "CopyProjectVersionResponseTypeDef",
     {
         "ProjectVersionArn": str,
-        "MinInferenceUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartProjectVersionRequestRequestTypeDef",
+
+CreateCollectionResponseTypeDef = TypedDict(
+    "CreateCollectionResponseTypeDef",
     {
-        "MaxInferenceUnits": int,
+        "StatusCode": int,
+        "CollectionArn": str,
+        "FaceModelVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class StartProjectVersionRequestRequestTypeDef(
-    _RequiredStartProjectVersionRequestRequestTypeDef,
-    _OptionalStartProjectVersionRequestRequestTypeDef,
-):
-    pass
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-StartProjectVersionResponseTypeDef = TypedDict(
-    "StartProjectVersionResponseTypeDef",
+CreateFaceLivenessSessionResponseTypeDef = TypedDict(
+    "CreateFaceLivenessSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectVersionResponseTypeDef = TypedDict(
+    "CreateProjectVersionResponseTypeDef",
+    {
+        "ProjectVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamProcessorResponseTypeDef = TypedDict(
+    "CreateStreamProcessorResponseTypeDef",
+    {
+        "StreamProcessorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCollectionResponseTypeDef = TypedDict(
+    "DeleteCollectionResponseTypeDef",
+    {
+        "StatusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Status": ProjectStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectVersionResponseTypeDef = TypedDict(
+    "DeleteProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartShotDetectionFilterTypeDef = TypedDict(
-    "StartShotDetectionFilterTypeDef",
+DescribeCollectionResponseTypeDef = TypedDict(
+    "DescribeCollectionResponseTypeDef",
     {
-        "MinSegmentConfidence": float,
+        "FaceCount": int,
+        "FaceModelVersion": str,
+        "CollectionARN": str,
+        "CreationTimestamp": datetime,
+        "UserCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartSegmentDetectionResponseTypeDef = TypedDict(
-    "StartSegmentDetectionResponseTypeDef",
+ListCollectionsResponseTypeDef = TypedDict(
+    "ListCollectionsResponseTypeDef",
+    {
+        "CollectionIds": List[str],
+        "NextToken": str,
+        "FaceModelVersions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProjectPolicyResponseTypeDef = TypedDict(
+    "PutProjectPolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCelebrityRecognitionResponseTypeDef = TypedDict(
+    "StartCelebrityRecognitionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamProcessingStopSelectorTypeDef = TypedDict(
-    "StreamProcessingStopSelectorTypeDef",
+StartContentModerationResponseTypeDef = TypedDict(
+    "StartContentModerationResponseTypeDef",
     {
-        "MaxDurationInSeconds": int,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-StartStreamProcessorResponseTypeDef = TypedDict(
-    "StartStreamProcessorResponseTypeDef",
+StartFaceDetectionResponseTypeDef = TypedDict(
+    "StartFaceDetectionResponseTypeDef",
     {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTextDetectionResponseTypeDef = TypedDict(
-    "StartTextDetectionResponseTypeDef",
+StartFaceSearchResponseTypeDef = TypedDict(
+    "StartFaceSearchResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionRequestRequestTypeDef = TypedDict(
-    "StopProjectVersionRequestRequestTypeDef",
+StartLabelDetectionResponseTypeDef = TypedDict(
+    "StartLabelDetectionResponseTypeDef",
     {
-        "ProjectVersionArn": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopProjectVersionResponseTypeDef = TypedDict(
-    "StopProjectVersionResponseTypeDef",
+StartPersonTrackingResponseTypeDef = TypedDict(
+    "StartPersonTrackingResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartProjectVersionResponseTypeDef = TypedDict(
+    "StartProjectVersionResponseTypeDef",
     {
         "Status": ProjectVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopStreamProcessorRequestRequestTypeDef = TypedDict(
-    "StopStreamProcessorRequestRequestTypeDef",
+StartSegmentDetectionResponseTypeDef = TypedDict(
+    "StartSegmentDetectionResponseTypeDef",
     {
-        "Name": str,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartStreamProcessorResponseTypeDef = TypedDict(
+    "StartStreamProcessorResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartTextDetectionResponseTypeDef = TypedDict(
+    "StartTextDetectionResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopProjectVersionResponseTypeDef = TypedDict(
+    "StopProjectVersionResponseTypeDef",
+    {
+        "Status": ProjectVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateFacesResponseTypeDef = TypedDict(
     "AssociateFacesResponseTypeDef",
     {
         "AssociatedFaces": List[AssociatedFaceTypeDef],
         "UnsuccessfulFaceAssociations": List[UnsuccessfulFaceAssociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedSourceImageFaceTypeDef = TypedDict(
     "ComparedSourceImageFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
     },
     total=False,
 )
 
 FaceTypeDef = TypedDict(
     "FaceTypeDef",
     {
         "FaceId": str,
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "ImageId": str,
         "ExternalImageId": str,
         "Confidence": float,
         "IndexFacesModelVersion": str,
         "UserId": str,
     },
     total=False,
 )
 
 AuditImageTypeDef = TypedDict(
     "AuditImageTypeDef",
     {
         "Bytes": bytes,
-        "S3Object": S3ObjectTypeDef,
-        "BoundingBox": BoundingBoxTypeDef,
-    },
-    total=False,
-)
-
-GroundTruthManifestTypeDef = TypedDict(
-    "GroundTruthManifestTypeDef",
-    {
-        "S3Object": S3ObjectTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
     },
     total=False,
 )
 
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
+GroundTruthManifestOutputTypeDef = TypedDict(
+    "GroundTruthManifestOutputTypeDef",
     {
-        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Object": S3ObjectTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
 SummaryTypeDef = TypedDict(
     "SummaryTypeDef",
     {
-        "S3Object": S3ObjectTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
-VideoTypeDef = TypedDict(
-    "VideoTypeDef",
+VideoOutputTypeDef = TypedDict(
+    "VideoOutputTypeDef",
     {
-        "S3Object": S3ObjectTypeDef,
+        "S3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
 StartTechnicalCueDetectionFilterTypeDef = TypedDict(
     "StartTechnicalCueDetectionFilterTypeDef",
     {
@@ -2170,22 +2115,22 @@
 
 GetCelebrityInfoResponseTypeDef = TypedDict(
     "GetCelebrityInfoResponseTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "KnownGender": KnownGenderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComparedFaceTypeDef = TypedDict(
     "ComparedFaceTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "Landmarks": List[LandmarkTypeDef],
         "Pose": PoseTypeDef,
         "Quality": ImageQualityTypeDef,
         "Emotions": List[EmotionTypeDef],
         "Smile": SmileTypeDef,
     },
@@ -2236,15 +2181,15 @@
     _OptionalCopyProjectVersionRequestRequestTypeDef,
 ):
     pass
 
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
     },
     total=False,
 )
 
@@ -2299,18 +2244,170 @@
 )
 
 DeleteFacesResponseTypeDef = TypedDict(
     "DeleteFacesResponseTypeDef",
     {
         "DeletedFaces": List[str],
         "UnsuccessfulFaceDeletions": List[UnsuccessfulFaceDeletionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef",
+    {
+        "VersionNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
+    _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+):
+    pass
+
+DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
+    "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
+    {
+        "ProjectNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+ListCollectionsRequestListCollectionsPaginateTypeDef = TypedDict(
+    "ListCollectionsRequestListCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "ContainsLabels": Sequence[str],
+        "Labeled": bool,
+        "SourceRefContains": str,
+        "HasErrors": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "DatasetArn": str,
+    },
+)
+_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
+    _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_RequiredListFacesRequestListFacesPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
+    "_OptionalListFacesRequestListFacesPaginateTypeDef",
+    {
+        "UserId": str,
+        "FaceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFacesRequestListFacesPaginateTypeDef(
+    _RequiredListFacesRequestListFacesPaginateTypeDef,
+    _OptionalListFacesRequestListFacesPaginateTypeDef,
+):
+    pass
+
+_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "ProjectArn": str,
+    },
+)
+_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
+    _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+):
+    pass
+
+ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
+    "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
@@ -2370,15 +2467,15 @@
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
 )
 
 DetectLabelsSettingsTypeDef = TypedDict(
@@ -2400,39 +2497,39 @@
 
 DetectModerationLabelsResponseTypeDef = TypedDict(
     "DetectModerationLabelsResponseTypeDef",
     {
         "ModerationLabels": List[ModerationLabelTypeDef],
         "ModerationModelVersion": str,
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFacesResponseTypeDef = TypedDict(
     "DisassociateFacesResponseTypeDef",
     {
         "DisassociatedFaces": List[DisassociatedFaceTypeDef],
         "UnsuccessfulFaceDisassociations": List[UnsuccessfulFaceDisassociationTypeDef],
         "UserStatus": UserStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DistributeDatasetEntriesRequestRequestTypeDef = TypedDict(
     "DistributeDatasetEntriesRequestRequestTypeDef",
     {
         "Datasets": Sequence[DistributeDatasetTypeDef],
     },
 )
 
 FaceDetailTypeDef = TypedDict(
     "FaceDetailTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "AgeRange": AgeRangeTypeDef,
         "Smile": SmileTypeDef,
         "Eyeglasses": EyeglassesTypeDef,
         "Sunglasses": SunglassesTypeDef,
         "Gender": GenderTypeDef,
         "Beard": BeardTypeDef,
         "Mustache": MustacheTypeDef,
@@ -2445,37 +2542,71 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
+StreamProcessorSettingsOutputTypeDef = TypedDict(
+    "StreamProcessorSettingsOutputTypeDef",
+    {
+        "FaceSearch": FaceSearchSettingsOutputTypeDef,
+        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": List[PointTypeDef],
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Polygon": List[PointOutputTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestTypeDef = TypedDict(
-    "RegionOfInterestTypeDef",
+RegionOfInterestOutputTypeDef = TypedDict(
+    "RegionOfInterestOutputTypeDef",
     {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": Sequence[PointTypeDef],
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Polygon": List[PointOutputTypeDef],
+    },
+    total=False,
+)
+
+GroundTruthManifestTypeDef = TypedDict(
+    "GroundTruthManifestTypeDef",
+    {
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
+    {
+        "Bytes": Union[str, bytes, IO[Any], StreamingBody],
+        "S3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
+VideoTypeDef = TypedDict(
+    "VideoTypeDef",
+    {
+        "S3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
@@ -2490,14 +2621,22 @@
     },
     total=False,
 )
 
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
+StreamProcessorInputOutputTypeDef = TypedDict(
+    "StreamProcessorInputOutputTypeDef",
+    {
+        "KinesisVideoStream": KinesisVideoStreamOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2511,45 +2650,54 @@
 )
 
 ListProjectPoliciesResponseTypeDef = TypedDict(
     "ListProjectPoliciesResponseTypeDef",
     {
         "ProjectPolicies": List[ProjectPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamProcessorsResponseTypeDef = TypedDict(
     "ListStreamProcessorsResponseTypeDef",
     {
         "NextToken": str,
         "StreamProcessors": List[StreamProcessorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserMatchTypeDef = TypedDict(
     "UserMatchTypeDef",
     {
         "Similarity": float,
         "User": MatchedUserTypeDef,
     },
     total=False,
 )
 
+RegionOfInterestTypeDef = TypedDict(
+    "RegionOfInterestTypeDef",
+    {
+        "BoundingBox": BoundingBoxTypeDef,
+        "Polygon": Sequence[PointTypeDef],
+    },
+    total=False,
+)
+
 StreamProcessorOutputTypeDef = TypedDict(
     "StreamProcessorOutputTypeDef",
     {
         "KinesisDataStream": KinesisDataStreamTypeDef,
         "S3Destination": S3DestinationTypeDef,
     },
     total=False,
@@ -2585,28 +2733,263 @@
 
 ListFacesResponseTypeDef = TypedDict(
     "ListFacesResponseTypeDef",
     {
         "Faces": List[FaceTypeDef],
         "NextToken": str,
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceLivenessSessionResultsResponseTypeDef = TypedDict(
     "GetFaceLivenessSessionResultsResponseTypeDef",
     {
         "SessionId": str,
         "Status": LivenessSessionStatusType,
         "Confidence": float,
         "ReferenceImage": AuditImageTypeDef,
         "AuditImages": List[AuditImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssetOutputTypeDef = TypedDict(
+    "AssetOutputTypeDef",
+    {
+        "GroundTruthManifest": GroundTruthManifestOutputTypeDef,
+    },
+    total=False,
+)
+
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
+    {
+        "F1Score": float,
+        "Summary": SummaryTypeDef,
+    },
+    total=False,
+)
+
+StartSegmentDetectionFiltersTypeDef = TypedDict(
+    "StartSegmentDetectionFiltersTypeDef",
+    {
+        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
+        "ShotFilter": StartShotDetectionFilterTypeDef,
+    },
+    total=False,
+)
+
+CelebrityTypeDef = TypedDict(
+    "CelebrityTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Face": ComparedFaceTypeDef,
+        "MatchConfidence": float,
+        "KnownGender": KnownGenderTypeDef,
     },
+    total=False,
+)
+
+CompareFacesMatchTypeDef = TypedDict(
+    "CompareFacesMatchTypeDef",
+    {
+        "Similarity": float,
+        "Face": ComparedFaceTypeDef,
+    },
+    total=False,
+)
+
+GetContentModerationResponseTypeDef = TypedDict(
+    "GetContentModerationResponseTypeDef",
+    {
+        "JobStatus": VideoJobStatusType,
+        "StatusMessage": str,
+        "VideoMetadata": VideoMetadataTypeDef,
+        "ModerationLabels": List[ContentModerationDetectionTypeDef],
+        "NextToken": str,
+        "ModerationModelVersion": str,
+        "JobId": str,
+        "Video": VideoOutputTypeDef,
+        "JobTag": str,
+        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProtectiveEquipmentBodyPartTypeDef = TypedDict(
+    "ProtectiveEquipmentBodyPartTypeDef",
+    {
+        "Name": BodyPartType,
+        "Confidence": float,
+        "EquipmentDetections": List[EquipmentDetectionTypeDef],
+    },
+    total=False,
+)
+
+CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
+    "CreateFaceLivenessSessionRequestRequestTypeDef",
+    {
+        "KmsKeyId": str,
+        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetDescription": DatasetDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatasetLabelsResponseTypeDef = TypedDict(
+    "ListDatasetLabelsResponseTypeDef",
+    {
+        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProjectsResponseTypeDef = TypedDict(
+    "DescribeProjectsResponseTypeDef",
+    {
+        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectLabelsImagePropertiesTypeDef = TypedDict(
+    "DetectLabelsImagePropertiesTypeDef",
+    {
+        "Quality": DetectLabelsImageQualityTypeDef,
+        "DominantColors": List[DominantColorTypeDef],
+        "Foreground": DetectLabelsImageForegroundTypeDef,
+        "Background": DetectLabelsImageBackgroundTypeDef,
+    },
+    total=False,
+)
+
+LabelTypeDef = TypedDict(
+    "LabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Instances": List[InstanceTypeDef],
+        "Parents": List[ParentTypeDef],
+        "Aliases": List[LabelAliasTypeDef],
+        "Categories": List[LabelCategoryTypeDef],
+    },
+    total=False,
+)
+
+CelebrityDetailTypeDef = TypedDict(
+    "CelebrityDetailTypeDef",
+    {
+        "Urls": List[str],
+        "Name": str,
+        "Id": str,
+        "Confidence": float,
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Face": FaceDetailTypeDef,
+        "KnownGender": KnownGenderTypeDef,
+    },
+    total=False,
+)
+
+DetectFacesResponseTypeDef = TypedDict(
+    "DetectFacesResponseTypeDef",
+    {
+        "FaceDetails": List[FaceDetailTypeDef],
+        "OrientationCorrection": OrientationCorrectionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FaceDetectionTypeDef = TypedDict(
+    "FaceDetectionTypeDef",
+    {
+        "Timestamp": int,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+FaceRecordTypeDef = TypedDict(
+    "FaceRecordTypeDef",
+    {
+        "Face": FaceTypeDef,
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+PersonDetailTypeDef = TypedDict(
+    "PersonDetailTypeDef",
+    {
+        "Index": int,
+        "BoundingBox": BoundingBoxOutputTypeDef,
+        "Face": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+SearchedFaceDetailsTypeDef = TypedDict(
+    "SearchedFaceDetailsTypeDef",
+    {
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnindexedFaceTypeDef = TypedDict(
+    "UnindexedFaceTypeDef",
+    {
+        "Reasons": List[ReasonType],
+        "FaceDetail": FaceDetailTypeDef,
+    },
+    total=False,
+)
+
+UnsearchedFaceTypeDef = TypedDict(
+    "UnsearchedFaceTypeDef",
+    {
+        "FaceDetails": FaceDetailTypeDef,
+        "Reasons": List[UnsearchedFaceReasonType],
+    },
+    total=False,
+)
+
+CustomLabelTypeDef = TypedDict(
+    "CustomLabelTypeDef",
+    {
+        "Name": str,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
+)
+
+TextDetectionTypeDef = TypedDict(
+    "TextDetectionTypeDef",
+    {
+        "DetectedText": str,
+        "Type": TextTypesType,
+        "Id": int,
+        "ParentId": int,
+        "Confidence": float,
+        "Geometry": GeometryTypeDef,
+    },
+    total=False,
 )
 
 AssetTypeDef = TypedDict(
     "AssetTypeDef",
     {
         "GroundTruthManifest": GroundTruthManifestTypeDef,
     },
@@ -2680,14 +3063,36 @@
 )
 
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
+_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectLabelsRequestRequestTypeDef",
+    {
+        "Image": ImageTypeDef,
+    },
+)
+_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectLabelsRequestRequestTypeDef",
+    {
+        "MaxLabels": int,
+        "MinConfidence": float,
+        "Features": Sequence[DetectLabelsFeatureNameType],
+        "Settings": DetectLabelsSettingsTypeDef,
+    },
+    total=False,
+)
+
+class DetectLabelsRequestRequestTypeDef(
+    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
+):
+    pass
+
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
@@ -2776,23 +3181,14 @@
 
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
-EvaluationResultTypeDef = TypedDict(
-    "EvaluationResultTypeDef",
-    {
-        "F1Score": float,
-        "Summary": SummaryTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCelebrityRecognitionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartCelebrityRecognitionRequestRequestTypeDef = TypedDict(
@@ -2876,176 +3272,14 @@
 )
 
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPersonTrackingRequestRequestTypeDef",
-    {
-        "Video": VideoTypeDef,
-    },
-)
-_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPersonTrackingRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "JobTag": str,
-    },
-    total=False,
-)
-
-class StartPersonTrackingRequestRequestTypeDef(
-    _RequiredStartPersonTrackingRequestRequestTypeDef,
-    _OptionalStartPersonTrackingRequestRequestTypeDef,
-):
-    pass
-
-StartSegmentDetectionFiltersTypeDef = TypedDict(
-    "StartSegmentDetectionFiltersTypeDef",
-    {
-        "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
-        "ShotFilter": StartShotDetectionFilterTypeDef,
-    },
-    total=False,
-)
-
-CelebrityTypeDef = TypedDict(
-    "CelebrityTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Face": ComparedFaceTypeDef,
-        "MatchConfidence": float,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-CompareFacesMatchTypeDef = TypedDict(
-    "CompareFacesMatchTypeDef",
-    {
-        "Similarity": float,
-        "Face": ComparedFaceTypeDef,
-    },
-    total=False,
-)
-
-GetContentModerationResponseTypeDef = TypedDict(
-    "GetContentModerationResponseTypeDef",
-    {
-        "JobStatus": VideoJobStatusType,
-        "StatusMessage": str,
-        "VideoMetadata": VideoMetadataTypeDef,
-        "ModerationLabels": List[ContentModerationDetectionTypeDef],
-        "NextToken": str,
-        "ModerationModelVersion": str,
-        "JobId": str,
-        "Video": VideoTypeDef,
-        "JobTag": str,
-        "GetRequestMetadata": GetContentModerationRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProtectiveEquipmentBodyPartTypeDef = TypedDict(
-    "ProtectiveEquipmentBodyPartTypeDef",
-    {
-        "Name": BodyPartType,
-        "Confidence": float,
-        "EquipmentDetections": List[EquipmentDetectionTypeDef],
-    },
-    total=False,
-)
-
-CreateFaceLivenessSessionRequestRequestTypeDef = TypedDict(
-    "CreateFaceLivenessSessionRequestRequestTypeDef",
-    {
-        "KmsKeyId": str,
-        "Settings": CreateFaceLivenessSessionRequestSettingsTypeDef,
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDatasetLabelsResponseTypeDef = TypedDict(
-    "ListDatasetLabelsResponseTypeDef",
-    {
-        "DatasetLabelDescriptions": List[DatasetLabelDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeProjectsResponseTypeDef = TypedDict(
-    "DescribeProjectsResponseTypeDef",
-    {
-        "ProjectDescriptions": List[ProjectDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DetectLabelsImagePropertiesTypeDef = TypedDict(
-    "DetectLabelsImagePropertiesTypeDef",
-    {
-        "Quality": DetectLabelsImageQualityTypeDef,
-        "DominantColors": List[DominantColorTypeDef],
-        "Foreground": DetectLabelsImageForegroundTypeDef,
-        "Background": DetectLabelsImageBackgroundTypeDef,
-    },
-    total=False,
-)
-
-LabelTypeDef = TypedDict(
-    "LabelTypeDef",
-    {
-        "Name": str,
-        "Confidence": float,
-        "Instances": List[InstanceTypeDef],
-        "Parents": List[ParentTypeDef],
-        "Aliases": List[LabelAliasTypeDef],
-        "Categories": List[LabelCategoryTypeDef],
-    },
-    total=False,
-)
-
-_RequiredDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectLabelsRequestRequestTypeDef",
-    {
-        "MaxLabels": int,
-        "MinConfidence": float,
-        "Features": Sequence[DetectLabelsFeatureNameType],
-        "Settings": DetectLabelsSettingsTypeDef,
-    },
-    total=False,
-)
-
-class DetectLabelsRequestRequestTypeDef(
-    _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
-):
-    pass
-
 _RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
@@ -3063,112 +3297,87 @@
 
 class StartLabelDetectionRequestRequestTypeDef(
     _RequiredStartLabelDetectionRequestRequestTypeDef,
     _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
-CelebrityDetailTypeDef = TypedDict(
-    "CelebrityDetailTypeDef",
-    {
-        "Urls": List[str],
-        "Name": str,
-        "Id": str,
-        "Confidence": float,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
-        "KnownGender": KnownGenderTypeDef,
-    },
-    total=False,
-)
-
-DetectFacesResponseTypeDef = TypedDict(
-    "DetectFacesResponseTypeDef",
+_RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPersonTrackingRequestRequestTypeDef",
     {
-        "FaceDetails": List[FaceDetailTypeDef],
-        "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Video": VideoTypeDef,
     },
 )
-
-FaceDetectionTypeDef = TypedDict(
-    "FaceDetectionTypeDef",
+_OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPersonTrackingRequestRequestTypeDef",
     {
-        "Timestamp": int,
-        "Face": FaceDetailTypeDef,
+        "ClientRequestToken": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "JobTag": str,
     },
     total=False,
 )
 
-FaceRecordTypeDef = TypedDict(
-    "FaceRecordTypeDef",
-    {
-        "Face": FaceTypeDef,
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
+class StartPersonTrackingRequestRequestTypeDef(
+    _RequiredStartPersonTrackingRequestRequestTypeDef,
+    _OptionalStartPersonTrackingRequestRequestTypeDef,
+):
+    pass
 
-PersonDetailTypeDef = TypedDict(
-    "PersonDetailTypeDef",
+_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
-        "Index": int,
-        "BoundingBox": BoundingBoxTypeDef,
-        "Face": FaceDetailTypeDef,
+        "Image": ImageTypeDef,
     },
-    total=False,
 )
-
-SearchedFaceDetailsTypeDef = TypedDict(
-    "SearchedFaceDetailsTypeDef",
+_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
+    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
     {
-        "FaceDetail": FaceDetailTypeDef,
+        "MinConfidence": float,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
     },
     total=False,
 )
 
-UnindexedFaceTypeDef = TypedDict(
-    "UnindexedFaceTypeDef",
-    {
-        "Reasons": List[ReasonType],
-        "FaceDetail": FaceDetailTypeDef,
-    },
-    total=False,
-)
+class DetectModerationLabelsRequestRequestTypeDef(
+    _RequiredDetectModerationLabelsRequestRequestTypeDef,
+    _OptionalDetectModerationLabelsRequestRequestTypeDef,
+):
+    pass
 
-UnsearchedFaceTypeDef = TypedDict(
-    "UnsearchedFaceTypeDef",
+_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredStartStreamProcessorRequestRequestTypeDef",
     {
-        "FaceDetails": FaceDetailTypeDef,
-        "Reasons": List[UnsearchedFaceReasonType],
+        "Name": str,
     },
-    total=False,
 )
-
-CustomLabelTypeDef = TypedDict(
-    "CustomLabelTypeDef",
+_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalStartStreamProcessorRequestRequestTypeDef",
     {
-        "Name": str,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
+        "StartSelector": StreamProcessingStartSelectorTypeDef,
+        "StopSelector": StreamProcessingStopSelectorTypeDef,
     },
     total=False,
 )
 
-TextDetectionTypeDef = TypedDict(
-    "TextDetectionTypeDef",
+class StartStreamProcessorRequestRequestTypeDef(
+    _RequiredStartStreamProcessorRequestRequestTypeDef,
+    _OptionalStartStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
     {
-        "DetectedText": str,
-        "Type": TextTypesType,
-        "Id": int,
-        "ParentId": int,
-        "Confidence": float,
-        "Geometry": GeometryTypeDef,
+        "UserMatches": List[UserMatchTypeDef],
+        "FaceModelVersion": str,
+        "SearchedFace": SearchedFaceTypeDef,
+        "SearchedUser": SearchedUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DetectTextFiltersTypeDef = TypedDict(
     "DetectTextFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
@@ -3204,67 +3413,14 @@
 
 class UpdateStreamProcessorRequestRequestTypeDef(
     _RequiredUpdateStreamProcessorRequestRequestTypeDef,
     _OptionalUpdateStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_RequiredDetectModerationLabelsRequestRequestTypeDef",
-    {
-        "Image": ImageTypeDef,
-    },
-)
-_OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
-    "_OptionalDetectModerationLabelsRequestRequestTypeDef",
-    {
-        "MinConfidence": float,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
-    },
-    total=False,
-)
-
-class DetectModerationLabelsRequestRequestTypeDef(
-    _RequiredDetectModerationLabelsRequestRequestTypeDef,
-    _OptionalDetectModerationLabelsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredStartStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalStartStreamProcessorRequestRequestTypeDef",
-    {
-        "StartSelector": StreamProcessingStartSelectorTypeDef,
-        "StopSelector": StreamProcessingStopSelectorTypeDef,
-    },
-    total=False,
-)
-
-class StartStreamProcessorRequestRequestTypeDef(
-    _RequiredStartStreamProcessorRequestRequestTypeDef,
-    _OptionalStartStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-SearchUsersResponseTypeDef = TypedDict(
-    "SearchUsersResponseTypeDef",
-    {
-        "UserMatches": List[UserMatchTypeDef],
-        "FaceModelVersion": str,
-        "SearchedFace": SearchedFaceTypeDef,
-        "SearchedUser": SearchedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamProcessorRequestRequestTypeDef",
     {
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "Name": str,
         "Settings": StreamProcessorSettingsTypeDef,
@@ -3294,109 +3450,89 @@
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
-        "Input": StreamProcessorInputTypeDef,
+        "Input": StreamProcessorInputOutputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "Settings": StreamProcessorSettingsOutputTypeDef,
+        "NotificationChannel": StreamProcessorNotificationChannelOutputTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": List[VideoMetadataTypeDef],
         "AudioMetadata": List[AudioMetadataTypeDef],
         "NextToken": str,
         "Segments": List[SegmentDetectionTypeDef],
         "SelectedSegmentTypes": List[SegmentTypeInfoTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesByImageResponseTypeDef = TypedDict(
     "SearchFacesByImageResponseTypeDef",
     {
-        "SearchedFaceBoundingBox": BoundingBoxTypeDef,
+        "SearchedFaceBoundingBox": BoundingBoxOutputTypeDef,
         "SearchedFaceConfidence": float,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFacesResponseTypeDef = TypedDict(
     "SearchFacesResponseTypeDef",
     {
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TestingDataTypeDef = TypedDict(
-    "TestingDataTypeDef",
+TestingDataOutputTypeDef = TypedDict(
+    "TestingDataOutputTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
+        "Assets": List[AssetOutputTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
-TrainingDataTypeDef = TypedDict(
-    "TrainingDataTypeDef",
+TrainingDataOutputTypeDef = TypedDict(
+    "TrainingDataOutputTypeDef",
     {
-        "Assets": Sequence[AssetTypeDef],
+        "Assets": List[AssetOutputTypeDef],
     },
     total=False,
 )
 
 ValidationDataTypeDef = TypedDict(
     "ValidationDataTypeDef",
     {
-        "Assets": List[AssetTypeDef],
+        "Assets": List[AssetOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "ProjectArn": str,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetSource": DatasetSourceTypeDef,
-    },
-    total=False,
-)
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -3419,49 +3555,49 @@
 
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompareFacesResponseTypeDef = TypedDict(
     "CompareFacesResponseTypeDef",
     {
         "SourceImageFace": ComparedSourceImageFaceTypeDef,
         "FaceMatches": List[CompareFacesMatchTypeDef],
         "UnmatchedFaces": List[ComparedFaceTypeDef],
         "SourceImageOrientationCorrection": OrientationCorrectionType,
         "TargetImageOrientationCorrection": OrientationCorrectionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectiveEquipmentPersonTypeDef = TypedDict(
     "ProtectiveEquipmentPersonTypeDef",
     {
         "BodyParts": List[ProtectiveEquipmentBodyPartTypeDef],
-        "BoundingBox": BoundingBoxTypeDef,
+        "BoundingBox": BoundingBoxOutputTypeDef,
         "Confidence": float,
         "Id": int,
     },
     total=False,
 )
 
 DetectLabelsResponseTypeDef = TypedDict(
     "DetectLabelsResponseTypeDef",
     {
         "Labels": List[LabelTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "LabelModelVersion": str,
         "ImageProperties": DetectLabelsImagePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LabelDetectionTypeDef = TypedDict(
     "LabelDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3487,17 +3623,17 @@
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Faces": List[FaceDetectionTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PersonDetectionTypeDef = TypedDict(
     "PersonDetectionTypeDef",
     {
         "Timestamp": int,
@@ -3519,55 +3655,92 @@
 IndexFacesResponseTypeDef = TypedDict(
     "IndexFacesResponseTypeDef",
     {
         "FaceRecords": List[FaceRecordTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "FaceModelVersion": str,
         "UnindexedFaces": List[UnindexedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchUsersByImageResponseTypeDef = TypedDict(
     "SearchUsersByImageResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceDetailsTypeDef,
         "UnsearchedFaces": List[UnsearchedFaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectCustomLabelsResponseTypeDef = TypedDict(
     "DetectCustomLabelsResponseTypeDef",
     {
         "CustomLabels": List[CustomLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectTextResponseTypeDef = TypedDict(
     "DetectTextResponseTypeDef",
     {
         "TextDetections": List[TextDetectionTypeDef],
         "TextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TextDetectionResultTypeDef = TypedDict(
     "TextDetectionResultTypeDef",
     {
         "Timestamp": int,
         "TextDetection": TextDetectionTypeDef,
     },
     total=False,
 )
 
+TestingDataTypeDef = TypedDict(
+    "TestingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+        "AutoCreate": bool,
+    },
+    total=False,
+)
+
+TrainingDataTypeDef = TypedDict(
+    "TrainingDataTypeDef",
+    {
+        "Assets": Sequence[AssetTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "ProjectArn": str,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetSource": DatasetSourceTypeDef,
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
 _RequiredDetectTextRequestRequestTypeDef = TypedDict(
     "_RequiredDetectTextRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectTextRequestRequestTypeDef = TypedDict(
@@ -3602,170 +3775,170 @@
 
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectVersionRequestRequestTypeDef",
-    {
-        "ProjectArn": str,
-        "VersionName": str,
-        "OutputConfig": OutputConfigTypeDef,
-    },
-)
-_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectVersionRequestRequestTypeDef",
-    {
-        "TrainingData": TrainingDataTypeDef,
-        "TestingData": TestingDataTypeDef,
-        "Tags": Mapping[str, str],
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class CreateProjectVersionRequestRequestTypeDef(
-    _RequiredCreateProjectVersionRequestRequestTypeDef,
-    _OptionalCreateProjectVersionRequestRequestTypeDef,
-):
-    pass
-
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataTypeDef,
-        "Output": TestingDataTypeDef,
+        "Input": TestingDataOutputTypeDef,
+        "Output": TestingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataTypeDef,
-        "Output": TrainingDataTypeDef,
+        "Input": TrainingDataOutputTypeDef,
+        "Output": TrainingDataOutputTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
     {
         "ProtectiveEquipmentModelVersion": str,
         "Persons": List[ProtectiveEquipmentPersonTypeDef],
         "Summary": ProtectiveEquipmentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLabelDetectionResponseTypeDef = TypedDict(
     "GetLabelDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Labels": List[LabelDetectionTypeDef],
         "LabelModelVersion": str,
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
         "GetRequestMetadata": GetLabelDetectionRequestMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCelebrityRecognitionResponseTypeDef = TypedDict(
     "GetCelebrityRecognitionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Celebrities": List[CelebrityRecognitionTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPersonTrackingResponseTypeDef = TypedDict(
     "GetPersonTrackingResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "NextToken": str,
         "Persons": List[PersonDetectionTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFaceSearchResponseTypeDef = TypedDict(
     "GetFaceSearchResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "NextToken": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "Persons": List[PersonMatchTypeDef],
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTextDetectionResponseTypeDef = TypedDict(
     "GetTextDetectionResponseTypeDef",
     {
         "JobStatus": VideoJobStatusType,
         "StatusMessage": str,
         "VideoMetadata": VideoMetadataTypeDef,
         "TextDetections": List[TextDetectionResultTypeDef],
         "NextToken": str,
         "TextModelVersion": str,
         "JobId": str,
-        "Video": VideoTypeDef,
+        "Video": VideoOutputTypeDef,
         "JobTag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectVersionRequestRequestTypeDef",
+    {
+        "ProjectArn": str,
+        "VersionName": str,
+        "OutputConfig": OutputConfigTypeDef,
+    },
+)
+_OptionalCreateProjectVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectVersionRequestRequestTypeDef",
+    {
+        "TrainingData": TrainingDataTypeDef,
+        "TestingData": TestingDataTypeDef,
+        "Tags": Mapping[str, str],
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class CreateProjectVersionRequestRequestTypeDef(
+    _RequiredCreateProjectVersionRequestRequestTypeDef,
+    _OptionalCreateProjectVersionRequestRequestTypeDef,
+):
+    pass
+
 ProjectVersionDescriptionTypeDef = TypedDict(
     "ProjectVersionDescriptionTypeDef",
     {
         "ProjectVersionArn": str,
         "CreationTimestamp": datetime,
         "MinInferenceUnits": int,
         "Status": ProjectVersionStatusType,
         "StatusMessage": str,
         "BillableTrainingTimeInSeconds": int,
         "TrainingEndTimestamp": datetime,
-        "OutputConfig": OutputConfigTypeDef,
+        "OutputConfig": OutputConfigOutputTypeDef,
         "TrainingDataResult": TrainingDataResultTypeDef,
         "TestingDataResult": TestingDataResultTypeDef,
         "EvaluationResult": EvaluationResultTypeDef,
-        "ManifestSummary": GroundTruthManifestTypeDef,
+        "ManifestSummary": GroundTruthManifestOutputTypeDef,
         "KmsKeyId": str,
         "MaxInferenceUnits": int,
         "SourceProjectVersionArn": str,
     },
     total=False,
 )
 
 DescribeProjectVersionsResponseTypeDef = TypedDict(
     "DescribeProjectVersionsResponseTypeDef",
     {
         "ProjectVersionDescriptions": List[ProjectVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/PKG-INFO` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.0
-Summary: Type annotations for boto3.Rekognition 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Rekognition 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rekognition"></a>
 
 # mypy-boto3-rekognition
 
 [![PyPI - mypy-boto3-rekognition](https://img.shields.io/pypi/v/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rekognition.svg?color=blue)](https://pypi.org/project/mypy-boto3-rekognition)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rekognition?color=blue)](https://pypistats.org/packages/mypy-boto3-rekognition)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rekognition)](https://pepy.tech/project/mypy-boto3-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Rekognition 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[boto3.Rekognition 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,69 +428,62 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rekognition.type_defs import (
     AgeRangeTypeDef,
     AssociateFacesRequestRequestTypeDef,
     AssociatedFaceTypeDef,
+    ResponseMetadataTypeDef,
     UnsuccessfulFaceAssociationTypeDef,
     AudioMetadataTypeDef,
-    BoundingBoxTypeDef,
-    S3ObjectTypeDef,
+    BoundingBoxOutputTypeDef,
+    S3ObjectOutputTypeDef,
     BeardTypeDef,
     BlackFrameTypeDef,
+    BoundingBoxTypeDef,
     KnownGenderTypeDef,
     EmotionTypeDef,
     ImageQualityTypeDef,
     LandmarkTypeDef,
     PoseTypeDef,
     SmileTypeDef,
     ConnectedHomeSettingsForUpdateTypeDef,
+    ConnectedHomeSettingsOutputTypeDef,
     ConnectedHomeSettingsTypeDef,
     ModerationLabelTypeDef,
     OutputConfigTypeDef,
-    CopyProjectVersionResponseTypeDef,
     CoversBodyPartTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    CreateCollectionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
     LivenessOutputConfigTypeDef,
-    CreateFaceLivenessSessionResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateProjectVersionResponseTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorNotificationChannelTypeDef,
-    CreateStreamProcessorResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DatasetChangesTypeDef,
     DatasetStatsTypeDef,
     DatasetLabelStatsTypeDef,
     DatasetMetadataTypeDef,
     DeleteCollectionRequestRequestTypeDef,
-    DeleteCollectionResponseTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteFacesRequestRequestTypeDef,
     UnsuccessfulFaceDeletionTypeDef,
     DeleteProjectPolicyRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteProjectVersionRequestRequestTypeDef,
-    DeleteProjectVersionResponseTypeDef,
     DeleteStreamProcessorRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeCollectionRequestRequestTypeDef,
-    DescribeCollectionResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
-    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeProjectVersionsRequestRequestTypeDef,
-    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
     DescribeProjectsRequestRequestTypeDef,
     DescribeStreamProcessorRequestRequestTypeDef,
+    StreamProcessorDataSharingPreferenceOutputTypeDef,
+    StreamProcessorNotificationChannelOutputTypeDef,
     DetectLabelsImageQualityTypeDef,
     DominantColorTypeDef,
     DetectLabelsImagePropertiesSettingsTypeDef,
     GeneralLabelsSettingsTypeDef,
     HumanLoopActivationOutputTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     ProtectiveEquipmentSummaryTypeDef,
@@ -503,190 +496,211 @@
     EyeOpenTypeDef,
     EyeglassesTypeDef,
     FaceOccludedTypeDef,
     GenderTypeDef,
     MouthOpenTypeDef,
     MustacheTypeDef,
     SunglassesTypeDef,
+    FaceSearchSettingsOutputTypeDef,
     FaceSearchSettingsTypeDef,
-    PointTypeDef,
+    PointOutputTypeDef,
     GetCelebrityInfoRequestRequestTypeDef,
     GetCelebrityRecognitionRequestRequestTypeDef,
     VideoMetadataTypeDef,
     GetContentModerationRequestMetadataTypeDef,
     GetContentModerationRequestRequestTypeDef,
     GetFaceDetectionRequestRequestTypeDef,
     GetFaceLivenessSessionResultsRequestRequestTypeDef,
     GetFaceSearchRequestRequestTypeDef,
     GetLabelDetectionRequestMetadataTypeDef,
     GetLabelDetectionRequestRequestTypeDef,
     GetPersonTrackingRequestRequestTypeDef,
     GetSegmentDetectionRequestRequestTypeDef,
     SegmentTypeInfoTypeDef,
     GetTextDetectionRequestRequestTypeDef,
+    S3ObjectTypeDef,
     HumanLoopDataAttributesTypeDef,
     KinesisDataStreamTypeDef,
+    KinesisVideoStreamOutputTypeDef,
     KinesisVideoStreamStartSelectorTypeDef,
     KinesisVideoStreamTypeDef,
     LabelAliasTypeDef,
     LabelCategoryTypeDef,
     ParentTypeDef,
-    ListCollectionsRequestListCollectionsPaginateTypeDef,
     ListCollectionsRequestRequestTypeDef,
-    ListCollectionsResponseTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     ListDatasetLabelsRequestRequestTypeDef,
-    ListFacesRequestListFacesPaginateTypeDef,
     ListFacesRequestRequestTypeDef,
-    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     ListProjectPoliciesRequestRequestTypeDef,
     ProjectPolicyTypeDef,
-    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
     ListStreamProcessorsRequestRequestTypeDef,
     StreamProcessorTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     MatchedUserTypeDef,
     NotificationChannelTypeDef,
-    PaginatorConfigTypeDef,
+    OutputConfigOutputTypeDef,
+    PointTypeDef,
     PutProjectPolicyRequestRequestTypeDef,
-    PutProjectPolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3DestinationTypeDef,
     SearchFacesRequestRequestTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchedFaceTypeDef,
     SearchedUserTypeDef,
     ShotSegmentTypeDef,
     TechnicalCueSegmentTypeDef,
+    StartProjectVersionRequestRequestTypeDef,
+    StartShotDetectionFilterTypeDef,
+    StreamProcessingStopSelectorTypeDef,
+    StopProjectVersionRequestRequestTypeDef,
+    StopStreamProcessorRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    CopyProjectVersionResponseTypeDef,
+    CreateCollectionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateFaceLivenessSessionResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateProjectVersionResponseTypeDef,
+    CreateStreamProcessorResponseTypeDef,
+    DeleteCollectionResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteProjectVersionResponseTypeDef,
+    DescribeCollectionResponseTypeDef,
+    ListCollectionsResponseTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutProjectPolicyResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
     StartFaceSearchResponseTypeDef,
     StartLabelDetectionResponseTypeDef,
     StartPersonTrackingResponseTypeDef,
-    StartProjectVersionRequestRequestTypeDef,
     StartProjectVersionResponseTypeDef,
-    StartShotDetectionFilterTypeDef,
     StartSegmentDetectionResponseTypeDef,
-    StreamProcessingStopSelectorTypeDef,
     StartStreamProcessorResponseTypeDef,
     StartTextDetectionResponseTypeDef,
-    StopProjectVersionRequestRequestTypeDef,
     StopProjectVersionResponseTypeDef,
-    StopStreamProcessorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     AssociateFacesResponseTypeDef,
     ComparedSourceImageFaceTypeDef,
     FaceTypeDef,
     AuditImageTypeDef,
-    GroundTruthManifestTypeDef,
-    ImageTypeDef,
+    GroundTruthManifestOutputTypeDef,
     SummaryTypeDef,
-    VideoTypeDef,
+    VideoOutputTypeDef,
     StartTechnicalCueDetectionFilterTypeDef,
     GetCelebrityInfoResponseTypeDef,
     ComparedFaceTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
     ContentModerationDetectionTypeDef,
     CopyProjectVersionRequestRequestTypeDef,
     EquipmentDetectionTypeDef,
     CreateFaceLivenessSessionRequestSettingsTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     DatasetDescriptionTypeDef,
     DatasetLabelDescriptionTypeDef,
     ProjectDescriptionTypeDef,
     DeleteFacesResponseTypeDef,
+    DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
+    DescribeProjectsRequestDescribeProjectsPaginateTypeDef,
+    ListCollectionsRequestListCollectionsPaginateTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
+    ListFacesRequestListFacesPaginateTypeDef,
+    ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
+    ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     DetectLabelsImageBackgroundTypeDef,
     DetectLabelsImageForegroundTypeDef,
     InstanceTypeDef,
     DetectLabelsSettingsTypeDef,
     LabelDetectionSettingsTypeDef,
     DetectModerationLabelsResponseTypeDef,
     DisassociateFacesResponseTypeDef,
     DistributeDatasetEntriesRequestRequestTypeDef,
     FaceDetailTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
     GeometryTypeDef,
-    RegionOfInterestTypeDef,
+    RegionOfInterestOutputTypeDef,
+    GroundTruthManifestTypeDef,
+    ImageTypeDef,
+    VideoTypeDef,
     HumanLoopConfigTypeDef,
+    StreamProcessorInputOutputTypeDef,
     StreamProcessingStartSelectorTypeDef,
     StreamProcessorInputTypeDef,
     ListProjectPoliciesResponseTypeDef,
     ListStreamProcessorsResponseTypeDef,
     ListUsersResponseTypeDef,
     UserMatchTypeDef,
+    RegionOfInterestTypeDef,
     StreamProcessorOutputTypeDef,
     SegmentDetectionTypeDef,
     FaceMatchTypeDef,
     ListFacesResponseTypeDef,
     GetFaceLivenessSessionResultsResponseTypeDef,
-    AssetTypeDef,
-    DatasetSourceTypeDef,
-    CompareFacesRequestRequestTypeDef,
-    DetectCustomLabelsRequestRequestTypeDef,
-    DetectFacesRequestRequestTypeDef,
-    DetectProtectiveEquipmentRequestRequestTypeDef,
-    IndexFacesRequestRequestTypeDef,
-    RecognizeCelebritiesRequestRequestTypeDef,
-    SearchFacesByImageRequestRequestTypeDef,
-    SearchUsersByImageRequestRequestTypeDef,
+    AssetOutputTypeDef,
     EvaluationResultTypeDef,
-    StartCelebrityRecognitionRequestRequestTypeDef,
-    StartContentModerationRequestRequestTypeDef,
-    StartFaceDetectionRequestRequestTypeDef,
-    StartFaceSearchRequestRequestTypeDef,
-    StartPersonTrackingRequestRequestTypeDef,
     StartSegmentDetectionFiltersTypeDef,
     CelebrityTypeDef,
     CompareFacesMatchTypeDef,
     GetContentModerationResponseTypeDef,
     ProtectiveEquipmentBodyPartTypeDef,
     CreateFaceLivenessSessionRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetLabelsResponseTypeDef,
     DescribeProjectsResponseTypeDef,
     DetectLabelsImagePropertiesTypeDef,
     LabelTypeDef,
-    DetectLabelsRequestRequestTypeDef,
-    StartLabelDetectionRequestRequestTypeDef,
     CelebrityDetailTypeDef,
     DetectFacesResponseTypeDef,
     FaceDetectionTypeDef,
     FaceRecordTypeDef,
     PersonDetailTypeDef,
     SearchedFaceDetailsTypeDef,
     UnindexedFaceTypeDef,
     UnsearchedFaceTypeDef,
     CustomLabelTypeDef,
     TextDetectionTypeDef,
-    DetectTextFiltersTypeDef,
-    StartTextDetectionFiltersTypeDef,
-    UpdateStreamProcessorRequestRequestTypeDef,
+    AssetTypeDef,
+    DatasetSourceTypeDef,
+    CompareFacesRequestRequestTypeDef,
+    DetectCustomLabelsRequestRequestTypeDef,
+    DetectFacesRequestRequestTypeDef,
+    DetectLabelsRequestRequestTypeDef,
+    DetectProtectiveEquipmentRequestRequestTypeDef,
+    IndexFacesRequestRequestTypeDef,
+    RecognizeCelebritiesRequestRequestTypeDef,
+    SearchFacesByImageRequestRequestTypeDef,
+    SearchUsersByImageRequestRequestTypeDef,
+    StartCelebrityRecognitionRequestRequestTypeDef,
+    StartContentModerationRequestRequestTypeDef,
+    StartFaceDetectionRequestRequestTypeDef,
+    StartFaceSearchRequestRequestTypeDef,
+    StartLabelDetectionRequestRequestTypeDef,
+    StartPersonTrackingRequestRequestTypeDef,
     DetectModerationLabelsRequestRequestTypeDef,
     StartStreamProcessorRequestRequestTypeDef,
     SearchUsersResponseTypeDef,
+    DetectTextFiltersTypeDef,
+    StartTextDetectionFiltersTypeDef,
+    UpdateStreamProcessorRequestRequestTypeDef,
     CreateStreamProcessorRequestRequestTypeDef,
     DescribeStreamProcessorResponseTypeDef,
     GetSegmentDetectionResponseTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
-    TestingDataTypeDef,
-    TrainingDataTypeDef,
+    TestingDataOutputTypeDef,
+    TrainingDataOutputTypeDef,
     ValidationDataTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     StartSegmentDetectionRequestRequestTypeDef,
     RecognizeCelebritiesResponseTypeDef,
     CompareFacesResponseTypeDef,
     ProtectiveEquipmentPersonTypeDef,
     DetectLabelsResponseTypeDef,
     LabelDetectionTypeDef,
     CelebrityRecognitionTypeDef,
@@ -694,25 +708,28 @@
     PersonDetectionTypeDef,
     PersonMatchTypeDef,
     IndexFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     DetectCustomLabelsResponseTypeDef,
     DetectTextResponseTypeDef,
     TextDetectionResultTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     DetectTextRequestRequestTypeDef,
     StartTextDetectionRequestRequestTypeDef,
-    CreateProjectVersionRequestRequestTypeDef,
     TestingDataResultTypeDef,
     TrainingDataResultTypeDef,
     DetectProtectiveEquipmentResponseTypeDef,
     GetLabelDetectionResponseTypeDef,
     GetCelebrityRecognitionResponseTypeDef,
     GetPersonTrackingResponseTypeDef,
     GetFaceSearchResponseTypeDef,
     GetTextDetectionResponseTypeDef,
+    CreateProjectVersionRequestRequestTypeDef,
     ProjectVersionDescriptionTypeDef,
     DescribeProjectVersionsResponseTypeDef,
 )
 
 
 def get_structure() -> AgeRangeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-rekognition-1.28.0/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.28.12/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.0/setup.py` & `mypy-boto3-rekognition-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Rekognition 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Rekognition 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

