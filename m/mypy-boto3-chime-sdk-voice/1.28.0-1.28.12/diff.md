# Comparing `tmp/mypy-boto3-chime-sdk-voice-1.28.0.tar.gz` & `tmp/mypy-boto3-chime-sdk-voice-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.28.0.tar", last modified: Thu Jul  6 20:59:07 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-voice-1.28.0.tar` & `mypy-boto3-chime-sdk-voice-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:07.610239 mypy-boto3-chime-sdk-voice-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-07-06 20:59:07.610239 mypy-boto3-chime-sdk-voice-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:07.590239 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66722 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66620 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-07-06 20:34:50.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-07-06 20:34:50.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70049 2023-07-06 20:34:53.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69998 2023-07-06 20:34:51.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:07.610239 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-07-06 20:59:07.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 20:59:07.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:07.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:07.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:07.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 20:59:07.000000 mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:07.610239 mypy-boto3-chime-sdk-voice-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-06 20:34:49.000000 mypy-boto3-chime-sdk-voice-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66722 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66620 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75322 2023-07-27 05:18:22.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-07-27 05:18:22.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/setup.py
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/LICENSE` & `mypy-boto3-chime-sdk-voice-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKVoice 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKVoice 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,14 +368,15 @@
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
+    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
@@ -386,187 +387,204 @@
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    VoiceConnectorSettingsTypeDef,
+    GeoMatchParamsOutputTypeDef,
+    VoiceConnectorSettingsOutputTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationOutputTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationOutputTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
-    TerminationTypeDef,
+    TerminationOutputTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
+    LoggingConfigurationTypeDef,
+    MediaInsightsConfigurationOutputTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
+    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
     PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
+    SipMediaApplicationEndpointOutputTypeDef,
+    SipRuleTargetApplicationOutputTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
+    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
+    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     UpdateVoiceProfileDomainRequestRequestTypeDef,
     UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    VoiceConnectorItemOutputTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
-    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
-    SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
-    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
-    PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
-    PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
+    SipMediaApplicationTypeDef,
+    SipRuleTypeDef,
     SpeakerSearchDetailsTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     GetVoiceToneAnalysisTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
