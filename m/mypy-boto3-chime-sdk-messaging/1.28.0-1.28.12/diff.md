# Comparing `tmp/mypy-boto3-chime-sdk-messaging-1.28.0.tar.gz` & `tmp/mypy-boto3-chime-sdk-messaging-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.28.0.tar", last modified: Thu Jul  6 20:59:07 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.28.12.tar", last modified: Thu Jul 27 05:34:23 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-messaging-1.28.0.tar` & `mypy-boto3-chime-sdk-messaging-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:07.170238 mypy-boto3-chime-sdk-messaging-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-06 20:59:07.162238 mypy-boto3-chime-sdk-messaging-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16808 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:07.162238 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-06 20:34:46.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47641 2023-07-06 20:34:48.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47584 2023-07-06 20:34:47.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:07.162238 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-06 20:59:06.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 20:59:06.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:06.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:06.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:06.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 20:59:06.000000 mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:07.170238 mypy-boto3-chime-sdk-messaging-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-06 20:34:45.000000 mypy-boto3-chime-sdk-messaging-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.944565 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50483 2023-07-27 05:18:19.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50424 2023-07-27 05:18:19.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/setup.py
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/LICENSE` & `mypy-boto3-chime-sdk-messaging-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime-sdk-messaging"></a>
 
 # mypy-boto3-chime-sdk-messaging
 
 [![PyPI - mypy-boto3-chime-sdk-messaging](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,26 +321,30 @@
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
     ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
+    PushNotificationPreferencesOutputTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
-    TargetTypeDef,
-    ElasticChannelConfigurationTypeDef,
-    ExpirationSettingsTypeDef,
+    MessageAttributeValueOutputTypeDef,
+    TargetOutputTypeDef,
+    ElasticChannelConfigurationOutputTypeDef,
+    ExpirationSettingsOutputTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
     CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
@@ -355,32 +359,36 @@
     DisassociateChannelFlowRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationOutputTypeDef,
+    LambdaConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    StreamingConfigurationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
     RedactChannelMessageResponseTypeDef,
     ResponseMetadataTypeDef,
     SearchFieldTypeDef,
+    TargetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
@@ -395,53 +403,56 @@
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
+    ChannelMembershipPreferencesOutputTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
-    PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
-    CreateChannelRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateChannelRequestRequestTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
-    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
+    ProcessorConfigurationOutputTypeDef,
     ProcessorConfigurationTypeDef,
     ListSubChannelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     SearchChannelsRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
-    PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
+    PutChannelMembershipPreferencesRequestRequestTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/README.md` & `mypy-boto3-chime-sdk-messaging-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-messaging"></a>
 
 # mypy-boto3-chime-sdk-messaging
 
 [![PyPI - mypy-boto3-chime-sdk-messaging](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,26 +289,30 @@
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
     ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
+    PushNotificationPreferencesOutputTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
-    TargetTypeDef,
-    ElasticChannelConfigurationTypeDef,
-    ExpirationSettingsTypeDef,
+    MessageAttributeValueOutputTypeDef,
+    TargetOutputTypeDef,
+    ElasticChannelConfigurationOutputTypeDef,
+    ExpirationSettingsOutputTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
     CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
@@ -323,32 +327,36 @@
     DisassociateChannelFlowRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationOutputTypeDef,
+    LambdaConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    StreamingConfigurationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
     RedactChannelMessageResponseTypeDef,
     ResponseMetadataTypeDef,
     SearchFieldTypeDef,
+    TargetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
@@ -363,53 +371,56 @@
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
+    ChannelMembershipPreferencesOutputTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
-    PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
-    CreateChannelRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateChannelRequestRequestTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
-    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
+    ProcessorConfigurationOutputTypeDef,
     ProcessorConfigurationTypeDef,
     ListSubChannelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     SearchChannelsRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
-    PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
+    PutChannelMembershipPreferencesRequestRequestTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/__main__.py` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMessaging 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMessaging 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/client.py` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/client.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/literals.py` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
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
@@ -277,26 +278,28 @@
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/literals.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
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
@@ -275,26 +276,28 @@
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/type_defs.py` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -37,36 +37,39 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
     "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
+    "PushNotificationPreferencesOutputTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
-    "TargetTypeDef",
-    "ElasticChannelConfigurationTypeDef",
-    "ExpirationSettingsTypeDef",
+    "MessageAttributeValueOutputTypeDef",
+    "TargetOutputTypeDef",
+    "ElasticChannelConfigurationOutputTypeDef",
+    "ExpirationSettingsOutputTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
     "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
+    "ElasticChannelConfigurationTypeDef",
+    "ExpirationSettingsTypeDef",
     "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
@@ -81,32 +84,36 @@
     "DisassociateChannelFlowRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
-    "StreamingConfigurationTypeDef",
+    "StreamingConfigurationOutputTypeDef",
+    "LambdaConfigurationOutputTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "StreamingConfigurationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
     "RedactChannelMessageResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
+    "TargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
@@ -121,53 +128,56 @@
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
+    "ChannelMembershipPreferencesOutputTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
-    "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
-    "CreateChannelRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateChannelRequestRequestTypeDef",
+    "PutChannelExpirationSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
+    "ProcessorConfigurationOutputTypeDef",
     "ProcessorConfigurationTypeDef",
     "ListSubChannelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "SearchChannelsRequestRequestTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
-    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
+    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
+    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
     "UpdateChannelFlowRequestRequestTypeDef",
     "ListChannelFlowsResponseTypeDef",
     "DescribeChannelFlowResponseTypeDef",
@@ -224,22 +234,20 @@
     {
         "Type": ChannelMembershipTypeType,
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
-
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -266,35 +274,53 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredPushNotificationPreferencesOutputTypeDef = TypedDict(
+    "_RequiredPushNotificationPreferencesOutputTypeDef",
+    {
+        "AllowNotifications": AllowNotificationsType,
+    },
+)
+_OptionalPushNotificationPreferencesOutputTypeDef = TypedDict(
+    "_OptionalPushNotificationPreferencesOutputTypeDef",
+    {
+        "FilterRule": str,
+    },
+    total=False,
+)
+
+class PushNotificationPreferencesOutputTypeDef(
+    _RequiredPushNotificationPreferencesOutputTypeDef,
+    _OptionalPushNotificationPreferencesOutputTypeDef,
+):
+    pass
+
 _RequiredPushNotificationPreferencesTypeDef = TypedDict(
     "_RequiredPushNotificationPreferencesTypeDef",
     {
         "AllowNotifications": AllowNotificationsType,
     },
 )
 _OptionalPushNotificationPreferencesTypeDef = TypedDict(
     "_OptionalPushNotificationPreferencesTypeDef",
     {
         "FilterRule": str,
     },
     total=False,
 )
 
-
 class PushNotificationPreferencesTypeDef(
     _RequiredPushNotificationPreferencesTypeDef, _OptionalPushNotificationPreferencesTypeDef
 ):
     pass
 
-
 MessageAttributeValueTypeDef = TypedDict(
     "MessageAttributeValueTypeDef",
     {
         "StringValues": Sequence[str],
     },
     total=False,
 )
@@ -314,33 +340,41 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
+MessageAttributeValueOutputTypeDef = TypedDict(
+    "MessageAttributeValueOutputTypeDef",
+    {
+        "StringValues": List[str],
+    },
+    total=False,
+)
+
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
 
-ElasticChannelConfigurationTypeDef = TypedDict(
-    "ElasticChannelConfigurationTypeDef",
+ElasticChannelConfigurationOutputTypeDef = TypedDict(
+    "ElasticChannelConfigurationOutputTypeDef",
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
 )
 
-ExpirationSettingsTypeDef = TypedDict(
-    "ExpirationSettingsTypeDef",
+ExpirationSettingsOutputTypeDef = TypedDict(
+    "ExpirationSettingsOutputTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": ExpirationCriterionType,
     },
 )
 
 CreateChannelBanRequestRequestTypeDef = TypedDict(
@@ -381,31 +415,46 @@
     "_OptionalCreateChannelMembershipRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class CreateChannelMembershipRequestRequestTypeDef(
     _RequiredCreateChannelMembershipRequestRequestTypeDef,
     _OptionalCreateChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
-
 CreateChannelModeratorRequestRequestTypeDef = TypedDict(
     "CreateChannelModeratorRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
+ElasticChannelConfigurationTypeDef = TypedDict(
+    "ElasticChannelConfigurationTypeDef",
+    {
+        "MaximumSubChannels": int,
+        "TargetMembershipsPerSubChannel": int,
+        "MinimumMembershipPercentage": int,
+    },
+)
+
+ExpirationSettingsTypeDef = TypedDict(
+    "ExpirationSettingsTypeDef",
+    {
+        "ExpirationDays": int,
+        "ExpirationCriterion": ExpirationCriterionType,
+    },
+)
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -438,22 +487,20 @@
     "_OptionalDeleteChannelMembershipRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class DeleteChannelMembershipRequestRequestTypeDef(
     _RequiredDeleteChannelMembershipRequestRequestTypeDef,
     _OptionalDeleteChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -462,22 +509,20 @@
     "_OptionalDeleteChannelMessageRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class DeleteChannelMessageRequestRequestTypeDef(
     _RequiredDeleteChannelMessageRequestRequestTypeDef,
     _OptionalDeleteChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteChannelModeratorRequestRequestTypeDef = TypedDict(
     "DeleteChannelModeratorRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
@@ -535,22 +580,20 @@
     "_OptionalDescribeChannelMembershipRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class DescribeChannelMembershipRequestRequestTypeDef(
     _RequiredDescribeChannelMembershipRequestRequestTypeDef,
     _OptionalDescribeChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "AppInstanceUserArn": str,
         "ChimeBearer": str,
     },
@@ -610,21 +653,19 @@
     "_OptionalGetChannelMessageRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class GetChannelMessageRequestRequestTypeDef(
     _RequiredGetChannelMessageRequestRequestTypeDef, _OptionalGetChannelMessageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetChannelMessageStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetChannelMessageStatusRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -633,22 +674,20 @@
     "_OptionalGetChannelMessageStatusRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class GetChannelMessageStatusRequestRequestTypeDef(
     _RequiredGetChannelMessageStatusRequestRequestTypeDef,
     _OptionalGetChannelMessageStatusRequestRequestTypeDef,
 ):
     pass
 
-
 MessagingSessionEndpointTypeDef = TypedDict(
     "MessagingSessionEndpointTypeDef",
     {
         "Url": str,
     },
     total=False,
 )
@@ -656,22 +695,30 @@
 GetMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
-StreamingConfigurationTypeDef = TypedDict(
-    "StreamingConfigurationTypeDef",
+StreamingConfigurationOutputTypeDef = TypedDict(
+    "StreamingConfigurationOutputTypeDef",
     {
         "DataType": MessagingDataTypeType,
         "ResourceArn": str,
     },
 )
 
+LambdaConfigurationOutputTypeDef = TypedDict(
+    "LambdaConfigurationOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "InvocationType": Literal["ASYNC"],
+    },
+)
+
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "ResourceArn": str,
         "InvocationType": Literal["ASYNC"],
     },
 )
@@ -688,21 +735,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelBansRequestRequestTypeDef(
     _RequiredListChannelBansRequestRequestTypeDef, _OptionalListChannelBansRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListChannelFlowsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelFlowsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 _OptionalListChannelFlowsRequestRequestTypeDef = TypedDict(
@@ -710,21 +755,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelFlowsRequestRequestTypeDef(
     _RequiredListChannelFlowsRequestRequestTypeDef, _OptionalListChannelFlowsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListChannelMembershipsForAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     {
         "ChimeBearer": str,
     },
 )
 _OptionalListChannelMembershipsForAppInstanceUserRequestRequestTypeDef = TypedDict(
@@ -733,22 +776,20 @@
         "AppInstanceUserArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef(
     _RequiredListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     _OptionalListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListChannelMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelMembershipsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -759,22 +800,20 @@
         "MaxResults": int,
         "NextToken": str,
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelMessagesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -787,22 +826,20 @@
         "MaxResults": int,
         "NextToken": str,
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class ListChannelMessagesRequestRequestTypeDef(
     _RequiredListChannelMessagesRequestRequestTypeDef,
     _OptionalListChannelMessagesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListChannelModeratorsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelModeratorsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -811,22 +848,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelModeratorsRequestRequestTypeDef(
     _RequiredListChannelModeratorsRequestRequestTypeDef,
     _OptionalListChannelModeratorsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListChannelsAssociatedWithChannelFlowRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     {
         "ChannelFlowArn": str,
     },
 )
 _OptionalListChannelsAssociatedWithChannelFlowRequestRequestTypeDef = TypedDict(
@@ -834,22 +869,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef(
     _RequiredListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     _OptionalListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListChannelsModeratedByAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     {
         "ChimeBearer": str,
     },
 )
 _OptionalListChannelsModeratedByAppInstanceUserRequestRequestTypeDef = TypedDict(
@@ -858,22 +891,20 @@
         "AppInstanceUserArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef(
     _RequiredListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     _OptionalListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "ChimeBearer": str,
     },
 )
@@ -883,21 +914,19 @@
         "Privacy": ChannelPrivacyType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChannelsRequestRequestTypeDef(
     _RequiredListChannelsRequestRequestTypeDef, _OptionalListChannelsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListSubChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListSubChannelsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -906,21 +935,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSubChannelsRequestRequestTypeDef(
     _RequiredListSubChannelsRequestRequestTypeDef, _OptionalListSubChannelsRequestRequestTypeDef
 ):
     pass
 
-
 SubChannelSummaryTypeDef = TypedDict(
     "SubChannelSummaryTypeDef",
     {
         "SubChannelId": str,
         "MembershipCount": int,
     },
     total=False,
@@ -929,14 +956,30 @@
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
+StreamingConfigurationTypeDef = TypedDict(
+    "StreamingConfigurationTypeDef",
+    {
+        "DataType": MessagingDataTypeType,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -945,22 +988,20 @@
     "_OptionalRedactChannelMessageRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
-
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-
 RedactChannelMessageResponseTypeDef = TypedDict(
     "RedactChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "SubChannelId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -983,14 +1024,22 @@
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
 )
 
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
+    {
+        "MemberArn": str,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1018,22 +1067,20 @@
         "Metadata": str,
         "SubChannelId": str,
         "ContentType": str,
     },
     total=False,
 )
 
-
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -1059,21 +1106,19 @@
         "Name": str,
         "Mode": ChannelModeType,
         "Metadata": str,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1218,14 +1263,22 @@
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ChannelMembershipPreferencesOutputTypeDef = TypedDict(
+    "ChannelMembershipPreferencesOutputTypeDef",
+    {
+        "PushNotifications": PushNotificationPreferencesOutputTypeDef,
+    },
+    total=False,
+)
+
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
     },
     total=False,
 )
@@ -1245,21 +1298,19 @@
         "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
         "ContentType": str,
     },
     total=False,
 )
 
-
 class ChannelMessageCallbackTypeDef(
     _RequiredChannelMessageCallbackTypeDef, _OptionalChannelMessageCallbackTypeDef
 ):
     pass
 
-
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
         "Status": ChannelMessageStatusStructureTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1295,17 +1346,17 @@
         "Type": ChannelMessageTypeType,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "ContentType": str,
-        "Target": List[TargetTypeDef],
+        "Target": List[TargetOutputTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1317,102 +1368,55 @@
         "CreatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "SubChannelId": str,
         "ContentType": str,
-        "Target": List[TargetTypeDef],
+        "Target": List[TargetOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "CreatedBy": IdentityTypeDef,
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ChannelFlowArn": str,
-        "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ElasticChannelConfiguration": ElasticChannelConfigurationOutputTypeDef,
+        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
+PutChannelExpirationSettingsResponseTypeDef = TypedDict(
+    "PutChannelExpirationSettingsResponseTypeDef",
     {
         "ChannelArn": str,
+        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
-    {
-        "ChimeBearer": str,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class PutChannelExpirationSettingsRequestRequestTypeDef(
-    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
-    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
-):
-    pass
-
 
-PutChannelExpirationSettingsResponseTypeDef = TypedDict(
-    "PutChannelExpirationSettingsResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ChannelArn": str,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1433,66 +1437,68 @@
         "ModeratorArns": Sequence[str],
         "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
         "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
     },
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ChimeBearer": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
+    total=False,
 )
 
+class PutChannelExpirationSettingsRequestRequestTypeDef(
+    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
+    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
+):
+    pass
+
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
+        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
+PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
+        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsResponseTypeDef",
+ProcessorConfigurationOutputTypeDef = TypedDict(
+    "ProcessorConfigurationOutputTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Lambda": LambdaConfigurationOutputTypeDef,
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
@@ -1505,14 +1511,30 @@
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
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
+PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
+    {
+        "AppInstanceArn": str,
+        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
+    },
+)
+
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
     },
 )
 _OptionalSearchChannelsRequestRequestTypeDef = TypedDict(
@@ -1521,20 +1543,48 @@
         "ChimeBearer": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchChannelsRequestRequestTypeDef(
     _RequiredSearchChannelsRequestRequestTypeDef, _OptionalSearchChannelsRequestRequestTypeDef
 ):
     pass
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
 
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1630,36 +1680,36 @@
 )
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "Preferences": ChannelMembershipPreferencesTypeDef,
+        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesRequestRequestTypeDef",
+PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
-        "MemberArn": str,
-        "ChimeBearer": str,
-        "Preferences": ChannelMembershipPreferencesTypeDef,
+        "Member": IdentityTypeDef,
+        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesResponseTypeDef",
+PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "Member": IdentityTypeDef,
+        "MemberArn": str,
+        "ChimeBearer": str,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1671,22 +1721,20 @@
     "_OptionalChannelFlowCallbackRequestRequestTypeDef",
     {
         "DeleteResource": bool,
     },
     total=False,
 )
 
-
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
-
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
@@ -1706,14 +1754,24 @@
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProcessorOutputTypeDef = TypedDict(
+    "ProcessorOutputTypeDef",
+    {
+        "Name": str,
+        "Configuration": ProcessorConfigurationOutputTypeDef,
+        "ExecutionOrder": int,
+        "FallbackAction": FallbackActionType,
+    },
+)
+
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
         "Configuration": ProcessorConfigurationTypeDef,
         "ExecutionOrder": int,
         "FallbackAction": FallbackActionType,
@@ -1721,24 +1779,24 @@
 )
 
 ChannelFlowSummaryTypeDef = TypedDict(
     "ChannelFlowSummaryTypeDef",
     {
         "ChannelFlowArn": str,
         "Name": str,
-        "Processors": List[ProcessorTypeDef],
+        "Processors": List[ProcessorOutputTypeDef],
     },
     total=False,
 )
 
 ChannelFlowTypeDef = TypedDict(
     "ChannelFlowTypeDef",
     {
         "ChannelFlowArn": str,
-        "Processors": List[ProcessorTypeDef],
+        "Processors": List[ProcessorOutputTypeDef],
         "Name": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
@@ -1755,21 +1813,19 @@
     "_OptionalCreateChannelFlowRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateChannelFlowRequestRequestTypeDef(
     _RequiredCreateChannelFlowRequestRequestTypeDef, _OptionalCreateChannelFlowRequestRequestTypeDef
 ):
     pass
 
-
 UpdateChannelFlowRequestRequestTypeDef = TypedDict(
     "UpdateChannelFlowRequestRequestTypeDef",
     {
         "ChannelFlowArn": str,
         "Processors": Sequence[ProcessorTypeDef],
         "Name": str,
     },
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging/type_defs.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,35 +37,40 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
     "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
+    "PushNotificationPreferencesOutputTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
-    "TargetTypeDef",
-    "ElasticChannelConfigurationTypeDef",
-    "ExpirationSettingsTypeDef",
+    "MessageAttributeValueOutputTypeDef",
+    "TargetOutputTypeDef",
+    "ElasticChannelConfigurationOutputTypeDef",
+    "ExpirationSettingsOutputTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
     "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
+    "ElasticChannelConfigurationTypeDef",
+    "ExpirationSettingsTypeDef",
     "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
@@ -80,32 +85,36 @@
     "DisassociateChannelFlowRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
-    "StreamingConfigurationTypeDef",
+    "StreamingConfigurationOutputTypeDef",
+    "LambdaConfigurationOutputTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "StreamingConfigurationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
     "RedactChannelMessageResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
+    "TargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
@@ -120,53 +129,56 @@
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
+    "ChannelMembershipPreferencesOutputTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
-    "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
-    "CreateChannelRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateChannelRequestRequestTypeDef",
+    "PutChannelExpirationSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
+    "ProcessorConfigurationOutputTypeDef",
     "ProcessorConfigurationTypeDef",
     "ListSubChannelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "SearchChannelsRequestRequestTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
-    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
+    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
+    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
     "UpdateChannelFlowRequestRequestTypeDef",
     "ListChannelFlowsResponseTypeDef",
     "DescribeChannelFlowResponseTypeDef",
@@ -223,20 +235,22 @@
     {
         "Type": ChannelMembershipTypeType,
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
+
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -263,33 +277,57 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredPushNotificationPreferencesOutputTypeDef = TypedDict(
+    "_RequiredPushNotificationPreferencesOutputTypeDef",
+    {
+        "AllowNotifications": AllowNotificationsType,
+    },
+)
+_OptionalPushNotificationPreferencesOutputTypeDef = TypedDict(
+    "_OptionalPushNotificationPreferencesOutputTypeDef",
+    {
+        "FilterRule": str,
+    },
+    total=False,
+)
+
+
+class PushNotificationPreferencesOutputTypeDef(
+    _RequiredPushNotificationPreferencesOutputTypeDef,
+    _OptionalPushNotificationPreferencesOutputTypeDef,
+):
+    pass
+
+
 _RequiredPushNotificationPreferencesTypeDef = TypedDict(
     "_RequiredPushNotificationPreferencesTypeDef",
     {
         "AllowNotifications": AllowNotificationsType,
     },
 )
 _OptionalPushNotificationPreferencesTypeDef = TypedDict(
     "_OptionalPushNotificationPreferencesTypeDef",
     {
         "FilterRule": str,
     },
     total=False,
 )
 
+
 class PushNotificationPreferencesTypeDef(
     _RequiredPushNotificationPreferencesTypeDef, _OptionalPushNotificationPreferencesTypeDef
 ):
     pass
 
+
 MessageAttributeValueTypeDef = TypedDict(
     "MessageAttributeValueTypeDef",
     {
         "StringValues": Sequence[str],
     },
     total=False,
 )
@@ -309,33 +347,41 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
+MessageAttributeValueOutputTypeDef = TypedDict(
+    "MessageAttributeValueOutputTypeDef",
+    {
+        "StringValues": List[str],
+    },
+    total=False,
+)
+
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
 
-ElasticChannelConfigurationTypeDef = TypedDict(
-    "ElasticChannelConfigurationTypeDef",
+ElasticChannelConfigurationOutputTypeDef = TypedDict(
+    "ElasticChannelConfigurationOutputTypeDef",
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
 )
 
-ExpirationSettingsTypeDef = TypedDict(
-    "ExpirationSettingsTypeDef",
+ExpirationSettingsOutputTypeDef = TypedDict(
+    "ExpirationSettingsOutputTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": ExpirationCriterionType,
     },
 )
 
 CreateChannelBanRequestRequestTypeDef = TypedDict(
@@ -376,29 +422,48 @@
     "_OptionalCreateChannelMembershipRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class CreateChannelMembershipRequestRequestTypeDef(
     _RequiredCreateChannelMembershipRequestRequestTypeDef,
     _OptionalCreateChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
+
 CreateChannelModeratorRequestRequestTypeDef = TypedDict(
     "CreateChannelModeratorRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
+ElasticChannelConfigurationTypeDef = TypedDict(
+    "ElasticChannelConfigurationTypeDef",
+    {
+        "MaximumSubChannels": int,
+        "TargetMembershipsPerSubChannel": int,
+        "MinimumMembershipPercentage": int,
+    },
+)
+
+ExpirationSettingsTypeDef = TypedDict(
+    "ExpirationSettingsTypeDef",
+    {
+        "ExpirationDays": int,
+        "ExpirationCriterion": ExpirationCriterionType,
+    },
+)
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -431,20 +496,22 @@
     "_OptionalDeleteChannelMembershipRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class DeleteChannelMembershipRequestRequestTypeDef(
     _RequiredDeleteChannelMembershipRequestRequestTypeDef,
     _OptionalDeleteChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -453,20 +520,22 @@
     "_OptionalDeleteChannelMessageRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class DeleteChannelMessageRequestRequestTypeDef(
     _RequiredDeleteChannelMessageRequestRequestTypeDef,
     _OptionalDeleteChannelMessageRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteChannelModeratorRequestRequestTypeDef = TypedDict(
     "DeleteChannelModeratorRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
@@ -524,20 +593,22 @@
     "_OptionalDescribeChannelMembershipRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class DescribeChannelMembershipRequestRequestTypeDef(
     _RequiredDescribeChannelMembershipRequestRequestTypeDef,
     _OptionalDescribeChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "AppInstanceUserArn": str,
         "ChimeBearer": str,
     },
@@ -597,19 +668,21 @@
     "_OptionalGetChannelMessageRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class GetChannelMessageRequestRequestTypeDef(
     _RequiredGetChannelMessageRequestRequestTypeDef, _OptionalGetChannelMessageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetChannelMessageStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetChannelMessageStatusRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -618,20 +691,22 @@
     "_OptionalGetChannelMessageStatusRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class GetChannelMessageStatusRequestRequestTypeDef(
     _RequiredGetChannelMessageStatusRequestRequestTypeDef,
     _OptionalGetChannelMessageStatusRequestRequestTypeDef,
 ):
     pass
 
+
 MessagingSessionEndpointTypeDef = TypedDict(
     "MessagingSessionEndpointTypeDef",
     {
         "Url": str,
     },
     total=False,
 )
@@ -639,22 +714,30 @@
 GetMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
-StreamingConfigurationTypeDef = TypedDict(
-    "StreamingConfigurationTypeDef",
+StreamingConfigurationOutputTypeDef = TypedDict(
+    "StreamingConfigurationOutputTypeDef",
     {
         "DataType": MessagingDataTypeType,
         "ResourceArn": str,
     },
 )
 
+LambdaConfigurationOutputTypeDef = TypedDict(
+    "LambdaConfigurationOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "InvocationType": Literal["ASYNC"],
+    },
+)
+
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "ResourceArn": str,
         "InvocationType": Literal["ASYNC"],
     },
 )
@@ -671,19 +754,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelBansRequestRequestTypeDef(
     _RequiredListChannelBansRequestRequestTypeDef, _OptionalListChannelBansRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListChannelFlowsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelFlowsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 _OptionalListChannelFlowsRequestRequestTypeDef = TypedDict(
@@ -691,19 +776,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelFlowsRequestRequestTypeDef(
     _RequiredListChannelFlowsRequestRequestTypeDef, _OptionalListChannelFlowsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListChannelMembershipsForAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     {
         "ChimeBearer": str,
     },
 )
 _OptionalListChannelMembershipsForAppInstanceUserRequestRequestTypeDef = TypedDict(
@@ -712,20 +799,22 @@
         "AppInstanceUserArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef(
     _RequiredListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     _OptionalListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListChannelMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelMembershipsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -736,20 +825,22 @@
         "MaxResults": int,
         "NextToken": str,
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelMessagesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -762,20 +853,22 @@
         "MaxResults": int,
         "NextToken": str,
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class ListChannelMessagesRequestRequestTypeDef(
     _RequiredListChannelMessagesRequestRequestTypeDef,
     _OptionalListChannelMessagesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListChannelModeratorsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelModeratorsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -784,20 +877,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelModeratorsRequestRequestTypeDef(
     _RequiredListChannelModeratorsRequestRequestTypeDef,
     _OptionalListChannelModeratorsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListChannelsAssociatedWithChannelFlowRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     {
         "ChannelFlowArn": str,
     },
 )
 _OptionalListChannelsAssociatedWithChannelFlowRequestRequestTypeDef = TypedDict(
@@ -805,20 +900,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef(
     _RequiredListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     _OptionalListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListChannelsModeratedByAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     {
         "ChimeBearer": str,
     },
 )
 _OptionalListChannelsModeratedByAppInstanceUserRequestRequestTypeDef = TypedDict(
@@ -827,20 +924,22 @@
         "AppInstanceUserArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef(
     _RequiredListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     _OptionalListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "ChimeBearer": str,
     },
 )
@@ -850,19 +949,21 @@
         "Privacy": ChannelPrivacyType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChannelsRequestRequestTypeDef(
     _RequiredListChannelsRequestRequestTypeDef, _OptionalListChannelsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListSubChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListSubChannelsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -871,19 +972,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSubChannelsRequestRequestTypeDef(
     _RequiredListSubChannelsRequestRequestTypeDef, _OptionalListSubChannelsRequestRequestTypeDef
 ):
     pass
 
+
 SubChannelSummaryTypeDef = TypedDict(
     "SubChannelSummaryTypeDef",
     {
         "SubChannelId": str,
         "MembershipCount": int,
     },
     total=False,
@@ -892,14 +995,30 @@
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
+StreamingConfigurationTypeDef = TypedDict(
+    "StreamingConfigurationTypeDef",
+    {
+        "DataType": MessagingDataTypeType,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -908,20 +1027,22 @@
     "_OptionalRedactChannelMessageRequestRequestTypeDef",
     {
         "SubChannelId": str,
     },
     total=False,
 )
 
+
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
+
 RedactChannelMessageResponseTypeDef = TypedDict(
     "RedactChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "SubChannelId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -944,14 +1065,22 @@
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
 )
 
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
+    {
+        "MemberArn": str,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -979,20 +1108,22 @@
         "Metadata": str,
         "SubChannelId": str,
         "ContentType": str,
     },
     total=False,
 )
 
+
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -1018,19 +1149,21 @@
         "Name": str,
         "Mode": ChannelModeType,
         "Metadata": str,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1175,14 +1308,22 @@
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ChannelMembershipPreferencesOutputTypeDef = TypedDict(
+    "ChannelMembershipPreferencesOutputTypeDef",
+    {
+        "PushNotifications": PushNotificationPreferencesOutputTypeDef,
+    },
+    total=False,
+)
+
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
     },
     total=False,
 )
@@ -1202,19 +1343,21 @@
         "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
         "ContentType": str,
     },
     total=False,
 )
 
+
 class ChannelMessageCallbackTypeDef(
     _RequiredChannelMessageCallbackTypeDef, _OptionalChannelMessageCallbackTypeDef
 ):
     pass
 
+
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
         "Status": ChannelMessageStatusStructureTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1250,17 +1393,17 @@
         "Type": ChannelMessageTypeType,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "ContentType": str,
-        "Target": List[TargetTypeDef],
+        "Target": List[TargetOutputTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1272,98 +1415,55 @@
         "CreatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "SubChannelId": str,
         "ContentType": str,
-        "Target": List[TargetTypeDef],
+        "Target": List[TargetOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "CreatedBy": IdentityTypeDef,
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ChannelFlowArn": str,
-        "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ElasticChannelConfiguration": ElasticChannelConfigurationOutputTypeDef,
+        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
+PutChannelExpirationSettingsResponseTypeDef = TypedDict(
+    "PutChannelExpirationSettingsResponseTypeDef",
     {
         "ChannelArn": str,
+        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
-    {
-        "ChimeBearer": str,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
-    },
-    total=False,
-)
-
-class PutChannelExpirationSettingsRequestRequestTypeDef(
-    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
-    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
-):
-    pass
 
-PutChannelExpirationSettingsResponseTypeDef = TypedDict(
-    "PutChannelExpirationSettingsResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ChannelArn": str,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1384,64 +1484,72 @@
         "ModeratorArns": Sequence[str],
         "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
         "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+
+_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
     },
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ChimeBearer": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
+    total=False,
 )
 
+
+class PutChannelExpirationSettingsRequestRequestTypeDef(
+    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
+    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
+):
+    pass
+
+
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
+        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
+PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
+        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsResponseTypeDef",
+ProcessorConfigurationOutputTypeDef = TypedDict(
+    "ProcessorConfigurationOutputTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Lambda": LambdaConfigurationOutputTypeDef,
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
@@ -1454,14 +1562,30 @@
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
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
+PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
+    {
+        "AppInstanceArn": str,
+        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
+    },
+)
+
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
     },
 )
 _OptionalSearchChannelsRequestRequestTypeDef = TypedDict(
@@ -1470,19 +1594,53 @@
         "ChimeBearer": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchChannelsRequestRequestTypeDef(
     _RequiredSearchChannelsRequestRequestTypeDef, _OptionalSearchChannelsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
+
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1577,36 +1735,36 @@
 )
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "Preferences": ChannelMembershipPreferencesTypeDef,
+        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesRequestRequestTypeDef",
+PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
-        "MemberArn": str,
-        "ChimeBearer": str,
-        "Preferences": ChannelMembershipPreferencesTypeDef,
+        "Member": IdentityTypeDef,
+        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesResponseTypeDef",
+PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "Member": IdentityTypeDef,
+        "MemberArn": str,
+        "ChimeBearer": str,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1618,20 +1776,22 @@
     "_OptionalChannelFlowCallbackRequestRequestTypeDef",
     {
         "DeleteResource": bool,
     },
     total=False,
 )
 
+
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
+
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
@@ -1651,14 +1811,24 @@
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProcessorOutputTypeDef = TypedDict(
+    "ProcessorOutputTypeDef",
+    {
+        "Name": str,
+        "Configuration": ProcessorConfigurationOutputTypeDef,
+        "ExecutionOrder": int,
+        "FallbackAction": FallbackActionType,
+    },
+)
+
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
         "Configuration": ProcessorConfigurationTypeDef,
         "ExecutionOrder": int,
         "FallbackAction": FallbackActionType,
@@ -1666,24 +1836,24 @@
 )
 
 ChannelFlowSummaryTypeDef = TypedDict(
     "ChannelFlowSummaryTypeDef",
     {
         "ChannelFlowArn": str,
         "Name": str,
-        "Processors": List[ProcessorTypeDef],
+        "Processors": List[ProcessorOutputTypeDef],
     },
     total=False,
 )
 
 ChannelFlowTypeDef = TypedDict(
     "ChannelFlowTypeDef",
     {
         "ChannelFlowArn": str,
-        "Processors": List[ProcessorTypeDef],
+        "Processors": List[ProcessorOutputTypeDef],
         "Name": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
@@ -1700,19 +1870,21 @@
     "_OptionalCreateChannelFlowRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateChannelFlowRequestRequestTypeDef(
     _RequiredCreateChannelFlowRequestRequestTypeDef, _OptionalCreateChannelFlowRequestRequestTypeDef
 ):
     pass
 
+
 UpdateChannelFlowRequestRequestTypeDef = TypedDict(
     "UpdateChannelFlowRequestRequestTypeDef",
     {
         "ChannelFlowArn": str,
         "Processors": Sequence[ProcessorTypeDef],
         "Name": str,
     },
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime-sdk-messaging"></a>
 
 # mypy-boto3-chime-sdk-messaging
 
 [![PyPI - mypy-boto3-chime-sdk-messaging](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,26 +321,30 @@
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
     ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
+    PushNotificationPreferencesOutputTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
-    TargetTypeDef,
-    ElasticChannelConfigurationTypeDef,
-    ExpirationSettingsTypeDef,
+    MessageAttributeValueOutputTypeDef,
+    TargetOutputTypeDef,
+    ElasticChannelConfigurationOutputTypeDef,
+    ExpirationSettingsOutputTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
     CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
@@ -355,32 +359,36 @@
     DisassociateChannelFlowRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationOutputTypeDef,
+    LambdaConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    StreamingConfigurationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
     RedactChannelMessageResponseTypeDef,
     ResponseMetadataTypeDef,
     SearchFieldTypeDef,
+    TargetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
@@ -395,53 +403,56 @@
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
+    ChannelMembershipPreferencesOutputTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
-    PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
-    CreateChannelRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateChannelRequestRequestTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
-    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
+    ProcessorConfigurationOutputTypeDef,
     ProcessorConfigurationTypeDef,
     ListSubChannelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     SearchChannelsRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
-    PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
+    PutChannelMembershipPreferencesRequestRequestTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.0/setup.py` & `mypy-boto3-chime-sdk-messaging-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-messaging",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMessaging 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ChimeSDKMessaging 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

