# Comparing `tmp/mypy-boto3-chime-1.28.0.tar.gz` & `tmp/mypy-boto3-chime-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-1.28.0.tar", last modified: Thu Jul  6 20:59:05 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
```

## Comparing `mypy-boto3-chime-1.28.0.tar` & `mypy-boto3-chime-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.694235 mypy-boto3-chime-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32557 2023-07-06 20:59:05.670235 mypy-boto3-chime-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31080 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.670235 mypy-boto3-chime-1.28.0/mypy_boto3_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-07-06 20:34:32.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-07-06 20:34:31.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-06 20:34:33.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-07-06 20:34:33.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-06 20:34:32.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-06 20:34:32.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   144728 2023-07-06 20:34:38.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144569 2023-07-06 20:34:35.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.670235 mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32557 2023-07-06 20:59:05.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 20:59:05.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:05.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 20:59:05.000000 mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:05.694235 mypy-boto3-chime-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:34:30.000000 mypy-boto3-chime-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33946 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32467 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/mypy_boto3_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   154447 2023-07-27 05:18:13.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154280 2023-07-27 05:18:11.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33946 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/setup.py
```

### Comparing `mypy-boto3-chime-1.28.0/LICENSE` & `mypy-boto3-chime-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/PKG-INFO` & `mypy-boto3-chime-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-chime
-Version: 1.28.0
-Summary: Type annotations for boto3.Chime 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,48 +338,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
+    AccountSettingsOutputTypeDef,
     AccountSettingsTypeDef,
-    SigninDelegateGroupTypeDef,
+    SigninDelegateGroupOutputTypeDef,
     AddressTypeDef,
+    AlexaForBusinessMetadataOutputTypeDef,
     AlexaForBusinessMetadataTypeDef,
     IdentityTypeDef,
+    ChannelRetentionSettingsOutputTypeDef,
     ChannelRetentionSettingsTypeDef,
+    AppInstanceStreamingConfigurationOutputTypeDef,
     AppInstanceStreamingConfigurationTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     AppInstanceUserMembershipSummaryTypeDef,
     AppInstanceUserSummaryTypeDef,
     AppInstanceUserTypeDef,
+    AudioArtifactsConfigurationOutputTypeDef,
+    ContentArtifactsConfigurationOutputTypeDef,
+    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
+    SigninDelegateGroupTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     BatchSuspendUserRequestRequestTypeDef,
     UserErrorTypeDef,
     BatchUnsuspendUserRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     BotTypeDef,
+    BusinessCallingSettingsOutputTypeDef,
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
+    ConversationRetentionSettingsOutputTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
@@ -432,14 +410,15 @@
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     CreateUserRequestRequestTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     CredentialTypeDef,
+    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeleteAccountRequestRequestTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
@@ -478,59 +457,61 @@
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
+    GeoMatchParamsOutputTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetEventsConfigurationRequestRequestTypeDef,
-    VoiceConnectorSettingsTypeDef,
+    VoiceConnectorSettingsOutputTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationOutputTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
     GetUserSettingsRequestRequestTypeDef,
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
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
     ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
@@ -551,41 +532,51 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
+    LoggingConfigurationTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
+    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
     PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
     RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
+    RoomRetentionSettingsOutputTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
     SendChannelMessageResponseTypeDef,
+    SipMediaApplicationEndpointOutputTypeDef,
+    SipRuleTargetApplicationOutputTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
+    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
+    TelephonySettingsOutputTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
     UpdateAppInstanceResponseTypeDef,
@@ -594,29 +585,30 @@
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    VoiceConnectorItemOutputTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
-    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
+    UserTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
-    UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
@@ -625,29 +617,32 @@
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateChannelBanResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    AppInstanceRetentionSettingsOutputTypeDef,
     AppInstanceRetentionSettingsTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     ListAppInstancesResponseTypeDef,
     DescribeAppInstanceResponseTypeDef,
     ListAppInstanceUsersResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
+    ArtifactsConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -664,159 +659,166 @@
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
-    ListAttendeeTagsResponseTypeDef,
-    ListMeetingTagsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagAttendeeRequestRequestTypeDef,
     TagMeetingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     ListRoomsResponseTypeDef,
     UpdateRoomResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
-    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
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
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
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
     InviteUsersResponseTypeDef,
+    ListAttendeeTagsResponseTypeDef,
+    ListMeetingTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    RetentionSettingsOutputTypeDef,
     RetentionSettingsTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    SipMediaApplicationTypeDef,
+    SipRuleTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
+    UserSettingsOutputTypeDef,
     UserSettingsTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
-    BatchUpdateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     ResetPersonalPINResponseTypeDef,
     UpdateUserResponseTypeDef,
+    BatchUpdateUserRequestRequestTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
-    PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
+    PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
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
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
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
     GetRetentionSettingsResponseTypeDef,
-    PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
+    PutRetentionSettingsRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
     MediaCapturePipelineTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_structure() -> AccountSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.0/README.md` & `mypy-boto3-chime-1.28.12/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-chime
+Version: 1.28.12
+Summary: Type annotations for boto3.Chime 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,48 +370,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
+    AccountSettingsOutputTypeDef,
     AccountSettingsTypeDef,
-    SigninDelegateGroupTypeDef,
+    SigninDelegateGroupOutputTypeDef,
     AddressTypeDef,
+    AlexaForBusinessMetadataOutputTypeDef,
     AlexaForBusinessMetadataTypeDef,
     IdentityTypeDef,
+    ChannelRetentionSettingsOutputTypeDef,
     ChannelRetentionSettingsTypeDef,
+    AppInstanceStreamingConfigurationOutputTypeDef,
     AppInstanceStreamingConfigurationTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     AppInstanceUserMembershipSummaryTypeDef,
     AppInstanceUserSummaryTypeDef,
     AppInstanceUserTypeDef,
+    AudioArtifactsConfigurationOutputTypeDef,
+    ContentArtifactsConfigurationOutputTypeDef,
+    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
+    SigninDelegateGroupTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     BatchSuspendUserRequestRequestTypeDef,
     UserErrorTypeDef,
     BatchUnsuspendUserRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     BotTypeDef,
+    BusinessCallingSettingsOutputTypeDef,
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
+    ConversationRetentionSettingsOutputTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
@@ -400,14 +442,15 @@
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     CreateUserRequestRequestTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     CredentialTypeDef,
+    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeleteAccountRequestRequestTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
@@ -446,59 +489,61 @@
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
+    GeoMatchParamsOutputTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetEventsConfigurationRequestRequestTypeDef,
-    VoiceConnectorSettingsTypeDef,
+    VoiceConnectorSettingsOutputTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationOutputTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
     GetUserSettingsRequestRequestTypeDef,
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
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
     ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
@@ -519,41 +564,51 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
+    LoggingConfigurationTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
+    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
     PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
     RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
+    RoomRetentionSettingsOutputTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
     SendChannelMessageResponseTypeDef,