-    CreateVoiceProfileDomainResponseTypeDef,
-    GetVoiceProfileDomainResponseTypeDef,
-    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
-    PutVoiceConnectorOriginationRequestRequestTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
     SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
     GetSpeakerSearchTaskResponseTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/README.md` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-chime-sdk-voice
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKVoice 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 chime-sdk-voice type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,14 +368,15 @@
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
+    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
@@ -354,187 +387,204 @@
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    VoiceConnectorSettingsTypeDef,
+    GeoMatchParamsOutputTypeDef,
+    VoiceConnectorSettingsOutputTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationOutputTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationOutputTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
-    TerminationTypeDef,
+    TerminationOutputTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
+    LoggingConfigurationTypeDef,
+    MediaInsightsConfigurationOutputTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
+    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
     PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
+    SipMediaApplicationEndpointOutputTypeDef,
+    SipRuleTargetApplicationOutputTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
+    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
+    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     UpdateVoiceProfileDomainRequestRequestTypeDef,
     UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    VoiceConnectorItemOutputTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
-    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
-    SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
-    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
-    PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
-    PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
+    SipMediaApplicationTypeDef,
+    SipRuleTypeDef,
     SpeakerSearchDetailsTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     GetVoiceToneAnalysisTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
-    CreateVoiceProfileDomainResponseTypeDef,
-    GetVoiceProfileDomainResponseTypeDef,
-    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
-    PutVoiceConnectorOriginationRequestRequestTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
     SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
     GetSpeakerSearchTaskResponseTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/__init__.py` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/__init__.pyi` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/__main__.py` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKVoice 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ChimeSDKVoice 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice\nOther"
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

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/client.py` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/client.pyi` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/literals.py` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,15 @@
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
@@ -326,26 +327,28 @@
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

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/literals.pyi` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,15 @@
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
@@ -324,26 +325,28 @@
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

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/paginator.py` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/paginator.pyi` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/type_defs.py` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
     "VoiceConnectorTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "CreateVoiceProfileRequestRequestTypeDef",
     "VoiceProfileTypeDef",
     "CredentialTypeDef",
+    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
     "DeleteSipRuleRequestRequestTypeDef",
     "DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorGroupRequestRequestTypeDef",
@@ -83,187 +84,204 @@
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     "DeleteVoiceProfileDomainRequestRequestTypeDef",
     "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "VoiceConnectorSettingsTypeDef",
+    "GeoMatchParamsOutputTypeDef",
+    "VoiceConnectorSettingsOutputTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
+    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    "LoggingConfigurationTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "GetVoiceConnectorOriginationRequestRequestTypeDef",
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationTypeDef",
+    "TerminationOutputTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
     "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "ListVoiceProfileDomainsRequestRequestTypeDef",
     "VoiceProfileDomainSummaryTypeDef",
     "ListVoiceProfilesRequestRequestTypeDef",
     "VoiceProfileSummaryTypeDef",
+    "LoggingConfigurationTypeDef",
+    "MediaInsightsConfigurationOutputTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
+    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    "SipMediaApplicationEndpointOutputTypeDef",
+    "SipRuleTargetApplicationOutputTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
+    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "UpdateVoiceProfileDomainRequestRequestTypeDef",
     "UpdateVoiceProfileRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
+    "VoiceConnectorItemOutputTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
-    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSipRuleRequestRequestTypeDef",
-    "SipRuleTypeDef",
     "UpdateSipRuleRequestRequestTypeDef",
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
-    "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
-    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
-    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
-    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
+    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "VoiceProfileDomainTypeDef",
+    "SipMediaApplicationTypeDef",
+    "SipRuleTypeDef",
     "SpeakerSearchDetailsTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    "VoiceConnectorGroupTypeDef",
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     "StartVoiceToneAnalysisTaskResponseTypeDef",
-    "CreateSipMediaApplicationResponseTypeDef",
-    "GetSipMediaApplicationResponseTypeDef",
-    "ListSipMediaApplicationsResponseTypeDef",
-    "UpdateSipMediaApplicationResponseTypeDef",
-    "CreateSipRuleResponseTypeDef",
-    "GetSipRuleResponseTypeDef",
-    "ListSipRulesResponseTypeDef",
-    "UpdateSipRuleResponseTypeDef",
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    "GetVoiceConnectorGroupResponseTypeDef",
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    "UpdateVoiceConnectorGroupResponseTypeDef",
-    "CreateVoiceProfileDomainResponseTypeDef",
-    "GetVoiceProfileDomainResponseTypeDef",
-    "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
+    "CreateVoiceProfileDomainResponseTypeDef",
+    "GetVoiceProfileDomainResponseTypeDef",
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    "CreateSipMediaApplicationResponseTypeDef",
+    "GetSipMediaApplicationResponseTypeDef",
+    "ListSipMediaApplicationsResponseTypeDef",
+    "UpdateSipMediaApplicationResponseTypeDef",
+    "CreateSipRuleResponseTypeDef",
+    "GetSipRuleResponseTypeDef",
+    "ListSipRulesResponseTypeDef",
+    "UpdateSipRuleResponseTypeDef",
     "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    "GetVoiceConnectorGroupResponseTypeDef",
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetSpeakerSearchTaskResponseTypeDef",
     "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
@@ -520,14 +538,37 @@
     {
         "Username": str,
         "Password": str,
     },
     total=False,
 )
 
+_RequiredDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDNISEmergencyCallingConfigurationOutputTypeDef",
+    {
+        "EmergencyPhoneNumber": str,
+        "CallingCountry": str,
+    },
+)
+_OptionalDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDNISEmergencyCallingConfigurationOutputTypeDef",
+    {
+        "TestPhoneNumber": str,
+    },
+    total=False,
+)
+
+
+class DNISEmergencyCallingConfigurationOutputTypeDef(
+    _RequiredDNISEmergencyCallingConfigurationOutputTypeDef,
+    _OptionalDNISEmergencyCallingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredDNISEmergencyCallingConfigurationTypeDef = TypedDict(
     "_RequiredDNISEmergencyCallingConfigurationTypeDef",
     {
         "EmergencyPhoneNumber": str,
         "CallingCountry": str,
     },
 )
@@ -666,16 +707,24 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VoiceConnectorSettingsTypeDef = TypedDict(
-    "VoiceConnectorSettingsTypeDef",
+GeoMatchParamsOutputTypeDef = TypedDict(
+    "GeoMatchParamsOutputTypeDef",
+    {
+        "Country": str,
+        "AreaCode": str,
+    },
+)
+
+VoiceConnectorSettingsOutputTypeDef = TypedDict(
+    "VoiceConnectorSettingsOutputTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetPhoneNumberOrderRequestRequestTypeDef = TypedDict(
@@ -712,31 +761,31 @@
 GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 
-SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+SipMediaApplicationAlexaSkillConfigurationOutputTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     {
         "AlexaSkillStatus": AlexaSkillStatusType,
         "AlexaSkillIds": List[str],
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 
-SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationLoggingConfigurationTypeDef",
+SipMediaApplicationLoggingConfigurationOutputTypeDef = TypedDict(
+    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
     {
         "EnableSipMediaApplicationMessageLogs": bool,
     },
     total=False,
 )
 
 GetSipMediaApplicationRequestRequestTypeDef = TypedDict(
@@ -778,16 +827,16 @@
 GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-LoggingConfigurationTypeDef = TypedDict(
-    "LoggingConfigurationTypeDef",
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
     {
         "EnableSIPLogs": bool,
         "EnableMediaMetricLogs": bool,
     },
     total=False,
 )
 
@@ -849,16 +898,16 @@
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
+TerminationOutputTypeDef = TypedDict(
+    "TerminationOutputTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
@@ -996,14 +1045,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 ListVoiceConnectorGroupsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1086,14 +1143,32 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ExpirationTimestamp": datetime,
     },
     total=False,
 )
 
+LoggingConfigurationTypeDef = TypedDict(
+    "LoggingConfigurationTypeDef",
+    {
+        "EnableSIPLogs": bool,
+        "EnableMediaMetricLogs": bool,
+    },
+    total=False,
+)
+
+MediaInsightsConfigurationOutputTypeDef = TypedDict(
+    "MediaInsightsConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "ConfigurationArn": str,
+    },
+    total=False,
+)
+
 MediaInsightsConfigurationTypeDef = TypedDict(
     "MediaInsightsConfigurationTypeDef",
     {
         "Disabled": bool,
         "ConfigurationArn": str,
     },
     total=False,
@@ -1104,14 +1179,26 @@
     {
         "E164PhoneNumber": str,
         "Status": OrderedPhoneNumberStatusType,
     },
     total=False,
 )
 
+OriginationRouteOutputTypeDef = TypedDict(
+    "OriginationRouteOutputTypeDef",
+    {
+        "Host": str,
+        "Port": int,
+        "Protocol": OriginationRouteProtocolType,
+        "Priority": int,
+        "Weight": int,
+    },
+    total=False,
+)
+
 OriginationRouteTypeDef = TypedDict(
     "OriginationRouteTypeDef",
     {
         "Host": str,
         "Port": int,
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
@@ -1158,14 +1245,30 @@
         "OutboundSMS": bool,
         "InboundMMS": bool,
         "OutboundMMS": bool,
     },
     total=False,
 )
 
+SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    {
+        "AlexaSkillStatus": AlexaSkillStatusType,
+        "AlexaSkillIds": Sequence[str],
+    },
+)
+
+SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationLoggingConfigurationTypeDef",
+    {
+        "EnableSipMediaApplicationMessageLogs": bool,
+    },
+    total=False,
+)
+
 _RequiredPutVoiceConnectorProxyRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorProxyRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "DefaultSessionExpiryMinutes": int,
         "PhoneNumberPoolCountries": Sequence[str],
     },
@@ -1183,14 +1286,26 @@
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
 
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
+    {
+        "CpsLimit": int,
+        "DefaultPhoneNumber": str,
+        "CallingRegions": Sequence[str],
+        "CidrAllowedList": Sequence[str],
+        "Disabled": bool,
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
@@ -1225,14 +1340,39 @@
     {
         "E164PhoneNumbers": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+)
+
+SipMediaApplicationEndpointOutputTypeDef = TypedDict(
+    "SipMediaApplicationEndpointOutputTypeDef",
+    {
+        "LambdaArn": str,
+    },
+    total=False,
+)
+
+SipRuleTargetApplicationOutputTypeDef = TypedDict(
+    "SipRuleTargetApplicationOutputTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "Priority": int,
+        "AwsRegion": str,
+    },
+    total=False,
+)
+
 SpeakerSearchResultTypeDef = TypedDict(
     "SpeakerSearchResultTypeDef",
     {
         "ConfidenceScore": float,
         "VoiceProfileId": str,
     },
     total=False,
@@ -1299,14 +1439,22 @@
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
     },
 )
 
+StreamingNotificationTargetOutputTypeDef = TypedDict(
+    "StreamingNotificationTargetOutputTypeDef",
+    {
+        "NotificationTarget": NotificationTargetType,
+    },
+    total=False,
+)
+
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
     total=False,
 )
@@ -1315,14 +1463,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+VoiceConnectorSettingsTypeDef = TypedDict(
+    "VoiceConnectorSettingsTypeDef",
+    {
+        "CdrBucket": str,
+    },
+    total=False,
+)
+
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -1430,14 +1586,22 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
+VoiceConnectorItemOutputTypeDef = TypedDict(
+    "VoiceConnectorItemOutputTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Priority": int,
+    },
+)
+
 AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1554,28 +1718,14 @@
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SipMediaApplicationTypeDef = TypedDict(
-    "SipMediaApplicationTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": List[SipMediaApplicationEndpointTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "SipMediaApplicationArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipMediaApplicationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 _OptionalUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
@@ -1639,22 +1789,14 @@
 class CreateVoiceConnectorRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorRequestRequestTypeDef,
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
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1679,29 +1821,14 @@
 
 class CreateSipRuleRequestRequestTypeDef(
     _RequiredCreateSipRuleRequestRequestTypeDef, _OptionalCreateSipRuleRequestRequestTypeDef
 ):
     pass
 
 
-SipRuleTypeDef = TypedDict(
-    "SipRuleTypeDef",
-    {
-        "SipRuleId": str,
-        "Name": str,
-        "Disabled": bool,
-        "TriggerType": SipRuleTriggerTypeType,
-        "TriggerValue": str,
-        "TargetApplications": List[SipRuleTargetApplicationTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
     },
 )
@@ -1748,27 +1875,14 @@
     {
         "VoiceConnectorGroupId": str,
         "Name": str,
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
 )
 
-VoiceConnectorGroupTypeDef = TypedDict(
-    "VoiceConnectorGroupTypeDef",
-    {
-        "VoiceConnectorGroupId": str,
-        "Name": str,
-        "VoiceConnectorItems": List[VoiceConnectorItemTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "VoiceConnectorGroupArn": str,
-    },
-    total=False,
-)
-
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1819,28 +1933,14 @@
 class CreateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
 
-VoiceProfileDomainTypeDef = TypedDict(
-    "VoiceProfileDomainTypeDef",
-    {
-        "VoiceProfileDomainId": str,
-        "VoiceProfileDomainArn": str,
-        "Name": str,
-        "Description": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 CreateVoiceProfileResponseTypeDef = TypedDict(
     "CreateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1879,140 +1979,90 @@
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
+EmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "EmergencyCallingConfigurationOutputTypeDef",
+    {
+        "DNIS": List[DNISEmergencyCallingConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
+        "DNIS": Sequence[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    {
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
-    },
-    total=False,
-)
-
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
+            SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-    },
-)
-_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ),
-    },
-    total=False,
-)
-
-
-class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
-    _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
+            SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "SipMediaApplicationLoggingConfiguration": (
+            SipMediaApplicationLoggingConfigurationOutputTypeDef
+        ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-    },
-)
-_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
-    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "SipMediaApplicationLoggingConfiguration": (
+            SipMediaApplicationLoggingConfigurationOutputTypeDef
+        ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-    },
-)
-
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
@@ -2036,43 +2086,43 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
-    },
-)
-
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2083,32 +2133,49 @@
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+    },
+)
+
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
         "ProductType": PhoneNumberProductTypeType,
         "Status": PhoneNumberOrderStatusType,
         "OrderType": PhoneNumberOrderTypeType,
         "OrderedPhoneNumbers": List[OrderedPhoneNumberTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+OriginationOutputTypeDef = TypedDict(
+    "OriginationOutputTypeDef",
+    {
+        "Routes": List[OriginationRouteOutputTypeDef],
+        "Disabled": bool,
+    },
+    total=False,
+)
+
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": List[OriginationRouteTypeDef],
+        "Routes": Sequence[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
@@ -2121,15 +2188,15 @@
         "Capabilities": List[CapabilityType],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "EndedTimestamp": datetime,
         "Participants": List[ParticipantTypeDef],
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
-        "GeoMatchParams": GeoMatchParamsTypeDef,
+        "GeoMatchParams": GeoMatchParamsOutputTypeDef,
     },
     total=False,
 )
 
 PhoneNumberTypeDef = TypedDict(
     "PhoneNumberTypeDef",
     {
@@ -2147,209 +2214,227 @@
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
         "OrderId": str,
     },
     total=False,
 )
 
-SpeakerSearchDetailsTypeDef = TypedDict(
-    "SpeakerSearchDetailsTypeDef",
-    {
-        "Results": List[SpeakerSearchResultTypeDef],
-        "VoiceprintGenerationStatus": str,
-    },
-    total=False,
-)
-
-_RequiredStreamingConfigurationTypeDef = TypedDict(
-    "_RequiredStreamingConfigurationTypeDef",
+_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
-        "DataRetentionInHours": int,
-        "Disabled": bool,
+        "SipMediaApplicationId": str,
     },
 )
-_OptionalStreamingConfigurationTypeDef = TypedDict(
-    "_OptionalStreamingConfigurationTypeDef",
+_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
-        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
+        "SipMediaApplicationAlexaSkillConfiguration": (
+            SipMediaApplicationAlexaSkillConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
 
-class StreamingConfigurationTypeDef(
-    _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
+class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "GetVoiceToneAnalysisTaskResponseTypeDef",
+_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationId": str,
     },
 )
-
-StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "StartVoiceToneAnalysisTaskResponseTypeDef",
+_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
     },
+    total=False,
 )
 
-CreateSipMediaApplicationResponseTypeDef = TypedDict(
-    "CreateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-GetSipMediaApplicationResponseTypeDef = TypedDict(
-    "GetSipMediaApplicationResponseTypeDef",
+class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
     },
 )
 
-ListSipMediaApplicationsResponseTypeDef = TypedDict(
-    "ListSipMediaApplicationsResponseTypeDef",
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
     {
-        "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
-UpdateSipMediaApplicationResponseTypeDef = TypedDict(
-    "UpdateSipMediaApplicationResponseTypeDef",
+SipMediaApplicationTypeDef = TypedDict(
+    "SipMediaApplicationTypeDef",
     {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationId": str,
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "SipMediaApplicationArn": str,
     },
+    total=False,
 )
 
-CreateSipRuleResponseTypeDef = TypedDict(
-    "CreateSipRuleResponseTypeDef",
+SipRuleTypeDef = TypedDict(
+    "SipRuleTypeDef",
     {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipRuleId": str,
+        "Name": str,
+        "Disabled": bool,
+        "TriggerType": SipRuleTriggerTypeType,
+        "TriggerValue": str,
+        "TargetApplications": List[SipRuleTargetApplicationOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
-GetSipRuleResponseTypeDef = TypedDict(
-    "GetSipRuleResponseTypeDef",
+SpeakerSearchDetailsTypeDef = TypedDict(
+    "SpeakerSearchDetailsTypeDef",
     {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Results": List[SpeakerSearchResultTypeDef],
+        "VoiceprintGenerationStatus": str,
     },
+    total=False,
 )
 
-ListSipRulesResponseTypeDef = TypedDict(
-    "ListSipRulesResponseTypeDef",
+_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationOutputTypeDef",
     {
-        "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataRetentionInHours": int,
+        "Disabled": bool,
     },
 )
-
-UpdateSipRuleResponseTypeDef = TypedDict(
-    "UpdateSipRuleResponseTypeDef",
+_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationOutputTypeDef",
     {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
-CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "CreateVoiceConnectorGroupResponseTypeDef",
+
+class StreamingConfigurationOutputTypeDef(
+    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
+):
+    pass
+
+
+_RequiredStreamingConfigurationTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationTypeDef",
     {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataRetentionInHours": int,
+        "Disabled": bool,
     },
 )
-
-GetVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "GetVoiceConnectorGroupResponseTypeDef",
+_OptionalStreamingConfigurationTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationTypeDef",
     {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
+    total=False,
 )
 
-ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorGroupsResponseTypeDef",
+
+class StreamingConfigurationTypeDef(
+    _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
+):
+    pass
+
+
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
     {
-        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
     },
+    total=False,
 )
 
-UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "UpdateVoiceConnectorGroupResponseTypeDef",
+VoiceConnectorGroupTypeDef = TypedDict(
+    "VoiceConnectorGroupTypeDef",
     {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnectorGroupId": str,
+        "Name": str,
+        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "VoiceConnectorGroupArn": str,
     },
+    total=False,
 )
 
-CreateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "CreateVoiceProfileDomainResponseTypeDef",
+GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
     {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetVoiceProfileDomainResponseTypeDef = TypedDict(
-    "GetVoiceProfileDomainResponseTypeDef",
+StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
     {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "UpdateVoiceProfileDomainResponseTypeDef",
+GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2370,32 +2455,32 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
+PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
@@ -2457,14 +2542,104 @@
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "CreateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetVoiceProfileDomainResponseTypeDef = TypedDict(
+    "GetVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSipMediaApplicationsResponseTypeDef = TypedDict(
+    "ListSipMediaApplicationsResponseTypeDef",
+    {
+        "SipMediaApplications": List[SipMediaApplicationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSipMediaApplicationResponseTypeDef = TypedDict(
+    "UpdateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSipRuleResponseTypeDef = TypedDict(
+    "CreateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSipRuleResponseTypeDef = TypedDict(
+    "GetSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSipRulesResponseTypeDef = TypedDict(
+    "ListSipRulesResponseTypeDef",
+    {
+        "SipRules": List[SipRuleTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSipRuleResponseTypeDef = TypedDict(
+    "UpdateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SpeakerSearchTaskTypeDef = TypedDict(
     "SpeakerSearchTaskTypeDef",
     {
         "SpeakerSearchTaskId": str,
         "SpeakerSearchTaskStatus": str,
         "CallDetails": CallDetailsTypeDef,
         "SpeakerSearchDetails": SpeakerSearchDetailsTypeDef,
@@ -2475,31 +2650,64 @@
     },
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    {
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "CreateVoiceConnectorGroupResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "GetVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    {
+        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "UpdateVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice/type_defs.pyi` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
     "VoiceConnectorTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "CreateVoiceProfileRequestRequestTypeDef",
     "VoiceProfileTypeDef",
     "CredentialTypeDef",
