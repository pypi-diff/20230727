# Comparing `tmp/mypy-boto3-comprehend-1.28.0.tar.gz` & `tmp/mypy-boto3-comprehend-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehend-1.28.0.tar", last modified: Thu Jul  6 20:59:17 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehend-1.28.12.tar", last modified: Thu Jul 27 05:34:30 2023, max compression
```

## Comparing `mypy-boto3-comprehend-1.28.0.tar` & `mypy-boto3-comprehend-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:17.506262 mypy-boto3-comprehend-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27612 2023-07-06 20:59:17.506262 mypy-boto3-comprehend-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26115 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:17.490262 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67084 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66983 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-07-06 20:36:33.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-07-06 20:36:32.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-06 20:36:32.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-06 20:36:32.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98639 2023-07-06 20:36:36.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98562 2023-07-06 20:36:35.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:17.490262 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27612 2023-07-06 20:59:17.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:17.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:17.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:17.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:17.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:17.000000 mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:17.506262 mypy-boto3-comprehend-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:36:31.000000 mypy-boto3-comprehend-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.268546 mypy-boto3-comprehend-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-07-27 05:34:30.260546 mypy-boto3-comprehend-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26872 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.260546 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67084 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66983 2023-07-27 05:19:24.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   107525 2023-07-27 05:19:27.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107426 2023-07-27 05:19:26.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.260546 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:30.268546 mypy-boto3-comprehend-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/setup.py
```

### Comparing `mypy-boto3-comprehend-1.28.0/LICENSE` & `mypy-boto3-comprehend-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/PKG-INFO` & `mypy-boto3-comprehend-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.28.0
-Summary: Type annotations for boto3.Comprehend 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Comprehend 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-comprehend"></a>
 
 # mypy-boto3-comprehend
 
 [![PyPI - mypy-boto3-comprehend](https://img.shields.io/pypi/v/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -398,14 +398,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_comprehend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
+    AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
@@ -429,14 +430,15 @@
     CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
+    VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
     DatasetPropertiesTypeDef,
@@ -466,27 +468,35 @@
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
+    DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
-    OutputDataConfigTypeDef,
+    OutputDataConfigOutputTypeDef,
+    DocumentClassifierDocumentsOutputTypeDef,
     DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
+    DocumentReaderConfigOutputTypeDef,
+    DocumentClassifierOutputDataConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
+    EntityTypesListItemOutputTypeDef,
     EntityTypesListItemTypeDef,
+    EntityRecognizerAnnotationsOutputTypeDef,
     EntityRecognizerAnnotationsTypeDef,
+    EntityRecognizerDocumentsOutputTypeDef,
     EntityRecognizerDocumentsTypeDef,
+    EntityRecognizerEntityListOutputTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
     EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
@@ -498,22 +508,25 @@
     ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
+    OutputDataConfigTypeDef,
     PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutResourcePolicyResponseTypeDef,
+    RedactionConfigTypeDef,
     ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
@@ -552,39 +565,43 @@
     ClassifierMetadataTypeDef,
     ClassifyDocumentRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     InputDataConfigTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
+    DataSecurityConfigOutputTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
     ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigOutputTypeDef,
+    InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
     ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
     ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
+    EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
+    EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
     ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
@@ -594,56 +611,61 @@
     GeometryTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
-    DocumentClassificationJobPropertiesTypeDef,
-    DominantLanguageDetectionJobPropertiesTypeDef,
-    EntitiesDetectionJobPropertiesTypeDef,
-    EventsDetectionJobPropertiesTypeDef,
-    KeyPhrasesDetectionJobPropertiesTypeDef,
-    PiiEntitiesDetectionJobPropertiesTypeDef,
-    SentimentDetectionJobPropertiesTypeDef,
     StartDocumentClassificationJobRequestRequestTypeDef,
     StartDominantLanguageDetectionJobRequestRequestTypeDef,
     StartEntitiesDetectionJobRequestRequestTypeDef,
     StartEventsDetectionJobRequestRequestTypeDef,
     StartKeyPhrasesDetectionJobRequestRequestTypeDef,
     StartPiiEntitiesDetectionJobRequestRequestTypeDef,
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
-    TargetedSentimentDetectionJobPropertiesTypeDef,
-    TopicsDetectionJobPropertiesTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
     DatasetInputDataConfigTypeDef,
     CreateDocumentClassifierRequestRequestTypeDef,
     DocumentClassifierPropertiesTypeDef,
+    DocumentClassificationJobPropertiesTypeDef,
+    DominantLanguageDetectionJobPropertiesTypeDef,
+    EntitiesDetectionJobPropertiesTypeDef,
+    EventsDetectionJobPropertiesTypeDef,
+    KeyPhrasesDetectionJobPropertiesTypeDef,
+    PiiEntitiesDetectionJobPropertiesTypeDef,
+    SentimentDetectionJobPropertiesTypeDef,
+    TargetedSentimentDetectionJobPropertiesTypeDef,
+    TopicsDetectionJobPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
+    TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -654,34 +676,31 @@
     ListPiiEntitiesDetectionJobsResponseTypeDef,
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
-    CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
+    CreateFlywheelRequestRequestTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemTypeDef:
+def get_structure() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehend-1.28.0/README.md` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-comprehend
+Version: 1.28.12
+Summary: Type annotations for boto3.Comprehend 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 comprehend type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-comprehend"></a>
 
 # mypy-boto3-comprehend
 
 [![PyPI - mypy-boto3-comprehend](https://img.shields.io/pypi/v/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,14 +398,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_comprehend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
+    AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
@@ -397,14 +430,15 @@
     CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
+    VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
     DatasetPropertiesTypeDef,
@@ -434,27 +468,35 @@
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
+    DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
-    OutputDataConfigTypeDef,
+    OutputDataConfigOutputTypeDef,
+    DocumentClassifierDocumentsOutputTypeDef,
     DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
+    DocumentReaderConfigOutputTypeDef,
+    DocumentClassifierOutputDataConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
+    EntityTypesListItemOutputTypeDef,
     EntityTypesListItemTypeDef,
+    EntityRecognizerAnnotationsOutputTypeDef,
     EntityRecognizerAnnotationsTypeDef,
+    EntityRecognizerDocumentsOutputTypeDef,
     EntityRecognizerDocumentsTypeDef,
+    EntityRecognizerEntityListOutputTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
     EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
@@ -466,22 +508,25 @@
     ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
+    OutputDataConfigTypeDef,
     PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutResourcePolicyResponseTypeDef,
+    RedactionConfigTypeDef,
     ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
@@ -520,39 +565,43 @@
     ClassifierMetadataTypeDef,
     ClassifyDocumentRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     InputDataConfigTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
+    DataSecurityConfigOutputTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
     ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigOutputTypeDef,
+    InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
     ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
     ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
+    EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
+    EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
     ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
@@ -562,56 +611,61 @@
     GeometryTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
-    DocumentClassificationJobPropertiesTypeDef,
-    DominantLanguageDetectionJobPropertiesTypeDef,
-    EntitiesDetectionJobPropertiesTypeDef,
-    EventsDetectionJobPropertiesTypeDef,
-    KeyPhrasesDetectionJobPropertiesTypeDef,
-    PiiEntitiesDetectionJobPropertiesTypeDef,
-    SentimentDetectionJobPropertiesTypeDef,
     StartDocumentClassificationJobRequestRequestTypeDef,
     StartDominantLanguageDetectionJobRequestRequestTypeDef,
     StartEntitiesDetectionJobRequestRequestTypeDef,
     StartEventsDetectionJobRequestRequestTypeDef,
     StartKeyPhrasesDetectionJobRequestRequestTypeDef,
     StartPiiEntitiesDetectionJobRequestRequestTypeDef,
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
-    TargetedSentimentDetectionJobPropertiesTypeDef,
-    TopicsDetectionJobPropertiesTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
     DatasetInputDataConfigTypeDef,
     CreateDocumentClassifierRequestRequestTypeDef,
     DocumentClassifierPropertiesTypeDef,
+    DocumentClassificationJobPropertiesTypeDef,
+    DominantLanguageDetectionJobPropertiesTypeDef,
+    EntitiesDetectionJobPropertiesTypeDef,
+    EventsDetectionJobPropertiesTypeDef,
+    KeyPhrasesDetectionJobPropertiesTypeDef,
+    PiiEntitiesDetectionJobPropertiesTypeDef,
+    SentimentDetectionJobPropertiesTypeDef,
+    TargetedSentimentDetectionJobPropertiesTypeDef,
+    TopicsDetectionJobPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
+    TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -622,34 +676,31 @@
     ListPiiEntitiesDetectionJobsResponseTypeDef,
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
-    CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
+    CreateFlywheelRequestRequestTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemTypeDef:
+def get_structure() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/__init__.py` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/__init__.pyi` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/__main__.py` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Comprehend 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Comprehend 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
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

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/client.py` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/client.pyi` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/literals.py` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,15 @@
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
@@ -437,26 +438,28 @@
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

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/literals.pyi` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -349,14 +349,15 @@
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
@@ -435,26 +436,28 @@
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

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/paginator.py` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/paginator.pyi` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/type_defs.py` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for comprehend service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_comprehend.type_defs import AugmentedManifestsListItemTypeDef
+    from mypy_boto3_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
 
-    data: AugmentedManifestsListItemTypeDef = {...}
+    data: AugmentedManifestsListItemOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -57,16 +57,16 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
@@ -90,14 +90,15 @@
     "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
     "CreateDocumentClassifierResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "CreateEntityRecognizerResponseTypeDef",
     "CreateFlywheelResponseTypeDef",
+    "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "DatasetFilterTypeDef",
     "DatasetPropertiesTypeDef",
@@ -127,27 +128,35 @@
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
+    "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
     "DocumentClassificationJobFilterTypeDef",
-    "OutputDataConfigTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "DocumentClassifierDocumentsOutputTypeDef",
     "DocumentClassifierDocumentsTypeDef",
     "DocumentClassifierFilterTypeDef",
+    "DocumentReaderConfigOutputTypeDef",
+    "DocumentClassifierOutputDataConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
+    "EntityTypesListItemOutputTypeDef",
     "EntityTypesListItemTypeDef",
+    "EntityRecognizerAnnotationsOutputTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
+    "EntityRecognizerDocumentsOutputTypeDef",
     "EntityRecognizerDocumentsTypeDef",
+    "EntityRecognizerEntityListOutputTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
     "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
     "EventsDetectionJobFilterTypeDef",
@@ -159,22 +168,25 @@
     "ImportModelResponseTypeDef",
     "KeyPhrasesDetectionJobFilterTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "PiiEntitiesDetectionJobFilterTypeDef",
     "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "TargetedSentimentDetectionJobFilterTypeDef",
     "TopicsDetectionJobFilterTypeDef",
+    "OutputDataConfigTypeDef",
     "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
-    "RedactionConfigTypeDef",
+    "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutResourcePolicyResponseTypeDef",
+    "RedactionConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
     "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
@@ -213,39 +225,43 @@
     "ClassifierMetadataTypeDef",
     "ClassifyDocumentRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
+    "DataSecurityConfigOutputTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
     "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
     "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigOutputTypeDef",
+    "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
     "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
+    "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
     "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
@@ -255,56 +271,61 @@
     "GeometryTypeDef",
     "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
-    "DocumentClassificationJobPropertiesTypeDef",
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    "EntitiesDetectionJobPropertiesTypeDef",
-    "EventsDetectionJobPropertiesTypeDef",
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    "SentimentDetectionJobPropertiesTypeDef",
     "StartDocumentClassificationJobRequestRequestTypeDef",
     "StartDominantLanguageDetectionJobRequestRequestTypeDef",
     "StartEntitiesDetectionJobRequestRequestTypeDef",
     "StartEventsDetectionJobRequestRequestTypeDef",
     "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    "TopicsDetectionJobPropertiesTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
     "DatasetInputDataConfigTypeDef",
     "CreateDocumentClassifierRequestRequestTypeDef",
     "DocumentClassifierPropertiesTypeDef",
+    "DocumentClassificationJobPropertiesTypeDef",
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    "EntitiesDetectionJobPropertiesTypeDef",
+    "EventsDetectionJobPropertiesTypeDef",
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    "SentimentDetectionJobPropertiesTypeDef",
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    "TopicsDetectionJobPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
+    "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -315,32 +336,53 @@
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
-    "CreateFlywheelRequestRequestTypeDef",
     "FlywheelPropertiesTypeDef",
+    "CreateFlywheelRequestRequestTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
     "UpdateFlywheelResponseTypeDef",
     "DescribeEntityRecognizerResponseTypeDef",
     "ListEntityRecognizersResponseTypeDef",
     "BatchDetectTargetedSentimentResponseTypeDef",
 )
 
+_RequiredAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_RequiredAugmentedManifestsListItemOutputTypeDef",
+    {
+        "S3Uri": str,
+        "AttributeNames": List[str],
+    },
+)
+_OptionalAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_OptionalAugmentedManifestsListItemOutputTypeDef",
+    {
+        "Split": SplitType,
+        "AnnotationDataS3Uri": str,
+        "SourceDocumentsS3Uri": str,
+        "DocumentType": AugmentedManifestsDocumentTypeFormatType,
+    },
+    total=False,
+)
+
+class AugmentedManifestsListItemOutputTypeDef(
+    _RequiredAugmentedManifestsListItemOutputTypeDef,
+    _OptionalAugmentedManifestsListItemOutputTypeDef,
+):
+    pass
+
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -351,21 +393,19 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
-
 class AugmentedManifestsListItemTypeDef(
     _RequiredAugmentedManifestsListItemTypeDef, _OptionalAugmentedManifestsListItemTypeDef
 ):
     pass
 
-
 DominantLanguageTypeDef = TypedDict(
     "DominantLanguageTypeDef",
     {
         "LanguageCode": str,
         "Score": float,
     },
     total=False,
@@ -506,21 +546,19 @@
     {
         "DocumentReadMode": DocumentReadModeType,
         "FeatureTypes": Sequence[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
-
 class DocumentReaderConfigTypeDef(
     _RequiredDocumentReaderConfigTypeDef, _OptionalDocumentReaderConfigTypeDef
 ):
     pass
 
-
 DocumentClassTypeDef = TypedDict(
     "DocumentClassTypeDef",
     {
         "Name": str,
         "Score": float,
         "Page": int,
     },
@@ -593,19 +631,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "DatasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -658,14 +694,22 @@
     {
         "FlywheelArn": str,
         "ActiveModelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
+
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
         "S3Uri": str,
     },
 )
@@ -675,44 +719,40 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
-
 class DatasetAugmentedManifestsListItemTypeDef(
     _RequiredDatasetAugmentedManifestsListItemTypeDef,
     _OptionalDatasetAugmentedManifestsListItemTypeDef,
 ):
     pass
 
-
 _RequiredDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_OptionalDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "LabelDelimiter": str,
     },
     total=False,
 )
 
-
 class DatasetDocumentClassifierInputDataConfigTypeDef(
     _RequiredDatasetDocumentClassifierInputDataConfigTypeDef,
     _OptionalDatasetDocumentClassifierInputDataConfigTypeDef,
 ):
     pass
 
-
 DatasetEntityRecognizerAnnotationsTypeDef = TypedDict(
     "DatasetEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -726,22 +766,20 @@
     "_OptionalDatasetEntityRecognizerDocumentsTypeDef",
     {
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
-
 class DatasetEntityRecognizerDocumentsTypeDef(
     _RequiredDatasetEntityRecognizerDocumentsTypeDef,
     _OptionalDatasetEntityRecognizerDocumentsTypeDef,
 ):
     pass
 
-
 DatasetEntityRecognizerEntityListTypeDef = TypedDict(
     "DatasetEntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -811,22 +849,20 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -1020,64 +1056,102 @@
     "DetectTargetedSentimentRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
 
+_RequiredDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentClassificationConfigOutputTypeDef",
+    {
+        "Mode": DocumentClassifierModeType,
+    },
+)
+_OptionalDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentClassificationConfigOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+    total=False,
+)
+
+class DocumentClassificationConfigOutputTypeDef(
+    _RequiredDocumentClassificationConfigOutputTypeDef,
+    _OptionalDocumentClassificationConfigOutputTypeDef,
+):
+    pass
+
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
     "_OptionalDocumentClassificationConfigTypeDef",
     {
         "Labels": Sequence[str],
     },
     total=False,
 )
 
-
 class DocumentClassificationConfigTypeDef(
     _RequiredDocumentClassificationConfigTypeDef, _OptionalDocumentClassificationConfigTypeDef
 ):
     pass
 
-
 DocumentClassificationJobFilterTypeDef = TypedDict(
     "DocumentClassificationJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
+_RequiredOutputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredOutputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
     },
 )
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
+_OptionalOutputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalOutputDataConfigOutputTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+class OutputDataConfigOutputTypeDef(
+    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
+):
     pass
 
+_RequiredDocumentClassifierDocumentsOutputTypeDef = TypedDict(
+    "_RequiredDocumentClassifierDocumentsOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalDocumentClassifierDocumentsOutputTypeDef = TypedDict(
+    "_OptionalDocumentClassifierDocumentsOutputTypeDef",
+    {
+        "TestS3Uri": str,
+    },
+    total=False,
+)
+
+class DocumentClassifierDocumentsOutputTypeDef(
+    _RequiredDocumentClassifierDocumentsOutputTypeDef,
+    _OptionalDocumentClassifierDocumentsOutputTypeDef,
+):
+    pass
 
 _RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
     "_RequiredDocumentClassifierDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
@@ -1085,32 +1159,60 @@
     "_OptionalDocumentClassifierDocumentsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
-
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
-
 DocumentClassifierFilterTypeDef = TypedDict(
     "DocumentClassifierFilterTypeDef",
     {
         "Status": ModelStatusType,
         "DocumentClassifierName": str,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentReaderConfigOutputTypeDef",
+    {
+        "DocumentReadAction": DocumentReadActionType,
+    },
+)
+_OptionalDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentReaderConfigOutputTypeDef",
+    {
+        "DocumentReadMode": DocumentReadModeType,
+        "FeatureTypes": List[DocumentReadFeatureTypesType],
+    },
+    total=False,
+)
+
+class DocumentReaderConfigOutputTypeDef(
+    _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
+):
+    pass
+
+DocumentClassifierOutputDataConfigOutputTypeDef = TypedDict(
+    "DocumentClassifierOutputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "KmsKeyId": str,
+        "FlywheelStatsS3Prefix": str,
+    },
+    total=False,
+)
+
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1157,41 +1259,86 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+EntityTypesListItemOutputTypeDef = TypedDict(
+    "EntityTypesListItemOutputTypeDef",
+    {
+        "Type": str,
+    },
+)
+
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
+_RequiredEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerAnnotationsOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerAnnotationsOutputTypeDef",
+    {
+        "TestS3Uri": str,
+    },
+    total=False,
+)
+
+class EntityRecognizerAnnotationsOutputTypeDef(
+    _RequiredEntityRecognizerAnnotationsOutputTypeDef,
+    _OptionalEntityRecognizerAnnotationsOutputTypeDef,
+):
+    pass
+
 _RequiredEntityRecognizerAnnotationsTypeDef = TypedDict(
     "_RequiredEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerAnnotationsTypeDef = TypedDict(
     "_OptionalEntityRecognizerAnnotationsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
-
 class EntityRecognizerAnnotationsTypeDef(
     _RequiredEntityRecognizerAnnotationsTypeDef, _OptionalEntityRecognizerAnnotationsTypeDef
 ):
     pass
 
+_RequiredEntityRecognizerDocumentsOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerDocumentsOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalEntityRecognizerDocumentsOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerDocumentsOutputTypeDef",
+    {
+        "TestS3Uri": str,
+        "InputFormat": InputFormatType,
+    },
+    total=False,
+)
+
+class EntityRecognizerDocumentsOutputTypeDef(
+    _RequiredEntityRecognizerDocumentsOutputTypeDef, _OptionalEntityRecognizerDocumentsOutputTypeDef
+):
+    pass
 
 _RequiredEntityRecognizerDocumentsTypeDef = TypedDict(
     "_RequiredEntityRecognizerDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
@@ -1200,20 +1347,25 @@
     {
         "TestS3Uri": str,
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
-
 class EntityRecognizerDocumentsTypeDef(
     _RequiredEntityRecognizerDocumentsTypeDef, _OptionalEntityRecognizerDocumentsTypeDef
 ):
     pass
 
+EntityRecognizerEntityListOutputTypeDef = TypedDict(
+    "EntityRecognizerEntityListOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
 
 EntityRecognizerEntityListTypeDef = TypedDict(
     "EntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
@@ -1397,14 +1549,31 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
     "TargetedSentimentDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
@@ -1419,14 +1588,31 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+    pass
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1452,23 +1638,21 @@
     "_OptionalPiiOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
-
-RedactionConfigTypeDef = TypedDict(
-    "RedactionConfigTypeDef",
+RedactionConfigOutputTypeDef = TypedDict(
+    "RedactionConfigOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
@@ -1484,29 +1668,37 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "PolicyRevisionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RedactionConfigTypeDef = TypedDict(
+    "RedactionConfigTypeDef",
+    {
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
+        "MaskMode": PiiEntitiesDetectionMaskModeType,
+        "MaskCharacter": str,
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
@@ -1566,22 +1758,20 @@
     "_OptionalStartFlywheelIterationRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class StartFlywheelIterationRequestRequestTypeDef(
     _RequiredStartFlywheelIterationRequestRequestTypeDef,
     _OptionalStartFlywheelIterationRequestRequestTypeDef,
 ):
     pass
 
-
 StartFlywheelIterationResponseTypeDef = TypedDict(
     "StartFlywheelIterationResponseTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1784,21 +1974,19 @@
         "DesiredInferenceUnits": int,
         "DesiredDataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class UpdateEndpointRequestRequestTypeDef(
     _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
-
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "DesiredModelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1899,21 +2087,19 @@
         "Text": str,
         "Bytes": Union[str, bytes, IO[Any], StreamingBody],
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-
 class ClassifyDocumentRequestRequestTypeDef(
     _RequiredClassifyDocumentRequestRequestTypeDef, _OptionalClassifyDocumentRequestRequestTypeDef
 ):
     pass
 
-
 DetectEntitiesRequestRequestTypeDef = TypedDict(
     "DetectEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
         "EndpointArn": str,
         "Bytes": Union[str, bytes, IO[Any], StreamingBody],
@@ -1933,19 +2119,17 @@
     {
         "InputFormat": InputFormatType,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1965,21 +2149,19 @@
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredImportModelRequestRequestTypeDef = TypedDict(
     "_RequiredImportModelRequestRequestTypeDef",
     {
         "SourceModelArn": str,
     },
 )
 _OptionalImportModelRequestRequestTypeDef = TypedDict(
@@ -1990,30 +2172,19 @@
         "ModelKmsKeyId": str,
         "DataAccessRoleArn": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportModelRequestRequestTypeDef(
     _RequiredImportModelRequestRequestTypeDef, _OptionalImportModelRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2035,14 +2206,25 @@
         "ModelKmsKeyId": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
+DataSecurityConfigOutputTypeDef = TypedDict(
+    "DataSecurityConfigOutputTypeDef",
+    {
+        "ModelKmsKeyId": str,
+        "VolumeKmsKeyId": str,
+        "DataLakeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2050,22 +2232,20 @@
     {
         "Annotations": DatasetEntityRecognizerAnnotationsTypeDef,
         "EntityList": DatasetEntityRecognizerEntityListTypeDef,
     },
     total=False,
 )
 
-
 class DatasetEntityRecognizerInputDataConfigTypeDef(
     _RequiredDatasetEntityRecognizerInputDataConfigTypeDef,
     _OptionalDatasetEntityRecognizerInputDataConfigTypeDef,
 ):
     pass
 
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "FlywheelArn": str,
         "Filter": DatasetFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
@@ -2164,14 +2344,49 @@
         "Filter": DocumentClassifierFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
+    "DocumentClassifierInputDataConfigOutputTypeDef",
+    {
+        "DataFormat": DocumentClassifierDataFormatType,
+        "S3Uri": str,
+        "TestS3Uri": str,
+        "LabelDelimiter": str,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
+        "DocumentType": DocumentClassifierDocumentTypeFormatType,
+        "Documents": DocumentClassifierDocumentsOutputTypeDef,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "InputFormat": InputFormatType,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
+    pass
+
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2241,21 +2456,52 @@
         "Filter": EntitiesDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+EntityRecognitionConfigOutputTypeDef = TypedDict(
+    "EntityRecognitionConfigOutputTypeDef",
+    {
+        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+    },
+)
+
 EntityRecognitionConfigTypeDef = TypedDict(
     "EntityRecognitionConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 
+_RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
+    {
+        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+    },
+)
+_OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
+    {
+        "DataFormat": EntityRecognizerDataFormatType,
+        "Documents": EntityRecognizerDocumentsOutputTypeDef,
+        "Annotations": EntityRecognizerAnnotationsOutputTypeDef,
+        "EntityList": EntityRecognizerEntityListOutputTypeDef,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
+    },
+    total=False,
+)
+
+class EntityRecognizerInputDataConfigOutputTypeDef(
+    _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
+    _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
+):
+    pass
+
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2266,21 +2512,19 @@
         "Annotations": EntityRecognizerAnnotationsTypeDef,
         "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
     },
     total=False,
 )
 
-
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
-
 ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
     "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     {
         "Filter": EntityRecognizerFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -2347,22 +2591,20 @@
         "Filter": FlywheelIterationFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListFlywheelIterationHistoryRequestRequestTypeDef(
     _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
     _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 FlywheelIterationPropertiesTypeDef = TypedDict(
     "FlywheelIterationPropertiesTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2448,14 +2690,23 @@
         "Filter": SentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     {
         "Filter": TargetedSentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2543,155 +2794,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
-DocumentClassificationJobPropertiesTypeDef = TypedDict(
-    "DocumentClassificationJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "DocumentClassifierArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-EntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "EntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "EntityRecognizerArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-EventsDetectionJobPropertiesTypeDef = TypedDict(
-    "EventsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "TargetEventTypes": List[str],
-    },
-    total=False,
-)
-
-KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": PiiOutputDataConfigTypeDef,
-        "RedactionConfig": RedactionConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "Mode": PiiEntitiesDetectionModeType,
-    },
-    total=False,
-)
-
-SentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "SentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartDocumentClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentClassificationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2706,22 +2816,20 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class StartDocumentClassificationJobRequestRequestTypeDef(
     _RequiredStartDocumentClassificationJobRequestRequestTypeDef,
     _OptionalStartDocumentClassificationJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2734,22 +2842,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartDominantLanguageDetectionJobRequestRequestTypeDef(
     _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef,
     _OptionalStartDominantLanguageDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2765,22 +2871,20 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
-
 class StartEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartEventsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEventsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2793,22 +2897,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartEventsDetectionJobRequestRequestTypeDef(
     _RequiredStartEventsDetectionJobRequestRequestTypeDef,
     _OptionalStartEventsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2822,22 +2924,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartKeyPhrasesDetectionJobRequestRequestTypeDef(
     _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef,
     _OptionalStartKeyPhrasesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "Mode": PiiEntitiesDetectionModeType,
         "DataAccessRoleArn": str,
@@ -2851,22 +2951,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartPiiEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartPiiEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2880,22 +2978,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2909,22 +3005,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartTargetedSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartTargetedSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartTopicsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTopicsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2938,62 +3032,20 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
-TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-TopicsDetectionJobPropertiesTypeDef = TypedDict(
-    "TopicsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "NumberOfTopics": int,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalUpdateFlywheelRequestRequestTypeDef = TypedDict(
@@ -3002,21 +3054,19 @@
         "ActiveModelArn": str,
         "DataAccessRoleArn": str,
         "DataSecurityConfig": UpdateDataSecurityConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
-
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
@@ -3045,61 +3095,258 @@
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
-
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
-
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
-        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
+        "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
+        "OutputDataConfig": DocumentClassifierOutputDataConfigOutputTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+DocumentClassificationJobPropertiesTypeDef = TypedDict(
+    "DocumentClassificationJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "DocumentClassifierArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "EntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "EntityRecognizerArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+EventsDetectionJobPropertiesTypeDef = TypedDict(
+    "EventsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "TargetEventTypes": List[str],
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": PiiOutputDataConfigTypeDef,
+        "RedactionConfig": RedactionConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "Mode": PiiEntitiesDetectionModeType,
+    },
+    total=False,
+)
+
+SentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "SentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobPropertiesTypeDef = TypedDict(
+    "TopicsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "NumberOfTopics": int,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTaskConfigOutputTypeDef = TypedDict(
+    "_RequiredTaskConfigOutputTypeDef",
+    {
+        "LanguageCode": LanguageCodeType,
+    },
+)
+_OptionalTaskConfigOutputTypeDef = TypedDict(
+    "_OptionalTaskConfigOutputTypeDef",
+    {
+        "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
+        "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
+    pass
+
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
 _OptionalTaskConfigTypeDef = TypedDict(
@@ -3107,19 +3354,17 @@
     {
         "DocumentClassificationConfig": DocumentClassificationConfigTypeDef,
         "EntityRecognitionConfig": EntityRecognitionConfigTypeDef,
     },
     total=False,
 )
 
-
 class TaskConfigTypeDef(_RequiredTaskConfigTypeDef, _OptionalTaskConfigTypeDef):
     pass
 
-
 _RequiredCreateEntityRecognizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRecognizerRequestRequestTypeDef",
     {
         "RecognizerName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -3135,22 +3380,20 @@
         "VpcConfig": VpcConfigTypeDef,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
-
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
-
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3219,14 +3462,55 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "DatasetName": str,
+        "InputDataConfig": DatasetInputDataConfigTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3376,57 +3660,33 @@
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
+FlywheelPropertiesTypeDef = TypedDict(
+    "FlywheelPropertiesTypeDef",
     {
         "FlywheelArn": str,
-        "DatasetName": str,
-        "InputDataConfig": DatasetInputDataConfigTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "Description": str,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "ActiveModelArn": str,
+        "DataAccessRoleArn": str,
+        "TaskConfig": TaskConfigOutputTypeDef,
+        "DataLakeS3Uri": str,
+        "DataSecurityConfig": DataSecurityConfigOutputTypeDef,
+        "Status": FlywheelStatusType,
+        "ModelType": ModelTypeType,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LatestFlywheelIteration": str,
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
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3440,56 +3700,35 @@
         "DataSecurityConfig": DataSecurityConfigTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
-
-FlywheelPropertiesTypeDef = TypedDict(
-    "FlywheelPropertiesTypeDef",
-    {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "DataAccessRoleArn": str,
-        "TaskConfig": TaskConfigTypeDef,
-        "DataLakeS3Uri": str,
-        "DataSecurityConfig": DataSecurityConfigTypeDef,
-        "Status": FlywheelStatusType,
-        "ModelType": ModelTypeType,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LatestFlywheelIteration": str,
-    },
-    total=False,
-)
-
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
+        "InputDataConfig": EntityRecognizerInputDataConfigOutputTypeDef,
         "RecognizerMetadata": EntityRecognizerMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
         "OutputDataConfig": EntityRecognizerOutputDataConfigTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend/type_defs.pyi` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for comprehend service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_comprehend.type_defs import AugmentedManifestsListItemTypeDef
+    from mypy_boto3_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
 
-    data: AugmentedManifestsListItemTypeDef = {...}
+    data: AugmentedManifestsListItemOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -57,15 +57,17 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
@@ -89,14 +91,15 @@
     "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
     "CreateDocumentClassifierResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "CreateEntityRecognizerResponseTypeDef",
     "CreateFlywheelResponseTypeDef",
+    "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "DatasetFilterTypeDef",
     "DatasetPropertiesTypeDef",
@@ -126,27 +129,35 @@
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
+    "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
     "DocumentClassificationJobFilterTypeDef",
-    "OutputDataConfigTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "DocumentClassifierDocumentsOutputTypeDef",
     "DocumentClassifierDocumentsTypeDef",
     "DocumentClassifierFilterTypeDef",
+    "DocumentReaderConfigOutputTypeDef",
+    "DocumentClassifierOutputDataConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
+    "EntityTypesListItemOutputTypeDef",
     "EntityTypesListItemTypeDef",
+    "EntityRecognizerAnnotationsOutputTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
+    "EntityRecognizerDocumentsOutputTypeDef",
     "EntityRecognizerDocumentsTypeDef",
+    "EntityRecognizerEntityListOutputTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
     "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
     "EventsDetectionJobFilterTypeDef",
@@ -158,22 +169,25 @@
     "ImportModelResponseTypeDef",
     "KeyPhrasesDetectionJobFilterTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "PiiEntitiesDetectionJobFilterTypeDef",
     "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "TargetedSentimentDetectionJobFilterTypeDef",
     "TopicsDetectionJobFilterTypeDef",
+    "OutputDataConfigTypeDef",
     "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
-    "RedactionConfigTypeDef",
+    "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutResourcePolicyResponseTypeDef",
+    "RedactionConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
     "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
@@ -212,39 +226,43 @@
     "ClassifierMetadataTypeDef",
     "ClassifyDocumentRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
+    "DataSecurityConfigOutputTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
     "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
     "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
+    "DocumentClassifierInputDataConfigOutputTypeDef",
+    "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
     "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
+    "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
+    "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
     "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
@@ -254,56 +272,61 @@
     "GeometryTypeDef",
     "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
-    "DocumentClassificationJobPropertiesTypeDef",
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    "EntitiesDetectionJobPropertiesTypeDef",
-    "EventsDetectionJobPropertiesTypeDef",
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    "SentimentDetectionJobPropertiesTypeDef",
     "StartDocumentClassificationJobRequestRequestTypeDef",
     "StartDominantLanguageDetectionJobRequestRequestTypeDef",
     "StartEntitiesDetectionJobRequestRequestTypeDef",
     "StartEventsDetectionJobRequestRequestTypeDef",
     "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    "TopicsDetectionJobPropertiesTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
     "DatasetInputDataConfigTypeDef",
     "CreateDocumentClassifierRequestRequestTypeDef",
     "DocumentClassifierPropertiesTypeDef",
+    "DocumentClassificationJobPropertiesTypeDef",
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    "EntitiesDetectionJobPropertiesTypeDef",
+    "EventsDetectionJobPropertiesTypeDef",
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    "SentimentDetectionJobPropertiesTypeDef",
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    "TopicsDetectionJobPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
+    "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -314,32 +337,55 @@
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
-    "CreateFlywheelRequestRequestTypeDef",
     "FlywheelPropertiesTypeDef",
+    "CreateFlywheelRequestRequestTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
     "UpdateFlywheelResponseTypeDef",
     "DescribeEntityRecognizerResponseTypeDef",
     "ListEntityRecognizersResponseTypeDef",
     "BatchDetectTargetedSentimentResponseTypeDef",
 )
 
+_RequiredAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_RequiredAugmentedManifestsListItemOutputTypeDef",
+    {
+        "S3Uri": str,
+        "AttributeNames": List[str],
+    },
+)
+_OptionalAugmentedManifestsListItemOutputTypeDef = TypedDict(
+    "_OptionalAugmentedManifestsListItemOutputTypeDef",
+    {
+        "Split": SplitType,
+        "AnnotationDataS3Uri": str,
+        "SourceDocumentsS3Uri": str,
+        "DocumentType": AugmentedManifestsDocumentTypeFormatType,
+    },
+    total=False,
+)
+
+
+class AugmentedManifestsListItemOutputTypeDef(
+    _RequiredAugmentedManifestsListItemOutputTypeDef,
+    _OptionalAugmentedManifestsListItemOutputTypeDef,
+):
+    pass
+
+
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -350,19 +396,21 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
+
 class AugmentedManifestsListItemTypeDef(
     _RequiredAugmentedManifestsListItemTypeDef, _OptionalAugmentedManifestsListItemTypeDef
 ):
     pass
 