+    SipMediaApplicationEndpointOutputTypeDef,
+    SipRuleTargetApplicationOutputTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
+    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
+    TelephonySettingsOutputTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
     UpdateAppInstanceResponseTypeDef,
@@ -562,29 +617,30 @@
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    VoiceConnectorItemOutputTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
-    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
+    UserTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
-    UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
@@ -593,29 +649,32 @@
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateChannelBanResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    AppInstanceRetentionSettingsOutputTypeDef,
     AppInstanceRetentionSettingsTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     ListAppInstancesResponseTypeDef,
     DescribeAppInstanceResponseTypeDef,
     ListAppInstanceUsersResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
+    ArtifactsConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -632,159 +691,166 @@
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
-    ListAttendeeTagsResponseTypeDef,
-    ListMeetingTagsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagAttendeeRequestRequestTypeDef,
     TagMeetingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     ListRoomsResponseTypeDef,
     UpdateRoomResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
-    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
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
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
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
     InviteUsersResponseTypeDef,
+    ListAttendeeTagsResponseTypeDef,
+    ListMeetingTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    RetentionSettingsOutputTypeDef,
     RetentionSettingsTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    SipMediaApplicationTypeDef,
+    SipRuleTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
+    UserSettingsOutputTypeDef,
     UserSettingsTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
-    BatchUpdateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     ResetPersonalPINResponseTypeDef,
     UpdateUserResponseTypeDef,
+    BatchUpdateUserRequestRequestTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
-    PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
+    PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
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
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
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
     GetRetentionSettingsResponseTypeDef,
