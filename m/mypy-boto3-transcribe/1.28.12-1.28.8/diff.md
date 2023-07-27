# Comparing `tmp/mypy-boto3-transcribe-1.28.12.tar.gz` & `tmp/mypy-boto3-transcribe-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transcribe-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-transcribe-1.28.8.tar", last modified: Thu Jul 20 19:47:57 2023, max compression
```

## Comparing `mypy-boto3-transcribe-1.28.12.tar` & `mypy-boto3-transcribe-1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.861449 mypy-boto3-transcribe-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-07-27 11:49:46.861449 mypy-boto3-transcribe-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.861449 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-27 11:48:05.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-27 11:48:05.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-27 11:48:05.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46420 2023-07-27 11:48:08.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46381 2023-07-27 11:48:08.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.861449 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-07-27 11:49:46.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 11:49:46.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:46.000000 mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.861449 mypy-boto3-transcribe-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 11:48:04.000000 mypy-boto3-transcribe-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44839 2023-07-20 19:47:45.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/setup.py
```

### Comparing `mypy-boto3-transcribe-1.28.12/LICENSE` & `mypy-boto3-transcribe-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.12/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.12
-Summary: Type annotations for boto3.TranscribeService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transcribe-1.28.12/README.md` & `mypy-boto3-transcribe-1.28.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/__main__.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TranscribeService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.TranscribeService 1.28.8\nVersion:         1.28.8\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/client.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/client.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/literals.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,14 @@
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
@@ -327,15 +326,14 @@
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

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/literals.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,14 @@
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
@@ -325,15 +324,14 @@
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

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/type_defs.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,58 +175,43 @@
     "AbsoluteTimeRangeOutputTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
-    total=False,
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
-    {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
-    total=False,
 )
 
-
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
-    pass
-
-
 LanguageIdSettingsOutputTypeDef = TypedDict(
     "LanguageIdSettingsOutputTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
@@ -262,42 +247,38 @@
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
 ChannelDefinitionOutputTypeDef = TypedDict(
     "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
 MediaOutputTypeDef = TypedDict(
     "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
-    total=False,
 )
 
 ChannelDefinitionTypeDef = TypedDict(
     "ChannelDefinitionTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
@@ -340,36 +321,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
-        "DataAccessRoleArn": str,
-    },
-)
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
-    {
         "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
     },
-    total=False,
 )
 
-
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
-    pass
-
-
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -482,15 +450,14 @@
     "RelativeTimeRangeOutputTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
-    total=False,
 )
 
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
@@ -502,15 +469,14 @@
 
 JobExecutionSettingsOutputTypeDef = TypedDict(
     "JobExecutionSettingsOutputTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
-    total=False,
 )
 
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
@@ -520,15 +486,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -580,15 +545,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -602,15 +566,14 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
@@ -659,15 +622,14 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 MediaTypeDef = TypedDict(
     "MediaTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
@@ -676,28 +638,26 @@
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
 )
 
 MedicalTranscriptionSettingOutputTypeDef = TypedDict(
     "MedicalTranscriptionSettingOutputTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
-    total=False,
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -710,15 +670,14 @@
 )
 
 ModelSettingsOutputTypeDef = TypedDict(
     "ModelSettingsOutputTypeDef",
     {
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
@@ -733,15 +692,14 @@
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
     },
-    total=False,
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
@@ -774,15 +732,14 @@
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
 )
 
 ToxicityDetectionSettingsOutputTypeDef = TypedDict(
     "ToxicityDetectionSettingsOutputTypeDef",
     {
         "ToxicityCategories": List[Literal["ALL"]],
     },
@@ -860,15 +817,14 @@
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "LanguageOptions": List[LanguageCodeType],
         "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
@@ -1130,89 +1086,60 @@
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelStatus": ModelStatusType,
         "UpgradeAvailability": bool,
         "FailureReason": str,
         "InputDataConfig": InputDataConfigOutputTypeDef,
     },
-    total=False,
 )
 
 InterruptionFilterOutputTypeDef = TypedDict(
     "InterruptionFilterOutputTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
 NonTalkTimeFilterOutputTypeDef = TypedDict(
     "NonTalkTimeFilterOutputTypeDef",
     {
         "Threshold": int,
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
     {
         "Sentiments": List[SentimentValueType],
-    },
-)
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
-    {
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
-    total=False,
 )
 
-
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
-
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
-    },
-)
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
-    {
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
+        "Targets": List[str],
     },
-    total=False,
 )
 