+
 DominantLanguageTypeDef = TypedDict(
     "DominantLanguageTypeDef",
     {
         "LanguageCode": str,
         "Score": float,
     },
     total=False,
@@ -503,19 +551,21 @@
     {
         "DocumentReadMode": DocumentReadModeType,
         "FeatureTypes": Sequence[DocumentReadFeatureTypesType],
     },
     total=False,
 )
 
+
 class DocumentReaderConfigTypeDef(
     _RequiredDocumentReaderConfigTypeDef, _OptionalDocumentReaderConfigTypeDef
 ):
     pass
 
+
 DocumentClassTypeDef = TypedDict(
     "DocumentClassTypeDef",
     {
         "Name": str,
         "Score": float,
         "Page": int,
     },
@@ -588,17 +638,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "DatasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -651,14 +703,22 @@
     {
         "FlywheelArn": str,
         "ActiveModelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
+
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
         "S3Uri": str,
     },
 )
@@ -668,40 +728,44 @@
         "AnnotationDataS3Uri": str,
         "SourceDocumentsS3Uri": str,
         "DocumentType": AugmentedManifestsDocumentTypeFormatType,
     },
     total=False,
 )
 
+
 class DatasetAugmentedManifestsListItemTypeDef(
     _RequiredDatasetAugmentedManifestsListItemTypeDef,
     _OptionalDatasetAugmentedManifestsListItemTypeDef,
 ):
     pass
 
