# Comparing `tmp/mypy-boto3-voice-id-1.28.0.tar.gz` & `tmp/mypy-boto3-voice-id-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-voice-id-1.28.0.tar", last modified: Thu Jul  6 21:00:49 2023, max compression
+gzip compressed data, was "mypy-boto3-voice-id-1.28.12.tar", last modified: Thu Jul 27 11:49:48 2023, max compression
```

## Comparing `mypy-boto3-voice-id-1.28.0.tar` & `mypy-boto3-voice-id-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.874456 mypy-boto3-voice-id-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-06 21:00:49.862456 mypy-boto3-voice-id-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.854456 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32487 2023-07-06 20:57:33.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32450 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.862456 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:49.874456 mypy-boto3-voice-id-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34377 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34338 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/setup.py
```

### Comparing `mypy-boto3-voice-id-1.28.0/LICENSE` & `mypy-boto3-voice-id-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.0/PKG-INFO` & `mypy-boto3-voice-id-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.0
-Summary: Type annotations for boto3.VoiceID 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.VoiceID 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-voice-id"></a>
 
 # mypy-boto3-voice-id
 
 [![PyPI - mypy-boto3-voice-id](https://img.shields.io/pypi/v/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,14 +353,15 @@
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -370,72 +371,78 @@
     DescribeFraudsterRegistrationJobRequestRequestTypeDef,
     DescribeFraudsterRequestRequestTypeDef,
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    InputDataConfigOutputTypeDef,
+    OutputDataConfigOutputTypeDef,
+    RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    InputDataConfigTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    TagOutputTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    OutputDataConfigTypeDef,
+    RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
     DomainTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
-    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.0/README.md` & `mypy-boto3-voice-id-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-voice-id"></a>
 
 # mypy-boto3-voice-id
 
 [![PyPI - mypy-boto3-voice-id](https://img.shields.io/pypi/v/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,14 +321,15 @@
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -338,72 +339,78 @@
     DescribeFraudsterRegistrationJobRequestRequestTypeDef,
     DescribeFraudsterRequestRequestTypeDef,
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    InputDataConfigOutputTypeDef,
+    OutputDataConfigOutputTypeDef,
+    RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    InputDataConfigTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    TagOutputTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    OutputDataConfigTypeDef,
+    RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
     DomainTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
-    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.py` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.pyi` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__main__.py` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VoiceID 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.VoiceID 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.py` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.pyi` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.py` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
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
@@ -278,26 +279,28 @@
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

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.pyi` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,15 @@
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
@@ -276,26 +277,28 @@
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

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.py` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
         """
 
 
@@ -86,15 +86,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
 
@@ -105,15 +105,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterspaginator)
         """
 
 
@@ -124,43 +124,43 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
 
 
 class ListSpeakersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpeakersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
         """
 
 
 class ListWatchlistsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWatchlistsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
         """
```

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.pyi` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
         """
 
 class ListFraudsterRegistrationJobsPaginator(Paginator):
@@ -82,15 +82,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
 class ListFraudstersPaginator(Paginator):
@@ -100,15 +100,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterspaginator)
         """
 
 class ListSpeakerEnrollmentJobsPaginator(Paginator):
@@ -118,41 +118,41 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
 
 class ListSpeakersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpeakersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
         """
 
 class ListWatchlistsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWatchlistsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
         """
```

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.py` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateFraudsterRequestRequestTypeDef",
     "FraudsterTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "TagTypeDef",
     "CreateWatchlistRequestRequestTypeDef",
     "WatchlistTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteFraudsterRequestRequestTypeDef",
@@ -52,72 +53,78 @@
     "DescribeFraudsterRegistrationJobRequestRequestTypeDef",
     "DescribeFraudsterRequestRequestTypeDef",
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
-    "InputDataConfigTypeDef",
-    "OutputDataConfigTypeDef",
-    "RegistrationConfigTypeDef",
+    "InputDataConfigOutputTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "RegistrationConfigOutputTypeDef",
     "FraudsterSummaryTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "InputDataConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
-    "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListFraudstersRequestRequestTypeDef",
-    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
-    "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "OutputDataConfigTypeDef",
+    "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
     "DomainTypeDef",
+    "EnrollmentConfigOutputTypeDef",
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
-    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+    "ListFraudstersRequestListFraudstersPaginateTypeDef",
+    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    "ListSpeakersRequestListSpeakersPaginateTypeDef",
+    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
+    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
@@ -146,14 +153,25 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
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
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "AcceptanceThreshold": int,
     },
 )
 
@@ -306,14 +324,21 @@
     {
         "DomainId": str,
         "FraudsterId": str,
         "WatchlistId": str,
     },
 )
 
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+)
+
 ServerSideEncryptionUpdateDetailsTypeDef = TypedDict(
     "ServerSideEncryptionUpdateDetailsTypeDef",
     {
         "Message": str,
         "OldKmsKeyId": str,
         "UpdateStatus": ServerSideEncryptionUpdateStatusType,
     },
@@ -323,27 +348,30 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EnrollmentJobFraudDetectionConfigOutputTypeDef = TypedDict(
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FraudDetectionAction": FraudDetectionActionType,
+        "RiskThreshold": int,
+        "WatchlistIds": List[str],
     },
+    total=False,
 )
 
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
-        "WatchlistIds": List[str],
+        "WatchlistIds": Sequence[str],
     },
     total=False,
 )
 
 EvaluateSessionRequestRequestTypeDef = TypedDict(
     "EvaluateSessionRequestRequestTypeDef",
     {
@@ -402,42 +430,44 @@
     "JobProgressTypeDef",
     {
         "PercentComplete": int,
     },
     total=False,
 )
 
-InputDataConfigTypeDef = TypedDict(
-    "InputDataConfigTypeDef",
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
     },
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
+class OutputDataConfigOutputTypeDef(
+    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
+):
     pass
 
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
+RegistrationConfigOutputTypeDef = TypedDict(
+    "RegistrationConfigOutputTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": List[str],
     },
     total=False,
 )
