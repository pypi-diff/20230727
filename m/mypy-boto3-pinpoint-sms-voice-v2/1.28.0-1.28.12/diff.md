# Comparing `tmp/mypy-boto3-pinpoint-sms-voice-v2-1.28.0.tar.gz` & `tmp/mypy-boto3-pinpoint-sms-voice-v2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-sms-voice-v2-1.28.0.tar", last modified: Thu Jul  6 21:00:19 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-sms-voice-v2-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0.tar` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.818395 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20896 2023-07-06 21:00:19.814395 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19358 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.802395 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39760 2023-07-06 20:49:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39699 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-07-06 20:49:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-06 20:49:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-06 20:49:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-06 20:49:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46929 2023-07-06 20:49:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46882 2023-07-06 20:49:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.814395 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20896 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:19.818395 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-06 20:49:35.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39760 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39699 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-27 11:41:38.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-27 11:41:38.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47600 2023-07-27 11:41:39.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-07-27 11:41:38.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/setup.py
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/LICENSE` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/PKG-INFO` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.28.0
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-sms-voice-v2?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-sms-voice-v2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,104 +394,107 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
-    AssociateOriginationIdentityResultTypeDef,
+    ResponseMetadataTypeDef,
+    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
-    DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
-    DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
-    DeleteKeywordResultTypeDef,
     DeleteOptOutListRequestRequestTypeDef,
-    DeleteOptOutListResultTypeDef,
     DeleteOptedOutNumberRequestRequestTypeDef,
-    DeleteOptedOutNumberResultTypeDef,
     DeletePoolRequestRequestTypeDef,
-    DeletePoolResultTypeDef,
-    DeleteTextMessageSpendLimitOverrideResultTypeDef,
-    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
-    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountAttributesRequestRequestTypeDef,
-    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsRequestRequestTypeDef,
     KeywordFilterTypeDef,
     KeywordInformationTypeDef,
-    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeOptOutListsRequestRequestTypeDef,
     OptOutListInformationTypeDef,
     OptedOutFilterTypeDef,
     OptedOutNumberInformationTypeDef,
     PhoneNumberFilterTypeDef,
     PhoneNumberInformationTypeDef,
     PoolFilterTypeDef,
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
-    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
-    DisassociateOriginationIdentityResultTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutKeywordRequestRequestTypeDef,
-    PutKeywordResultTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
-    PutOptedOutNumberResultTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
-    ReleasePhoneNumberResultTypeDef,
-    ResponseMetadataTypeDef,
     SendTextMessageRequestRequestTypeDef,
-    SendTextMessageResultTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
-    SendVoiceMessageResultTypeDef,
     SetDefaultMessageTypeRequestRequestTypeDef,
-    SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdRequestRequestTypeDef,
-    SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideRequestRequestTypeDef,
-    SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef,
-    SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResultTypeDef,
     UpdatePoolRequestRequestTypeDef,
-    UpdatePoolResultTypeDef,
+    AssociateOriginationIdentityResultTypeDef,
+    DeleteDefaultMessageTypeResultTypeDef,
+    DeleteDefaultSenderIdResultTypeDef,
+    DeleteKeywordResultTypeDef,
+    DeleteOptOutListResultTypeDef,
+    DeleteOptedOutNumberResultTypeDef,
+    DeletePoolResultTypeDef,
+    DeleteTextMessageSpendLimitOverrideResultTypeDef,
+    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
-    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
+    DisassociateOriginationIdentityResultTypeDef,
+    PutKeywordResultTypeDef,
+    PutOptedOutNumberResultTypeDef,
+    ReleasePhoneNumberResultTypeDef,
+    SendTextMessageResultTypeDef,
+    SendVoiceMessageResultTypeDef,
+    SetDefaultMessageTypeResultTypeDef,
+    SetDefaultSenderIdResultTypeDef,
+    SetTextMessageSpendLimitOverrideResultTypeDef,
+    SetVoiceMessageSpendLimitOverrideResultTypeDef,
+    UpdatePhoneNumberResultTypeDef,
+    UpdatePoolResultTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateConfigurationSetResultTypeDef,
     CreateOptOutListRequestRequestTypeDef,
-    CreateOptOutListResultTypeDef,
     CreatePoolRequestRequestTypeDef,
+    RequestPhoneNumberRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateConfigurationSetResultTypeDef,
+    CreateOptOutListResultTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
-    EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
+    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
+    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
+    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
+    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
+    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     DescribeKeywordsRequestRequestTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     DescribeOptedOutNumbersRequestRequestTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
@@ -501,14 +504,15 @@
     DescribePoolsRequestDescribePoolsPaginateTypeDef,
     DescribePoolsRequestRequestTypeDef,
     DescribePoolsResultTypeDef,
     DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef,
     DescribeSenderIdsRequestRequestTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