-
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
-    pass
-
-
 InterruptionFilterTypeDef = TypedDict(
     "InterruptionFilterTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
@@ -1341,15 +1268,14 @@
         "FailureReason": str,
         "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
         "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1437,15 +1363,14 @@
         "ModelSettings": ModelSettingsOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
@@ -1468,15 +1393,14 @@
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
         "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
@@ -1490,15 +1414,14 @@
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
         "Settings": CallAnalyticsJobSettingsOutputTypeDef,
         "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1545,15 +1468,14 @@
     "RuleOutputTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
         "InterruptionFilter": InterruptionFilterOutputTypeDef,
         "TranscriptFilter": TranscriptFilterOutputTypeDef,
         "SentimentFilter": SentimentFilterOutputTypeDef,
     },
-    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
@@ -1626,15 +1548,14 @@
     {
         "CategoryName": str,
         "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
         "Rules": Sequence[RuleTypeDef],
```

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe/type_defs.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -174,56 +174,43 @@
     "AbsoluteTimeRangeOutputTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
-    total=False,
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
-    {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
-    total=False,
 )
 
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
-    pass
-
 LanguageIdSettingsOutputTypeDef = TypedDict(
     "LanguageIdSettingsOutputTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
@@ -257,42 +244,38 @@
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
 ChannelDefinitionOutputTypeDef = TypedDict(
     "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
 MediaOutputTypeDef = TypedDict(
     "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
-    total=False,
 )
 
 ChannelDefinitionTypeDef = TypedDict(
     "ChannelDefinitionTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
@@ -333,34 +316,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
-        "DataAccessRoleArn": str,
-    },
-)
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
-    {
         "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
     },
-    total=False,
 )
 
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
-    pass
-
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -473,15 +445,14 @@
     "RelativeTimeRangeOutputTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
-    total=False,
 )
 
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
@@ -493,15 +464,14 @@
 
 JobExecutionSettingsOutputTypeDef = TypedDict(
     "JobExecutionSettingsOutputTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
-    total=False,
 )
 
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
@@ -511,15 +481,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -571,15 +540,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -593,15 +561,14 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
@@ -650,15 +617,14 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 MediaTypeDef = TypedDict(
     "MediaTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
@@ -667,28 +633,26 @@
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
 )
 
 MedicalTranscriptionSettingOutputTypeDef = TypedDict(
     "MedicalTranscriptionSettingOutputTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
-    total=False,
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -701,15 +665,14 @@
 )
 
 ModelSettingsOutputTypeDef = TypedDict(
     "ModelSettingsOutputTypeDef",
     {
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
@@ -724,15 +687,14 @@
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
     },
-    total=False,
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
@@ -765,15 +727,14 @@
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
 )
 
 ToxicityDetectionSettingsOutputTypeDef = TypedDict(
     "ToxicityDetectionSettingsOutputTypeDef",
     {
         "ToxicityCategories": List[Literal["ALL"]],
     },
@@ -847,15 +808,14 @@
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "LanguageOptions": List[LanguageCodeType],
         "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
@@ -1109,85 +1069,60 @@
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelStatus": ModelStatusType,
         "UpgradeAvailability": bool,
         "FailureReason": str,
         "InputDataConfig": InputDataConfigOutputTypeDef,
     },
-    total=False,
 )
 
 InterruptionFilterOutputTypeDef = TypedDict(
     "InterruptionFilterOutputTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
 NonTalkTimeFilterOutputTypeDef = TypedDict(
     "NonTalkTimeFilterOutputTypeDef",
     {
         "Threshold": int,
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
     {
         "Sentiments": List[SentimentValueType],
-    },
-)
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
-    {
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
-    total=False,
 )
 
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
-    },
-)
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
-    {
         "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
         "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
+        "Targets": List[str],
     },
-    total=False,
 )
 
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
-    pass
-
 InterruptionFilterTypeDef = TypedDict(
     "InterruptionFilterTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
@@ -1312,15 +1247,14 @@
         "FailureReason": str,
         "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
         "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1404,15 +1338,14 @@
         "ModelSettings": ModelSettingsOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
@@ -1435,15 +1368,14 @@
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
         "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
@@ -1457,15 +1389,14 @@
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
         "Settings": CallAnalyticsJobSettingsOutputTypeDef,
         "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1510,15 +1441,14 @@
     "RuleOutputTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
         "InterruptionFilter": InterruptionFilterOutputTypeDef,
         "TranscriptFilter": TranscriptFilterOutputTypeDef,
         "SentimentFilter": SentimentFilterOutputTypeDef,
     },
-    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
@@ -1591,15 +1521,14 @@
     {
         "CategoryName": str,
         "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
         "Rules": Sequence[RuleTypeDef],
```

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.12
-Summary: Type annotations for boto3.TranscribeService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transcribe-1.28.12/mypy_boto3_transcribe.egg-info/SOURCES.txt` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.12/setup.py` & `mypy-boto3-transcribe-1.28.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transcribe",
-    version="1.28.12",
+    version="1.28.8",
     packages=["mypy_boto3_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TranscribeService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.TranscribeService 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