+
 _RequiredDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalDatasetDocumentClassifierInputDataConfigTypeDef = TypedDict(
     "_OptionalDatasetDocumentClassifierInputDataConfigTypeDef",
     {
         "LabelDelimiter": str,
     },
     total=False,
 )
 
+
 class DatasetDocumentClassifierInputDataConfigTypeDef(
     _RequiredDatasetDocumentClassifierInputDataConfigTypeDef,
     _OptionalDatasetDocumentClassifierInputDataConfigTypeDef,
 ):
     pass
 
+
 DatasetEntityRecognizerAnnotationsTypeDef = TypedDict(
     "DatasetEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -715,20 +779,22 @@
     "_OptionalDatasetEntityRecognizerDocumentsTypeDef",
     {
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
+
 class DatasetEntityRecognizerDocumentsTypeDef(
     _RequiredDatasetEntityRecognizerDocumentsTypeDef,
     _OptionalDatasetEntityRecognizerDocumentsTypeDef,
 ):
     pass
 
+
 DatasetEntityRecognizerEntityListTypeDef = TypedDict(
     "DatasetEntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -798,20 +864,22 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 
@@ -1005,91 +1073,175 @@
     "DetectTargetedSentimentRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
 
+_RequiredDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentClassificationConfigOutputTypeDef",
+    {
+        "Mode": DocumentClassifierModeType,
+    },
+)
+_OptionalDocumentClassificationConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentClassificationConfigOutputTypeDef",
+    {
+        "Labels": List[str],
+    },
+    total=False,
+)
+
+
+class DocumentClassificationConfigOutputTypeDef(
+    _RequiredDocumentClassificationConfigOutputTypeDef,
+    _OptionalDocumentClassificationConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
     "_OptionalDocumentClassificationConfigTypeDef",
     {
         "Labels": Sequence[str],
     },
     total=False,
 )
 
+
 class DocumentClassificationConfigTypeDef(
     _RequiredDocumentClassificationConfigTypeDef, _OptionalDocumentClassificationConfigTypeDef
 ):
     pass
 
+
 DocumentClassificationJobFilterTypeDef = TypedDict(
     "DocumentClassificationJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
+_RequiredOutputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredOutputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
     },
 )
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
+_OptionalOutputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalOutputDataConfigOutputTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+
+class OutputDataConfigOutputTypeDef(
+    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
+):
     pass
 
