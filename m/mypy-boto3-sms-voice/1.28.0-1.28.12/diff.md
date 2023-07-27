# Comparing `tmp/mypy-boto3-sms-voice-1.28.0.tar.gz` & `tmp/mypy-boto3-sms-voice-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sms-voice-1.28.0.tar", last modified: Thu Jul  6 21:00:40 2023, max compression
+gzip compressed data, was "mypy-boto3-sms-voice-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
```

## Comparing `mypy-boto3-sms-voice-1.28.0.tar` & `mypy-boto3-sms-voice-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.158436 mypy-boto3-sms-voice-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-06 21:00:40.158436 mypy-boto3-sms-voice-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.150436 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:05.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.158436 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-06 21:00:39.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 21:00:39.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:39.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:39.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:39.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:39.000000 mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:40.158436 mypy-boto3-sms-voice-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:56:04.000000 mypy-boto3-sms-voice-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.149315 mypy-boto3-sms-voice-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-27 11:49:41.145316 mypy-boto3-sms-voice-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.137315 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.145316 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-27 11:49:40.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 11:49:40.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:40.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:40.000000 mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.149315 mypy-boto3-sms-voice-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:47:04.000000 mypy-boto3-sms-voice-1.28.12/setup.py
```

### Comparing `mypy-boto3-sms-voice-1.28.0/LICENSE` & `mypy-boto3-sms-voice-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-voice-1.28.0/PKG-INFO` & `mypy-boto3-sms-voice-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms-voice
-Version: 1.28.0
-Summary: Type annotations for boto3.PinpointSMSVoice 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PinpointSMSVoice 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sms-voice"></a>
 
 # mypy-boto3-sms-voice
 
 [![PyPI - mypy-boto3-sms-voice](https://img.shields.io/pypi/v/mypy-boto3-sms-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-sms-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms-voice)](https://pepy.tech/project/mypy-boto3-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
+[boto3.PinpointSMSVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
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
 [mypy-boto3-sms-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,29 +296,32 @@
 
 `mypy_boto3_sms_voice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms_voice.type_defs import (
     CallInstructionsMessageTypeTypeDef,
+    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     PlainTextMessageTypeTypeDef,
-    ResponseMetadataTypeDef,
     SSMLMessageTypeTypeDef,
-    SendVoiceMessageResponseTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    SendVoiceMessageResponseTypeDef,
     VoiceMessageContentTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-sms-voice-1.28.0/README.md` & `mypy-boto3-sms-voice-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sms-voice"></a>
 
 # mypy-boto3-sms-voice
 
 [![PyPI - mypy-boto3-sms-voice](https://img.shields.io/pypi/v/mypy-boto3-sms-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-sms-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms-voice)](https://pepy.tech/project/mypy-boto3-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
+[boto3.PinpointSMSVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
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
 [mypy-boto3-sms-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,29 +264,32 @@
 
 `mypy_boto3_sms_voice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms_voice.type_defs import (
     CallInstructionsMessageTypeTypeDef,
+    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     PlainTextMessageTypeTypeDef,
-    ResponseMetadataTypeDef,
     SSMLMessageTypeTypeDef,
-    SendVoiceMessageResponseTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    SendVoiceMessageResponseTypeDef,
     VoiceMessageContentTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/__main__.py` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointSMSVoice 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PinpointSMSVoice 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice\nOther"
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

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/client.py` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/client.pyi` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/literals.py` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
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
@@ -227,26 +228,28 @@
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

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/literals.pyi` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
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
@@ -225,26 +226,28 @@
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

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/type_defs.py` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -17,32 +17,34 @@
 from .literals import EventTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CallInstructionsMessageTypeTypeDef",
+    "CloudWatchLogsDestinationOutputTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "PlainTextMessageTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "SSMLMessageTypeTypeDef",
-    "SendVoiceMessageResponseTypeDef",
     "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "SendVoiceMessageResponseTypeDef",
     "VoiceMessageContentTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
 )
 
@@ -50,14 +52,23 @@
     "CallInstructionsMessageTypeTypeDef",
     {
         "Text": str,
     },
     total=False,
 )
 
+CloudWatchLogsDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationOutputTypeDef",
+    {
+        "IamRoleArn": str,
+        "LogGroupArn": str,
+    },
+    total=False,
+)
+
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
         "LogGroupArn": str,
     },
     total=False,
@@ -99,76 +110,76 @@
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-GetConfigurationSetEventDestinationsRequestRequestTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
     {
-        "ConfigurationSetName": str,
-    },
-)
-
-ListConfigurationSetsRequestRequestTypeDef = TypedDict(
-    "ListConfigurationSetsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": str,
+        "DeliveryStreamArn": str,
+        "IamRoleArn": str,
     },
     total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