+    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
     "DeleteSipRuleRequestRequestTypeDef",
     "DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorGroupRequestRequestTypeDef",
@@ -82,187 +83,204 @@
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     "DeleteVoiceProfileDomainRequestRequestTypeDef",
     "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "VoiceConnectorSettingsTypeDef",
+    "GeoMatchParamsOutputTypeDef",
+    "VoiceConnectorSettingsOutputTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
+    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    "LoggingConfigurationTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "GetVoiceConnectorOriginationRequestRequestTypeDef",
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationTypeDef",
+    "TerminationOutputTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
     "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "ListVoiceProfileDomainsRequestRequestTypeDef",
     "VoiceProfileDomainSummaryTypeDef",
     "ListVoiceProfilesRequestRequestTypeDef",
     "VoiceProfileSummaryTypeDef",
+    "LoggingConfigurationTypeDef",
+    "MediaInsightsConfigurationOutputTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
+    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    "SipMediaApplicationEndpointOutputTypeDef",
+    "SipRuleTargetApplicationOutputTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
+    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "UpdateVoiceProfileDomainRequestRequestTypeDef",
     "UpdateVoiceProfileRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
+    "VoiceConnectorItemOutputTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
-    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSipRuleRequestRequestTypeDef",
-    "SipRuleTypeDef",
     "UpdateSipRuleRequestRequestTypeDef",
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
-    "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
-    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
-    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
-    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
+    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "VoiceProfileDomainTypeDef",
+    "SipMediaApplicationTypeDef",
+    "SipRuleTypeDef",
     "SpeakerSearchDetailsTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    "VoiceConnectorGroupTypeDef",
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     "StartVoiceToneAnalysisTaskResponseTypeDef",
-    "CreateSipMediaApplicationResponseTypeDef",
-    "GetSipMediaApplicationResponseTypeDef",
-    "ListSipMediaApplicationsResponseTypeDef",
-    "UpdateSipMediaApplicationResponseTypeDef",
-    "CreateSipRuleResponseTypeDef",
-    "GetSipRuleResponseTypeDef",
-    "ListSipRulesResponseTypeDef",
-    "UpdateSipRuleResponseTypeDef",
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    "GetVoiceConnectorGroupResponseTypeDef",
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    "UpdateVoiceConnectorGroupResponseTypeDef",
-    "CreateVoiceProfileDomainResponseTypeDef",
-    "GetVoiceProfileDomainResponseTypeDef",
-    "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
+    "CreateVoiceProfileDomainResponseTypeDef",
+    "GetVoiceProfileDomainResponseTypeDef",
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    "CreateSipMediaApplicationResponseTypeDef",
+    "GetSipMediaApplicationResponseTypeDef",
+    "ListSipMediaApplicationsResponseTypeDef",
+    "UpdateSipMediaApplicationResponseTypeDef",
+    "CreateSipRuleResponseTypeDef",
+    "GetSipRuleResponseTypeDef",
+    "ListSipRulesResponseTypeDef",
+    "UpdateSipRuleResponseTypeDef",
     "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    "GetVoiceConnectorGroupResponseTypeDef",
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetSpeakerSearchTaskResponseTypeDef",
     "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