+    EventDestinationTypeDef,
     ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
     ListPoolOriginationIdentitiesRequestRequestTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ConfigurationSetInformationTypeDef,
     CreateEventDestinationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteEventDestinationResultTypeDef,
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/README.md` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-sms-voice-v2?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-sms-voice-v2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,104 +362,107 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
-    AssociateOriginationIdentityResultTypeDef,
+    ResponseMetadataTypeDef,
+    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
-    DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
-    DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
-    DeleteKeywordResultTypeDef,
     DeleteOptOutListRequestRequestTypeDef,
-    DeleteOptOutListResultTypeDef,
     DeleteOptedOutNumberRequestRequestTypeDef,
-    DeleteOptedOutNumberResultTypeDef,
     DeletePoolRequestRequestTypeDef,
-    DeletePoolResultTypeDef,
-    DeleteTextMessageSpendLimitOverrideResultTypeDef,
-    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
-    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountAttributesRequestRequestTypeDef,
-    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsRequestRequestTypeDef,
     KeywordFilterTypeDef,
     KeywordInformationTypeDef,
-    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeOptOutListsRequestRequestTypeDef,
     OptOutListInformationTypeDef,
     OptedOutFilterTypeDef,
     OptedOutNumberInformationTypeDef,
     PhoneNumberFilterTypeDef,
     PhoneNumberInformationTypeDef,
     PoolFilterTypeDef,
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
-    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
-    DisassociateOriginationIdentityResultTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutKeywordRequestRequestTypeDef,
-    PutKeywordResultTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
-    PutOptedOutNumberResultTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
-    ReleasePhoneNumberResultTypeDef,
-    ResponseMetadataTypeDef,
     SendTextMessageRequestRequestTypeDef,
-    SendTextMessageResultTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
-    SendVoiceMessageResultTypeDef,
     SetDefaultMessageTypeRequestRequestTypeDef,
-    SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdRequestRequestTypeDef,
-    SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideRequestRequestTypeDef,
-    SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef,
-    SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResultTypeDef,
     UpdatePoolRequestRequestTypeDef,
-    UpdatePoolResultTypeDef,
+    AssociateOriginationIdentityResultTypeDef,
+    DeleteDefaultMessageTypeResultTypeDef,
+    DeleteDefaultSenderIdResultTypeDef,
+    DeleteKeywordResultTypeDef,
+    DeleteOptOutListResultTypeDef,
+    DeleteOptedOutNumberResultTypeDef,
+    DeletePoolResultTypeDef,
+    DeleteTextMessageSpendLimitOverrideResultTypeDef,
+    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
-    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
+    DisassociateOriginationIdentityResultTypeDef,
+    PutKeywordResultTypeDef,
+    PutOptedOutNumberResultTypeDef,
+    ReleasePhoneNumberResultTypeDef,
+    SendTextMessageResultTypeDef,
+    SendVoiceMessageResultTypeDef,
+    SetDefaultMessageTypeResultTypeDef,
+    SetDefaultSenderIdResultTypeDef,
+    SetTextMessageSpendLimitOverrideResultTypeDef,
+    SetVoiceMessageSpendLimitOverrideResultTypeDef,
+    UpdatePhoneNumberResultTypeDef,
+    UpdatePoolResultTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateConfigurationSetResultTypeDef,
     CreateOptOutListRequestRequestTypeDef,
-    CreateOptOutListResultTypeDef,
     CreatePoolRequestRequestTypeDef,
+    RequestPhoneNumberRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateConfigurationSetResultTypeDef,
+    CreateOptOutListResultTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
-    EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
+    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
+    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
+    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
+    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
+    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     DescribeKeywordsRequestRequestTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     DescribeOptedOutNumbersRequestRequestTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
@@ -469,14 +472,15 @@
     DescribePoolsRequestDescribePoolsPaginateTypeDef,
     DescribePoolsRequestRequestTypeDef,
     DescribePoolsResultTypeDef,
     DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef,
     DescribeSenderIdsRequestRequestTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
+    EventDestinationTypeDef,
     ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
     ListPoolOriginationIdentitiesRequestRequestTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ConfigurationSetInformationTypeDef,
     CreateEventDestinationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteEventDestinationResultTypeDef,
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/__main__.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2\nOther"
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/client.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/client.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/literals.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,14 +316,15 @@
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
@@ -402,26 +403,28 @@
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,15 @@
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
@@ -400,26 +401,28 @@
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,30 +94,30 @@
 class DescribeAccountAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountAttributesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
         """
 
 
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
         """
 
 
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
 
@@ -148,15 +148,15 @@
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
 
@@ -166,15 +166,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
 
@@ -186,15 +186,15 @@
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
 
@@ -205,15 +205,15 @@
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
 
@@ -224,15 +224,15 @@
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
 
@@ -243,30 +243,30 @@
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
 
 class DescribeSpendLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSpendLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
         """
 
 
@@ -277,13 +277,13 @@
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,29 +91,29 @@
 class DescribeAccountAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountAttributesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
         """
 
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeConfigurationSetsPaginator(Paginator):
@@ -123,15 +123,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
 class DescribeKeywordsPaginator(Paginator):
@@ -142,15 +142,15 @@
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
 class DescribeOptOutListsPaginator(Paginator):
@@ -159,15 +159,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
 class DescribeOptedOutNumbersPaginator(Paginator):
@@ -178,15 +178,15 @@
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
 class DescribePhoneNumbersPaginator(Paginator):
@@ -196,15 +196,15 @@
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
 class DescribePoolsPaginator(Paginator):
@@ -214,15 +214,15 @@
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
 class DescribeSenderIdsPaginator(Paginator):
@@ -232,29 +232,29 @@
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
 class DescribeSpendLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSpendLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
         """
 
 class ListPoolOriginationIdentitiesPaginator(Paginator):
@@ -264,13 +264,13 @@
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,104 +46,107 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
-    "AssociateOriginationIdentityResultTypeDef",
+    "ResponseMetadataTypeDef",
+    "CloudWatchLogsDestinationOutputTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
-    "DeleteDefaultMessageTypeResultTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
-    "DeleteDefaultSenderIdResultTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
-    "DeleteKeywordResultTypeDef",
     "DeleteOptOutListRequestRequestTypeDef",
-    "DeleteOptOutListResultTypeDef",
     "DeleteOptedOutNumberRequestRequestTypeDef",
-    "DeleteOptedOutNumberResultTypeDef",
     "DeletePoolRequestRequestTypeDef",
-    "DeletePoolResultTypeDef",
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountAttributesRequestRequestTypeDef",
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsRequestRequestTypeDef",
     "KeywordFilterTypeDef",
     "KeywordInformationTypeDef",
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
     "DescribeOptOutListsRequestRequestTypeDef",
     "OptOutListInformationTypeDef",
     "OptedOutFilterTypeDef",
     "OptedOutNumberInformationTypeDef",
     "PhoneNumberFilterTypeDef",
     "PhoneNumberInformationTypeDef",
     "PoolFilterTypeDef",
     "PoolInformationTypeDef",
     "SenderIdAndCountryTypeDef",
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
-    "DisassociateOriginationIdentityResultTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutKeywordRequestRequestTypeDef",
-    "PutKeywordResultTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
-    "PutOptedOutNumberResultTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
-    "ReleasePhoneNumberResultTypeDef",
-    "ResponseMetadataTypeDef",
     "SendTextMessageRequestRequestTypeDef",
-    "SendTextMessageResultTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
-    "SendVoiceMessageResultTypeDef",
     "SetDefaultMessageTypeRequestRequestTypeDef",
-    "SetDefaultMessageTypeResultTypeDef",
     "SetDefaultSenderIdRequestRequestTypeDef",
-    "SetDefaultSenderIdResultTypeDef",
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
-    "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolRequestRequestTypeDef",
-    "UpdatePoolResultTypeDef",
+    "AssociateOriginationIdentityResultTypeDef",
+    "DeleteDefaultMessageTypeResultTypeDef",
+    "DeleteDefaultSenderIdResultTypeDef",
+    "DeleteKeywordResultTypeDef",
+    "DeleteOptOutListResultTypeDef",
+    "DeleteOptedOutNumberResultTypeDef",
+    "DeletePoolResultTypeDef",
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "DescribeAccountLimitsResultTypeDef",
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+    "DisassociateOriginationIdentityResultTypeDef",
+    "PutKeywordResultTypeDef",
+    "PutOptedOutNumberResultTypeDef",
+    "ReleasePhoneNumberResultTypeDef",
+    "SendTextMessageResultTypeDef",
+    "SendVoiceMessageResultTypeDef",
+    "SetDefaultMessageTypeResultTypeDef",
+    "SetDefaultSenderIdResultTypeDef",
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
+    "UpdatePhoneNumberResultTypeDef",
+    "UpdatePoolResultTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "CreateConfigurationSetResultTypeDef",
     "CreateOptOutListRequestRequestTypeDef",
-    "CreateOptOutListResultTypeDef",
     "CreatePoolRequestRequestTypeDef",
+    "RequestPhoneNumberRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateConfigurationSetResultTypeDef",
+    "CreateOptOutListResultTypeDef",
     "CreatePoolResultTypeDef",
     "ListTagsForResourceResultTypeDef",
-    "RequestPhoneNumberRequestRequestTypeDef",
     "RequestPhoneNumberResultTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateEventDestinationRequestRequestTypeDef",
-    "EventDestinationTypeDef",
     "UpdateEventDestinationRequestRequestTypeDef",
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     "DescribeKeywordsRequestRequestTypeDef",
     "DescribeKeywordsResultTypeDef",
     "DescribeOptOutListsResultTypeDef",
     "DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     "DescribeOptedOutNumbersRequestRequestTypeDef",
     "DescribeOptedOutNumbersResultTypeDef",
@@ -153,14 +156,15 @@
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     "DescribePoolsRequestRequestTypeDef",
     "DescribePoolsResultTypeDef",
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     "DescribeSenderIdsRequestRequestTypeDef",
     "DescribeSenderIdsResultTypeDef",
     "DescribeSpendLimitsResultTypeDef",
+    "EventDestinationTypeDef",
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     "ListPoolOriginationIdentitiesRequestRequestTypeDef",
     "ListPoolOriginationIdentitiesResultTypeDef",
     "ConfigurationSetInformationTypeDef",
     "CreateEventDestinationResultTypeDef",
     "DeleteConfigurationSetResultTypeDef",
     "DeleteEventDestinationResultTypeDef",
@@ -205,23 +209,30 @@
 class AssociateOriginationIdentityRequestRequestTypeDef(
     _RequiredAssociateOriginationIdentityRequestRequestTypeDef,
     _OptionalAssociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateOriginationIdentityResultTypeDef = TypedDict(
-    "AssociateOriginationIdentityResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+CloudWatchLogsDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationOutputTypeDef",
+    {
+        "IamRoleArn": str,
+        "LogGroupArn": str,
     },
 )
 
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
@@ -241,14 +252,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IamRoleArn": str,
         "DeliveryStreamArn": str,
     },
 )
@@ -270,41 +289,21 @@
 DeleteDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-DeleteDefaultMessageTypeResultTypeDef = TypedDict(
-    "DeleteDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-DeleteDefaultSenderIdResultTypeDef = TypedDict(
-    "DeleteDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -313,128 +312,55 @@
     "DeleteKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
     },
 )
 
-DeleteKeywordResultTypeDef = TypedDict(
-    "DeleteKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOptOutListRequestRequestTypeDef = TypedDict(
     "DeleteOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 
-DeleteOptOutListResultTypeDef = TypedDict(
-    "DeleteOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOptedOutNumberRequestRequestTypeDef = TypedDict(
     "DeleteOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
-DeleteOptedOutNumberResultTypeDef = TypedDict(
-    "DeleteOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePoolRequestRequestTypeDef = TypedDict(
     "DeletePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 
-DeletePoolResultTypeDef = TypedDict(
-    "DeletePoolResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
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
 
 DescribeAccountAttributesRequestRequestTypeDef = TypedDict(
     "DescribeAccountAttributesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAccountLimitsRequestRequestTypeDef = TypedDict(
     "DescribeAccountLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -453,23 +379,14 @@
     {
         "Keyword": str,
         "KeywordMessage": str,
         "KeywordAction": KeywordActionType,
     },
 )
 
-DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
-    {
-        "OptOutListNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOptOutListsRequestRequestTypeDef = TypedDict(
     "DescribeOptOutListsRequestRequestTypeDef",
     {
         "OptOutListNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -604,22 +521,14 @@
         "SenderId": str,
         "IsoCountryCode": str,
         "MessageTypes": List[MessageTypeType],
         "MonthlyLeasingPrice": str,
     },
 )
 
-DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSpendLimitsRequestRequestTypeDef = TypedDict(
     "DescribeSpendLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -655,23 +564,26 @@
 class DisassociateOriginationIdentityRequestRequestTypeDef(
     _RequiredDisassociateOriginationIdentityRequestRequestTypeDef,
     _OptionalDisassociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
 
-DisassociateOriginationIdentityResultTypeDef = TypedDict(
-    "DisassociateOriginationIdentityResultTypeDef",
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
     {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IamRoleArn": str,
+        "DeliveryStreamArn": str,
+    },
+)
+
+SnsDestinationOutputTypeDef = TypedDict(
+    "SnsDestinationOutputTypeDef",
+    {
+        "TopicArn": str,
     },
 )
 
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
@@ -692,24 +604,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
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
 _RequiredPutKeywordRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
     },
@@ -725,85 +627,29 @@
 
 class PutKeywordRequestRequestTypeDef(
     _RequiredPutKeywordRequestRequestTypeDef, _OptionalPutKeywordRequestRequestTypeDef
 ):
     pass
 
 
-PutKeywordResultTypeDef = TypedDict(
-    "PutKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutOptedOutNumberRequestRequestTypeDef = TypedDict(
     "PutOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
-PutOptedOutNumberResultTypeDef = TypedDict(
-    "PutOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReleasePhoneNumberRequestRequestTypeDef = TypedDict(
     "ReleasePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-ReleasePhoneNumberResultTypeDef = TypedDict(
-    "ReleasePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
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
 _RequiredSendTextMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendTextMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
     },
 )
 _OptionalSendTextMessageRequestRequestTypeDef = TypedDict(
@@ -826,22 +672,14 @@
 
 class SendTextMessageRequestRequestTypeDef(
     _RequiredSendTextMessageRequestRequestTypeDef, _OptionalSendTextMessageRequestRequestTypeDef
 ):
     pass
 
 
-SendTextMessageResultTypeDef = TypedDict(
-    "SendTextMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendVoiceMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendVoiceMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": str,
     },
 )
@@ -863,88 +701,44 @@
 
 class SendVoiceMessageRequestRequestTypeDef(
     _RequiredSendVoiceMessageRequestRequestTypeDef, _OptionalSendVoiceMessageRequestRequestTypeDef
 ):
     pass
 
 
-SendVoiceMessageResultTypeDef = TypedDict(
-    "SendVoiceMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "SetDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
     },
 )
 
-SetDefaultMessageTypeResultTypeDef = TypedDict(
-    "SetDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "SetDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "SenderId": str,
     },
 )
 
-SetDefaultSenderIdResultTypeDef = TypedDict(
-    "SetDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetTextMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
-SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
-SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -970,36 +764,14 @@
 
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
 
-UpdatePhoneNumberResultTypeDef = TypedDict(
-    "UpdatePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "DeletionProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 _OptionalUpdatePoolRequestRequestTypeDef = TypedDict(
@@ -1018,58 +790,278 @@
 
 class UpdatePoolRequestRequestTypeDef(
     _RequiredUpdatePoolRequestRequestTypeDef, _OptionalUpdatePoolRequestRequestTypeDef
 ):
     pass
 
 
-UpdatePoolResultTypeDef = TypedDict(
-    "UpdatePoolResultTypeDef",
+AssociateOriginationIdentityResultTypeDef = TypedDict(
+    "AssociateOriginationIdentityResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDefaultMessageTypeResultTypeDef = TypedDict(
+    "DeleteDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDefaultSenderIdResultTypeDef = TypedDict(
+    "DeleteDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteKeywordResultTypeDef = TypedDict(
+    "DeleteKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOptOutListResultTypeDef = TypedDict(
+    "DeleteOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOptedOutNumberResultTypeDef = TypedDict(
+    "DeleteOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePoolResultTypeDef = TypedDict(
+    "DeletePoolResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "Status": PoolStatusType,
         "MessageType": MessageTypeType,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountLimitsResultTypeDef = TypedDict(
     "DescribeAccountLimitsResultTypeDef",
     {
         "AccountLimits": List[AccountLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+DisassociateOriginationIdentityResultTypeDef = TypedDict(
+    "DisassociateOriginationIdentityResultTypeDef",
     {
-        "ConfigurationSetNames": Sequence[str],
-        "Filters": Sequence[ConfigurationSetFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutKeywordResultTypeDef = TypedDict(
+    "PutKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutOptedOutNumberResultTypeDef = TypedDict(
+    "PutOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReleasePhoneNumberResultTypeDef = TypedDict(
+    "ReleasePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendTextMessageResultTypeDef = TypedDict(
+    "SendTextMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendVoiceMessageResultTypeDef = TypedDict(
+    "SendVoiceMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultMessageTypeResultTypeDef = TypedDict(
+    "SetDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultSenderIdResultTypeDef = TypedDict(
+    "SetDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePhoneNumberResultTypeDef = TypedDict(
+    "UpdatePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "DeletionProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePoolResultTypeDef = TypedDict(
+    "UpdatePoolResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeConfigurationSetsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationSetsRequestRequestTypeDef",
     {
         "ConfigurationSetNames": Sequence[str],
         "Filters": Sequence[ConfigurationSetFilterTypeDef],
@@ -1098,25 +1090,14 @@
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
 
-CreateConfigurationSetResultTypeDef = TypedDict(
-    "CreateConfigurationSetResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "Tags": List[TagTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateOptOutListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalCreateOptOutListRequestRequestTypeDef = TypedDict(
@@ -1131,25 +1112,14 @@
 
 class CreateOptOutListRequestRequestTypeDef(
     _RequiredCreateOptOutListRequestRequestTypeDef, _OptionalCreateOptOutListRequestRequestTypeDef
 ):
     pass
 
 
-CreateOptOutListResultTypeDef = TypedDict(
-    "CreateOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "Tags": List[TagTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePoolRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
     },
@@ -1167,42 +1137,14 @@
 
 class CreatePoolRequestRequestTypeDef(
     _RequiredCreatePoolRequestRequestTypeDef, _OptionalCreatePoolRequestRequestTypeDef
 ):
     pass
 
 
-CreatePoolResultTypeDef = TypedDict(
-    "CreatePoolResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
-        "Tags": List[TagTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRequestPhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredRequestPhoneNumberRequestRequestTypeDef",
     {
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
         "NumberCapabilities": Sequence[NumberCapabilityType],
         "NumberType": RequestableNumberTypeType,
@@ -1225,14 +1167,72 @@
 class RequestPhoneNumberRequestRequestTypeDef(
     _RequiredRequestPhoneNumberRequestRequestTypeDef,
     _OptionalRequestPhoneNumberRequestRequestTypeDef,
 ):
     pass
 
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateConfigurationSetResultTypeDef = TypedDict(
+    "CreateConfigurationSetResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "Tags": List[TagOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOptOutListResultTypeDef = TypedDict(
+    "CreateOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "Tags": List[TagOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePoolResultTypeDef = TypedDict(
+    "CreatePoolResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
+        "Tags": List[TagOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RequestPhoneNumberResultTypeDef = TypedDict(
     "RequestPhoneNumberResultTypeDef",
     {
         "PhoneNumberArn": str,
         "PhoneNumberId": str,
         "PhoneNumber": str,
         "Status": NumberStatusType,
@@ -1243,25 +1243,17 @@
         "MonthlyLeasingPrice": str,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "DeletionProtectionEnabled": bool,
         "PoolId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -1284,37 +1276,14 @@
 class CreateEventDestinationRequestRequestTypeDef(
     _RequiredCreateEventDestinationRequestRequestTypeDef,
     _OptionalCreateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredEventDestinationTypeDef = TypedDict(
-    "_RequiredEventDestinationTypeDef",
-    {
-        "EventDestinationName": str,
-        "Enabled": bool,
-        "MatchingEventTypes": List[EventTypeType],
-    },
-)
-_OptionalEventDestinationTypeDef = TypedDict(
-    "_OptionalEventDestinationTypeDef",
-    {
-        "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-    },
-    total=False,
-)
-
-
-class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
-    pass
-
-
 _RequiredUpdateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -1334,26 +1303,69 @@
 class UpdateEventDestinationRequestRequestTypeDef(
     _RequiredUpdateEventDestinationRequestRequestTypeDef,
     _OptionalUpdateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+    {
+        "ConfigurationSetNames": Sequence[str],
+        "Filters": Sequence[ConfigurationSetFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
+    {
+        "OptOutListNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "OriginationIdentity": str,
     },
 )
 _OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "Keywords": Sequence[str],
         "Filters": Sequence[KeywordFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef(
     _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
@@ -1389,39 +1401,39 @@
 DescribeKeywordsResultTypeDef = TypedDict(
     "DescribeKeywordsResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keywords": List[KeywordInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOptOutListsResultTypeDef = TypedDict(
     "DescribeOptOutListsResultTypeDef",
     {
         "OptOutLists": List[OptOutListInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptedOutNumbers": Sequence[str],
         "Filters": Sequence[OptedOutFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef(
     _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
@@ -1458,24 +1470,24 @@
 DescribeOptedOutNumbersResultTypeDef = TypedDict(
     "DescribeOptedOutNumbersResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "OptedOutNumbers": List[OptedOutNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef = TypedDict(
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
         "Filters": Sequence[PhoneNumberFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePhoneNumbersRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumbersRequestRequestTypeDef",
     {
@@ -1488,24 +1500,24 @@
 )
 
 DescribePhoneNumbersResultTypeDef = TypedDict(
     "DescribePhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePoolsRequestDescribePoolsPaginateTypeDef = TypedDict(
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     {
         "PoolIds": Sequence[str],
         "Filters": Sequence[PoolFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePoolsRequestRequestTypeDef = TypedDict(
     "DescribePoolsRequestRequestTypeDef",
     {
@@ -1518,24 +1530,24 @@
 )
 
 DescribePoolsResultTypeDef = TypedDict(
     "DescribePoolsResultTypeDef",
     {
         "Pools": List[PoolInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef = TypedDict(
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     {
         "SenderIds": Sequence[SenderIdAndCountryTypeDef],
         "Filters": Sequence[SenderIdFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSenderIdsRequestRequestTypeDef = TypedDict(
     "DescribeSenderIdsRequestRequestTypeDef",
     {
@@ -1548,41 +1560,64 @@
 )
 
 DescribeSenderIdsResultTypeDef = TypedDict(
     "DescribeSenderIdsResultTypeDef",
     {
         "SenderIds": List[SenderIdInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpendLimitsResultTypeDef = TypedDict(
     "DescribeSpendLimitsResultTypeDef",
     {
         "SpendLimits": List[SpendLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredEventDestinationTypeDef = TypedDict(
+    "_RequiredEventDestinationTypeDef",
+    {
+        "EventDestinationName": str,
+        "Enabled": bool,
+        "MatchingEventTypes": List[EventTypeType],
     },
 )
+_OptionalEventDestinationTypeDef = TypedDict(
+    "_OptionalEventDestinationTypeDef",
+    {
+        "CloudWatchLogsDestination": CloudWatchLogsDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
+    pass
+
 
 _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "PoolId": str,
         },
     )
 )
 _OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "Filters": Sequence[PoolOriginationIdentitiesFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
+            "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
 
 class ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef(
@@ -1619,15 +1654,15 @@
 ListPoolOriginationIdentitiesResultTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentities": List[OriginationIdentityMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfigurationSetInformationTypeDef = TypedDict(
     "_RequiredConfigurationSetInformationTypeDef",
     {
         "ConfigurationSetArn": str,
@@ -1654,52 +1689,52 @@
 
 CreateEventDestinationResultTypeDef = TypedDict(
     "CreateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConfigurationSetResultTypeDef = TypedDict(
     "DeleteConfigurationSetResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestinations": List[EventDestinationTypeDef],
         "DefaultMessageType": MessageTypeType,
         "DefaultSenderId": str,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventDestinationResultTypeDef = TypedDict(
     "DeleteEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventDestinationResultTypeDef = TypedDict(
     "UpdateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationSetsResultTypeDef = TypedDict(
     "DescribeConfigurationSetsResultTypeDef",
     {
         "ConfigurationSets": List[ConfigurationSetInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -45,104 +45,107 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
-    "AssociateOriginationIdentityResultTypeDef",
+    "ResponseMetadataTypeDef",
+    "CloudWatchLogsDestinationOutputTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
-    "DeleteDefaultMessageTypeResultTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
-    "DeleteDefaultSenderIdResultTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
-    "DeleteKeywordResultTypeDef",
     "DeleteOptOutListRequestRequestTypeDef",
-    "DeleteOptOutListResultTypeDef",
     "DeleteOptedOutNumberRequestRequestTypeDef",
-    "DeleteOptedOutNumberResultTypeDef",
     "DeletePoolRequestRequestTypeDef",
-    "DeletePoolResultTypeDef",
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountAttributesRequestRequestTypeDef",
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsRequestRequestTypeDef",
     "KeywordFilterTypeDef",
     "KeywordInformationTypeDef",
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
     "DescribeOptOutListsRequestRequestTypeDef",
     "OptOutListInformationTypeDef",
     "OptedOutFilterTypeDef",
     "OptedOutNumberInformationTypeDef",
     "PhoneNumberFilterTypeDef",
     "PhoneNumberInformationTypeDef",
     "PoolFilterTypeDef",
     "PoolInformationTypeDef",
     "SenderIdAndCountryTypeDef",
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
-    "DisassociateOriginationIdentityResultTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutKeywordRequestRequestTypeDef",
-    "PutKeywordResultTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
-    "PutOptedOutNumberResultTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
-    "ReleasePhoneNumberResultTypeDef",
-    "ResponseMetadataTypeDef",
     "SendTextMessageRequestRequestTypeDef",
-    "SendTextMessageResultTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
-    "SendVoiceMessageResultTypeDef",
     "SetDefaultMessageTypeRequestRequestTypeDef",
-    "SetDefaultMessageTypeResultTypeDef",
     "SetDefaultSenderIdRequestRequestTypeDef",
-    "SetDefaultSenderIdResultTypeDef",
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
-    "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolRequestRequestTypeDef",
-    "UpdatePoolResultTypeDef",
+    "AssociateOriginationIdentityResultTypeDef",
+    "DeleteDefaultMessageTypeResultTypeDef",
+    "DeleteDefaultSenderIdResultTypeDef",
+    "DeleteKeywordResultTypeDef",
+    "DeleteOptOutListResultTypeDef",
+    "DeleteOptedOutNumberResultTypeDef",
+    "DeletePoolResultTypeDef",
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "DescribeAccountLimitsResultTypeDef",
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+    "DisassociateOriginationIdentityResultTypeDef",
+    "PutKeywordResultTypeDef",
+    "PutOptedOutNumberResultTypeDef",
+    "ReleasePhoneNumberResultTypeDef",
+    "SendTextMessageResultTypeDef",
+    "SendVoiceMessageResultTypeDef",
+    "SetDefaultMessageTypeResultTypeDef",
+    "SetDefaultSenderIdResultTypeDef",
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
+    "UpdatePhoneNumberResultTypeDef",
+    "UpdatePoolResultTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "CreateConfigurationSetResultTypeDef",
     "CreateOptOutListRequestRequestTypeDef",
-    "CreateOptOutListResultTypeDef",
     "CreatePoolRequestRequestTypeDef",
+    "RequestPhoneNumberRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateConfigurationSetResultTypeDef",
+    "CreateOptOutListResultTypeDef",
     "CreatePoolResultTypeDef",
     "ListTagsForResourceResultTypeDef",
-    "RequestPhoneNumberRequestRequestTypeDef",
     "RequestPhoneNumberResultTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateEventDestinationRequestRequestTypeDef",
-    "EventDestinationTypeDef",
     "UpdateEventDestinationRequestRequestTypeDef",
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     "DescribeKeywordsRequestRequestTypeDef",
     "DescribeKeywordsResultTypeDef",
     "DescribeOptOutListsResultTypeDef",
     "DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     "DescribeOptedOutNumbersRequestRequestTypeDef",
     "DescribeOptedOutNumbersResultTypeDef",
@@ -152,14 +155,15 @@
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     "DescribePoolsRequestRequestTypeDef",
     "DescribePoolsResultTypeDef",
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     "DescribeSenderIdsRequestRequestTypeDef",
     "DescribeSenderIdsResultTypeDef",
     "DescribeSpendLimitsResultTypeDef",
+    "EventDestinationTypeDef",
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     "ListPoolOriginationIdentitiesRequestRequestTypeDef",
     "ListPoolOriginationIdentitiesResultTypeDef",
     "ConfigurationSetInformationTypeDef",
     "CreateEventDestinationResultTypeDef",
     "DeleteConfigurationSetResultTypeDef",
     "DeleteEventDestinationResultTypeDef",
@@ -202,23 +206,30 @@
 
 class AssociateOriginationIdentityRequestRequestTypeDef(
     _RequiredAssociateOriginationIdentityRequestRequestTypeDef,
     _OptionalAssociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
-AssociateOriginationIdentityResultTypeDef = TypedDict(
-    "AssociateOriginationIdentityResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+CloudWatchLogsDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationOutputTypeDef",
+    {
+        "IamRoleArn": str,
+        "LogGroupArn": str,
     },
 )
 
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
@@ -238,14 +249,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IamRoleArn": str,
         "DeliveryStreamArn": str,
     },
 )
@@ -267,41 +286,21 @@
 DeleteDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-DeleteDefaultMessageTypeResultTypeDef = TypedDict(
-    "DeleteDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-DeleteDefaultSenderIdResultTypeDef = TypedDict(
-    "DeleteDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -310,128 +309,55 @@
     "DeleteKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
     },
 )
 
-DeleteKeywordResultTypeDef = TypedDict(
-    "DeleteKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOptOutListRequestRequestTypeDef = TypedDict(
     "DeleteOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 
-DeleteOptOutListResultTypeDef = TypedDict(
-    "DeleteOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOptedOutNumberRequestRequestTypeDef = TypedDict(
     "DeleteOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
-DeleteOptedOutNumberResultTypeDef = TypedDict(
-    "DeleteOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePoolRequestRequestTypeDef = TypedDict(
     "DeletePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 
-DeletePoolResultTypeDef = TypedDict(
-    "DeletePoolResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
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
 
 DescribeAccountAttributesRequestRequestTypeDef = TypedDict(
     "DescribeAccountAttributesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAccountLimitsRequestRequestTypeDef = TypedDict(
     "DescribeAccountLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -450,23 +376,14 @@
     {
         "Keyword": str,
         "KeywordMessage": str,
         "KeywordAction": KeywordActionType,
     },
 )
 
-DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
-    {
-        "OptOutListNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOptOutListsRequestRequestTypeDef = TypedDict(
     "DescribeOptOutListsRequestRequestTypeDef",
     {
         "OptOutListNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -597,22 +514,14 @@
         "SenderId": str,
         "IsoCountryCode": str,
         "MessageTypes": List[MessageTypeType],
         "MonthlyLeasingPrice": str,
     },
 )
 
-DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSpendLimitsRequestRequestTypeDef = TypedDict(
     "DescribeSpendLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -646,23 +555,26 @@
 
 class DisassociateOriginationIdentityRequestRequestTypeDef(
     _RequiredDisassociateOriginationIdentityRequestRequestTypeDef,
     _OptionalDisassociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
-DisassociateOriginationIdentityResultTypeDef = TypedDict(
-    "DisassociateOriginationIdentityResultTypeDef",
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
     {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IamRoleArn": str,
+        "DeliveryStreamArn": str,
+    },
+)
+
+SnsDestinationOutputTypeDef = TypedDict(
+    "SnsDestinationOutputTypeDef",
+    {
+        "TopicArn": str,
     },
 )
 
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
@@ -683,24 +595,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
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
 _RequiredPutKeywordRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
     },
@@ -714,85 +616,29 @@
 )
 
 class PutKeywordRequestRequestTypeDef(
     _RequiredPutKeywordRequestRequestTypeDef, _OptionalPutKeywordRequestRequestTypeDef
 ):
     pass
 
-PutKeywordResultTypeDef = TypedDict(
-    "PutKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutOptedOutNumberRequestRequestTypeDef = TypedDict(
     "PutOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
-PutOptedOutNumberResultTypeDef = TypedDict(
-    "PutOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReleasePhoneNumberRequestRequestTypeDef = TypedDict(
     "ReleasePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-ReleasePhoneNumberResultTypeDef = TypedDict(
-    "ReleasePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
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
 _RequiredSendTextMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendTextMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
     },
 )
 _OptionalSendTextMessageRequestRequestTypeDef = TypedDict(
@@ -813,22 +659,14 @@
 )
 
 class SendTextMessageRequestRequestTypeDef(
     _RequiredSendTextMessageRequestRequestTypeDef, _OptionalSendTextMessageRequestRequestTypeDef
 ):
     pass
 
-SendTextMessageResultTypeDef = TypedDict(
-    "SendTextMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendVoiceMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendVoiceMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": str,
     },
 )
@@ -848,88 +686,44 @@
 )
 
 class SendVoiceMessageRequestRequestTypeDef(
     _RequiredSendVoiceMessageRequestRequestTypeDef, _OptionalSendVoiceMessageRequestRequestTypeDef
 ):
     pass
 
-SendVoiceMessageResultTypeDef = TypedDict(
-    "SendVoiceMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "SetDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
     },
 )
 
-SetDefaultMessageTypeResultTypeDef = TypedDict(
-    "SetDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "SetDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "SenderId": str,
     },
 )
 
-SetDefaultSenderIdResultTypeDef = TypedDict(
-    "SetDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetTextMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
-SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
-SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -953,36 +747,14 @@
 )
 
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
-UpdatePhoneNumberResultTypeDef = TypedDict(
-    "UpdatePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "DeletionProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 _OptionalUpdatePoolRequestRequestTypeDef = TypedDict(
@@ -999,58 +771,278 @@
 )
 
 class UpdatePoolRequestRequestTypeDef(
     _RequiredUpdatePoolRequestRequestTypeDef, _OptionalUpdatePoolRequestRequestTypeDef
 ):
     pass
 
-UpdatePoolResultTypeDef = TypedDict(
-    "UpdatePoolResultTypeDef",
+AssociateOriginationIdentityResultTypeDef = TypedDict(
+    "AssociateOriginationIdentityResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDefaultMessageTypeResultTypeDef = TypedDict(
+    "DeleteDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDefaultSenderIdResultTypeDef = TypedDict(
+    "DeleteDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteKeywordResultTypeDef = TypedDict(
+    "DeleteKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOptOutListResultTypeDef = TypedDict(
+    "DeleteOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOptedOutNumberResultTypeDef = TypedDict(
+    "DeleteOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePoolResultTypeDef = TypedDict(
+    "DeletePoolResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "Status": PoolStatusType,
         "MessageType": MessageTypeType,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountLimitsResultTypeDef = TypedDict(
     "DescribeAccountLimitsResultTypeDef",
     {
         "AccountLimits": List[AccountLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+DisassociateOriginationIdentityResultTypeDef = TypedDict(
+    "DisassociateOriginationIdentityResultTypeDef",
     {
-        "ConfigurationSetNames": Sequence[str],
-        "Filters": Sequence[ConfigurationSetFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutKeywordResultTypeDef = TypedDict(
+    "PutKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutOptedOutNumberResultTypeDef = TypedDict(
+    "PutOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReleasePhoneNumberResultTypeDef = TypedDict(
+    "ReleasePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendTextMessageResultTypeDef = TypedDict(
+    "SendTextMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendVoiceMessageResultTypeDef = TypedDict(
+    "SendVoiceMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultMessageTypeResultTypeDef = TypedDict(
+    "SetDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultSenderIdResultTypeDef = TypedDict(
+    "SetDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePhoneNumberResultTypeDef = TypedDict(
+    "UpdatePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "DeletionProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePoolResultTypeDef = TypedDict(
+    "UpdatePoolResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeConfigurationSetsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationSetsRequestRequestTypeDef",
     {
         "ConfigurationSetNames": Sequence[str],
         "Filters": Sequence[ConfigurationSetFilterTypeDef],
@@ -1077,25 +1069,14 @@
 
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-CreateConfigurationSetResultTypeDef = TypedDict(
-    "CreateConfigurationSetResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "Tags": List[TagTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateOptOutListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalCreateOptOutListRequestRequestTypeDef = TypedDict(
@@ -1108,25 +1089,14 @@
 )
 
 class CreateOptOutListRequestRequestTypeDef(
     _RequiredCreateOptOutListRequestRequestTypeDef, _OptionalCreateOptOutListRequestRequestTypeDef
 ):
     pass
 
-CreateOptOutListResultTypeDef = TypedDict(
-    "CreateOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "Tags": List[TagTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePoolRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
     },
@@ -1142,42 +1112,14 @@
 )
 
 class CreatePoolRequestRequestTypeDef(
     _RequiredCreatePoolRequestRequestTypeDef, _OptionalCreatePoolRequestRequestTypeDef
 ):
     pass
 
-CreatePoolResultTypeDef = TypedDict(
-    "CreatePoolResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
-        "Tags": List[TagTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRequestPhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredRequestPhoneNumberRequestRequestTypeDef",
     {
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
         "NumberCapabilities": Sequence[NumberCapabilityType],
         "NumberType": RequestableNumberTypeType,
@@ -1198,14 +1140,72 @@
 
 class RequestPhoneNumberRequestRequestTypeDef(
     _RequiredRequestPhoneNumberRequestRequestTypeDef,
     _OptionalRequestPhoneNumberRequestRequestTypeDef,
 ):
     pass
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateConfigurationSetResultTypeDef = TypedDict(
+    "CreateConfigurationSetResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "Tags": List[TagOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOptOutListResultTypeDef = TypedDict(
+    "CreateOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "Tags": List[TagOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePoolResultTypeDef = TypedDict(
+    "CreatePoolResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
+        "Tags": List[TagOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RequestPhoneNumberResultTypeDef = TypedDict(
     "RequestPhoneNumberResultTypeDef",
     {
         "PhoneNumberArn": str,
         "PhoneNumberId": str,
         "PhoneNumber": str,
         "Status": NumberStatusType,
@@ -1216,25 +1216,17 @@
         "MonthlyLeasingPrice": str,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "DeletionProtectionEnabled": bool,
         "PoolId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -1255,35 +1247,14 @@
 
 class CreateEventDestinationRequestRequestTypeDef(
     _RequiredCreateEventDestinationRequestRequestTypeDef,
     _OptionalCreateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredEventDestinationTypeDef = TypedDict(
-    "_RequiredEventDestinationTypeDef",
-    {
-        "EventDestinationName": str,
-        "Enabled": bool,
-        "MatchingEventTypes": List[EventTypeType],
-    },
-)
-_OptionalEventDestinationTypeDef = TypedDict(
-    "_OptionalEventDestinationTypeDef",
-    {
-        "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-    },
-    total=False,
-)
-
-class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
-    pass
-
 _RequiredUpdateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -1301,26 +1272,69 @@
 
 class UpdateEventDestinationRequestRequestTypeDef(
     _RequiredUpdateEventDestinationRequestRequestTypeDef,
     _OptionalUpdateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
+DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
+    {
+        "ConfigurationSetNames": Sequence[str],
+        "Filters": Sequence[ConfigurationSetFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
+    {
+        "OptOutListNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "OriginationIdentity": str,
     },
 )
 _OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "Keywords": Sequence[str],
         "Filters": Sequence[KeywordFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef(
     _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     _OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
@@ -1352,39 +1366,39 @@
 DescribeKeywordsResultTypeDef = TypedDict(
     "DescribeKeywordsResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keywords": List[KeywordInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOptOutListsResultTypeDef = TypedDict(
     "DescribeOptOutListsResultTypeDef",
     {
         "OptOutLists": List[OptOutListInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptedOutNumbers": Sequence[str],
         "Filters": Sequence[OptedOutFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef(
     _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     _OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
@@ -1417,24 +1431,24 @@
 DescribeOptedOutNumbersResultTypeDef = TypedDict(
     "DescribeOptedOutNumbersResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "OptedOutNumbers": List[OptedOutNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef = TypedDict(
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
         "Filters": Sequence[PhoneNumberFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePhoneNumbersRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumbersRequestRequestTypeDef",
     {
@@ -1447,24 +1461,24 @@
 )
 
 DescribePhoneNumbersResultTypeDef = TypedDict(
     "DescribePhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePoolsRequestDescribePoolsPaginateTypeDef = TypedDict(
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     {
         "PoolIds": Sequence[str],
         "Filters": Sequence[PoolFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePoolsRequestRequestTypeDef = TypedDict(
     "DescribePoolsRequestRequestTypeDef",
     {
@@ -1477,24 +1491,24 @@
 )
 
 DescribePoolsResultTypeDef = TypedDict(
     "DescribePoolsResultTypeDef",
     {
         "Pools": List[PoolInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef = TypedDict(
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     {
         "SenderIds": Sequence[SenderIdAndCountryTypeDef],
         "Filters": Sequence[SenderIdFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSenderIdsRequestRequestTypeDef = TypedDict(
     "DescribeSenderIdsRequestRequestTypeDef",
     {
@@ -1507,41 +1521,62 @@
 )
 
 DescribeSenderIdsResultTypeDef = TypedDict(
     "DescribeSenderIdsResultTypeDef",
     {
         "SenderIds": List[SenderIdInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpendLimitsResultTypeDef = TypedDict(
     "DescribeSpendLimitsResultTypeDef",
     {
         "SpendLimits": List[SpendLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredEventDestinationTypeDef = TypedDict(
+    "_RequiredEventDestinationTypeDef",
+    {
+        "EventDestinationName": str,
+        "Enabled": bool,
+        "MatchingEventTypes": List[EventTypeType],
+    },
+)
+_OptionalEventDestinationTypeDef = TypedDict(
+    "_OptionalEventDestinationTypeDef",
+    {
+        "CloudWatchLogsDestination": CloudWatchLogsDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationOutputTypeDef,
+    },
+    total=False,
+)
+
+class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
+    pass
+
 _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "PoolId": str,
         },
     )
 )
 _OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "Filters": Sequence[PoolOriginationIdentitiesFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
+            "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
 class ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef(
     _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
@@ -1574,15 +1609,15 @@
 ListPoolOriginationIdentitiesResultTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentities": List[OriginationIdentityMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfigurationSetInformationTypeDef = TypedDict(
     "_RequiredConfigurationSetInformationTypeDef",
     {
         "ConfigurationSetArn": str,
@@ -1607,52 +1642,52 @@
 
 CreateEventDestinationResultTypeDef = TypedDict(
     "CreateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConfigurationSetResultTypeDef = TypedDict(
     "DeleteConfigurationSetResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestinations": List[EventDestinationTypeDef],
         "DefaultMessageType": MessageTypeType,
         "DefaultSenderId": str,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventDestinationResultTypeDef = TypedDict(
     "DeleteEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventDestinationResultTypeDef = TypedDict(
     "UpdateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationSetsResultTypeDef = TypedDict(
     "DescribeConfigurationSetsResultTypeDef",
     {
         "ConfigurationSets": List[ConfigurationSetInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.28.0
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-sms-voice-v2?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-sms-voice-v2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,104 +394,107 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
-    AssociateOriginationIdentityResultTypeDef,
+    ResponseMetadataTypeDef,
+    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
-    DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
-    DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
-    DeleteKeywordResultTypeDef,
     DeleteOptOutListRequestRequestTypeDef,
-    DeleteOptOutListResultTypeDef,
     DeleteOptedOutNumberRequestRequestTypeDef,
-    DeleteOptedOutNumberResultTypeDef,
     DeletePoolRequestRequestTypeDef,
-    DeletePoolResultTypeDef,
-    DeleteTextMessageSpendLimitOverrideResultTypeDef,
-    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
-    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountAttributesRequestRequestTypeDef,
-    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsRequestRequestTypeDef,
     KeywordFilterTypeDef,
     KeywordInformationTypeDef,
-    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeOptOutListsRequestRequestTypeDef,
     OptOutListInformationTypeDef,
     OptedOutFilterTypeDef,
     OptedOutNumberInformationTypeDef,
     PhoneNumberFilterTypeDef,
     PhoneNumberInformationTypeDef,
     PoolFilterTypeDef,
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
-    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
-    DisassociateOriginationIdentityResultTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutKeywordRequestRequestTypeDef,
-    PutKeywordResultTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
-    PutOptedOutNumberResultTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
-    ReleasePhoneNumberResultTypeDef,
-    ResponseMetadataTypeDef,
     SendTextMessageRequestRequestTypeDef,
-    SendTextMessageResultTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
-    SendVoiceMessageResultTypeDef,
     SetDefaultMessageTypeRequestRequestTypeDef,
-    SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdRequestRequestTypeDef,
-    SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideRequestRequestTypeDef,
-    SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef,
-    SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResultTypeDef,
     UpdatePoolRequestRequestTypeDef,
-    UpdatePoolResultTypeDef,
+    AssociateOriginationIdentityResultTypeDef,
+    DeleteDefaultMessageTypeResultTypeDef,
+    DeleteDefaultSenderIdResultTypeDef,
+    DeleteKeywordResultTypeDef,
+    DeleteOptOutListResultTypeDef,
+    DeleteOptedOutNumberResultTypeDef,
+    DeletePoolResultTypeDef,
+    DeleteTextMessageSpendLimitOverrideResultTypeDef,
+    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
-    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
+    DisassociateOriginationIdentityResultTypeDef,
+    PutKeywordResultTypeDef,
+    PutOptedOutNumberResultTypeDef,
+    ReleasePhoneNumberResultTypeDef,
+    SendTextMessageResultTypeDef,
+    SendVoiceMessageResultTypeDef,
+    SetDefaultMessageTypeResultTypeDef,
+    SetDefaultSenderIdResultTypeDef,
+    SetTextMessageSpendLimitOverrideResultTypeDef,
+    SetVoiceMessageSpendLimitOverrideResultTypeDef,
+    UpdatePhoneNumberResultTypeDef,
+    UpdatePoolResultTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateConfigurationSetResultTypeDef,
     CreateOptOutListRequestRequestTypeDef,
-    CreateOptOutListResultTypeDef,
     CreatePoolRequestRequestTypeDef,
+    RequestPhoneNumberRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateConfigurationSetResultTypeDef,
+    CreateOptOutListResultTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
-    EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
+    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
+    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
+    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
+    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
+    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     DescribeKeywordsRequestRequestTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     DescribeOptedOutNumbersRequestRequestTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
@@ -501,14 +504,15 @@
     DescribePoolsRequestDescribePoolsPaginateTypeDef,
     DescribePoolsRequestRequestTypeDef,
     DescribePoolsResultTypeDef,
     DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef,
     DescribeSenderIdsRequestRequestTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
+    EventDestinationTypeDef,
     ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
     ListPoolOriginationIdentitiesRequestRequestTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ConfigurationSetInformationTypeDef,
     CreateEventDestinationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteEventDestinationResultTypeDef,
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.0/setup.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-sms-voice-v2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_pinpoint_sms_voice_v2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