+SnsDestinationOutputTypeDef = TypedDict(
+    "SnsDestinationOutputTypeDef",
     {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TopicArn": str,
     },
+    total=False,
 )
 
-PlainTextMessageTypeTypeDef = TypedDict(
-    "PlainTextMessageTypeTypeDef",
+GetConfigurationSetEventDestinationsRequestRequestTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     {
-        "LanguageCode": str,
-        "Text": str,
-        "VoiceId": str,
+        "ConfigurationSetName": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-SSMLMessageTypeTypeDef = TypedDict(
-    "SSMLMessageTypeTypeDef",
+ListConfigurationSetsRequestRequestTypeDef = TypedDict(
+    "ListConfigurationSetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": str,
+    },
+    total=False,
+)
+
+PlainTextMessageTypeTypeDef = TypedDict(
+    "PlainTextMessageTypeTypeDef",
     {
         "LanguageCode": str,
         "Text": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-SendVoiceMessageResponseTypeDef = TypedDict(
-    "SendVoiceMessageResponseTypeDef",
+SSMLMessageTypeTypeDef = TypedDict(
+    "SSMLMessageTypeTypeDef",
     {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LanguageCode": str,
+        "Text": str,
+        "VoiceId": str,
     },
+    total=False,
 )
 
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
         "Enabled": bool,
@@ -178,24 +189,41 @@
     },
     total=False,
 )
 
 EventDestinationTypeDef = TypedDict(
     "EventDestinationTypeDef",
     {
-        "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
+        "CloudWatchLogsDestination": CloudWatchLogsDestinationOutputTypeDef,
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
         "MatchingEventTypes": List[EventTypeType],
         "Name": str,
-        "SnsDestination": SnsDestinationTypeDef,
+        "SnsDestination": SnsDestinationOutputTypeDef,
     },
     total=False,
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendVoiceMessageResponseTypeDef = TypedDict(
+    "SendVoiceMessageResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VoiceMessageContentTypeDef = TypedDict(
     "VoiceMessageContentTypeDef",
     {
         "CallInstructionsMessage": CallInstructionsMessageTypeTypeDef,
         "PlainTextMessage": PlainTextMessageTypeTypeDef,
         "SSMLMessage": SSMLMessageTypeTypeDef,
     },
@@ -213,22 +241,20 @@
     {
         "EventDestination": EventDestinationDefinitionTypeDef,
         "EventDestinationName": str,
     },
     total=False,
 )
 
-
 class CreateConfigurationSetEventDestinationRequestRequestTypeDef(
     _RequiredCreateConfigurationSetEventDestinationRequestRequestTypeDef,
     _OptionalCreateConfigurationSetEventDestinationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -236,27 +262,25 @@
     "_OptionalUpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class UpdateConfigurationSetEventDestinationRequestRequestTypeDef(
     _RequiredUpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     _OptionalUpdateConfigurationSetEventDestinationRequestRequestTypeDef,
 ):
     pass
 
-
 GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
         "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendVoiceMessageRequestRequestTypeDef = TypedDict(
     "SendVoiceMessageRequestRequestTypeDef",
     {
         "CallerId": str,
```

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice/type_defs.pyi` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,31 +17,35 @@
 from .literals import EventTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CallInstructionsMessageTypeTypeDef",
+    "CloudWatchLogsDestinationOutputTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "PlainTextMessageTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "SSMLMessageTypeTypeDef",
-    "SendVoiceMessageResponseTypeDef",
     "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "SendVoiceMessageResponseTypeDef",
     "VoiceMessageContentTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
 )
 
@@ -49,14 +53,23 @@
     "CallInstructionsMessageTypeTypeDef",
     {
         "Text": str,
     },
     total=False,
 )
 
+CloudWatchLogsDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationOutputTypeDef",
+    {
+        "IamRoleArn": str,
+        "LogGroupArn": str,
+    },
+    total=False,
+)
+
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
         "LogGroupArn": str,
     },
     total=False,
@@ -98,76 +111,76 @@
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-GetConfigurationSetEventDestinationsRequestRequestTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
     {
-        "ConfigurationSetName": str,
-    },
-)
-
-ListConfigurationSetsRequestRequestTypeDef = TypedDict(
-    "ListConfigurationSetsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": str,
+        "DeliveryStreamArn": str,
+        "IamRoleArn": str,
     },
     total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