@@ -511,14 +529,35 @@
     {
         "Username": str,
         "Password": str,
     },
     total=False,
 )
 
+_RequiredDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDNISEmergencyCallingConfigurationOutputTypeDef",
+    {
+        "EmergencyPhoneNumber": str,
+        "CallingCountry": str,
+    },
+)
+_OptionalDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDNISEmergencyCallingConfigurationOutputTypeDef",
+    {
+        "TestPhoneNumber": str,
+    },
+    total=False,
+)
+
+class DNISEmergencyCallingConfigurationOutputTypeDef(
+    _RequiredDNISEmergencyCallingConfigurationOutputTypeDef,
+    _OptionalDNISEmergencyCallingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredDNISEmergencyCallingConfigurationTypeDef = TypedDict(
     "_RequiredDNISEmergencyCallingConfigurationTypeDef",
     {
         "EmergencyPhoneNumber": str,
         "CallingCountry": str,
     },
 )
@@ -655,16 +694,24 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VoiceConnectorSettingsTypeDef = TypedDict(
-    "VoiceConnectorSettingsTypeDef",
+GeoMatchParamsOutputTypeDef = TypedDict(
+    "GeoMatchParamsOutputTypeDef",
+    {
+        "Country": str,
+        "AreaCode": str,
+    },
+)
+
+VoiceConnectorSettingsOutputTypeDef = TypedDict(
+    "VoiceConnectorSettingsOutputTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetPhoneNumberOrderRequestRequestTypeDef = TypedDict(
@@ -701,31 +748,31 @@
 GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 
-SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+SipMediaApplicationAlexaSkillConfigurationOutputTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     {
         "AlexaSkillStatus": AlexaSkillStatusType,
         "AlexaSkillIds": List[str],
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 
-SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationLoggingConfigurationTypeDef",
+SipMediaApplicationLoggingConfigurationOutputTypeDef = TypedDict(
+    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
     {
         "EnableSipMediaApplicationMessageLogs": bool,
     },
     total=False,
 )
 
 GetSipMediaApplicationRequestRequestTypeDef = TypedDict(
@@ -767,16 +814,16 @@
 GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-LoggingConfigurationTypeDef = TypedDict(
-    "LoggingConfigurationTypeDef",
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
     {
         "EnableSIPLogs": bool,
         "EnableMediaMetricLogs": bool,
     },
     total=False,
 )
 
@@ -838,16 +885,16 @@
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
+TerminationOutputTypeDef = TypedDict(
+    "TerminationOutputTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
@@ -983,14 +1030,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 ListVoiceConnectorGroupsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1071,14 +1126,32 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ExpirationTimestamp": datetime,
     },
     total=False,
 )
 
+LoggingConfigurationTypeDef = TypedDict(
+    "LoggingConfigurationTypeDef",
+    {
+        "EnableSIPLogs": bool,
+        "EnableMediaMetricLogs": bool,
+    },
+    total=False,
+)
+
+MediaInsightsConfigurationOutputTypeDef = TypedDict(
+    "MediaInsightsConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "ConfigurationArn": str,
+    },
+    total=False,
+)
+
 MediaInsightsConfigurationTypeDef = TypedDict(
     "MediaInsightsConfigurationTypeDef",
     {
         "Disabled": bool,
         "ConfigurationArn": str,
     },
     total=False,
@@ -1089,14 +1162,26 @@
     {
         "E164PhoneNumber": str,
         "Status": OrderedPhoneNumberStatusType,
     },
     total=False,
 )
 
+OriginationRouteOutputTypeDef = TypedDict(
+    "OriginationRouteOutputTypeDef",
+    {
+        "Host": str,
+        "Port": int,
+        "Protocol": OriginationRouteProtocolType,
+        "Priority": int,
+        "Weight": int,
+    },
+    total=False,
+)
+
 OriginationRouteTypeDef = TypedDict(
     "OriginationRouteTypeDef",
     {
         "Host": str,
         "Port": int,
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
@@ -1143,14 +1228,30 @@
         "OutboundSMS": bool,
         "InboundMMS": bool,
         "OutboundMMS": bool,
     },
     total=False,
 )
 
+SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    {
+        "AlexaSkillStatus": AlexaSkillStatusType,
+        "AlexaSkillIds": Sequence[str],
+    },
+)
+
+SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationLoggingConfigurationTypeDef",
+    {
+        "EnableSipMediaApplicationMessageLogs": bool,
+    },
+    total=False,
+)
+
 _RequiredPutVoiceConnectorProxyRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorProxyRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "DefaultSessionExpiryMinutes": int,
         "PhoneNumberPoolCountries": Sequence[str],
     },