-    PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
+    PutRetentionSettingsRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
     MediaCapturePipelineTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_structure() -> AccountSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/__init__.py` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/__init__.pyi` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/client.py` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/client.pyi` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/literals.py` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,15 @@
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
@@ -396,26 +397,28 @@
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

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/literals.pyi` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,15 @@
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
@@ -394,26 +395,28 @@
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

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/paginator.py` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/paginator.pyi` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/type_defs.py` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime.type_defs import AccountSettingsTypeDef
+    from mypy_boto3_chime.type_defs import AccountSettingsOutputTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -67,48 +67,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AccountSettingsOutputTypeDef",
     "AccountSettingsTypeDef",
-    "SigninDelegateGroupTypeDef",
+    "SigninDelegateGroupOutputTypeDef",
     "AddressTypeDef",
+    "AlexaForBusinessMetadataOutputTypeDef",
     "AlexaForBusinessMetadataTypeDef",
     "IdentityTypeDef",
+    "ChannelRetentionSettingsOutputTypeDef",
     "ChannelRetentionSettingsTypeDef",
+    "AppInstanceStreamingConfigurationOutputTypeDef",
     "AppInstanceStreamingConfigurationTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "AppInstanceUserMembershipSummaryTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "AppInstanceUserTypeDef",
+    "AudioArtifactsConfigurationOutputTypeDef",
+    "ContentArtifactsConfigurationOutputTypeDef",
+    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
+    "SigninDelegateGroupTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "BatchSuspendUserRequestRequestTypeDef",
     "UserErrorTypeDef",
     "BatchUnsuspendUserRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "BotTypeDef",
+    "BusinessCallingSettingsOutputTypeDef",
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
+    "ConversationRetentionSettingsOutputTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
     "CreateAppInstanceResponseTypeDef",
     "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
@@ -129,14 +139,15 @@
     "SipMediaApplicationEndpointTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "CreateUserRequestRequestTypeDef",
     "VoiceConnectorItemTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
     "CredentialTypeDef",
+    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeleteAccountRequestRequestTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
@@ -175,59 +186,61 @@
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
+    "GeoMatchParamsOutputTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetEventsConfigurationRequestRequestTypeDef",
-    "VoiceConnectorSettingsTypeDef",
+    "VoiceConnectorSettingsOutputTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
+    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetUserRequestRequestTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
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
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
     "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
@@ -248,41 +261,51 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
+    "LoggingConfigurationTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
+    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
     "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
+    "RoomRetentionSettingsOutputTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
     "SendChannelMessageResponseTypeDef",
+    "SipMediaApplicationEndpointOutputTypeDef",
+    "SipRuleTargetApplicationOutputTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
+    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
+    "TelephonySettingsOutputTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
     "UpdateAppInstanceResponseTypeDef",
@@ -291,29 +314,30 @@
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
+    "VoiceConnectorItemOutputTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+    "UserTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
-    "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
@@ -322,29 +346,32 @@
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
     "CreateAppInstanceAdminResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
+    "AppInstanceRetentionSettingsOutputTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "ListAppInstancesResponseTypeDef",
     "DescribeAppInstanceResponseTypeDef",
     "ListAppInstanceUsersResponseTypeDef",
     "DescribeAppInstanceUserResponseTypeDef",
+    "ArtifactsConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -361,168 +388,184 @@
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "CreateChannelRequestRequestTypeDef",
-    "ListAttendeeTagsResponseTypeDef",
-    "ListMeetingTagsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagAttendeeRequestRequestTypeDef",
     "TagMeetingRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "ListRoomsResponseTypeDef",
     "UpdateRoomResponseTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
-    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
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
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
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
     "InviteUsersResponseTypeDef",
+    "ListAttendeeTagsResponseTypeDef",
+    "ListMeetingTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "RetentionSettingsOutputTypeDef",
     "RetentionSettingsTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "SipMediaApplicationTypeDef",
+    "SipRuleTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
+    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    "VoiceConnectorGroupTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
-    "BatchUpdateUserRequestRequestTypeDef",
     "CreateUserResponseTypeDef",
     "GetUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ResetPersonalPINResponseTypeDef",
     "UpdateUserResponseTypeDef",
+    "BatchUpdateUserRequestRequestTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
-    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "PutAppInstanceRetentionSettingsResponseTypeDef",
+    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
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
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
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
     "GetRetentionSettingsResponseTypeDef",
-    "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
+    "PutRetentionSettingsRequestRequestTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
+    "CreateSipMediaApplicationResponseTypeDef",
+    "GetSipMediaApplicationResponseTypeDef",
+    "ListSipMediaApplicationsResponseTypeDef",
+    "UpdateSipMediaApplicationResponseTypeDef",
+    "CreateSipRuleResponseTypeDef",
+    "GetSipRuleResponseTypeDef",
+    "ListSipRulesResponseTypeDef",
+    "UpdateSipRuleResponseTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    "GetVoiceConnectorGroupResponseTypeDef",
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    "UpdateVoiceConnectorGroupResponseTypeDef",
     "MediaCapturePipelineTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
+AccountSettingsOutputTypeDef = TypedDict(
+    "AccountSettingsOutputTypeDef",
+    {
+        "DisableRemoteControl": bool,
+        "EnableDialOut": bool,
+    },
+    total=False,
+)
+
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "DisableRemoteControl": bool,
         "EnableDialOut": bool,
     },
     total=False,
 )
 
-SigninDelegateGroupTypeDef = TypedDict(
-    "SigninDelegateGroupTypeDef",
+SigninDelegateGroupOutputTypeDef = TypedDict(
+    "SigninDelegateGroupOutputTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
 AddressTypeDef = TypedDict(
@@ -538,14 +581,23 @@
         "postalCode": str,
         "postalCodePlus4": str,
         "country": str,
     },
     total=False,
 )
 
+AlexaForBusinessMetadataOutputTypeDef = TypedDict(
+    "AlexaForBusinessMetadataOutputTypeDef",
+    {
+        "IsAlexaForBusinessEnabled": bool,
+        "AlexaForBusinessRoomArn": str,
+    },
+    total=False,
+)
+
 AlexaForBusinessMetadataTypeDef = TypedDict(
     "AlexaForBusinessMetadataTypeDef",
     {
         "IsAlexaForBusinessEnabled": bool,
         "AlexaForBusinessRoomArn": str,
     },
     total=False,
@@ -556,22 +608,38 @@
     {
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
+ChannelRetentionSettingsOutputTypeDef = TypedDict(
+    "ChannelRetentionSettingsOutputTypeDef",
+    {
+        "RetentionDays": int,
+    },
+    total=False,
+)
+
 ChannelRetentionSettingsTypeDef = TypedDict(
     "ChannelRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
 
+AppInstanceStreamingConfigurationOutputTypeDef = TypedDict(
+    "AppInstanceStreamingConfigurationOutputTypeDef",
+    {
+        "AppInstanceDataType": AppInstanceDataTypeType,
+        "ResourceArn": str,
+    },
+)
+
 AppInstanceStreamingConfigurationTypeDef = TypedDict(
     "AppInstanceStreamingConfigurationTypeDef",
     {
         "AppInstanceDataType": AppInstanceDataTypeType,
         "ResourceArn": str,
     },
 )
@@ -625,14 +693,65 @@
         "CreatedTimestamp": datetime,
         "Metadata": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+AudioArtifactsConfigurationOutputTypeDef = TypedDict(
+    "AudioArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": AudioMuxTypeType,
+    },
+)
+
+_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContentArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+    },
+)
+_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContentArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": Literal["ContentOnly"],
+    },
+    total=False,
+)
+
+
+class ContentArtifactsConfigurationOutputTypeDef(
+    _RequiredContentArtifactsConfigurationOutputTypeDef,
+    _OptionalContentArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
+
+_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+    },
+)
+_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": Literal["VideoOnly"],
+    },
+    total=False,
+)
+
+
+class VideoArtifactsConfigurationOutputTypeDef(
+    _RequiredVideoArtifactsConfigurationOutputTypeDef,
+    _OptionalVideoArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
+
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -739,14 +858,22 @@
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
 
+SigninDelegateGroupTypeDef = TypedDict(
+    "SigninDelegateGroupTypeDef",
+    {
+        "GroupName": str,
+    },
+    total=False,
+)
+
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
     },
@@ -883,14 +1010,22 @@
         "UpdatedTimestamp": datetime,
         "BotEmail": str,
         "SecurityToken": str,
     },
     total=False,
 )
 
+BusinessCallingSettingsOutputTypeDef = TypedDict(
+    "BusinessCallingSettingsOutputTypeDef",
+    {
+        "CdrBucket": str,
+    },
+    total=False,
+)
+
 BusinessCallingSettingsTypeDef = TypedDict(
     "BusinessCallingSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
@@ -918,14 +1053,22 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
+ConversationRetentionSettingsOutputTypeDef = TypedDict(
+    "ConversationRetentionSettingsOutputTypeDef",
+    {
+        "RetentionDays": int,
+    },
+    total=False,
+)
+
 ConversationRetentionSettingsTypeDef = TypedDict(
     "ConversationRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -1294,14 +1437,37 @@
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
@@ -1853,14 +2019,22 @@
         "BotId": str,
         "OutboundEventsHTTPSEndpoint": str,
         "LambdaFunctionArn": str,
     },
     total=False,
 )
 
+GeoMatchParamsOutputTypeDef = TypedDict(
+    "GeoMatchParamsOutputTypeDef",
+    {
+        "Country": str,
+        "AreaCode": str,
+    },
+)
+
 GetAccountRequestRequestTypeDef = TypedDict(
     "GetAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -1927,16 +2101,16 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
 
-VoiceConnectorSettingsTypeDef = TypedDict(
-    "VoiceConnectorSettingsTypeDef",
+VoiceConnectorSettingsOutputTypeDef = TypedDict(
+    "VoiceConnectorSettingsOutputTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
@@ -2010,16 +2184,16 @@
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
@@ -2069,16 +2243,16 @@
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
 
@@ -2140,16 +2314,16 @@
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
@@ -2269,14 +2443,22 @@
     "ListAttendeeTagsRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
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
 _RequiredListAttendeesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttendeesRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 _OptionalListAttendeesRequestRequestTypeDef = TypedDict(
@@ -2698,14 +2880,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
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
 LogoutUserRequestRequestTypeDef = TypedDict(
     "LogoutUserRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
     },
 )
@@ -2742,14 +2933,26 @@
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
@@ -2820,14 +3023,22 @@
 class PutEventsConfigurationRequestRequestTypeDef(
     _RequiredPutEventsConfigurationRequestRequestTypeDef,
     _OptionalPutEventsConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
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
@@ -2845,14 +3056,26 @@
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
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
     },
 )
@@ -2929,14 +3152,22 @@
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
+RoomRetentionSettingsOutputTypeDef = TypedDict(
+    "RoomRetentionSettingsOutputTypeDef",
+    {
+        "RetentionDays": int,
+    },
+    total=False,
+)
+
 RoomRetentionSettingsTypeDef = TypedDict(
     "RoomRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -2961,14 +3192,23 @@
     {
         "E164PhoneNumbers": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
+    {
+        "AttendeeIds": List[str],
+        "ExternalUserIds": List[str],
+    },
+    total=False,
+)
+
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -3006,28 +3246,62 @@
     {
         "ChannelArn": str,
         "MessageId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
+StreamingNotificationTargetOutputTypeDef = TypedDict(
+    "StreamingNotificationTargetOutputTypeDef",
+    {
+        "NotificationTarget": NotificationTargetType,
+    },
+)
+
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
 )
 
+TelephonySettingsOutputTypeDef = TypedDict(
+    "TelephonySettingsOutputTypeDef",
+    {
+        "InboundCalling": bool,
+        "OutboundCalling": bool,
+        "SMS": bool,
+    },
+)
+
 TelephonySettingsTypeDef = TypedDict(
     "TelephonySettingsTypeDef",
     {
         "InboundCalling": bool,
         "OutboundCalling": bool,
         "SMS": bool,
     },
@@ -3255,14 +3529,22 @@
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -3385,18 +3667,26 @@
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
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
-        "AccountSettings": AccountSettingsTypeDef,
+        "AccountSettings": AccountSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
@@ -3417,32 +3707,54 @@
     "_OptionalAccountTypeDef",
     {
         "AccountType": AccountTypeType,
         "CreatedTimestamp": datetime,
         "DefaultLicense": LicenseType,
         "SupportedLicenses": List[LicenseType],
         "AccountStatus": AccountStatusType,
-        "SigninDelegateGroups": List[SigninDelegateGroupTypeDef],
+        "SigninDelegateGroups": List[SigninDelegateGroupOutputTypeDef],
     },
     total=False,
 )
 
 
 class AccountTypeDef(_RequiredAccountTypeDef, _OptionalAccountTypeDef):
     pass
 
 
-AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+_RequiredUserTypeDef = TypedDict(
+    "_RequiredUserTypeDef",
+    {
+        "UserId": str,
+    },
+)
+_OptionalUserTypeDef = TypedDict(
+    "_OptionalUserTypeDef",
     {
         "AccountId": str,
-        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
+        "PrimaryEmail": str,
+        "PrimaryProvisionedNumber": str,
+        "DisplayName": str,
+        "LicenseType": LicenseType,
+        "UserType": UserTypeType,
+        "UserRegistrationStatus": RegistrationStatusType,
+        "UserInvitationStatus": InviteStatusType,
+        "RegisteredOn": datetime,
+        "InvitedOn": datetime,
+        "AlexaForBusinessMetadata": AlexaForBusinessMetadataOutputTypeDef,
+        "PersonalPIN": str,
     },
+    total=False,
 )
 
+
+class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
+    pass
+
+
 _RequiredUpdateUserRequestItemTypeDef = TypedDict(
     "_RequiredUpdateUserRequestItemTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalUpdateUserRequestItemTypeDef = TypedDict(
@@ -3482,44 +3794,14 @@
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
-    {
-        "AccountId": str,
-        "PrimaryEmail": str,
-        "PrimaryProvisionedNumber": str,
-        "DisplayName": str,
-        "LicenseType": LicenseType,
-        "UserType": UserTypeType,
-        "UserRegistrationStatus": RegistrationStatusType,
-        "UserInvitationStatus": InviteStatusType,
-        "RegisteredOn": datetime,
-        "InvitedOn": datetime,
-        "AlexaForBusinessMetadata": AlexaForBusinessMetadataTypeDef,
-        "PersonalPIN": str,
-    },
-    total=False,
-)
-
-
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
-
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -3686,43 +3968,51 @@
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AppInstanceRetentionSettingsOutputTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsOutputTypeDef",
+    {
+        "ChannelRetentionSettings": ChannelRetentionSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AppInstanceRetentionSettingsTypeDef = TypedDict(
     "AppInstanceRetentionSettingsTypeDef",
     {
         "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
     total=False,
 )
 
 GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
     },
 )
 
 ListAppInstancesResponseTypeDef = TypedDict(
     "ListAppInstancesResponseTypeDef",
     {
         "AppInstances": List[AppInstanceSummaryTypeDef],
@@ -3753,14 +4043,23 @@
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ArtifactsConfigurationOutputTypeDef = TypedDict(
+    "ArtifactsConfigurationOutputTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationOutputTypeDef,
+        "Video": VideoArtifactsConfigurationOutputTypeDef,
+        "Content": ContentArtifactsConfigurationOutputTypeDef,
+    },
+)
+
 ArtifactsConfigurationTypeDef = TypedDict(
     "ArtifactsConfigurationTypeDef",
     {
         "Audio": AudioArtifactsConfigurationTypeDef,
         "Video": VideoArtifactsConfigurationTypeDef,
         "Content": ContentArtifactsConfigurationTypeDef,
     },
@@ -3810,14 +4109,22 @@
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
+    },
+)
+
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4089,38 +4396,14 @@
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
 
-ListAttendeeTagsResponseTypeDef = TypedDict(
-    "ListAttendeeTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListMeetingTagsResponseTypeDef = TypedDict(
-    "ListMeetingTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -4249,27 +4532,14 @@
     {
         "AwsRegion": str,
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
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
@@ -4309,29 +4579,14 @@
 
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
@@ -4378,27 +4633,14 @@
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
@@ -4446,18 +4688,26 @@
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
 
 TranscriptionConfigurationTypeDef = TypedDict(
     "TranscriptionConfigurationTypeDef",
     {
@@ -4482,95 +4732,60 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "BusinessCalling": BusinessCallingSettingsTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "BusinessCalling": BusinessCallingSettingsOutputTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    {
-        "BusinessCalling": BusinessCallingSettingsTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
-    },
-    total=False,
-)
-
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
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
@@ -4594,51 +4809,75 @@
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
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListAttendeeTagsResponseTypeDef = TypedDict(
+    "ListAttendeeTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMeetingTagsResponseTypeDef = TypedDict(
+    "ListMeetingTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
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
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
         "ExternalMeetingId": str,
         "MediaPlacement": MediaPlacementTypeDef,
         "MediaRegion": str,
@@ -4667,18 +4906,27 @@
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
@@ -4691,15 +4939,15 @@
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
@@ -4716,60 +4964,186 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationId": str,
+    },
+)
+_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+
+RetentionSettingsOutputTypeDef = TypedDict(
+    "RetentionSettingsOutputTypeDef",
+    {
+        "RoomRetentionSettings": RoomRetentionSettingsOutputTypeDef,
+        "ConversationRetentionSettings": ConversationRetentionSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+SipMediaApplicationTypeDef = TypedDict(
+    "SipMediaApplicationTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+SipRuleTypeDef = TypedDict(
+    "SipRuleTypeDef",
+    {
+        "SipRuleId": str,
+        "Name": str,
+        "Disabled": bool,
+        "TriggerType": SipRuleTriggerTypeType,
+        "TriggerValue": str,
+        "TargetApplications": List[SipRuleTargetApplicationOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationOutputTypeDef",
+    {
+        "DataRetentionInHours": int,
+    },
+)
+_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class StreamingConfigurationOutputTypeDef(
+    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
 
+UserSettingsOutputTypeDef = TypedDict(
+    "UserSettingsOutputTypeDef",
+    {
+        "Telephony": TelephonySettingsOutputTypeDef,
+    },
+)
+
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "Telephony": TelephonySettingsTypeDef,
     },
 )
 
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    {
+        "BusinessCalling": BusinessCallingSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+    },
+    total=False,
+)
+
+VoiceConnectorGroupTypeDef = TypedDict(
+    "VoiceConnectorGroupTypeDef",
+    {
+        "VoiceConnectorGroupId": str,
+        "Name": str,
+        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "VoiceConnectorGroupArn": str,
+    },
+    total=False,
+)
+
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4795,22 +5169,14 @@
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchUpdateUserRequestRequestTypeDef = TypedDict(
-    "BatchUpdateUserRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
-    },
-)
-
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4844,14 +5210,22 @@
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchUpdateUserRequestRequestTypeDef = TypedDict(
+    "BatchUpdateUserRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
+    },
+)
+
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4954,34 +5328,34 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
         "InitiateDeletionTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
+PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsResponseTypeDef",
+PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
+        "AppInstanceArn": str,
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
@@ -5046,137 +5420,38 @@
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSipMediaApplicationResponseTypeDef = TypedDict(
-    "CreateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipMediaApplicationResponseTypeDef = TypedDict(
-    "GetSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipMediaApplicationsResponseTypeDef = TypedDict(
-    "ListSipMediaApplicationsResponseTypeDef",
-    {
-        "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipMediaApplicationResponseTypeDef = TypedDict(
-    "UpdateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSipRuleResponseTypeDef = TypedDict(
-    "CreateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipRuleResponseTypeDef = TypedDict(
-    "GetSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipRulesResponseTypeDef = TypedDict(
-    "ListSipRulesResponseTypeDef",
-    {
-        "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipRuleResponseTypeDef = TypedDict(
-    "UpdateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "GetVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    {
-        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "UpdateVoiceConnectorGroupResponseTypeDef",
+GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
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
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
         "TranscriptionConfiguration": TranscriptionConfigurationTypeDef,
     },
 )
@@ -5265,32 +5540,32 @@
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
@@ -5355,87 +5630,211 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
-        "RetentionSettings": RetentionSettingsTypeDef,
+        "RetentionSettings": RetentionSettingsOutputTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutRetentionSettingsResponseTypeDef = TypedDict(
+    "PutRetentionSettingsResponseTypeDef",
+    {
+        "RetentionSettings": RetentionSettingsOutputTypeDef,
         "InitiateDeletionTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutRetentionSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "RetentionSettings": RetentionSettingsTypeDef,
     },
 )
 
-PutRetentionSettingsResponseTypeDef = TypedDict(
-    "PutRetentionSettingsResponseTypeDef",
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
-        "RetentionSettings": RetentionSettingsTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "SipMediaApplication": SipMediaApplicationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
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
+GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
+    {
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "StreamingConfiguration": StreamingConfigurationTypeDef,
+    },
+)
+
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
-        "UserSettings": UserSettingsTypeDef,
+        "UserSettings": UserSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
     },
 )
 
+CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    {
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
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+MediaCapturePipelineTypeDef = TypedDict(
+    "MediaCapturePipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "Status": MediaPipelineStatusType,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -5454,30 +5853,14 @@
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
 
-MediaCapturePipelineTypeDef = TypedDict(
-    "MediaCapturePipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "Status": MediaPipelineStatusType,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
-    },
-    total=False,
-)
-
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime/type_defs.pyi` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime.type_defs import AccountSettingsTypeDef
+    from mypy_boto3_chime.type_defs import AccountSettingsOutputTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -66,48 +66,58 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccountSettingsOutputTypeDef",
     "AccountSettingsTypeDef",