+
+_RequiredDocumentClassifierDocumentsOutputTypeDef = TypedDict(
+    "_RequiredDocumentClassifierDocumentsOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalDocumentClassifierDocumentsOutputTypeDef = TypedDict(
+    "_OptionalDocumentClassifierDocumentsOutputTypeDef",
+    {
+        "TestS3Uri": str,
+    },
+    total=False,
+)
+
+
+class DocumentClassifierDocumentsOutputTypeDef(
+    _RequiredDocumentClassifierDocumentsOutputTypeDef,
+    _OptionalDocumentClassifierDocumentsOutputTypeDef,
+):
+    pass
+
+
 _RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
     "_RequiredDocumentClassifierDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalDocumentClassifierDocumentsTypeDef = TypedDict(
     "_OptionalDocumentClassifierDocumentsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
+
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
+
 DocumentClassifierFilterTypeDef = TypedDict(
     "DocumentClassifierFilterTypeDef",
     {
         "Status": ModelStatusType,
         "DocumentClassifierName": str,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_RequiredDocumentReaderConfigOutputTypeDef",
+    {
+        "DocumentReadAction": DocumentReadActionType,
+    },
+)
+_OptionalDocumentReaderConfigOutputTypeDef = TypedDict(
+    "_OptionalDocumentReaderConfigOutputTypeDef",
+    {
+        "DocumentReadMode": DocumentReadModeType,
+        "FeatureTypes": List[DocumentReadFeatureTypesType],
+    },
+    total=False,
+)
+
+
+class DocumentReaderConfigOutputTypeDef(
+    _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
+):
+    pass
+
+
+DocumentClassifierOutputDataConfigOutputTypeDef = TypedDict(
+    "DocumentClassifierOutputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "KmsKeyId": str,
+        "FlywheelStatsS3Prefix": str,
+    },
+    total=False,
+)
+
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1136,40 +1288,93 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+EntityTypesListItemOutputTypeDef = TypedDict(
+    "EntityTypesListItemOutputTypeDef",
+    {
+        "Type": str,
+    },
+)
+
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
+_RequiredEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerAnnotationsOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerAnnotationsOutputTypeDef",
+    {
+        "TestS3Uri": str,
+    },
+    total=False,
+)
+
+
+class EntityRecognizerAnnotationsOutputTypeDef(
+    _RequiredEntityRecognizerAnnotationsOutputTypeDef,
+    _OptionalEntityRecognizerAnnotationsOutputTypeDef,
+):
+    pass
+
+
 _RequiredEntityRecognizerAnnotationsTypeDef = TypedDict(
     "_RequiredEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerAnnotationsTypeDef = TypedDict(
     "_OptionalEntityRecognizerAnnotationsTypeDef",
     {
         "TestS3Uri": str,
     },
     total=False,
 )
 