@@ -1166,14 +1267,26 @@
 
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
+    {
+        "CpsLimit": int,
+        "DefaultPhoneNumber": str,
+        "CallingRegions": Sequence[str],
+        "CidrAllowedList": Sequence[str],
+        "Disabled": bool,
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
@@ -1208,14 +1321,39 @@
     {
         "E164PhoneNumbers": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+)
+
+SipMediaApplicationEndpointOutputTypeDef = TypedDict(
+    "SipMediaApplicationEndpointOutputTypeDef",
+    {
+        "LambdaArn": str,
+    },
+    total=False,
+)
+
+SipRuleTargetApplicationOutputTypeDef = TypedDict(
+    "SipRuleTargetApplicationOutputTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "Priority": int,
+        "AwsRegion": str,
+    },
+    total=False,
+)
+
 SpeakerSearchResultTypeDef = TypedDict(
     "SpeakerSearchResultTypeDef",
     {
         "ConfidenceScore": float,
         "VoiceProfileId": str,
     },
     total=False,
@@ -1278,14 +1416,22 @@
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
     },
 )
 
+StreamingNotificationTargetOutputTypeDef = TypedDict(
+    "StreamingNotificationTargetOutputTypeDef",
+    {
+        "NotificationTarget": NotificationTargetType,
+    },
+    total=False,
+)
+
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
     total=False,
 )