-    "SigninDelegateGroupTypeDef",
+    "SigninDelegateGroupOutputTypeDef",
     "AddressTypeDef",
+    "AlexaForBusinessMetadataOutputTypeDef",
     "AlexaForBusinessMetadataTypeDef",
     "IdentityTypeDef",
+    "ChannelRetentionSettingsOutputTypeDef",
     "ChannelRetentionSettingsTypeDef",
+    "AppInstanceStreamingConfigurationOutputTypeDef",
     "AppInstanceStreamingConfigurationTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "AppInstanceUserMembershipSummaryTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "AppInstanceUserTypeDef",
+    "AudioArtifactsConfigurationOutputTypeDef",
+    "ContentArtifactsConfigurationOutputTypeDef",
+    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
+    "SigninDelegateGroupTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "BatchSuspendUserRequestRequestTypeDef",
     "UserErrorTypeDef",
     "BatchUnsuspendUserRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "BotTypeDef",
+    "BusinessCallingSettingsOutputTypeDef",
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
+    "ConversationRetentionSettingsOutputTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
     "CreateAppInstanceResponseTypeDef",
     "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
@@ -128,14 +138,15 @@
     "SipMediaApplicationEndpointTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "CreateUserRequestRequestTypeDef",
     "VoiceConnectorItemTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
     "CredentialTypeDef",