+
 class EntityRecognizerAnnotationsTypeDef(
     _RequiredEntityRecognizerAnnotationsTypeDef, _OptionalEntityRecognizerAnnotationsTypeDef
 ):
     pass
 
+
+_RequiredEntityRecognizerDocumentsOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerDocumentsOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalEntityRecognizerDocumentsOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerDocumentsOutputTypeDef",
+    {
+        "TestS3Uri": str,
+        "InputFormat": InputFormatType,
+    },
+    total=False,
+)
+
+
+class EntityRecognizerDocumentsOutputTypeDef(
+    _RequiredEntityRecognizerDocumentsOutputTypeDef, _OptionalEntityRecognizerDocumentsOutputTypeDef
+):
+    pass
+
+
 _RequiredEntityRecognizerDocumentsTypeDef = TypedDict(
     "_RequiredEntityRecognizerDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerDocumentsTypeDef = TypedDict(
@@ -1177,19 +1382,28 @@
     {
         "TestS3Uri": str,
         "InputFormat": InputFormatType,
     },
     total=False,
 )
 
+
 class EntityRecognizerDocumentsTypeDef(
     _RequiredEntityRecognizerDocumentsTypeDef, _OptionalEntityRecognizerDocumentsTypeDef
 ):
     pass
 
+
+EntityRecognizerEntityListOutputTypeDef = TypedDict(
+    "EntityRecognizerEntityListOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+
 EntityRecognizerEntityListTypeDef = TypedDict(
     "EntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -1372,14 +1586,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
     "TargetedSentimentDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
@@ -1394,14 +1627,33 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+    pass
+
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1427,21 +1679,23 @@
     "_OptionalPiiOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
-RedactionConfigTypeDef = TypedDict(
-    "RedactionConfigTypeDef",
+
+RedactionConfigOutputTypeDef = TypedDict(
+    "RedactionConfigOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
@@ -1457,27 +1711,39 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "PolicyRevisionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RedactionConfigTypeDef = TypedDict(
+    "RedactionConfigTypeDef",
+    {
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
+        "MaskMode": PiiEntitiesDetectionMaskModeType,
+        "MaskCharacter": str,
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
@@ -1537,20 +1803,22 @@
     "_OptionalStartFlywheelIterationRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class StartFlywheelIterationRequestRequestTypeDef(
     _RequiredStartFlywheelIterationRequestRequestTypeDef,
     _OptionalStartFlywheelIterationRequestRequestTypeDef,
 ):
     pass
 
+
 StartFlywheelIterationResponseTypeDef = TypedDict(
     "StartFlywheelIterationResponseTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1753,19 +2021,21 @@
         "DesiredInferenceUnits": int,
         "DesiredDataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class UpdateEndpointRequestRequestTypeDef(
     _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
+
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "DesiredModelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1866,19 +2136,21 @@
         "Text": str,
         "Bytes": Union[str, bytes, IO[Any], StreamingBody],
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
+
 class ClassifyDocumentRequestRequestTypeDef(
     _RequiredClassifyDocumentRequestRequestTypeDef, _OptionalClassifyDocumentRequestRequestTypeDef
 ):
     pass
 
+
 DetectEntitiesRequestRequestTypeDef = TypedDict(
     "DetectEntitiesRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
         "EndpointArn": str,
         "Bytes": Union[str, bytes, IO[Any], StreamingBody],
@@ -1898,17 +2170,19 @@
     {
         "InputFormat": InputFormatType,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
+
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
+
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1928,19 +2202,21 @@
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredImportModelRequestRequestTypeDef = TypedDict(
     "_RequiredImportModelRequestRequestTypeDef",
     {
         "SourceModelArn": str,
     },
 )
 _OptionalImportModelRequestRequestTypeDef = TypedDict(
@@ -1951,27 +2227,20 @@
         "ModelKmsKeyId": str,
         "DataAccessRoleArn": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportModelRequestRequestTypeDef(
     _RequiredImportModelRequestRequestTypeDef, _OptionalImportModelRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -1994,14 +2263,25 @@
         "ModelKmsKeyId": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
+DataSecurityConfigOutputTypeDef = TypedDict(
+    "DataSecurityConfigOutputTypeDef",
+    {
+        "ModelKmsKeyId": str,
+        "VolumeKmsKeyId": str,
+        "DataLakeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2009,20 +2289,22 @@
     {
         "Annotations": DatasetEntityRecognizerAnnotationsTypeDef,
         "EntityList": DatasetEntityRecognizerEntityListTypeDef,
     },
     total=False,
 )
 
+
 class DatasetEntityRecognizerInputDataConfigTypeDef(
     _RequiredDatasetEntityRecognizerInputDataConfigTypeDef,
     _OptionalDatasetEntityRecognizerInputDataConfigTypeDef,
 ):
     pass
 
+
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "FlywheelArn": str,
         "Filter": DatasetFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
@@ -2121,14 +2403,51 @@
         "Filter": DocumentClassifierFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
+    "DocumentClassifierInputDataConfigOutputTypeDef",
+    {
+        "DataFormat": DocumentClassifierDataFormatType,
+        "S3Uri": str,
+        "TestS3Uri": str,
+        "LabelDelimiter": str,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
+        "DocumentType": DocumentClassifierDocumentTypeFormatType,
+        "Documents": DocumentClassifierDocumentsOutputTypeDef,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "InputFormat": InputFormatType,
+        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
+    pass
+
+
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2198,21 +2517,54 @@
         "Filter": EntitiesDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+EntityRecognitionConfigOutputTypeDef = TypedDict(
+    "EntityRecognitionConfigOutputTypeDef",
+    {
+        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+    },
+)
+
 EntityRecognitionConfigTypeDef = TypedDict(
     "EntityRecognitionConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 
+_RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
+    {
+        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+    },
+)
+_OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
+    {
+        "DataFormat": EntityRecognizerDataFormatType,
+        "Documents": EntityRecognizerDocumentsOutputTypeDef,
+        "Annotations": EntityRecognizerAnnotationsOutputTypeDef,
+        "EntityList": EntityRecognizerEntityListOutputTypeDef,
+        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class EntityRecognizerInputDataConfigOutputTypeDef(
+    _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
+    _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2223,19 +2575,21 @@
         "Annotations": EntityRecognizerAnnotationsTypeDef,
         "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": Sequence[AugmentedManifestsListItemTypeDef],
     },
     total=False,
 )
 
+
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
+
 ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
     "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     {
         "Filter": EntityRecognizerFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -2302,20 +2656,22 @@
         "Filter": FlywheelIterationFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListFlywheelIterationHistoryRequestRequestTypeDef(
     _RequiredListFlywheelIterationHistoryRequestRequestTypeDef,
     _OptionalListFlywheelIterationHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 FlywheelIterationPropertiesTypeDef = TypedDict(
     "FlywheelIterationPropertiesTypeDef",
     {
         "FlywheelArn": str,
         "FlywheelIterationId": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2401,14 +2757,23 @@
         "Filter": SentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     {
         "Filter": TargetedSentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2496,155 +2861,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
-DocumentClassificationJobPropertiesTypeDef = TypedDict(
-    "DocumentClassificationJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "DocumentClassifierArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-EntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "EntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "EntityRecognizerArn": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-EventsDetectionJobPropertiesTypeDef = TypedDict(
-    "EventsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "TargetEventTypes": List[str],
-    },
-    total=False,
-)
-
-KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": PiiOutputDataConfigTypeDef,
-        "RedactionConfig": RedactionConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "Mode": PiiEntitiesDetectionModeType,
-    },
-    total=False,
-)
-
-SentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "SentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartDocumentClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentClassificationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2659,20 +2883,22 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class StartDocumentClassificationJobRequestRequestTypeDef(
     _RequiredStartDocumentClassificationJobRequestRequestTypeDef,
     _OptionalStartDocumentClassificationJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2685,20 +2911,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartDominantLanguageDetectionJobRequestRequestTypeDef(
     _RequiredStartDominantLanguageDetectionJobRequestRequestTypeDef,
     _OptionalStartDominantLanguageDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2714,20 +2942,22 @@
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "FlywheelArn": str,
     },
     total=False,
 )
 
+
 class StartEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartEventsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEventsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2740,20 +2970,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartEventsDetectionJobRequestRequestTypeDef(
     _RequiredStartEventsDetectionJobRequestRequestTypeDef,
     _OptionalStartEventsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2767,20 +2999,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartKeyPhrasesDetectionJobRequestRequestTypeDef(
     _RequiredStartKeyPhrasesDetectionJobRequestRequestTypeDef,
     _OptionalStartKeyPhrasesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "Mode": PiiEntitiesDetectionModeType,
         "DataAccessRoleArn": str,
@@ -2794,20 +3028,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartPiiEntitiesDetectionJobRequestRequestTypeDef(
     _RequiredStartPiiEntitiesDetectionJobRequestRequestTypeDef,
     _OptionalStartPiiEntitiesDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2821,20 +3057,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": LanguageCodeType,
@@ -2848,20 +3086,22 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartTargetedSentimentDetectionJobRequestRequestTypeDef(
     _RequiredStartTargetedSentimentDetectionJobRequestRequestTypeDef,
     _OptionalStartTargetedSentimentDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartTopicsDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTopicsDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2875,59 +3115,21 @@
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
-TopicsDetectionJobPropertiesTypeDef = TypedDict(
-    "TopicsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "NumberOfTopics": int,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
 
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
@@ -2937,19 +3139,21 @@
         "ActiveModelArn": str,
         "DataAccessRoleArn": str,
         "DataSecurityConfig": UpdateDataSecurityConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
+
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
@@ -2978,59 +3182,262 @@
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
+
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
+
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
-        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
+        "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
+        "OutputDataConfig": DocumentClassifierOutputDataConfigOutputTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
+DocumentClassificationJobPropertiesTypeDef = TypedDict(
+    "DocumentClassificationJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "DocumentClassifierArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "EntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "EntityRecognizerArn": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+EventsDetectionJobPropertiesTypeDef = TypedDict(
+    "EventsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "TargetEventTypes": List[str],
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": PiiOutputDataConfigTypeDef,
+        "RedactionConfig": RedactionConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "Mode": PiiEntitiesDetectionModeType,
+    },
+    total=False,
+)
+
+SentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "SentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobPropertiesTypeDef = TypedDict(
+    "TopicsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "NumberOfTopics": int,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTaskConfigOutputTypeDef = TypedDict(
+    "_RequiredTaskConfigOutputTypeDef",
+    {
+        "LanguageCode": LanguageCodeType,
+    },
+)
+_OptionalTaskConfigOutputTypeDef = TypedDict(
+    "_OptionalTaskConfigOutputTypeDef",
+    {
+        "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
+        "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
+    pass
+
+
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
 _OptionalTaskConfigTypeDef = TypedDict(
@@ -3038,17 +3445,19 @@
     {
         "DocumentClassificationConfig": DocumentClassificationConfigTypeDef,
         "EntityRecognitionConfig": EntityRecognitionConfigTypeDef,
     },
     total=False,
 )
 
+
 class TaskConfigTypeDef(_RequiredTaskConfigTypeDef, _OptionalTaskConfigTypeDef):
     pass
 
+
 _RequiredCreateEntityRecognizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRecognizerRequestRequestTypeDef",
     {
         "RecognizerName": str,
         "DataAccessRoleArn": str,
         "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
@@ -3064,20 +3473,22 @@
         "VpcConfig": VpcConfigTypeDef,
         "ModelKmsKeyId": str,
         "ModelPolicy": str,
     },
     total=False,
 )
 
+
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
+
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3146,14 +3557,57 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "FlywheelArn": str,
+        "DatasetName": str,
+        "InputDataConfig": DatasetInputDataConfigTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
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
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3303,55 +3757,33 @@
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
+FlywheelPropertiesTypeDef = TypedDict(
+    "FlywheelPropertiesTypeDef",
     {
         "FlywheelArn": str,
-        "DatasetName": str,
-        "InputDataConfig": DatasetInputDataConfigTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "Description": str,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "ActiveModelArn": str,
+        "DataAccessRoleArn": str,
+        "TaskConfig": TaskConfigOutputTypeDef,
+        "DataLakeS3Uri": str,
+        "DataSecurityConfig": DataSecurityConfigOutputTypeDef,
+        "Status": FlywheelStatusType,
+        "ModelType": ModelTypeType,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LatestFlywheelIteration": str,
     },
     total=False,
 )
 
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3365,54 +3797,37 @@
         "DataSecurityConfig": DataSecurityConfigTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
-FlywheelPropertiesTypeDef = TypedDict(
-    "FlywheelPropertiesTypeDef",
-    {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "DataAccessRoleArn": str,
-        "TaskConfig": TaskConfigTypeDef,
-        "DataLakeS3Uri": str,
-        "DataSecurityConfig": DataSecurityConfigTypeDef,
-        "Status": FlywheelStatusType,
-        "ModelType": ModelTypeType,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LatestFlywheelIteration": str,
-    },
-    total=False,
-)
 
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
+        "InputDataConfig": EntityRecognizerInputDataConfigOutputTypeDef,
         "RecognizerMetadata": EntityRecognizerMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
         "OutputDataConfig": EntityRecognizerOutputDataConfigTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/PKG-INFO` & `mypy-boto3-comprehend-1.28.12/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-comprehend
-Version: 1.28.0
-Summary: Type annotations for boto3.Comprehend 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 comprehend type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-comprehend"></a>
 
 # mypy-boto3-comprehend
 
 [![PyPI - mypy-boto3-comprehend](https://img.shields.io/pypi/v/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehend?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -398,14 +366,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_comprehend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehend.type_defs import (
+    AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
@@ -429,14 +398,15 @@
     CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
+    VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
     DatasetPropertiesTypeDef,
@@ -466,27 +436,35 @@
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
+    DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
-    OutputDataConfigTypeDef,
+    OutputDataConfigOutputTypeDef,
+    DocumentClassifierDocumentsOutputTypeDef,
     DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
+    DocumentReaderConfigOutputTypeDef,
+    DocumentClassifierOutputDataConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
+    EntityTypesListItemOutputTypeDef,
     EntityTypesListItemTypeDef,
+    EntityRecognizerAnnotationsOutputTypeDef,
     EntityRecognizerAnnotationsTypeDef,
+    EntityRecognizerDocumentsOutputTypeDef,
     EntityRecognizerDocumentsTypeDef,
+    EntityRecognizerEntityListOutputTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
     EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
@@ -498,22 +476,25 @@
     ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
+    OutputDataConfigTypeDef,
     PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
-    RedactionConfigTypeDef,
+    RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutResourcePolicyResponseTypeDef,
+    RedactionConfigTypeDef,
     ResponseMetadataTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
@@ -552,39 +533,43 @@
     ClassifierMetadataTypeDef,
     ClassifyDocumentRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     InputDataConfigTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
+    DataSecurityConfigOutputTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
     ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
+    DocumentClassifierInputDataConfigOutputTypeDef,
+    InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
     ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
     ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
+    EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
+    EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
     ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
@@ -594,56 +579,61 @@
     GeometryTypeDef,
     ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
     TargetedSentimentMentionTypeDef,
     EntityTypeDef,
-    DocumentClassificationJobPropertiesTypeDef,
-    DominantLanguageDetectionJobPropertiesTypeDef,
-    EntitiesDetectionJobPropertiesTypeDef,
-    EventsDetectionJobPropertiesTypeDef,
-    KeyPhrasesDetectionJobPropertiesTypeDef,
-    PiiEntitiesDetectionJobPropertiesTypeDef,
-    SentimentDetectionJobPropertiesTypeDef,
     StartDocumentClassificationJobRequestRequestTypeDef,
     StartDominantLanguageDetectionJobRequestRequestTypeDef,
     StartEntitiesDetectionJobRequestRequestTypeDef,
     StartEventsDetectionJobRequestRequestTypeDef,
     StartKeyPhrasesDetectionJobRequestRequestTypeDef,
     StartPiiEntitiesDetectionJobRequestRequestTypeDef,
     StartSentimentDetectionJobRequestRequestTypeDef,
     StartTargetedSentimentDetectionJobRequestRequestTypeDef,
     StartTopicsDetectionJobRequestRequestTypeDef,
-    TargetedSentimentDetectionJobPropertiesTypeDef,
-    TopicsDetectionJobPropertiesTypeDef,
     UpdateFlywheelRequestRequestTypeDef,
     DatasetInputDataConfigTypeDef,
     CreateDocumentClassifierRequestRequestTypeDef,
     DocumentClassifierPropertiesTypeDef,
+    DocumentClassificationJobPropertiesTypeDef,
+    DominantLanguageDetectionJobPropertiesTypeDef,
+    EntitiesDetectionJobPropertiesTypeDef,
+    EventsDetectionJobPropertiesTypeDef,
+    KeyPhrasesDetectionJobPropertiesTypeDef,
+    PiiEntitiesDetectionJobPropertiesTypeDef,
+    SentimentDetectionJobPropertiesTypeDef,
+    TargetedSentimentDetectionJobPropertiesTypeDef,
+    TopicsDetectionJobPropertiesTypeDef,
     ClassifyDocumentResponseTypeDef,
+    TaskConfigOutputTypeDef,
     TaskConfigTypeDef,
     CreateEntityRecognizerRequestRequestTypeDef,
     EntityRecognizerMetadataTypeDef,
     DescribeFlywheelIterationResponseTypeDef,
     ListFlywheelIterationHistoryResponseTypeDef,
     BlockTypeDef,
     BatchDetectSyntaxItemResultTypeDef,
     DetectSyntaxResponseTypeDef,
     TargetedSentimentEntityTypeDef,
     BatchDetectEntitiesItemResultTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    DescribeDocumentClassifierResponseTypeDef,
+    ListDocumentClassifiersResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     DescribeEntitiesDetectionJobResponseTypeDef,
     ListEntitiesDetectionJobsResponseTypeDef,
     DescribeEventsDetectionJobResponseTypeDef,
@@ -654,34 +644,31 @@
     ListPiiEntitiesDetectionJobsResponseTypeDef,
     DescribeSentimentDetectionJobResponseTypeDef,
     ListSentimentDetectionJobsResponseTypeDef,
     DescribeTargetedSentimentDetectionJobResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     DescribeTopicsDetectionJobResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    DescribeDocumentClassifierResponseTypeDef,
-    ListDocumentClassifiersResponseTypeDef,
-    CreateFlywheelRequestRequestTypeDef,
     FlywheelPropertiesTypeDef,
+    CreateFlywheelRequestRequestTypeDef,
     EntityRecognizerPropertiesTypeDef,
     DetectEntitiesResponseTypeDef,
     BatchDetectSyntaxResponseTypeDef,
     BatchDetectTargetedSentimentItemResultTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     BatchDetectEntitiesResponseTypeDef,
     DescribeFlywheelResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
     DescribeEntityRecognizerResponseTypeDef,
     ListEntityRecognizersResponseTypeDef,
     BatchDetectTargetedSentimentResponseTypeDef,
 )
 
 
-def get_structure() -> AugmentedManifestsListItemTypeDef:
+def get_structure() -> AugmentedManifestsListItemOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehend-1.28.0/mypy_boto3_comprehend.egg-info/SOURCES.txt` & `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.0/setup.py` & `mypy-boto3-comprehend-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehend",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Comprehend 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Comprehend 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