@@ -1294,14 +1440,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+VoiceConnectorSettingsTypeDef = TypedDict(
+    "VoiceConnectorSettingsTypeDef",
+    {
+        "CdrBucket": str,
+    },
+    total=False,
+)
+
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -1403,14 +1557,22 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
+VoiceConnectorItemOutputTypeDef = TypedDict(
+    "VoiceConnectorItemOutputTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Priority": int,
+    },
+)
+
 AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1525,28 +1687,14 @@
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SipMediaApplicationTypeDef = TypedDict(
-    "SipMediaApplicationTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": List[SipMediaApplicationEndpointTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "SipMediaApplicationArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipMediaApplicationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 _OptionalUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
@@ -1604,22 +1752,14 @@
 
 class CreateVoiceConnectorRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorRequestRequestTypeDef,
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
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1642,29 +1782,14 @@
 )
 
 class CreateSipRuleRequestRequestTypeDef(
     _RequiredCreateSipRuleRequestRequestTypeDef, _OptionalCreateSipRuleRequestRequestTypeDef
 ):
     pass
 
-SipRuleTypeDef = TypedDict(
-    "SipRuleTypeDef",
-    {
-        "SipRuleId": str,
-        "Name": str,
-        "Disabled": bool,
-        "TriggerType": SipRuleTriggerTypeType,
-        "TriggerValue": str,
-        "TargetApplications": List[SipRuleTargetApplicationTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
     },
 )
@@ -1707,27 +1832,14 @@
     {
         "VoiceConnectorGroupId": str,
         "Name": str,
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
 )
 
-VoiceConnectorGroupTypeDef = TypedDict(
-    "VoiceConnectorGroupTypeDef",
-    {
-        "VoiceConnectorGroupId": str,
-        "Name": str,
-        "VoiceConnectorItems": List[VoiceConnectorItemTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "VoiceConnectorGroupArn": str,
-    },
-    total=False,
-)
-
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1776,28 +1888,14 @@
 
 class CreateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
-VoiceProfileDomainTypeDef = TypedDict(
-    "VoiceProfileDomainTypeDef",
-    {
-        "VoiceProfileDomainId": str,
-        "VoiceProfileDomainArn": str,
-        "Name": str,
-        "Description": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 CreateVoiceProfileResponseTypeDef = TypedDict(
     "CreateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1834,136 +1932,90 @@
 
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
+EmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "EmergencyCallingConfigurationOutputTypeDef",
+    {
+        "DNIS": List[DNISEmergencyCallingConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
+        "DNIS": Sequence[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    {
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
-    },
-    total=False,
-)
-
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
+            SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-    },
-)
-_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ),
-    },
-    total=False,
-)
-
-class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
-    _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-):
-    pass
-
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
+            SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "SipMediaApplicationLoggingConfiguration": (
+            SipMediaApplicationLoggingConfigurationOutputTypeDef
+        ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-    },
-)
-_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
-    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
-
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "SipMediaApplicationLoggingConfiguration": (
+            SipMediaApplicationLoggingConfigurationOutputTypeDef
+        ),
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-    },
-)
-
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
@@ -1987,43 +2039,43 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
-    },
-)
-
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2034,32 +2086,49 @@
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+    },
+)
+
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
         "ProductType": PhoneNumberProductTypeType,
         "Status": PhoneNumberOrderStatusType,
         "OrderType": PhoneNumberOrderTypeType,
         "OrderedPhoneNumbers": List[OrderedPhoneNumberTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+OriginationOutputTypeDef = TypedDict(
+    "OriginationOutputTypeDef",
+    {
+        "Routes": List[OriginationRouteOutputTypeDef],
+        "Disabled": bool,
+    },
+    total=False,
+)
+
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": List[OriginationRouteTypeDef],
+        "Routes": Sequence[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
@@ -2072,15 +2141,15 @@
         "Capabilities": List[CapabilityType],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "EndedTimestamp": datetime,
         "Participants": List[ParticipantTypeDef],
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
-        "GeoMatchParams": GeoMatchParamsTypeDef,
+        "GeoMatchParams": GeoMatchParamsOutputTypeDef,
     },
     total=False,
 )
 
 PhoneNumberTypeDef = TypedDict(
     "PhoneNumberTypeDef",
     {
@@ -2098,207 +2167,219 @@
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
         "OrderId": str,
     },
     total=False,
 )
 