+    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeleteAccountRequestRequestTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
@@ -174,59 +185,61 @@
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
+    "GeoMatchParamsOutputTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetEventsConfigurationRequestRequestTypeDef",
-    "VoiceConnectorSettingsTypeDef",
+    "VoiceConnectorSettingsOutputTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
+    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetUserRequestRequestTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
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
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
     "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
@@ -247,41 +260,51 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
+    "LoggingConfigurationTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
+    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
     "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
+    "RoomRetentionSettingsOutputTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
     "SendChannelMessageResponseTypeDef",
+    "SipMediaApplicationEndpointOutputTypeDef",
+    "SipRuleTargetApplicationOutputTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
+    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
+    "TelephonySettingsOutputTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
     "UpdateAppInstanceResponseTypeDef",
@@ -290,29 +313,30 @@
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
+    "VoiceConnectorItemOutputTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+    "UserTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
-    "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
@@ -321,29 +345,32 @@
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
     "CreateAppInstanceAdminResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
+    "AppInstanceRetentionSettingsOutputTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "ListAppInstancesResponseTypeDef",
     "DescribeAppInstanceResponseTypeDef",
     "ListAppInstanceUsersResponseTypeDef",
     "DescribeAppInstanceUserResponseTypeDef",
+    "ArtifactsConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -360,168 +387,184 @@
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "CreateChannelRequestRequestTypeDef",
-    "ListAttendeeTagsResponseTypeDef",
-    "ListMeetingTagsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagAttendeeRequestRequestTypeDef",
     "TagMeetingRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "ListRoomsResponseTypeDef",
     "UpdateRoomResponseTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
-    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
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
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
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
     "InviteUsersResponseTypeDef",
+    "ListAttendeeTagsResponseTypeDef",
+    "ListMeetingTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "RetentionSettingsOutputTypeDef",
     "RetentionSettingsTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "SipMediaApplicationTypeDef",
+    "SipRuleTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
+    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    "VoiceConnectorGroupTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
-    "BatchUpdateUserRequestRequestTypeDef",
     "CreateUserResponseTypeDef",
     "GetUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ResetPersonalPINResponseTypeDef",
     "UpdateUserResponseTypeDef",
+    "BatchUpdateUserRequestRequestTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
-    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "PutAppInstanceRetentionSettingsResponseTypeDef",
+    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
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
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
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
     "GetRetentionSettingsResponseTypeDef",
-    "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
+    "PutRetentionSettingsRequestRequestTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
+    "CreateSipMediaApplicationResponseTypeDef",
+    "GetSipMediaApplicationResponseTypeDef",
+    "ListSipMediaApplicationsResponseTypeDef",
+    "UpdateSipMediaApplicationResponseTypeDef",
+    "CreateSipRuleResponseTypeDef",
+    "GetSipRuleResponseTypeDef",
+    "ListSipRulesResponseTypeDef",
+    "UpdateSipRuleResponseTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    "GetVoiceConnectorGroupResponseTypeDef",
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    "UpdateVoiceConnectorGroupResponseTypeDef",
     "MediaCapturePipelineTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