@@ -449,58 +479,40 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+InputDataConfigTypeDef = TypedDict(
+    "InputDataConfigTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "DomainId": str,
-        },
-    )
-)
-_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "JobStatus": FraudsterRegistrationJobStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
-    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudsterRegistrationJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
@@ -517,37 +529,14 @@
 class ListFraudsterRegistrationJobsRequestRequestTypeDef(
     _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef,
     _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "WatchlistId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFraudstersRequestListFraudstersPaginateTypeDef(
-    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
-    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFraudstersRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudstersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudstersRequestRequestTypeDef = TypedDict(
@@ -563,37 +552,14 @@
 
 class ListFraudstersRequestRequestTypeDef(
     _RequiredListFraudstersRequestRequestTypeDef, _OptionalListFraudstersRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "JobStatus": SpeakerEnrollmentJobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
-    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
@@ -610,36 +576,14 @@
 class ListSpeakerEnrollmentJobsRequestRequestTypeDef(
     _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef,
     _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSpeakersRequestListSpeakersPaginateTypeDef(
-    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
-    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSpeakersRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakersRequestRequestTypeDef = TypedDict(
@@ -675,36 +619,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-
-class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
-    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
-    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -741,33 +671,41 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "S3Uri": str,
+    },
+)
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
+    {
+        "KmsKeyId": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+    pass
+
+
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DuplicateRegistrationAction": DuplicateRegistrationActionType,
+        "FraudsterSimilarityThreshold": int,
+        "WatchlistIds": Sequence[str],
     },
+    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -797,31 +735,38 @@
     pass
 
 
 AssociateFraudsterResponseTypeDef = TypedDict(
     "AssociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterResponseTypeDef = TypedDict(
     "DescribeFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFraudsterResponseTypeDef = TypedDict(
     "DisassociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
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
 
 AuthenticationResultTypeDef = TypedDict(
     "AuthenticationResultTypeDef",
     {
         "AudioAggregationEndedAt": datetime,
@@ -879,80 +824,72 @@
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
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
 
 CreateWatchlistResponseTypeDef = TypedDict(
     "CreateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWatchlistResponseTypeDef = TypedDict(
     "DescribeWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWatchlistResponseTypeDef = TypedDict(
     "UpdateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerResponseTypeDef = TypedDict(
     "DescribeSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OptOutSpeakerResponseTypeDef = TypedDict(
     "OptOutSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
@@ -961,22 +898,31 @@
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigOutputTypeDef = TypedDict(
+    "EnrollmentConfigOutputTypeDef",
+    {
+        "ExistingEnrollmentAction": ExistingEnrollmentActionType,
+        "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 EnrollmentConfigTypeDef = TypedDict(
     "EnrollmentConfigTypeDef",
     {
         "ExistingEnrollmentAction": ExistingEnrollmentActionType,
         "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigTypeDef,
     },
     total=False,
@@ -1024,127 +970,260 @@
     "FraudsterRegistrationJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "RegistrationConfig": RegistrationConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+ListFraudstersResponseTypeDef = TypedDict(
+    "ListFraudstersResponseTypeDef",
+    {
+        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "DomainId": str,
+        },
+    )
+)
+_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "JobStatus": FraudsterRegistrationJobStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
+    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "DataAccessRoleArn": str,
         "DomainId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
     },
 )
-_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "ClientToken": str,
-        "JobName": str,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "WatchlistId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class StartFraudsterRegistrationJobRequestRequestTypeDef(
-    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
-    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+class ListFraudstersRequestListFraudstersPaginateTypeDef(
+    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
+    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
 ):
     pass
 
 
-ListFraudstersResponseTypeDef = TypedDict(
-    "ListFraudstersResponseTypeDef",
+_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     {
-        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "JobStatus": SpeakerEnrollmentJobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
+    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSpeakersRequestListSpeakersPaginateTypeDef(
+    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
+    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "DomainId": str,
     },
 )
+_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
+    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
+):
+    pass
+
 
 ListSpeakersResponseTypeDef = TypedDict(
     "ListSpeakersResponseTypeDef",
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "DataAccessRoleArn": str,
+        "DomainId": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
     },
 )
+_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "JobName": str,
+        "RegistrationConfig": RegistrationConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class StartFraudsterRegistrationJobRequestRequestTypeDef(
+    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
+    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+):
+    pass
+
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
-        "EnrollmentConfig": EnrollmentConfigTypeDef,
+        "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
@@ -1187,64 +1266,64 @@
 )
 
 ListFraudsterRegistrationJobsResponseTypeDef = TypedDict(
     "ListFraudsterRegistrationJobsResponseTypeDef",
     {
         "JobSummaries": List[FraudsterRegistrationJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeakerEnrollmentJobsResponseTypeDef = TypedDict(
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     {
         "JobSummaries": List[SpeakerEnrollmentJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "StartFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "StartSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateSessionResponseTypeDef = TypedDict(
     "EvaluateSessionResponseTypeDef",
     {
         "AuthenticationResult": AuthenticationResultTypeDef,
         "DomainId": str,
         "FraudDetectionResult": FraudDetectionResultTypeDef,
         "SessionId": str,
         "SessionName": str,
         "StreamingStatus": StreamingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.pyi` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateFraudsterRequestRequestTypeDef",
     "FraudsterTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "TagTypeDef",
     "CreateWatchlistRequestRequestTypeDef",
     "WatchlistTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteFraudsterRequestRequestTypeDef",
@@ -51,72 +52,78 @@
     "DescribeFraudsterRegistrationJobRequestRequestTypeDef",
     "DescribeFraudsterRequestRequestTypeDef",
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
-    "InputDataConfigTypeDef",
-    "OutputDataConfigTypeDef",
-    "RegistrationConfigTypeDef",
+    "InputDataConfigOutputTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "RegistrationConfigOutputTypeDef",
     "FraudsterSummaryTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "InputDataConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
-    "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListFraudstersRequestRequestTypeDef",
-    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
-    "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "OutputDataConfigTypeDef",
+    "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
     "DomainTypeDef",
+    "EnrollmentConfigOutputTypeDef",
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
-    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+    "ListFraudstersRequestListFraudstersPaginateTypeDef",
+    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    "ListSpeakersRequestListSpeakersPaginateTypeDef",
+    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
+    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
@@ -145,14 +152,25 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
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
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "AcceptanceThreshold": int,
     },
 )
 
@@ -303,14 +321,21 @@
     {
         "DomainId": str,
         "FraudsterId": str,
         "WatchlistId": str,
     },
 )
 
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+)
+
 ServerSideEncryptionUpdateDetailsTypeDef = TypedDict(
     "ServerSideEncryptionUpdateDetailsTypeDef",
     {
         "Message": str,
         "OldKmsKeyId": str,
         "UpdateStatus": ServerSideEncryptionUpdateStatusType,
     },
@@ -320,27 +345,30 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EnrollmentJobFraudDetectionConfigOutputTypeDef = TypedDict(
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FraudDetectionAction": FraudDetectionActionType,
+        "RiskThreshold": int,
+        "WatchlistIds": List[str],
     },
+    total=False,
 )
 
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
-        "WatchlistIds": List[str],
+        "WatchlistIds": Sequence[str],
     },
     total=False,
 )
 
 EvaluateSessionRequestRequestTypeDef = TypedDict(
     "EvaluateSessionRequestRequestTypeDef",
     {
@@ -397,40 +425,42 @@
     "JobProgressTypeDef",
     {
         "PercentComplete": int,
     },
     total=False,
 )
 
-InputDataConfigTypeDef = TypedDict(
-    "InputDataConfigTypeDef",
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
     },
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
+class OutputDataConfigOutputTypeDef(
+    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
+):
     pass
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
+RegistrationConfigOutputTypeDef = TypedDict(
+    "RegistrationConfigOutputTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": List[str],
     },
     total=False,
 )
@@ -442,56 +472,40 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+InputDataConfigTypeDef = TypedDict(
+    "InputDataConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "S3Uri": str,
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "DomainId": str,
-        },
-    )
-)
-_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "JobStatus": FraudsterRegistrationJobStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
-    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudsterRegistrationJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
@@ -506,35 +520,14 @@
 
 class ListFraudsterRegistrationJobsRequestRequestTypeDef(
     _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef,
     _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "WatchlistId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFraudstersRequestListFraudstersPaginateTypeDef(
-    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
-    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
-):
-    pass
-
 _RequiredListFraudstersRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudstersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudstersRequestRequestTypeDef = TypedDict(
@@ -548,35 +541,14 @@
 )
 
 class ListFraudstersRequestRequestTypeDef(
     _RequiredListFraudstersRequestRequestTypeDef, _OptionalListFraudstersRequestRequestTypeDef
 ):
     pass
 
-_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "JobStatus": SpeakerEnrollmentJobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
-    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
@@ -591,34 +563,14 @@
 
 class ListSpeakerEnrollmentJobsRequestRequestTypeDef(
     _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef,
     _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSpeakersRequestListSpeakersPaginateTypeDef(
-    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
-    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
-):
-    pass
-
 _RequiredListSpeakersRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakersRequestRequestTypeDef = TypedDict(
@@ -652,34 +604,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
-    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
-    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
-):
-    pass
-
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -714,33 +654,39 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "S3Uri": str,
+    },
+)
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
+    {
+        "KmsKeyId": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+    pass
+
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DuplicateRegistrationAction": DuplicateRegistrationActionType,
+        "FraudsterSimilarityThreshold": int,
+        "WatchlistIds": Sequence[str],
     },
+    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -768,31 +714,38 @@
 ):
     pass
 
 AssociateFraudsterResponseTypeDef = TypedDict(
     "AssociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterResponseTypeDef = TypedDict(
     "DescribeFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFraudsterResponseTypeDef = TypedDict(
     "DisassociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
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
 
 AuthenticationResultTypeDef = TypedDict(
     "AuthenticationResultTypeDef",
     {
         "AudioAggregationEndedAt": datetime,
@@ -846,80 +799,72 @@
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
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
 
 CreateWatchlistResponseTypeDef = TypedDict(
     "CreateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWatchlistResponseTypeDef = TypedDict(
     "DescribeWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWatchlistResponseTypeDef = TypedDict(
     "UpdateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerResponseTypeDef = TypedDict(
     "DescribeSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OptOutSpeakerResponseTypeDef = TypedDict(
     "OptOutSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
@@ -928,22 +873,31 @@
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigOutputTypeDef = TypedDict(
+    "EnrollmentConfigOutputTypeDef",
+    {
+        "ExistingEnrollmentAction": ExistingEnrollmentActionType,
+        "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 EnrollmentConfigTypeDef = TypedDict(
     "EnrollmentConfigTypeDef",
     {
         "ExistingEnrollmentAction": ExistingEnrollmentActionType,
         "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigTypeDef,
     },
     total=False,
@@ -991,125 +945,248 @@
     "FraudsterRegistrationJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "RegistrationConfig": RegistrationConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+ListFraudstersResponseTypeDef = TypedDict(
+    "ListFraudstersResponseTypeDef",
+    {
+        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "DomainId": str,
+        },
+    )
+)
+_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "JobStatus": FraudsterRegistrationJobStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
+    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "DataAccessRoleArn": str,
         "DomainId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
     },
 )
-_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "ClientToken": str,
-        "JobName": str,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "WatchlistId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class StartFraudsterRegistrationJobRequestRequestTypeDef(
-    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
-    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+class ListFraudstersRequestListFraudstersPaginateTypeDef(
+    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
+    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
 ):
     pass
 
-ListFraudstersResponseTypeDef = TypedDict(
-    "ListFraudstersResponseTypeDef",
+_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     {
-        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "JobStatus": SpeakerEnrollmentJobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
+    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSpeakersRequestListSpeakersPaginateTypeDef(
+    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
+    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
+):
+    pass
+
+_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
+    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
+):
+    pass
+
 ListSpeakersResponseTypeDef = TypedDict(
     "ListSpeakersResponseTypeDef",
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "DataAccessRoleArn": str,
+        "DomainId": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+    },
+)
+_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "JobName": str,
+        "RegistrationConfig": RegistrationConfigTypeDef,
+    },
+    total=False,
+)
+
+class StartFraudsterRegistrationJobRequestRequestTypeDef(
+    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
+    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+):
+    pass
+
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
-        "EnrollmentConfig": EnrollmentConfigTypeDef,
+        "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
@@ -1150,64 +1227,64 @@
 )
 
 ListFraudsterRegistrationJobsResponseTypeDef = TypedDict(
     "ListFraudsterRegistrationJobsResponseTypeDef",
     {
         "JobSummaries": List[FraudsterRegistrationJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeakerEnrollmentJobsResponseTypeDef = TypedDict(
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     {
         "JobSummaries": List[SpeakerEnrollmentJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "StartFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "StartSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateSessionResponseTypeDef = TypedDict(
     "EvaluateSessionResponseTypeDef",
     {
         "AuthenticationResult": AuthenticationResultTypeDef,
         "DomainId": str,
         "FraudDetectionResult": FraudDetectionResultTypeDef,
         "SessionId": str,
         "SessionName": str,
         "StreamingStatus": StreamingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/PKG-INFO` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.0
-Summary: Type annotations for boto3.VoiceID 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.VoiceID 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-voice-id"></a>
 
 # mypy-boto3-voice-id
 
 [![PyPI - mypy-boto3-voice-id](https://img.shields.io/pypi/v/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,14 +353,15 @@
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -370,72 +371,78 @@
     DescribeFraudsterRegistrationJobRequestRequestTypeDef,
     DescribeFraudsterRequestRequestTypeDef,
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    InputDataConfigOutputTypeDef,
+    OutputDataConfigOutputTypeDef,
+    RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    InputDataConfigTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    TagOutputTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    OutputDataConfigTypeDef,
+    RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
     DomainTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
-    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/SOURCES.txt` & `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.0/setup.py` & `mypy-boto3-voice-id-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-voice-id",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VoiceID 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.VoiceID 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