-SpeakerSearchDetailsTypeDef = TypedDict(
-    "SpeakerSearchDetailsTypeDef",
-    {
-        "Results": List[SpeakerSearchResultTypeDef],
-        "VoiceprintGenerationStatus": str,
-    },
-    total=False,
-)
-
-_RequiredStreamingConfigurationTypeDef = TypedDict(
-    "_RequiredStreamingConfigurationTypeDef",
+_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
-        "DataRetentionInHours": int,
-        "Disabled": bool,
+        "SipMediaApplicationId": str,
     },
 )
-_OptionalStreamingConfigurationTypeDef = TypedDict(
-    "_OptionalStreamingConfigurationTypeDef",
+_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
-        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
+        "SipMediaApplicationAlexaSkillConfiguration": (
+            SipMediaApplicationAlexaSkillConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
-class StreamingConfigurationTypeDef(
-    _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
+class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "GetVoiceToneAnalysisTaskResponseTypeDef",
+_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationId": str,
     },
 )
-
-StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "StartVoiceToneAnalysisTaskResponseTypeDef",
+_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
     },
+    total=False,
 )
 
-CreateSipMediaApplicationResponseTypeDef = TypedDict(
-    "CreateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
 
-GetSipMediaApplicationResponseTypeDef = TypedDict(
-    "GetSipMediaApplicationResponseTypeDef",
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
     },
 )
 