+AccountSettingsOutputTypeDef = TypedDict(
+    "AccountSettingsOutputTypeDef",
+    {
+        "DisableRemoteControl": bool,
+        "EnableDialOut": bool,
+    },
+    total=False,
+)
+
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "DisableRemoteControl": bool,
         "EnableDialOut": bool,
     },
     total=False,
 )
 
-SigninDelegateGroupTypeDef = TypedDict(
-    "SigninDelegateGroupTypeDef",
+SigninDelegateGroupOutputTypeDef = TypedDict(
+    "SigninDelegateGroupOutputTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
 AddressTypeDef = TypedDict(
@@ -537,14 +580,23 @@
         "postalCode": str,
         "postalCodePlus4": str,
         "country": str,
     },
     total=False,
 )
 
+AlexaForBusinessMetadataOutputTypeDef = TypedDict(
+    "AlexaForBusinessMetadataOutputTypeDef",
+    {
+        "IsAlexaForBusinessEnabled": bool,
+        "AlexaForBusinessRoomArn": str,
+    },
+    total=False,
+)
+
 AlexaForBusinessMetadataTypeDef = TypedDict(
     "AlexaForBusinessMetadataTypeDef",
     {
         "IsAlexaForBusinessEnabled": bool,
         "AlexaForBusinessRoomArn": str,
     },
     total=False,
@@ -555,22 +607,38 @@
     {
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
+ChannelRetentionSettingsOutputTypeDef = TypedDict(
+    "ChannelRetentionSettingsOutputTypeDef",
+    {
+        "RetentionDays": int,
+    },
+    total=False,
+)
+
 ChannelRetentionSettingsTypeDef = TypedDict(
     "ChannelRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
 
+AppInstanceStreamingConfigurationOutputTypeDef = TypedDict(
+    "AppInstanceStreamingConfigurationOutputTypeDef",
+    {
+        "AppInstanceDataType": AppInstanceDataTypeType,
+        "ResourceArn": str,
+    },
+)
+
 AppInstanceStreamingConfigurationTypeDef = TypedDict(
     "AppInstanceStreamingConfigurationTypeDef",
     {
         "AppInstanceDataType": AppInstanceDataTypeType,
         "ResourceArn": str,
     },
 )
@@ -624,14 +692,61 @@
         "CreatedTimestamp": datetime,
         "Metadata": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+AudioArtifactsConfigurationOutputTypeDef = TypedDict(
+    "AudioArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": AudioMuxTypeType,
+    },
+)
+
+_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContentArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+    },
+)
+_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContentArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": Literal["ContentOnly"],
+    },
+    total=False,
+)
+
+class ContentArtifactsConfigurationOutputTypeDef(
+    _RequiredContentArtifactsConfigurationOutputTypeDef,
+    _OptionalContentArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "State": ArtifactsStateType,
+    },
+)
+_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
+    {
+        "MuxType": Literal["VideoOnly"],
+    },
+    total=False,
+)
+
+class VideoArtifactsConfigurationOutputTypeDef(
+    _RequiredVideoArtifactsConfigurationOutputTypeDef,
+    _OptionalVideoArtifactsConfigurationOutputTypeDef,
+):
+    pass
+
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -730,14 +845,22 @@
 
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
+SigninDelegateGroupTypeDef = TypedDict(
+    "SigninDelegateGroupTypeDef",
+    {
+        "GroupName": str,
+    },
+    total=False,
+)
+
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
     },
@@ -870,14 +993,22 @@
         "UpdatedTimestamp": datetime,
         "BotEmail": str,
         "SecurityToken": str,
     },
     total=False,
 )
 
+BusinessCallingSettingsOutputTypeDef = TypedDict(
+    "BusinessCallingSettingsOutputTypeDef",
+    {
+        "CdrBucket": str,
+    },
+    total=False,
+)
+
 BusinessCallingSettingsTypeDef = TypedDict(
     "BusinessCallingSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
@@ -905,14 +1036,22 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
+ConversationRetentionSettingsOutputTypeDef = TypedDict(
+    "ConversationRetentionSettingsOutputTypeDef",
+    {
+        "RetentionDays": int,
+    },
+    total=False,
+)
+
 ConversationRetentionSettingsTypeDef = TypedDict(
     "ConversationRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -1263,14 +1402,35 @@
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
@@ -1796,14 +1956,22 @@
         "BotId": str,
         "OutboundEventsHTTPSEndpoint": str,
         "LambdaFunctionArn": str,
     },
     total=False,
 )
 