+SnsDestinationOutputTypeDef = TypedDict(
+    "SnsDestinationOutputTypeDef",
     {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TopicArn": str,
     },
+    total=False,
 )
 
-PlainTextMessageTypeTypeDef = TypedDict(
-    "PlainTextMessageTypeTypeDef",
+GetConfigurationSetEventDestinationsRequestRequestTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     {
-        "LanguageCode": str,
-        "Text": str,
-        "VoiceId": str,
+        "ConfigurationSetName": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-SSMLMessageTypeTypeDef = TypedDict(
-    "SSMLMessageTypeTypeDef",
+ListConfigurationSetsRequestRequestTypeDef = TypedDict(
+    "ListConfigurationSetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": str,
+    },
+    total=False,
+)
+
+PlainTextMessageTypeTypeDef = TypedDict(
+    "PlainTextMessageTypeTypeDef",
     {
         "LanguageCode": str,
         "Text": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-SendVoiceMessageResponseTypeDef = TypedDict(
-    "SendVoiceMessageResponseTypeDef",
+SSMLMessageTypeTypeDef = TypedDict(
+    "SSMLMessageTypeTypeDef",
     {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LanguageCode": str,
+        "Text": str,
+        "VoiceId": str,
     },
+    total=False,
 )
 
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
         "Enabled": bool,
@@ -177,24 +190,41 @@
     },
     total=False,
 )
 
 EventDestinationTypeDef = TypedDict(
     "EventDestinationTypeDef",
     {
-        "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
+        "CloudWatchLogsDestination": CloudWatchLogsDestinationOutputTypeDef,
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
         "MatchingEventTypes": List[EventTypeType],
         "Name": str,
-        "SnsDestination": SnsDestinationTypeDef,
+        "SnsDestination": SnsDestinationOutputTypeDef,
     },
     total=False,
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendVoiceMessageResponseTypeDef = TypedDict(
+    "SendVoiceMessageResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VoiceMessageContentTypeDef = TypedDict(
     "VoiceMessageContentTypeDef",
     {
         "CallInstructionsMessage": CallInstructionsMessageTypeTypeDef,
         "PlainTextMessage": PlainTextMessageTypeTypeDef,
         "SSMLMessage": SSMLMessageTypeTypeDef,
     },
@@ -212,20 +242,22 @@
     {
         "EventDestination": EventDestinationDefinitionTypeDef,
         "EventDestinationName": str,
     },
     total=False,
 )
 
+
 class CreateConfigurationSetEventDestinationRequestRequestTypeDef(
     _RequiredCreateConfigurationSetEventDestinationRequestRequestTypeDef,
     _OptionalCreateConfigurationSetEventDestinationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -233,25 +265,27 @@
     "_OptionalUpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class UpdateConfigurationSetEventDestinationRequestRequestTypeDef(
     _RequiredUpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     _OptionalUpdateConfigurationSetEventDestinationRequestRequestTypeDef,
 ):
     pass
 
+
 GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
         "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendVoiceMessageRequestRequestTypeDef = TypedDict(
     "SendVoiceMessageRequestRequestTypeDef",
     {
         "CallerId": str,
```

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/PKG-INFO` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms-voice
-Version: 1.28.0
-Summary: Type annotations for boto3.PinpointSMSVoice 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PinpointSMSVoice 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sms-voice"></a>
 
 # mypy-boto3-sms-voice
 
 [![PyPI - mypy-boto3-sms-voice](https://img.shields.io/pypi/v/mypy-boto3-sms-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-sms-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms-voice)](https://pepy.tech/project/mypy-boto3-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
+[boto3.PinpointSMSVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
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
 [mypy-boto3-sms-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,29 +296,32 @@
 
 `mypy_boto3_sms_voice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms_voice.type_defs import (
     CallInstructionsMessageTypeTypeDef,
+    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     PlainTextMessageTypeTypeDef,
-    ResponseMetadataTypeDef,
     SSMLMessageTypeTypeDef,
-    SendVoiceMessageResponseTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    SendVoiceMessageResponseTypeDef,
     VoiceMessageContentTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-sms-voice-1.28.0/mypy_boto3_sms_voice.egg-info/SOURCES.txt` & `mypy-boto3-sms-voice-1.28.12/mypy_boto3_sms_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-voice-1.28.0/setup.py` & `mypy-boto3-sms-voice-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sms-voice",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sms_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointSMSVoice 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.PinpointSMSVoice 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