-ListSipMediaApplicationsResponseTypeDef = TypedDict(
-    "ListSipMediaApplicationsResponseTypeDef",
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
     {
-        "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
-UpdateSipMediaApplicationResponseTypeDef = TypedDict(
-    "UpdateSipMediaApplicationResponseTypeDef",
+SipMediaApplicationTypeDef = TypedDict(
+    "SipMediaApplicationTypeDef",
     {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationId": str,
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "SipMediaApplicationArn": str,
     },
+    total=False,
 )
 
-CreateSipRuleResponseTypeDef = TypedDict(
-    "CreateSipRuleResponseTypeDef",
+SipRuleTypeDef = TypedDict(
+    "SipRuleTypeDef",
     {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipRuleId": str,
+        "Name": str,
+        "Disabled": bool,
+        "TriggerType": SipRuleTriggerTypeType,
+        "TriggerValue": str,
+        "TargetApplications": List[SipRuleTargetApplicationOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
-GetSipRuleResponseTypeDef = TypedDict(
-    "GetSipRuleResponseTypeDef",
+SpeakerSearchDetailsTypeDef = TypedDict(
+    "SpeakerSearchDetailsTypeDef",
     {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Results": List[SpeakerSearchResultTypeDef],
+        "VoiceprintGenerationStatus": str,
     },
+    total=False,
 )
 
-ListSipRulesResponseTypeDef = TypedDict(
-    "ListSipRulesResponseTypeDef",
+_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationOutputTypeDef",
     {
-        "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataRetentionInHours": int,
+        "Disabled": bool,
     },
 )
-
-UpdateSipRuleResponseTypeDef = TypedDict(
-    "UpdateSipRuleResponseTypeDef",
+_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationOutputTypeDef",
     {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
-CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "CreateVoiceConnectorGroupResponseTypeDef",
+class StreamingConfigurationOutputTypeDef(
+    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredStreamingConfigurationTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationTypeDef",
     {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataRetentionInHours": int,
+        "Disabled": bool,
     },
 )
-
-GetVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "GetVoiceConnectorGroupResponseTypeDef",
+_OptionalStreamingConfigurationTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationTypeDef",
     {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
+    total=False,
 )
 
-ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorGroupsResponseTypeDef",
+class StreamingConfigurationTypeDef(
+    _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
+):
+    pass
+
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
     {
-        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
     },
+    total=False,
 )
 
-UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "UpdateVoiceConnectorGroupResponseTypeDef",
+VoiceConnectorGroupTypeDef = TypedDict(
+    "VoiceConnectorGroupTypeDef",
     {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnectorGroupId": str,
+        "Name": str,
+        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "VoiceConnectorGroupArn": str,
     },
+    total=False,
 )
 
-CreateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "CreateVoiceProfileDomainResponseTypeDef",
+GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
     {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetVoiceProfileDomainResponseTypeDef = TypedDict(
-    "GetVoiceProfileDomainResponseTypeDef",
+StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
     {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "UpdateVoiceProfileDomainResponseTypeDef",
+GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2319,32 +2400,32 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
+PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
@@ -2406,14 +2487,104 @@
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "CreateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetVoiceProfileDomainResponseTypeDef = TypedDict(
+    "GetVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSipMediaApplicationsResponseTypeDef = TypedDict(
+    "ListSipMediaApplicationsResponseTypeDef",
+    {
+        "SipMediaApplications": List[SipMediaApplicationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSipMediaApplicationResponseTypeDef = TypedDict(
+    "UpdateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSipRuleResponseTypeDef = TypedDict(
+    "CreateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSipRuleResponseTypeDef = TypedDict(
+    "GetSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSipRulesResponseTypeDef = TypedDict(
+    "ListSipRulesResponseTypeDef",
+    {
+        "SipRules": List[SipRuleTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSipRuleResponseTypeDef = TypedDict(
+    "UpdateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SpeakerSearchTaskTypeDef = TypedDict(
     "SpeakerSearchTaskTypeDef",
     {
         "SpeakerSearchTaskId": str,
         "SpeakerSearchTaskStatus": str,
         "CallDetails": CallDetailsTypeDef,
         "SpeakerSearchDetails": SpeakerSearchDetailsTypeDef,
@@ -2424,31 +2595,64 @@
     },
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    {
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "CreateVoiceConnectorGroupResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "GetVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    {
+        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "UpdateVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.28.12/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-chime-sdk-voice
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKVoice 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime-sdk-voice type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,14 +336,15 @@
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
+    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
@@ -386,187 +355,204 @@
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    VoiceConnectorSettingsTypeDef,
+    GeoMatchParamsOutputTypeDef,
+    VoiceConnectorSettingsOutputTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationOutputTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationOutputTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
-    TerminationTypeDef,
+    TerminationOutputTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
+    LoggingConfigurationTypeDef,
+    MediaInsightsConfigurationOutputTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
+    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
     PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
+    SipMediaApplicationEndpointOutputTypeDef,
+    SipRuleTargetApplicationOutputTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
+    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
+    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     UpdateVoiceProfileDomainRequestRequestTypeDef,
     UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    VoiceConnectorItemOutputTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
-    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
-    SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
-    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
-    PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
-    PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
+    SipMediaApplicationTypeDef,
+    SipRuleTypeDef,
     SpeakerSearchDetailsTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     GetVoiceToneAnalysisTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
-    CreateVoiceProfileDomainResponseTypeDef,
-    GetVoiceProfileDomainResponseTypeDef,
-    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
-    PutVoiceConnectorOriginationRequestRequestTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
     SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
     GetSpeakerSearchTaskResponseTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.0/setup.py` & `mypy-boto3-chime-sdk-voice-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-voice",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_chime_sdk_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKVoice 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ChimeSDKVoice 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