+GeoMatchParamsOutputTypeDef = TypedDict(
+    "GeoMatchParamsOutputTypeDef",
+    {
+        "Country": str,
+        "AreaCode": str,
+    },
+)
+
 GetAccountRequestRequestTypeDef = TypedDict(
     "GetAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -1868,16 +2036,16 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
 
-VoiceConnectorSettingsTypeDef = TypedDict(
-    "VoiceConnectorSettingsTypeDef",
+VoiceConnectorSettingsOutputTypeDef = TypedDict(
+    "VoiceConnectorSettingsOutputTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
@@ -1951,16 +2119,16 @@
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
@@ -2010,16 +2178,16 @@
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
 
@@ -2081,16 +2249,16 @@
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
@@ -2204,14 +2372,22 @@
     "ListAttendeeTagsRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
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
 _RequiredListAttendeesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttendeesRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 _OptionalListAttendeesRequestRequestTypeDef = TypedDict(
@@ -2609,14 +2785,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
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
 LogoutUserRequestRequestTypeDef = TypedDict(
     "LogoutUserRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
     },
 )
@@ -2653,14 +2838,26 @@
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
@@ -2729,14 +2926,22 @@
 
 class PutEventsConfigurationRequestRequestTypeDef(
     _RequiredPutEventsConfigurationRequestRequestTypeDef,
     _OptionalPutEventsConfigurationRequestRequestTypeDef,
 ):
     pass
 
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
@@ -2752,14 +2957,26 @@
 
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
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
     },
 )
@@ -2834,14 +3051,22 @@
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
+RoomRetentionSettingsOutputTypeDef = TypedDict(
+    "RoomRetentionSettingsOutputTypeDef",
+    {
+        "RetentionDays": int,
+    },
+    total=False,
+)
+
 RoomRetentionSettingsTypeDef = TypedDict(
     "RoomRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -2866,14 +3091,23 @@
     {
         "E164PhoneNumbers": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
+    {
+        "AttendeeIds": List[str],
+        "ExternalUserIds": List[str],
+    },
+    total=False,
+)
+
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -2909,28 +3143,62 @@
     {
         "ChannelArn": str,
         "MessageId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
+StreamingNotificationTargetOutputTypeDef = TypedDict(
+    "StreamingNotificationTargetOutputTypeDef",
+    {
+        "NotificationTarget": NotificationTargetType,
+    },
+)
+
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
 )
 
+TelephonySettingsOutputTypeDef = TypedDict(
+    "TelephonySettingsOutputTypeDef",
+    {
+        "InboundCalling": bool,
+        "OutboundCalling": bool,
+        "SMS": bool,
+    },
+)
+
 TelephonySettingsTypeDef = TypedDict(
     "TelephonySettingsTypeDef",
     {
         "InboundCalling": bool,
         "OutboundCalling": bool,
         "SMS": bool,
     },
@@ -3144,14 +3412,22 @@
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -3266,18 +3542,26 @@
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
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
-        "AccountSettings": AccountSettingsTypeDef,
+        "AccountSettings": AccountSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
@@ -3298,30 +3582,50 @@
     "_OptionalAccountTypeDef",
     {
         "AccountType": AccountTypeType,
         "CreatedTimestamp": datetime,
         "DefaultLicense": LicenseType,
         "SupportedLicenses": List[LicenseType],
         "AccountStatus": AccountStatusType,
-        "SigninDelegateGroups": List[SigninDelegateGroupTypeDef],
+        "SigninDelegateGroups": List[SigninDelegateGroupOutputTypeDef],
     },
     total=False,
 )
 
 class AccountTypeDef(_RequiredAccountTypeDef, _OptionalAccountTypeDef):
     pass
 
-AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+_RequiredUserTypeDef = TypedDict(
+    "_RequiredUserTypeDef",
+    {
+        "UserId": str,
+    },
+)
+_OptionalUserTypeDef = TypedDict(
+    "_OptionalUserTypeDef",
     {
         "AccountId": str,
-        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
+        "PrimaryEmail": str,
+        "PrimaryProvisionedNumber": str,
+        "DisplayName": str,
+        "LicenseType": LicenseType,
+        "UserType": UserTypeType,
+        "UserRegistrationStatus": RegistrationStatusType,
+        "UserInvitationStatus": InviteStatusType,
+        "RegisteredOn": datetime,
+        "InvitedOn": datetime,
+        "AlexaForBusinessMetadata": AlexaForBusinessMetadataOutputTypeDef,
+        "PersonalPIN": str,
     },
+    total=False,
 )
 
+class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
+    pass
+
 _RequiredUpdateUserRequestItemTypeDef = TypedDict(
     "_RequiredUpdateUserRequestItemTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalUpdateUserRequestItemTypeDef = TypedDict(
@@ -3357,42 +3661,14 @@
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
-    {
-        "AccountId": str,
-        "PrimaryEmail": str,
-        "PrimaryProvisionedNumber": str,
-        "DisplayName": str,
-        "LicenseType": LicenseType,
-        "UserType": UserTypeType,
-        "UserRegistrationStatus": RegistrationStatusType,
-        "UserInvitationStatus": InviteStatusType,
-        "RegisteredOn": datetime,
-        "InvitedOn": datetime,
-        "AlexaForBusinessMetadata": AlexaForBusinessMetadataTypeDef,
-        "PersonalPIN": str,
-    },
-    total=False,
-)
-
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -3559,43 +3835,51 @@
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AppInstanceRetentionSettingsOutputTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsOutputTypeDef",
+    {
+        "ChannelRetentionSettings": ChannelRetentionSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 AppInstanceRetentionSettingsTypeDef = TypedDict(
     "AppInstanceRetentionSettingsTypeDef",
     {
         "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
     total=False,
 )
 
 GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
     },
 )
 
 ListAppInstancesResponseTypeDef = TypedDict(
     "ListAppInstancesResponseTypeDef",
     {
         "AppInstances": List[AppInstanceSummaryTypeDef],
@@ -3626,14 +3910,23 @@
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ArtifactsConfigurationOutputTypeDef = TypedDict(
+    "ArtifactsConfigurationOutputTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationOutputTypeDef,
+        "Video": VideoArtifactsConfigurationOutputTypeDef,
+        "Content": ContentArtifactsConfigurationOutputTypeDef,
+    },
+)
+
 ArtifactsConfigurationTypeDef = TypedDict(
     "ArtifactsConfigurationTypeDef",
     {
         "Audio": AudioArtifactsConfigurationTypeDef,
         "Video": VideoArtifactsConfigurationTypeDef,
         "Content": ContentArtifactsConfigurationTypeDef,
     },
@@ -3683,14 +3976,22 @@
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
+    },
+)
+
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3952,38 +4253,14 @@
 )
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-ListAttendeeTagsResponseTypeDef = TypedDict(
-    "ListAttendeeTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListMeetingTagsResponseTypeDef = TypedDict(
-    "ListMeetingTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -4108,27 +4385,14 @@
     {
         "AwsRegion": str,
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
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
@@ -4164,29 +4428,14 @@
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
@@ -4229,27 +4478,14 @@
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
@@ -4295,18 +4531,26 @@
 
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
 
 TranscriptionConfigurationTypeDef = TypedDict(
     "TranscriptionConfigurationTypeDef",
     {
@@ -4331,93 +4575,60 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "BusinessCalling": BusinessCallingSettingsTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "BusinessCalling": BusinessCallingSettingsOutputTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    {
-        "BusinessCalling": BusinessCallingSettingsTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
-    },
-    total=False,
-)
-
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
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
@@ -4441,51 +4652,75 @@
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
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListAttendeeTagsResponseTypeDef = TypedDict(
+    "ListAttendeeTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMeetingTagsResponseTypeDef = TypedDict(
+    "ListMeetingTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
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
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
         "ExternalMeetingId": str,
         "MediaPlacement": MediaPlacementTypeDef,
         "MediaRegion": str,
@@ -4514,18 +4749,27 @@
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
@@ -4538,15 +4782,15 @@
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
@@ -4563,58 +4807,180 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationId": str,
+    },
+)
+_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+
+RetentionSettingsOutputTypeDef = TypedDict(
+    "RetentionSettingsOutputTypeDef",
+    {
+        "RoomRetentionSettings": RoomRetentionSettingsOutputTypeDef,
+        "ConversationRetentionSettings": ConversationRetentionSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+SipMediaApplicationTypeDef = TypedDict(
+    "SipMediaApplicationTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+SipRuleTypeDef = TypedDict(
+    "SipRuleTypeDef",
+    {
+        "SipRuleId": str,
+        "Name": str,
+        "Disabled": bool,
+        "TriggerType": SipRuleTriggerTypeType,
+        "TriggerValue": str,
+        "TargetApplications": List[SipRuleTargetApplicationOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationOutputTypeDef",
+    {
+        "DataRetentionInHours": int,
+    },
+)
+_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
+    },
+    total=False,
+)
+
+class StreamingConfigurationOutputTypeDef(
+    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
+UserSettingsOutputTypeDef = TypedDict(
+    "UserSettingsOutputTypeDef",
+    {
+        "Telephony": TelephonySettingsOutputTypeDef,
+    },
+)
+
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "Telephony": TelephonySettingsTypeDef,
     },
 )
 
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    {
+        "BusinessCalling": BusinessCallingSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+    },
+    total=False,
+)
+
+VoiceConnectorGroupTypeDef = TypedDict(
+    "VoiceConnectorGroupTypeDef",
+    {
+        "VoiceConnectorGroupId": str,
+        "Name": str,
+        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "VoiceConnectorGroupArn": str,
+    },
+    total=False,
+)
+
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4640,22 +5006,14 @@
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchUpdateUserRequestRequestTypeDef = TypedDict(
-    "BatchUpdateUserRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
-    },
-)
-
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4689,14 +5047,22 @@
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchUpdateUserRequestRequestTypeDef = TypedDict(
+    "BatchUpdateUserRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
+    },
+)
+
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4799,34 +5165,34 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
         "InitiateDeletionTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
+PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsResponseTypeDef",
+PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
+        "AppInstanceArn": str,
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
@@ -4889,137 +5255,38 @@
 
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
-CreateSipMediaApplicationResponseTypeDef = TypedDict(
-    "CreateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipMediaApplicationResponseTypeDef = TypedDict(
-    "GetSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipMediaApplicationsResponseTypeDef = TypedDict(
-    "ListSipMediaApplicationsResponseTypeDef",
-    {
-        "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipMediaApplicationResponseTypeDef = TypedDict(
-    "UpdateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSipRuleResponseTypeDef = TypedDict(
-    "CreateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipRuleResponseTypeDef = TypedDict(
-    "GetSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipRulesResponseTypeDef = TypedDict(
-    "ListSipRulesResponseTypeDef",
-    {
-        "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipRuleResponseTypeDef = TypedDict(
-    "UpdateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "GetVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorGroupsResponseTypeDef",
+GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "UpdateVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
         "TranscriptionConfiguration": TranscriptionConfigurationTypeDef,
     },
 )
@@ -5108,32 +5375,32 @@
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
@@ -5198,127 +5465,235 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
-        "RetentionSettings": RetentionSettingsTypeDef,
+        "RetentionSettings": RetentionSettingsOutputTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutRetentionSettingsResponseTypeDef = TypedDict(
+    "PutRetentionSettingsResponseTypeDef",
+    {
+        "RetentionSettings": RetentionSettingsOutputTypeDef,
         "InitiateDeletionTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutRetentionSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "RetentionSettings": RetentionSettingsTypeDef,
     },
 )
 
-PutRetentionSettingsResponseTypeDef = TypedDict(
-    "PutRetentionSettingsResponseTypeDef",
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
-        "RetentionSettings": RetentionSettingsTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "SipMediaApplication": SipMediaApplicationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
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
+GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
+    {
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "StreamingConfiguration": StreamingConfigurationTypeDef,
+    },
+)
+
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
-        "UserSettings": UserSettingsTypeDef,
+        "UserSettings": UserSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
     },
 )
 
-_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
+CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "CreateVoiceConnectorGroupResponseTypeDef",
     {
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
+
+GetVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "GetVoiceConnectorGroupResponseTypeDef",
     {
-        "ClientRequestToken": str,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class CreateMediaCapturePipelineRequestRequestTypeDef(
-    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
-    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
-):
-    pass
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
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "Status": MediaPipelineStatusType,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
+    {
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
+    },
+)
+_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
     },
     total=False,
 )
 
+class CreateMediaCapturePipelineRequestRequestTypeDef(
+    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
+    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
+):
+    pass
+
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/PKG-INFO` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.28.0
-Summary: Type annotations for boto3.Chime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Chime 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,48 +370,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
+    AccountSettingsOutputTypeDef,
     AccountSettingsTypeDef,
-    SigninDelegateGroupTypeDef,
+    SigninDelegateGroupOutputTypeDef,
     AddressTypeDef,
+    AlexaForBusinessMetadataOutputTypeDef,
     AlexaForBusinessMetadataTypeDef,
     IdentityTypeDef,
+    ChannelRetentionSettingsOutputTypeDef,
     ChannelRetentionSettingsTypeDef,
+    AppInstanceStreamingConfigurationOutputTypeDef,
     AppInstanceStreamingConfigurationTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     AppInstanceUserMembershipSummaryTypeDef,
     AppInstanceUserSummaryTypeDef,
     AppInstanceUserTypeDef,
+    AudioArtifactsConfigurationOutputTypeDef,
+    ContentArtifactsConfigurationOutputTypeDef,
+    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
+    SigninDelegateGroupTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     BatchSuspendUserRequestRequestTypeDef,
     UserErrorTypeDef,
     BatchUnsuspendUserRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     BotTypeDef,
+    BusinessCallingSettingsOutputTypeDef,
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
+    ConversationRetentionSettingsOutputTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
@@ -432,14 +442,15 @@
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     CreateUserRequestRequestTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     CredentialTypeDef,
+    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeleteAccountRequestRequestTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
@@ -478,59 +489,61 @@
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
+    GeoMatchParamsOutputTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetEventsConfigurationRequestRequestTypeDef,
-    VoiceConnectorSettingsTypeDef,
+    VoiceConnectorSettingsOutputTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
+    SipMediaApplicationLoggingConfigurationOutputTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
     GetUserSettingsRequestRequestTypeDef,
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
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
     ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
@@ -551,41 +564,51 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
+    LoggingConfigurationTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
+    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
     PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
     RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
+    RoomRetentionSettingsOutputTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
     SendChannelMessageResponseTypeDef,
+    SipMediaApplicationEndpointOutputTypeDef,
+    SipRuleTargetApplicationOutputTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
+    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
+    TelephonySettingsOutputTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
     UpdateAppInstanceResponseTypeDef,
@@ -594,29 +617,30 @@
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    VoiceConnectorItemOutputTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
-    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
+    UserTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
-    UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
@@ -625,29 +649,32 @@
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateChannelBanResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    AppInstanceRetentionSettingsOutputTypeDef,
     AppInstanceRetentionSettingsTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     ListAppInstancesResponseTypeDef,
     DescribeAppInstanceResponseTypeDef,
     ListAppInstanceUsersResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
+    ArtifactsConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -664,159 +691,166 @@
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
-    ListAttendeeTagsResponseTypeDef,
-    ListMeetingTagsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagAttendeeRequestRequestTypeDef,
     TagMeetingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     ListRoomsResponseTypeDef,
     UpdateRoomResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
-    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
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
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
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
     InviteUsersResponseTypeDef,
+    ListAttendeeTagsResponseTypeDef,
+    ListMeetingTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    RetentionSettingsOutputTypeDef,
     RetentionSettingsTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    SipMediaApplicationTypeDef,
+    SipRuleTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
+    UserSettingsOutputTypeDef,
     UserSettingsTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
-    BatchUpdateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     ResetPersonalPINResponseTypeDef,
     UpdateUserResponseTypeDef,
+    BatchUpdateUserRequestRequestTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
-    PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
+    PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
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
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
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
     GetRetentionSettingsResponseTypeDef,
-    PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
+    PutRetentionSettingsRequestRequestTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
     MediaCapturePipelineTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_structure() -> AccountSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.0/mypy_boto3_chime.egg-info/SOURCES.txt` & `mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.0/setup.py` & `mypy-boto3-chime-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Chime 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Chime 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

